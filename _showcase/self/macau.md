---
show: true
width: 4
date: 2025-12-10 00:01:00 +0800
group: Not Just Research
---
<!-- 卡片主体 -->
<div class="card border-0 shadow-sm h-100" 
     style="border-radius: 8px; overflow: hidden; cursor: pointer; transition: all 0.3s ease;"
     data-toggle="modal" data-target="#modal-macau"
     onmouseover="this.style.transform='translateY(-6px)'; this.classList.add('shadow');" 
     onmouseout="this.style.transform='translateY(0)'; this.classList.remove('shadow');">
    
    <!-- 缩略图：aspect-ratio 3/4 竖版显示 -->
    <img data-src="{{ '/assets/images/etc/macau.jpg' | relative_url }}" 
         class="lazy w-100" 
         style="aspect-ratio: 3/4; object-fit: cover; border-top-left-radius: 8px; border-top-right-radius: 8px;" 
         src="{{ '/assets/images/etc/macau.jpg' | relative_url }}">
    
    <!-- 文字区域 -->
    <div class="card-body p-3 bg-light d-flex flex-column">
        <p class="card-text mb-1" style="font-size: 0.9em; color: #444; display: -webkit-box; -webkit-line-clamp: 4; -webkit-box-orient: vertical; overflow: hidden; text-overflow: ellipsis;">
            Macau, China – a city with an exceptionally great experience! The environment here is great, there's lots of delicious food, and the people are very welcoming!
        </p>
        <div class="mt-auto text-right">
            <span style="font-size: 0.85rem; color: #555; font-weight: bold;">... Read More</span>
        </div>
    </div>
</div>

<!-- 弹窗 (Modal) -->
<div class="modal fade" id="modal-macau" tabindex="-1" role="dialog" aria-hidden="true">
    <div class="modal-dialog modal-lg modal-dialog-centered" role="document">
        <div class="modal-content shadow-lg" style="border-radius: 12px; overflow: hidden; border: none;">
            
            <!-- 关闭按钮 -->
            <button type="button" class="close position-absolute" data-dismiss="modal" aria-label="Close" style="right: 15px; top: 10px; z-index: 10; text-shadow: 0 1px 0 #fff; opacity: .8; background: rgba(255,255,255,0.7); border-radius: 50%; width: 30px; height: 30px; line-height: 24px;">
                <span aria-hidden="true" style="font-size: 1.5rem; color: #000;">&times;</span>
            </button>

            <!-- 完整图片 -->
            <img src="{{ '/assets/images/etc/macau.jpg' | relative_url }}" class="w-100" style="max-height: 70vh; object-fit: contain; background-color: #f0f0f0;">
            
            <!-- 完整文字 -->
            <div class="modal-body p-4 bg-white">
                <p style="font-size: 1rem; color: #333; line-height: 1.6; margin-bottom: 0;">
                    Macau, China – a city with an exceptionally great experience! The environment here is great, there's lots of delicious food, and the people are very welcoming!
                </p>
            </div>
            
        </div>
    </div>
</div>
