<!DOCTYPE html>
<html lang="zh-CN" data-theme="light">
    <head prefix="og: http://ogp.me/ns# article: http://ogp.me/ns/article#">
    <meta charset="UTF-8" />

    <meta name="theme-color" content="#fff" />
        <script>
            const theme = localStorage.getItem('theme');
            if (theme === "dark") {
                document.documentElement.setAttribute('data-theme', 'dark');
                document.querySelector('meta[name="theme-color"]').setAttribute('content', '#1c1c21');
            } else if (theme === "light") {
                document.documentElement.setAttribute('data-theme', 'light');
                document.querySelector('meta[name="theme-color"]').setAttribute('content', '#fff');
            }
        </script>

    

    
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=2.0, user-scalable=yes" />
    
    <meta http-equiv="X-UA-Compatible" content="IE=edge, chrome=1" />
    
    <meta name="format-detection" content="telephone=no, date=no, address=no, email=no" />
    
    <meta http-equiv="Cache-Control" content="no-transform" />
    
    <meta http-equiv="Cache-Control" content="no-siteapp" />
    
    <meta name="renderer" content="webkit" />

    <meta name="generator" content="Hugo 0.63.2" />

    <title>jiajie</title>

    <link rel="stylesheet" href="/css/meme.min.12355d9f83e5a83fa528c18fffe66a867e8bf139bf9577d2d81cafa56c202fcb.css" integrity="sha256-EjVdn4PlqD+lKMGP/+Zqhn6L8Tm/lXfS2ByvpWwgL8s=" data-instant-track />

    <link href="https://fonts.googleapis.com/css?family=EB+Garamond:400,400i,500,700,700i|Noto+Serif+SC:400,500,700|Source+Code+Pro:400,400i,700,700i&display=swap&subset=chinese-simplified" rel="stylesheet" />

    <meta name="author" content="jiajie" />
    <meta name="description" content="jiajie的个人博客" />
    <meta name="keywords" content="c, cpp, cuda, cv, dl, face-reconstruction, hugo, jazz, mask-rcnn, python, pytorch, sfm, slam, 三维重建, 主题, 人体重建, 卷积神经网络, 多视图几何, 学习笔记, 实时重建, 数据结构与算法, 点云配准, 爬虫, 环境配置, 碎碎念, 笔记, 编译, 英语, 规划, 论文解读, 高性能编程, post, life, broken-thoughts, tech, human-body-reconstruction, slam-sfm, day-day-up, multi-view-geometry, tools" />
    
    <link rel="shortcut icon" type="image/ico" href="/favicon.ico" />
    <link rel="mask-icon" href="/icons/safari-pinned-tab.svg" color="#2a6df4" />
    <link rel="apple-touch-icon" sizes="180x180" href="/icons/apple-touch-icon.png" />
    <meta name="apple-mobile-web-app-capable" content="yes" />
    <meta name="apple-mobile-web-app-title" content="jiajie" />
    <meta name="apple-mobile-web-app-status-bar-style" content="black-translucent" />
    <meta name="mobile-web-app-capable" content="yes" />
    <meta name="application-name" content="jiajie" />
    <meta name="msapplication-starturl" content="./" />
    <meta name="msapplication-TileColor" content="#fff" />
    <meta name="msapplication-TileImage" content="./icons/mstile-150x150.png" />
    <link rel="manifest" href="/manifest.json" />

    
    <link rel="alternate" type="application/atom+xml" href="https://jiajiewu.gitee.io/atom.xml" title="jiajie" />
    <link rel="alternate" type="application/rss+xml" href="https://jiajiewu.gitee.io/rss.xml" title="jiajie" />
    

    
    <link rel="canonical" href="https://jiajiewu.gitee.io/" />




<script type="application/ld+json">
    {
        "@context": "https://schema.org",
        "@type": "WebSite",
        "datePublished": "2019-11-16T20:17:43+00:00",
        "dateModified": "2020-05-14T22:44:38+08:00",
        "url": "https://jiajiewu.gitee.io/",
        "description": "jiajie的个人博客",
        "keywords": "c, cpp, cuda, cv, dl, face-reconstruction, hugo, jazz, mask-rcnn, python, pytorch, sfm, slam, 三维重建, 主题, 人体重建, 卷积神经网络, 多视图几何, 学习笔记, 实时重建, 数据结构与算法, 点云配准, 爬虫, 环境配置, 碎碎念, 笔记, 编译, 英语, 规划, 论文解读, 高性能编程, post, life, broken-thoughts, tech, human-body-reconstruction, slam-sfm, day-day-up, multi-view-geometry, tools",
        "image": "https://jiajiewu.gitee.io/icons/apple-touch-icon.png",
        "author": {
            "@type": "Person",
            "description": "学习，生活",
            "email": "3208920286@qq.com",
            "image": "https://jiajiewu.gitee.io/icons/apple-touch-icon.png",
            "url": "https://jiajiewu.gitee.io/",
            "name": "jiajie"
        },
        "license": "[CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.zh)",
        "name": "jiajie"
    }
</script>

    



<meta name="twitter:card" content="summary" />


    






<meta property="og:title" content="jiajie" />
<meta property="og:description" content="jiajie的个人博客" />
<meta property="og:url" content="https://jiajiewu.gitee.io/" />
<meta property="og:site_name" content="jiajie" />
<meta property="og:locale" content="zh-CN" /><meta property="og:image" content="https://jiajiewu.gitee.io/icons/apple-touch-icon.png" />
    <meta property="og:type" content="website" />
        <meta name="google-site-verification" content="cjNXc2AEYk3vl2-qiFXeVz-0jFUbTm5BiOPMiNROc2U" />
        




    
    <script>
        window.ga=window.ga||function(){(ga.q=ga.q||[]).push(arguments)};ga.l=+new Date;
        ga('create', 'UA-139409990-1', 'auto');
        ga('send', 'pageview');
    </script>
    <script async src='https://www.google-analytics.com/analytics.js'></script>
    


    
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/aplayer/dist/APlayer.min.css">
<script src="https://cdn.jsdelivr.net/npm/aplayer/dist/APlayer.min.js"></script>

<script src="https://cdn.jsdelivr.net/npm/meting@2/dist/Meting.min.js"></script>





</head>

    <body>
        <div class="container">
            
    <header class="header">
        <div class="site-brand">
            
            <a href="/" class="brand">jiajie</a>
            
        </div>
    </header>

            
    <nav class="nav">
        <ul class="menu" id="menu">
            
                
            
            
            
        </ul>
    </nav>

            
            
    
        
            
        
        <div id="theme-toggle" onclick="modeSwitcher()">🌞</div>
    

            
    
    
        <main class="home">
    <div class="poetry">
        
            <p>我无限的热爱着新的一日</p>
        
            <p>今天的太阳 今天的马 今天的花楸树</p>
        
            <p>使我健康 富足 拥有一生</p>
        
            <p>从黎明到黄昏</p>
        
            <p>阳光充足</p>
        
            <p>胜过一切过去的诗</p>
        
    </div>
    <div class="links">
        <a href="/post/tech/" class="links-item"><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" class="icon "><path d="M512 256c0 141.2-114.7 256-256 256C114.8 512 0 397.3 0 256S114.7 0 256 0s256 114.7 256 256zm-32 0c0-123.2-100.3-224-224-224C132.5 32 32 132.5 32 256s100.5 224 224 224 224-100.5 224-224zM160.9 124.6l86.9 37.1-37.1 86.9-86.9-37.1 37.1-86.9zm110 169.1l46.6 94h-14.6l-50-100-48.9 100h-14l51.1-106.9-22.3-9.4 6-14 68.6 29.1-6 14.3-16.5-7.1zm-11.8-116.3l68.6 29.4-29.4 68.3L230 246l29.1-68.6zm80.3 42.9l54.6 23.1-23.4 54.3-54.3-23.1 23.1-54.3z"/></svg>tech</a>
        <a href="/post/life/" class="links-item"><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" class="icon "><path d="M497.9 142.1l-46.1 46.1c-4.7 4.7-12.3 4.7-17 0l-111-111c-4.7-4.7-4.7-12.3 0-17l46.1-46.1c18.7-18.7 49.1-18.7 67.9 0l60.1 60.1c18.8 18.7 18.8 49.1 0 67.9zM284.2 99.8L21.6 362.4.4 483.9c-2.9 16.4 11.4 30.6 27.8 27.8l121.5-21.3 262.6-262.6c4.7-4.7 4.7-12.3 0-17l-111-111c-4.8-4.7-12.4-4.7-17.1 0zM124.1 339.9c-5.5-5.5-5.5-14.3 0-19.8l154-154c5.5-5.5 14.3-5.5 19.8 0s5.5 14.3 0 19.8l-154 154c-5.5 5.5-14.3 5.5-19.8 0zM88 424h48v36.3l-64.5 11.3-31.1-31.1L51.7 376H88v48z"/></svg>life</a>
        <a href="/categories/" class="links-item"><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" class="icon "><path d="M464 128H272l-54.63-54.63c-6-6-14.14-9.37-22.63-9.37H48C21.49 64 0 85.49 0 112v288c0 26.51 21.49 48 48 48h416c26.51 0 48-21.49 48-48V176c0-26.51-21.49-48-48-48zm0 272H48V112h140.12l54.63 54.63c6 6 14.14 9.37 22.63 9.37H464v224z"/></svg>article</a>
        <a href="/about/" class="links-item"><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" class="icon "><path d="M256 8C119 8 8 119 8 256s111 248 248 248 248-111 248-248S393 8 256 8zm144 276c0 6.6-5.4 12-12 12h-92v92c0 6.6-5.4 12-12 12h-56c-6.6 0-12-5.4-12-12v-92h-92c-6.6 0-12-5.4-12-12v-56c0-6.6 5.4-12 12-12h92v-92c0-6.6 5.4-12 12-12h56c6.6 0 12 5.4 12 12v92h92c6.6 0 12 5.4 12 12v56z"/></svg>more</a>
        
    </div>
</main>
    
    
    
    
    
    
    

            
    <a href="#" class="back-to-top"><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512" class="icon"><path d="M34.9 289.5l-22.2-22.2c-9.4-9.4-9.4-24.6 0-33.9L207 39c9.4-9.4 24.6-9.4 33.9 0l194.3 194.3c9.4 9.4 9.4 24.6 0 33.9L413 289.4c-9.5 9.5-25 9.3-34.3-.4L264 168.6V456c0 13.3-10.7 24-24 24h-32c-13.3 0-24-10.7-24-24V168.6L69.2 289.1c-9.3 9.8-24.8 10-34.3.4z"/></svg></a>

            
        </div>
        <script src="/js/meme.min.535088d2894d2a0bfac5b83091fb5a73d17ef26116dd4ef1d9cca5fc40d02120.js" integrity="sha256-U1CI0olNKgv6xbgwkftac9F+8mEW3U7x2cyl/EDQISA=" data-no-instant></script>


    <script data-no-instant>InstantClick.init();</script>


    <script data-no-instant>
        InstantClick.on('change', function () {
            const theme = localStorage.getItem('theme');
            if (theme === "dark") {
                goDarkMeta();
                goDark();
            } else if (theme === "light") {
                goLightMeta();
                goLight();
            }
        });
    </script>
<script data-no-instant>
            InstantClick.on('change', function () {
                ga('send', 'pageview', location.pathname + location.search);
            });
        </script>
    
    
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/katex@0.11.0/dist/katex.min.css" integrity="sha384-BdGj8xC2eZkQaxoQ8nSLefg4AV4/AwB3Fj+8SUSo7pnKP6Eoy18liIKTPn9oBYNG" crossorigin="anonymous" />
<script>
    if (typeof renderMathInElement === 'undefined') {
        var getScript = (options) => {
            var script = document.createElement('script');
            script.defer = true;
            script.crossOrigin = 'anonymous';
            script['data-no-instant'] = true;
            Object.keys(options).forEach((key) => {
                script[key] = options[key];
            });
            document.body.appendChild(script);
        };
        getScript({
            src: 'https://cdn.jsdelivr.net/npm/katex@0.11.0/dist/katex.min.js',
            integrity: 'sha384-JiKN5O8x9Hhs/UE5cT5AAJqieYlOZbGT3CHws/y97o3ty4R7/O5poG9F3JoiOYw1',
            onload: () => {
                getScript({
                    src: 'https://cdn.jsdelivr.net/npm/katex@0.11.0/dist/contrib/mhchem.min.js',
                    integrity: 'sha384-oa0lfxCGjaU1LdYckhq8LZcP+JTf8cyJXe69O6VE6UrShzWveT6KiCElJrck/stm',
                    onload: () => {
                        getScript({
                            src: 'https://cdn.jsdelivr.net/npm/katex@0.11.0/dist/contrib/auto-render.min.js',
                            integrity: 'sha384-kWPLUVMOks5AQFrykwIup5lo0m3iMkkHrD0uJ4H5cjeGihAutqP0yW0J6dpFiVkI',
                            onload: () => {
                                renderMathInElement(
                                    document.body,
                                    {
                                        delimiters: [
                                            {left: "$$", right: "$$", display: true},
                                            {left: "\\[", right: "\\]", display: true},
                                            {left: "$", right: "$", display: false},
                                            {left: "\\(", right: "\\)", display: false}
                                        ]
                                    }
                                );
                            }
                        });
                    }
                });
            }
        });
    } else {
        renderMathInElement(
            document.body,
            {
                delimiters: [
                    {left: "$$", right: "$$", display: true},
                    {left: "\\[", right: "\\]", display: true},
                    {left: "$", right: "$", display: false},
                    {left: "\\(", right: "\\)", display: false}
                ]
            }
        );
    }
</script>





    






    
        <script async src="https://busuanzi.ibruce.info/busuanzi/2.3/busuanzi.pure.mini.js"></script>
    



    </body>
</html>

## Welcome to ZhuZifa's Pages

<table border="0">
  <tr>
    <td width="75%">
      <h1>朱自发</h1>
      <p><b>博士研究生</b></p>
      <p><b>中国科学院光电技术研究所</b></p>
      <p><b>邮箱：zhuzifa123@126.com</b></p>
      <p><b>地址：四川省成都市双流区光电大道光电技术研究所</b></p>
      <p><a href="/index-en.html">English Version</a></p>
    </td>
    <td width="25%">
      <img src="/profile picture.jpg" width="115%">
    </td>
  </tr>
</table>

---

张三，男，个人简介个人简介个人简介个人简介个人简介个人简介个人简介个人简介个人简介个人简介个人简介个人简介个人简介个人简介个人简介个人简介个人简介个人简介个人简介个人简介个人简介个人简介个人简介个人简介

---

### 最新消息
1. 消息1×××

### 研究方向
- 文本挖掘
- 知识图谱

### 荣誉奖励
- 奖学金
- 荣誉称号
- 比赛获奖

### 项目研究
#### 公司/学校/研究所（2013.9~2017.6）
- **项目1**  
项目描述
- **项目2**  
项目描述

#### 公司/学校/研究所（2017.9~至今）
- **项目1**  
项目描述
- **项目2**  
项目描述
