<!DOCTYPE html>
<!-- saved from url=(0037)http://www.jianshu.com/p/6b18b1ad08af -->
<html><!--<![endif]--><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
  
  <meta http-equiv="X-UA-Compatible" content="IE=Edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0,user-scalable=no">

  <!-- Start of Baidu Transcode -->
  <meta http-equiv="Cache-Control" content="no-siteapp">
  <meta http-equiv="Cache-Control" content="no-transform">
  <meta name="applicable-device" content="pc,mobile">
  <meta name="MobileOptimized" content="width">
  <meta name="HandheldFriendly" content="true">
  <meta name="mobile-agent" content="format=html5;url=http://www.jianshu.com/p/6b18b1ad08af">
  <!-- End of Baidu Transcode -->

    <meta name="description" content="1vim 1.1vim基本概念 命令行模式使用vim+文件名，进入时处于命令行模式，该模式下可以控制屏幕光标的移动，字符、字、行的删除。 插入模式在命令行模式下输入【i】,切换到插入模式，点击【Esc】再次回到命令行模式。该模式下仅可以插入数据。 底行模式对文件进行保存、退出、重命名等操作，在命令行模式下，输入【：】进入底行模式。 1.2vim各个模式下的功能键 命令行模式进入插入模式【i】...">

  <meta name="360-site-verification" content="604a14b53c6b871206001285921e81d8">
  <meta property="wb:webmaster" content="294ec9de89e7fadb">
  <meta property="qc:admins" content="104102651453316562112116375">
  <meta property="qc:admins" content="11635613706305617">
  <meta property="qc:admins" content="1163561616621163056375">
  <meta name="google-site-verification" content="cV4-qkUJZR6gmFeajx_UyPe47GW9vY6cnCrYtCHYNh4">
  <meta name="google-site-verification" content="HF7lfF8YEGs1qtCE-kPml8Z469e2RHhGajy6JPVy5XI">
  <meta http-equiv="mobile-agent" content="format=html5; url=http://www.jianshu.com/p/6b18b1ad08af">

  <!-- Apple -->
  <meta name="apple-mobile-web-app-title" content="简书">

    <!--  Meta for Smart App Banner -->
  <meta name="apple-itunes-app" content="app-id=888237539, app-argument=jianshu://notes/14404544">
  <!-- End -->

  <!--  Meta for Twitter Card -->
  <meta content="summary" property="twitter:card">
  <meta content="@jianshucom" property="twitter:site">
  <meta content="vim使用介绍" property="twitter:title">
  <meta content="1vim 1.1vim基本概念 命令行模式使用vim+文件名，进入时处于命令行模式，该模式下可以控制屏幕光标的移动，字符、字、行的删除。 插入模式在命令行模式下输入【i】,切换到插入模式，点击【Esc】再次回到命令行模式。该模式下仅可以插入数据。 底行模式对文件进行保存、退出、重命名等操作，在命令行模式下，输入【：】进入底行模式。 1.2vim各个模式下的功能键 命令行模式进入插入模式【i】- 进入插入模式，光标从点前位置插入；【o】- 进入插入模式，当前行下新建一行，将光标移动到新建行的行首进行插入。【a】- 进入插入模式，光标当前位置向后一个字符进行插入。进入底行模式【：】- 进入底..." property="twitter:description">
  <meta content="http://www.jianshu.com/p/6b18b1ad08af" property="twitter:url">
  <!-- End -->

  <!--  Meta for OpenGraph -->
  <meta property="fb:app_id" content="865829053512461">
  <meta property="og:site_name" content="简书">
  <meta property="og:title" content="vim使用介绍">
  <meta property="og:type" content="article">
  <meta property="og:url" content="http://www.jianshu.com/p/6b18b1ad08af">
  <meta property="og:description" content="1vim 1.1vim基本概念 命令行模式使用vim+文件名，进入时处于命令行模式，该模式下可以控制屏幕光标的移动，字符、字、行的删除。 插入模式在命令行模式下输入【i】,切换到插入模式，点击【...">
  <!-- End -->

  <!--  Meta for Facebook Applinks -->
  <meta property="al:ios:url" content="jianshu://notes/14404544">
  <meta property="al:ios:app_store_id" content="888237539">
  <meta property="al:ios:app_name" content="简书">

  <meta property="al:android:url" content="jianshu://notes/14404544">
  <meta property="al:android:package" content="com.jianshu.haruki">
  <meta property="al:android:app_name" content="简书">
  <!-- End -->


    <title>vim使用介绍 - 简书</title>

  <meta name="csrf-param" content="authenticity_token">
<meta name="csrf-token" content="yYPPXTVWftOi0wf49zMrXvmH19s7JM6bb7Wvp81AB4zNHpEIRxQ9kbngmYAPru8ZEeU+D6+0LWGkh6L5QSp4aQ==">

  <link rel="stylesheet" media="all" href="./vim使用介绍 - 简书_files/web-5bf8d755f816e9590279.css">
  
  <link rel="stylesheet" media="all" href="./vim使用介绍 - 简书_files/entry-5bf8d755f816e9590279.css">

  <link href="http://cdn2.jianshu.io/assets/favicons/favicon-783beb88ed621ceab614de960376ac0c.ico" rel="icon">
      <link rel="apple-touch-icon-precomposed" href="http://cdn2.jianshu.io/assets/apple-touch-icons/57-47624b2e2161e8eb144462c85db0a5ff.png" sizes="57x57">
      <link rel="apple-touch-icon-precomposed" href="http://cdn2.jianshu.io/assets/apple-touch-icons/72-c00cde7cf98fc49e50cbb3ee1dcd5804.png" sizes="72x72">
      <link rel="apple-touch-icon-precomposed" href="http://cdn2.jianshu.io/assets/apple-touch-icons/76-e8af0bdeaf1ba31e303b1fde8b5e66c4.png" sizes="76x76">
      <link rel="apple-touch-icon-precomposed" href="http://cdn2.jianshu.io/assets/apple-touch-icons/114-f4c78569bbf1977e8382a5fd90c9237a.png" sizes="114x114">
      <link rel="apple-touch-icon-precomposed" href="http://cdn2.jianshu.io/assets/apple-touch-icons/120-cf10c3711dba269522743729efe66bbc.png" sizes="120x120">
      <link rel="apple-touch-icon-precomposed" href="http://cdn2.jianshu.io/assets/apple-touch-icons/152-7bd60457b5f3ecbf1343f0e6241be4f8.png" sizes="152x152">
<link rel="stylesheet" href="blob:http://www.jianshu.com/17eb4c59-09f0-410a-b3c9-dc4805b3e05e"><link rel="stylesheet" href="blob:http://www.jianshu.com/6369bbad-3d68-4ab6-b9ae-a5a06f1ecc48"></head>

  <body lang="zh-CN" class="reader-black-font">
    <!-- 全局顶部导航栏 -->
<nav class="navbar navbar-default navbar-fixed-top" role="navigation">
  <div class="width-limit">
    <!-- 左上方 Logo -->
    <a class="logo" href="http://www.jianshu.com/"><img src="./vim使用介绍 - 简书_files/logo-58fd04f6f0de908401aa561cda6a0688.png" alt="Logo"></a>

    <!-- 右上角 -->
      <!-- 登录显示写文章 -->
      <a class="btn write-btn" target="_blank" href="http://www.jianshu.com/writer#/">
        <i class="iconfont ic-write"></i>写文章
</a>
    <!-- 如果用户登录，显示下拉菜单 -->
      <div class="user">
        <div data-hover="dropdown">
          <a class="avatar" href="http://www.jianshu.com/u/e3fc527be9e0"><img src="./vim使用介绍 - 简书_files/15-a7ac401939dd4df837e3bbf82abaa2a8.jpg" alt="120"></a>
        </div>
        <ul class="dropdown-menu">
          <li>
            <a href="http://www.jianshu.com/u/e3fc527be9e0">
              <i class="iconfont ic-navigation-profile"></i><span>我的主页</span>
</a>          </li>
          <li>
            <!-- TODO bookmarks_path -->
            <a href="http://www.jianshu.com/bookmarks">
              <i class="iconfont ic-navigation-mark"></i><span>收藏的文章</span>
</a>          </li>
          <li>
            <a href="http://www.jianshu.com/users/e3fc527be9e0/liked_notes">
              <i class="iconfont ic-navigation-like"></i><span>喜欢的文章</span>
</a>          </li>
          <li>
            <a href="http://www.jianshu.com/wallet">
              <i class="iconfont ic-navigation-wallet"></i><span>我的钱包</span>
</a>          </li>
          <li>
            <a href="http://www.jianshu.com/settings">
              <i class="iconfont ic-navigation-settings"></i><span>设置</span>
</a>          </li>
          <li>
            <a href="http://www.jianshu.com/faqs">
              <i class="iconfont ic-navigation-feedback"></i><span>帮助与反馈</span>
</a>          </li>
          <li>
            <a rel="nofollow" data-method="delete" href="http://www.jianshu.com/sign_out">
              <i class="iconfont ic-navigation-signout"></i><span>退出</span>
</a>          </li>
        </ul>
      </div>

    <div class="style-mode"><a class="style-mode-btn"><i class="iconfont ic-navigation-mode"></i></a> <div class="popover-modal" style="left: 0px; display: none;"><div class="meta"><i class="iconfont ic-navigation-night"></i><span>夜间模式</span></div> <div class="switch day-night-group"><a class="switch-btn">开</a> <a class="switch-btn active">关</a></div> <hr> <div class="switch font-family-group"><a class="switch-btn font-song">宋体</a> <a class="switch-btn font-hei active">黑体</a></div> <div class="switch"><a class="switch-btn active">简</a> <a class="switch-btn">繁</a></div></div></div>
    <div class="container">
      <div class="navbar-header">
        <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#menu" aria-expanded="false">
          <span class="icon-bar"></span>
          <span class="icon-bar"></span>
          <span class="icon-bar"></span>
        </button>
      </div>
      <div class="collapse navbar-collapse" id="menu">
        <ul class="nav navbar-nav">
            <li class="">
              <a href="http://www.jianshu.com/">
                <span class="menu-text">发现</span><i class="iconfont ic-navigation-discover menu-icon"></i>
</a>            </li>
            <li class="">
              <a href="http://www.jianshu.com/subscriptions">
                <span class="menu-text">关注</span><i class="iconfont ic-navigation-follow menu-icon"></i>
</a>            </li>
            <li class="notification"><a data-hover="dropdown" href="http://www.jianshu.com/notifications" class="notification-btn"><span class="menu-text">消息</span> <i class="iconfont ic-navigation-notification menu-icon"></i> <!----> <!----></a> <ul class="dropdown-menu"><li><a href="http://www.jianshu.com/notifications#/comments"><i class="iconfont ic-comments"></i> <span>评论</span> <!----></a></li><li><a href="http://www.jianshu.com/notifications#/chats"><i class="iconfont ic-chats"></i> <span>简信</span> <!----></a></li><li><a href="http://www.jianshu.com/notifications#/requests"><i class="iconfont ic-requests"></i> <span>投稿请求</span> <!----></a></li><li><a href="http://www.jianshu.com/notifications#/likes"><i class="iconfont ic-likes"></i> <span>喜欢和赞</span> <!----></a></li><li><a href="http://www.jianshu.com/notifications#/follows"><i class="iconfont ic-follows"></i> <span>关注</span> <!----></a></li><li><a href="http://www.jianshu.com/notifications#/money"><i class="iconfont ic-money"></i> <span>赞赏</span> <!----></a></li><li><a href="http://www.jianshu.com/notifications#/others"><i class="iconfont ic-others"></i> <span>其他消息</span> <!----></a></li></ul></li>
          <li class="search">
            <form target="_blank" action="http://www.jianshu.com/search" accept-charset="UTF-8" method="get"><input name="utf8" type="hidden" value="✓">
              <input type="text" name="q" id="q" value="" placeholder="搜索" class="search-input">
              <a class="search-btn" href="javascript:void(null)"><i class="iconfont ic-search"></i></a>
              <!-- <div id="navbar-trending-search"></div> -->
</form>          </li>
        </ul>
      </div>
    </div>
  </div>
</nav>

    
<div class="note">
  <div class="post">
    <div class="article">
        <h1 class="title">vim使用介绍</h1>

        <!-- 作者区域 -->
        <div class="author">
          <a class="avatar" href="http://www.jianshu.com/u/e3fc527be9e0">
            <img src="./vim使用介绍 - 简书_files/15-a7ac401939dd4df837e3bbf82abaa2a8(1).jpg" alt="144">
</a>          <div class="info">
            <span class="tag">作者</span>
            <span class="name"><a href="http://www.jianshu.com/u/e3fc527be9e0">IsGirl</a></span>
            <!-- 关注用户按钮 -->
            <div data-author-follow-button=""></div>
            <!-- 文章数据信息 -->
            <div class="meta">
              <!-- 如果文章更新时间大于发布时间，那么使用 tooltip 显示更新时间 -->
                <span class="publish-time">2017.07.10 17:59</span>
              <span class="wordage">字数 810</span>
            <span class="views-count">阅读 0</span><span class="comments-count">评论 0</span><span class="likes-count">喜欢 0</span></div>
          </div>
          <!-- 如果是当前作者，加入编辑按钮 -->
        <a href="http://www.jianshu.com/writer#/notebooks/13343224/notes/14404544" target="_blank" class="edit">编辑文章</a></div>
        <!-- -->

        <!-- 文章内容 -->
        <div class="show-content">
          <hr>
<h1>1vim</h1>
<h2>1.1vim基本概念</h2>
<ul>
<li>命令行模式<br>使用vim+文件名，进入时处于命令行模式，该模式下可以控制屏幕光标的移动，字符、字、行的删除。</li>
<li>插入模式<br>在命令行模式下输入【i】,切换到插入模式，点击【Esc】再次回到命令行模式。该模式下仅可以插入数据。</li>
<li>底行模式<br>对文件进行保存、退出、重命名等操作，在命令行模式下，输入【：】进入底行模式。</li>
</ul>
<h2>1.2vim各个模式下的功能键</h2>
<ul>
<li>命令行模式<ol>
<li>进入插入模式<br>【i】- 进入插入模式，光标从点前位置插入；<br>【o】- 进入插入模式，当前行下新建一行，将光标移动到新建行的行首进行插入。<br>【a】- 进入插入模式，光标当前位置向后一个字符进行插入。</li>
<li>进入底行模式<br>【：】- 进入底行模式</li>
<li>文本操作键<br>【h】- 光标左移<br>【j】- 光标下移<br>【k】- 光标上移<br>【l】- 光标右移<br>【0】- 光标移动到文件首部（Linux）<br>【G】- 光标移动到文件尾部（Linux）<br>【^】- 光标移动到所在行的首部<br>【Home】- 光标移动到所在行的首部（Windows下git）<br>【End】或【$】- 光标移动到所在行最后一个字符的前一个位置（Windows下git）<br>【x】- 删除光标向后的一个字符<br>【n+x】- 删除光标向后的n个字符 eg:6x<br>【X】- 删除光标向前的一个字符<br>【n+X】- 删除光标向前的n个字符<br>【dd】- 删除光标所在行整行<br>【n+dd】- 删除所在行向下包括本行,共n(表示数字)行，eg:3dd表示删除所在行一下包括本行共3行。<br>【yw】- 赋值光标到所在行的行尾到缓冲区<br>【yy】- 赋值光标所在行整行到缓冲区<br>【nyy】- 赋值光标所在行包括本行共n行到缓冲区<br>【r】- 替换光标所在处字符。先按下r再按下希望替换的字符<br>【R】- 替换光标所到之处的字符一直向后替换，直到按下「ESC」键为止。<br>【u】- 恢复上次操作<br>【cw】- 改变光标到行位的内容<br>【cnw】- 改变光标所在行包括所在行向下共n行的内容 eg:c3w</li>
</ol>
</li>
</ul>
<ul>
<li>
<p>插入模式<br>【Esc】- 切换到命令行模式</p>
</li>
<li>
<p>底行模式<br>【set mu】- 显示文件中所有行的行号<br>【n】- n代表数字，调到n行<br>【/+目前关键词】- 查找目标关键词 eg: /k 在文件寻找k,按n知道找到k继续按n寻找下一个，从前向后找<br>【？+目标关键词】- 查找关键词同上，区别：从后向前找<br>【w】- 保存当前文件<br>【q】- 退出vim编辑<br>【q!】- 不保存修改强制退出</p>
</li>
</ul>
<hr>

        </div>
        <!--  -->

        <div class="show-foot">
          <a class="notebook" href="http://www.jianshu.com/nb/13343224">
            <i class="iconfont ic-search-notebook"></i> <span>随笔</span>
</a>          <div class="copyright" data-toggle="tooltip" data-html="true" data-original-title="转载请联系作者获得授权，并标注“简书作者”。">
            © 著作权归作者所有
          </div>
          
        </div>
    </div>

    <!-- 文章底部作者信息 -->
      <div class="follow-detail">
        <div class="info">
          <a class="avatar" href="http://www.jianshu.com/u/e3fc527be9e0">
            <img src="./vim使用介绍 - 简书_files/15-a7ac401939dd4df837e3bbf82abaa2a8(1).jpg" alt="144">
</a>          <div data-author-follow-button=""></div>
          <a class="title" href="http://www.jianshu.com/u/e3fc527be9e0">IsGirl</a>
        <p>写了 810 字，被 0 人关注，获得了 0 个喜欢</p></div>
      </div>

      <div class="support-author"></div>

    <div class="meta-bottom">
      <div class="like"><div class="btn like-group"><div class="btn-like"><a><i class="iconfont ic-like"></i>喜欢</a></div> <div class="modal-wrap"><a>0</a></div></div> <!----></div>
      <div class="share-group">
        <a class="share-circle" data-action="weixin-share" data-toggle="tooltip" data-original-title="分享到微信">
          <i class="iconfont ic-wechat"></i>
        </a>
        <a class="share-circle" data-toggle="tooltip" href="javascript:void((function(s,d,e,r,l,p,t,z,c){var%20f=&#39;http://v.t.sina.com.cn/share/share.php?appkey=1881139527&#39;,u=z||d.location,p=[&#39;&amp;url=&#39;,e(u),&#39;&amp;title=&#39;,e(t||d.title),&#39;&amp;source=&#39;,e(r),&#39;&amp;sourceUrl=&#39;,e(l),&#39;&amp;content=&#39;,c||&#39;gb2312&#39;,&#39;&amp;pic=&#39;,e(p||&#39;&#39;)].join(&#39;&#39;);function%20a(){if(!window.open([f,p].join(&#39;&#39;),&#39;mb&#39;,[&#39;toolbar=0,status=0,resizable=1,width=440,height=430,left=&#39;,(s.width-440)/2,&#39;,top=&#39;,(s.height-430)/2].join(&#39;&#39;)))u.href=[f,p].join(&#39;&#39;);};if(/Firefox/.test(navigator.userAgent))setTimeout(a,0);else%20a();})(screen,document,encodeURIComponent,&#39;&#39;,&#39;&#39;,&#39;http://cwb.assets.jianshu.io/notes/images/14404544/weibo/image_2c5c297a47ff.jpg&#39;, &#39;我写了新文章《vim使用介绍》（ 分享自 @简书 ）&#39;,&#39;http://www.jianshu.com/p/6b18b1ad08af?utm_campaign=maleskine&amp;utm_content=note&amp;utm_medium=reader_share&amp;utm_source=weibo&#39;,&#39;页面编码gb2312|utf-8默认gb2312&#39;));" data-original-title="分享到微博">
          <i class="iconfont ic-weibo"></i>
        </a>
          <a class="share-circle" data-toggle="tooltip" href="http://cwb.assets.jianshu.io/notes/images/14404544/weibo/image_2c5c297a47ff.jpg" target="_blank" data-original-title="下载长微博图片">
            <i class="iconfont ic-picture"></i>
          </a>
        <a class="share-circle more-share" tabindex="0" data-toggle="popover" data-placement="top" data-html="true" data-trigger="focus" href="javascript:void(0);" data-content="
          &lt;ul class=&quot;share-list&quot;&gt;
            &lt;li&gt;&lt;a href=&quot;javascript:void(function(){var d=document,e=encodeURIComponent,r=&#39;http://sns.qzone.qq.com/cgi-bin/qzshare/cgi_qzshare_onekey?url=&#39;+e(&#39;http://www.jianshu.com/p/6b18b1ad08af?utm_campaign=maleskine&amp;utm_content=note&amp;utm_medium=reader_share&amp;utm_source=qzone&#39;)+&#39;&amp;title=&#39;+e(&#39;我写了新文章《vim使用介绍》&#39;),x=function(){if(!window.open(r,&#39;qzone&#39;,&#39;toolbar=0,resizable=1,scrollbars=yes,status=1,width=600,height=600&#39;))location.href=r};if(/Firefox/.test(navigator.userAgent)){setTimeout(x,0)}else{x()}})();&quot;&gt;&lt;i class=&quot;social-icon-sprite social-icon-zone&quot;&gt;&lt;/i&gt;&lt;span&gt;分享到QQ空间&lt;/span&gt;&lt;/a&gt;&lt;/li&gt;
            &lt;li&gt;&lt;a href=&quot;javascript:void(function(){var d=document,e=encodeURIComponent,r=&#39;https://twitter.com/share?url=&#39;+e(&#39;http://www.jianshu.com/p/6b18b1ad08af?utm_campaign=maleskine&amp;utm_content=note&amp;utm_medium=reader_share&amp;utm_source=twitter&#39;)+&#39;&amp;text=&#39;+e(&#39;我写了新文章《vim使用介绍》（ 分享自 @jianshucom ）&#39;)+&#39;&amp;related=&#39;+e(&#39;jianshucom&#39;),x=function(){if(!window.open(r,&#39;twitter&#39;,&#39;toolbar=0,resizable=1,scrollbars=yes,status=1,width=600,height=600&#39;))location.href=r};if(/Firefox/.test(navigator.userAgent)){setTimeout(x,0)}else{x()}})();&quot;&gt;&lt;i class=&quot;social-icon-sprite social-icon-twitter&quot;&gt;&lt;/i&gt;&lt;span&gt;分享到Twitter&lt;/span&gt;&lt;/a&gt;&lt;/li&gt;
            &lt;li&gt;&lt;a href=&quot;javascript:void(function(){var d=document,e=encodeURIComponent,r=&#39;https://www.facebook.com/dialog/share?app_id=483126645039390&amp;display=popup&amp;href=http://www.jianshu.com/p/6b18b1ad08af?utm_campaign=maleskine&amp;utm_content=note&amp;utm_medium=reader_share&amp;utm_source=facebook&#39;,x=function(){if(!window.open(r,&#39;facebook&#39;,&#39;toolbar=0,resizable=1,scrollbars=yes,status=1,width=450,height=330&#39;))location.href=r};if(/Firefox/.test(navigator.userAgent)){setTimeout(x,0)}else{x()}})();&quot;&gt;&lt;i class=&quot;social-icon-sprite social-icon-facebook&quot;&gt;&lt;/i&gt;&lt;span&gt;分享到Facebook&lt;/span&gt;&lt;/a&gt;&lt;/li&gt;
            &lt;li&gt;&lt;a href=&quot;javascript:void(function(){var d=document,e=encodeURIComponent,r=&#39;https://plus.google.com/share?url=&#39;+e(&#39;http://www.jianshu.com/p/6b18b1ad08af?utm_campaign=maleskine&amp;utm_content=note&amp;utm_medium=reader_share&amp;utm_source=google_plus&#39;),x=function(){if(!window.open(r,&#39;google_plus&#39;,&#39;toolbar=0,resizable=1,scrollbars=yes,status=1,width=450,height=330&#39;))location.href=r};if(/Firefox/.test(navigator.userAgent)){setTimeout(x,0)}else{x()}})();&quot;&gt;&lt;i class=&quot;social-icon-sprite social-icon-google&quot;&gt;&lt;/i&gt;&lt;span&gt;分享到Google+&lt;/span&gt;&lt;/a&gt;&lt;/li&gt;
            &lt;li&gt;&lt;a href=&quot;javascript:void(function(){var d=document,e=encodeURIComponent,s1=window.getSelection,s2=d.getSelection,s3=d.selection,s=s1?s1():s2?s2():s3?s3.createRange().text:&#39;&#39;,r=&#39;http://www.douban.com/recommend/?url=&#39;+e(&#39;http://www.jianshu.com/p/6b18b1ad08af?utm_campaign=maleskine&amp;utm_content=note&amp;utm_medium=reader_share&amp;utm_source=douban&#39;)+&#39;&amp;title=&#39;+e(&#39;vim使用介绍&#39;)+&#39;&amp;sel=&#39;+e(s)+&#39;&amp;v=1&#39;,x=function(){if(!window.open(r,&#39;douban&#39;,&#39;toolbar=0,resizable=1,scrollbars=yes,status=1,width=450,height=330&#39;))location.href=r+&#39;&amp;r=1&#39;};if(/Firefox/.test(navigator.userAgent)){setTimeout(x,0)}else{x()}})()&quot;&gt;&lt;i class=&quot;social-icon-sprite social-icon-douban&quot;&gt;&lt;/i&gt;&lt;span&gt;分享到豆瓣&lt;/span&gt;&lt;/a&gt;&lt;/li&gt;
          &lt;/ul&gt;
        " data-original-title="" title="">更多分享</a>
      </div>
    </div>
    <div id="vue_comment"></div>
  </div>

  <div class="side-tool"><ul><li data-placement="left" data-toggle="tooltip" data-container="body" data-original-title="回到顶部" style="display: none;"><a class="function-button"><i class="iconfont ic-backtop"></i></a></li> <li data-placement="left" data-toggle="tooltip" data-container="body" data-original-title="文章投稿"><a class="js-submit-button"><i class="iconfont ic-note-requests"></i></a> <!----></li> <li data-placement="left" data-toggle="tooltip" data-container="body" data-original-title="收藏文章"><a class="function-button"><i class="iconfont ic-mark"></i></a></li> <li data-placement="left" data-toggle="tooltip" data-container="body" data-original-title="分享文章"><a tabindex="0" role="button" data-toggle="popover" data-placement="left" data-html="true" data-trigger="focus" href="javascript:void(0);" data-content="&lt;ul class=&#39;share-list&#39;&gt;
                &lt;li&gt;&lt;a class=&quot;weixin-share&quot;&gt;&lt;i class=&quot;social-icon-sprite social-icon-weixin&quot;&gt;&lt;/i&gt;&lt;span&gt;分享到微信&lt;/span&gt;&lt;/a&gt;&lt;/li&gt;
                &lt;li&gt;&lt;a href=&quot;javascript:void((function(s,d,e,r,l,p,t,z,c){var%20f=&#39;http://v.t.sina.com.cn/share/share.php?appkey=1881139527&#39;,u=z||d.location,p=[&#39;&amp;url=&#39;,e(u),&#39;&amp;title=&#39;,e(t||d.title),&#39;&amp;source=&#39;,e(r),&#39;&amp;sourceUrl=&#39;,e(l),&#39;&amp;content=&#39;,c||&#39;gb2312&#39;,&#39;&amp;pic=&#39;,e(p||&#39;&#39;)].join(&#39;&#39;);function%20a(){if(!window.open([f,p].join(&#39;&#39;),&#39;mb&#39;,[&#39;toolbar=0,status=0,resizable=1,width=440,height=430,left=&#39;,(s.width-440)/2,&#39;,top=&#39;,(s.height-430)/2].join(&#39;&#39;)))u.href=[f,p].join(&#39;&#39;);};if(/Firefox/.test(navigator.userAgent))setTimeout(a,0);else%20a();})(screen,document,encodeURIComponent,&#39;&#39;,&#39;&#39;,&#39;http://cwb.assets.jianshu.io/notes/images/14404544/weibo/image_2c5c297a47ff.jpg&#39;, &#39;我写了新文章《vim使用介绍》（ 分享自 @简书 ）&#39;,&#39;http://www.jianshu.com/p/6b18b1ad08af?utm_campaign=maleskine&amp;utm_content=note&amp;utm_medium=reader_share&amp;utm_source=weibo&#39;,&#39;页面编码gb2312|utf-8默认gb2312&#39;));&quot;&gt;&lt;i class=&#39;social-icon-sprite social-icon-weibo&#39;&gt;&lt;/i&gt;&lt;span&gt;分享到微博&lt;/span&gt;&lt;/a&gt;&lt;/li&gt;
                &lt;li&gt;&lt;a href=&quot;http://cwb.assets.jianshu.io/notes/images/14404544/weibo/image_2c5c297a47ff.jpg&quot; target=&quot;_blank&quot;&gt;&lt;i class=&quot;social-icon-sprite social-icon-picture&quot;&gt;&lt;/i&gt;&lt;span&gt;下载长微博图片&lt;/span&gt;&lt;/a&gt;&lt;/li&gt;
                &lt;li&gt;&lt;a href=&quot;javascript:void(function(){var d=document,e=encodeURIComponent,r=&#39;http://sns.qzone.qq.com/cgi-bin/qzshare/cgi_qzshare_onekey?url=&#39;+e(&#39;http://www.jianshu.com/p/6b18b1ad08af?utm_campaign=maleskine&amp;utm_content=note&amp;utm_medium=reader_share&amp;utm_source=qzone&#39;)+&#39;&amp;title=&#39;+e(&#39;我写了新文章《vim使用介绍》&#39;),x=function(){if(!window.open(r,&#39;qzone&#39;,&#39;toolbar=0,resizable=1,scrollbars=yes,status=1,width=600,height=600&#39;))location.href=r};if(/Firefox/.test(navigator.userAgent)){setTimeout(x,0)}else{x()}})();&quot;&gt;&lt;i class=&#39;social-icon-sprite social-icon-zone&#39;&gt;&lt;/i&gt;&lt;span&gt;分享到QQ空间&lt;/span&gt;&lt;/a&gt;&lt;/li&gt;
                &lt;li&gt;&lt;a href=&quot;javascript:void(function(){var d=document,e=encodeURIComponent,r=&#39;https://twitter.com/share?url=&#39;+e(&#39;http://www.jianshu.com/p/6b18b1ad08af?utm_campaign=maleskine&amp;utm_content=note&amp;utm_medium=reader_share&amp;utm_source=twitter&#39;)+&#39;&amp;text=&#39;+e(&#39;我写了新文章《vim使用介绍》（ 分享自 @jianshucom ）&#39;)+&#39;&amp;related=&#39;+e(&#39;jianshucom&#39;),x=function(){if(!window.open(r,&#39;twitter&#39;,&#39;toolbar=0,resizable=1,scrollbars=yes,status=1,width=600,height=600&#39;))location.href=r};if(/Firefox/.test(navigator.userAgent)){setTimeout(x,0)}else{x()}})();&quot;&gt;&lt;i class=&#39;social-icon-sprite social-icon-twitter&#39;&gt;&lt;/i&gt;&lt;span&gt;分享到Twitter&lt;/span&gt;&lt;/a&gt;&lt;/li&gt;
                &lt;li&gt;&lt;a href=&quot;javascript:void(function(){var d=document,e=encodeURIComponent,r=&#39;https://www.facebook.com/dialog/share?app_id=483126645039390&amp;display=popup&amp;href=http://www.jianshu.com/p/6b18b1ad08af?utm_campaign=maleskine&amp;utm_content=note&amp;utm_medium=reader_share&amp;utm_source=facebook&#39;,x=function(){if(!window.open(r,&#39;facebook&#39;,&#39;toolbar=0,resizable=1,scrollbars=yes,status=1,width=450,height=330&#39;))location.href=r};if(/Firefox/.test(navigator.userAgent)){setTimeout(x,0)}else{x()}})();&quot;&gt;&lt;i class=&#39;social-icon-sprite social-icon-facebook&#39;&gt;&lt;/i&gt;&lt;span&gt;分享到Facebook&lt;/span&gt;&lt;/a&gt;&lt;/li&gt;
                &lt;li&gt;&lt;a href=&quot;javascript:void(function(){var d=document,e=encodeURIComponent,r=&#39;https://plus.google.com/share?url=&#39;+e(&#39;http://www.jianshu.com/p/6b18b1ad08af?utm_campaign=maleskine&amp;utm_content=note&amp;utm_medium=reader_share&amp;utm_source=google_plus&#39;),x=function(){if(!window.open(r,&#39;google_plus&#39;,&#39;toolbar=0,resizable=1,scrollbars=yes,status=1,width=450,height=330&#39;))location.href=r};if(/Firefox/.test(navigator.userAgent)){setTimeout(x,0)}else{x()}})();&quot;&gt;&lt;i class=&#39;social-icon-sprite social-icon-google&#39;&gt;&lt;/i&gt;&lt;span&gt;分享到Google+&lt;/span&gt;&lt;/a&gt;&lt;/li&gt;
                &lt;li&gt;&lt;a href=&quot;javascript:void(function(){var d=document,e=encodeURIComponent,s1=window.getSelection,s2=d.getSelection,s3=d.selection,s=s1?s1():s2?s2():s3?s3.createRange().text:&#39;&#39;,r=&#39;http://www.douban.com/recommend/?url=&#39;+e(&#39;http://www.jianshu.com/p/6b18b1ad08af?utm_campaign=maleskine&amp;utm_content=note&amp;utm_medium=reader_share&amp;utm_source=douban&#39;)+&#39;&amp;title=&#39;+e(&#39;vim使用介绍&#39;)+&#39;&amp;sel=&#39;+e(s)+&#39;&amp;v=1&#39;,x=function(){if(!window.open(r,&#39;douban&#39;,&#39;toolbar=0,resizable=1,scrollbars=yes,status=1,width=450,height=330&#39;))location.href=r+&#39;&amp;r=1&#39;};if(/Firefox/.test(navigator.userAgent)){setTimeout(x,0)}else{x()}})()&quot;&gt;&lt;i class=&#39;social-icon-sprite social-icon-douban&#39;&gt;&lt;/i&gt;&lt;span&gt;分享到豆瓣&lt;/span&gt;&lt;/a&gt;&lt;/li&gt;
              &lt;/ul&gt;" data-original-title="" title="" class="function-button"><i class="iconfont ic-share"></i></a> <!----></li></ul></div>
</div>
<div class="note-bottom">
  <div><div class="main"><div class="title">被以下专题收入，发现更多相似内容</div> <a class="collection-settings"><i class="iconfont ic-settings-account"></i><span>投稿管理</span></a> <div class="include-collection"><div class="modal-wrap add-collection-wrap"><a class="add-collection"><i class="iconfont ic-follow"></i>收入我的专题</a></div>  <!----></div></div> <!----> <!----></div>
  <div data-vcomp="recommended-notes" data-note-id="14404544"></div>
</div>

    <script src="./vim使用介绍 - 简书_files/push.js.下载"></script><script src="./vim使用介绍 - 简书_files/hm.js.下载"></script><script async="" src="./vim使用介绍 - 简书_files/analytics.js.下载"></script><script type="application/json" data-name="page-data">{"user_signed_in":true,"locale":"zh-CN","os":"windows","read_mode":"day","read_font":"font2","current_user":{"id":6408556,"nickname":"IsGirl","slug":"e3fc527be9e0","avatar":"http://cdn2.jianshu.io/assets/default_avatar/15-a7ac401939dd4df837e3bbf82abaa2a8.jpg","unread_counts":{"chats":0,"total":0},"has_editable_collection":false},"note_show":{"is_author":true,"is_following_author":false,"is_liked_note":false,"uuid":"d20e167d-84dd-4cb0-a305-0ffbd51a9798"},"note":{"id":14404544,"slug":"6b18b1ad08af","user_id":6408556,"notebook_id":13343224,"commentable":true,"likes_count":0,"views_count":0,"public_wordage":810,"comments_count":0,"author":{"total_wordage":810,"followers_count":0,"total_likes_count":0}}}</script>
    
    <script src="./vim使用介绍 - 简书_files/babel-polyfill-2f826c52f92197490a6c.js.下载"></script>
    <script src="./vim使用介绍 - 简书_files/web-base-5bf8d755f816e9590279.js.下载"></script>
<script src="./vim使用介绍 - 简书_files/web-32581b5ffc42ba6430ad.js.下载"></script>
    
    <script src="./vim使用介绍 - 简书_files/entry-dc1a2aa60bcfbd75ce19.js.下载"></script>
    <script>
  (function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;i[r]=i[r]||function(){
  (i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o),
  m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;m.parentNode.insertBefore(a,m)
  })(window,document,'script','https://www.google-analytics.com/analytics.js','ga');

  ga('create', 'UA-35169517-1', 'auto');
  ga('send', 'pageview');
</script>

<script>
  var _hmt = _hmt || [];
  (function() {
    var hm = document.createElement("script");
    hm.src = "//hm.baidu.com/hm.js?0c0e9d9b1e7d617b3e6842e85b9fb068";
    var s = document.getElementsByTagName("script")[0];
    s.parentNode.insertBefore(hm, s);
  })();
</script>

<script>
  (function(){
      var bp = document.createElement('script');
      var curProtocol = window.location.protocol.split(':')[0];
      if (curProtocol === 'https') {
          bp.src = 'https://zz.bdstatic.com/linksubmit/push.js';
      }
      else {
          bp.src = 'http://push.zhanzhang.baidu.com/push.js';
      }
      var s = document.getElementsByTagName("script")[0];
      s.parentNode.insertBefore(bp, s);
  })();
</script>

  

<!----></body></html>