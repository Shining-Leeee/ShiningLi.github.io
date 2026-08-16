---
show: true
width: 4
date: 2025-12-12 00:01:00 +0800
group: Not Just Research
---
 【需求1 & 3】外层卡片：h-100保证底端对齐；加入 transition 动画、鼠标悬停浮动阴影与手型；绑定点击弹窗 -->
<div class="card border-0 shadow-sm h-100" 
     style="border-radius: 8px; overflow: hidden; cursor: pointer; transition: all 0.3s ease;"
     data-toggle="modal" data-target="#modal-shanghai"
     onmouseover="this.style.transform='translateY(-6px)'; this.classList.add('shadow');" 
     onmouseout="this.style.transform='translateY(0)'; this.classList.remove('shadow');">
    
    <!-- 【需求2】缩略图：aspect-ratio: 3/14 宽3高4 保证正方形大占比显示，裁切居中 -->
    <img data-src="{{ '/assets/images/etc/shanghai.jpg' | relative_url }}" 
         class="lazy w-100" 
         style="aspect-ratio: 3/4; object-fit: cover; border-top-left-radius: 8px; border-top-right-radius: 8px;" 
         src="{{ '/assets/images/etc/shanghai.jpg' | relative_url }}">
    
    <!-- 卡片主体：d-flex flex-column 自动撑开底部对齐 -->
    <div class="card-body p-3 bg-light d-flex flex-column">
        <!-- 【需求2】截断文字：严格限制 4 行，超出自动隐藏并显示原生省略号 -->
        <p class="card-text mb-1" style="font-size: 0.9em; color: #444; display: -webkit-box; -webkit-line-clamp: 4; -webkit-box-orient: vertical; overflow: hidden; text-overflow: ellipsis;">
        I was under a lot of pressure when I was facing thesis proposal defense, so I came to Shanghai Disneyland to relax and had a magical day! 
        After returning to school, I threw myself into the thesis proposal defense again and achieved excellent results!
        </p>
        <!-- 引导点击的加粗提示 -->
        <div class="mt-auto text-right">
            <span style="font-size: 0.85rem; color: #555; font-weight: bold;">... Read More</span>
        </div>
    </div>
</div>

<!-- 【需求3】弹窗 (Modal) 代码：优雅的全屏居中放大框 -->
<!-- ⚠️ 重点：每张照片的 id 必须唯一！ -->
<div class="modal fade" id="modal-dongwu" tabindex="-1" role="dialog" aria-hidden="true">
    <div class="modal-dialog modal-lg modal-dialog-centered" role="document">
        <div class="modal-content shadow-lg" style="border-radius: 12px; overflow: hidden; border: none;">
            
            <!-- 弹窗右上角关闭按钮 -->
            <button type="button" class="close position-absolute" data-dismiss="modal" aria-label="Close" style="right: 15px; top: 10px; z-index: 10; text-shadow: 0 1px 0 #fff; opacity: .8; background: rgba(255,255,255,0.7); border-radius: 50%; width: 30px; height: 30px; line-height: 24px;">
                <span aria-hidden="true" style="font-size: 1.5rem; color: #000;">&times;</span>
            </button>

            <!-- 弹窗内的完整原始图片（取消裁剪，展示全貌，最高占屏幕高度的 70%） -->
            <img src="{{ '/assets/images/etc/shanghai.jpg' | relative_url }}" class="w-100" style="max-height: 70vh; object-fit: contain; background-color: #f0f0f0;">
            
            <!-- 弹窗内的全部未截断文字 -->
            <div class="modal-body p-4 bg-white">
                <p style="font-size: 1rem; color: #333; line-height: 1.6; margin-bottom: 0;">
                    I was under a lot of pressure when I was facing thesis proposal defense, so I came to Shanghai Disneyland to relax and had a magical day! 
                    After returning to school, I threw myself into the thesis proposal defense again and achieved excellent results!
                </p>
            </div>
            
        </div>
    </div>
</div>

