---
show: true
width: 4
date: 2025-12-12 00:01:00 +0800
group: Not Just Research
---
<div class="card border-0 shadow-sm h-100" style="border-radius: 8px; overflow: hidden;">
    <!-- 照片部分：将圆角改为了 rounded-top 以贴合卡片顶部 -->
    <img data-src="{{ 'assets/images/etc/shanghai.jpg' | relative_url }}" class="lazy w-100" style="aspect-ratio: 4/3; object-fit: cover; border-top-left-radius: 8px; border-top-right-radius: 8px;" src="{{ '/assets/images/etc/shanghai.jpg' | relative_url }}">
    
    <!-- 文字心情部分：带有内边距的卡片主体 -->
    <div class="card-body p-3 bg-light d-flex flex-column">
        <p class="card-text mb-0" style="font-size: 0.9em; color: #444;">
            I was under a lot of pressure when I was facing thesis proposal defense, so I came to Shanghai Disneyland to relax and had a magical day! 
            After returning to school, I threw myself into the thesis proposal defense again and achieved excellent results!
        </p>
    </div>
</div>
