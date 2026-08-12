---
show: true
width: 6
date: 2024-12-12 00:01:00 +0800
group: Not Just Research
---
<div class="card border-0 shadow-sm" style="border-radius: 8px; overflow: hidden;">
    <!-- 照片部分：将圆角改为了 rounded-top 以贴合卡片顶部 -->
    <img data-src="{{ 'assets/images/etc/hangzhou.jpg' | relative_url }}" class="lazy w-100" style="border-top-left-radius: 8px; border-top-right-radius: 8px;" src="{{ '/assets/images/etc/hangzhou.jpg' | relative_url }}">
    
    <!-- 文字心情部分：带有内边距的卡片主体 -->
    <div class="card-body p-3 bg-light">
        <p class="card-text mb-0" style="font-size: 0.9em; color: #444;">
            I arrived at West Lake in Hangzhou and enjoyed its scenery.
        </p>
    </div>
</div>
