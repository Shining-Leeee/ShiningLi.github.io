---
show: true
width: 4  #<--- 就是这里！改成 4 即可（这个学术页面的模板是12栅格系统，也就是将整个页面宽度分成了12份。这里是4 代表一行展示三张）
date: 2024-12-12 00:01:00 +0800 #Jekyll 博客系统（通常也是这类学术主页模板的底层框架）默认是按照时间倒序来排列这些展示区块的。最新的排在最前面，最旧的排在最后面。
group: Not Just Research
---
<div class="card border-0 shadow-sm" style="border-radius: 8px; overflow: hidden;">
    <!-- 照片部分：将圆角改为了 rounded-top 以贴合卡片顶部 -->
    <img data-src="{{ 'assets/images/etc/dongwu.jpg' | relative_url }}" class="lazy w-100" style="aspect-ratio: 4/3; object-fit: cover; border-top-left-radius: 8px; border-top-right-radius: 8px;" src="{{ '/assets/images/etc/dongwu.jpg' | relative_url }}">
    
    <!-- 文字心情部分：带有内边距的卡片主体 -->
    <div class="card-body p-3 bg-light">
        <p class="card-text mb-0" style="font-size: 0.9em; color: #444;">
           I love animals, although I can be a little scared of them sometimes. This year, I spent my birthday with my puppies!
        </p>
    </div>
</div>
