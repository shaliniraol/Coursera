


<!DOCTYPE html>
<html lang="en" class="">
  <head prefix="og: http://ogp.me/ns# fb: http://ogp.me/ns/fb# object: http://ogp.me/ns/object# article: http://ogp.me/ns/article# profile: http://ogp.me/ns/profile#">
    <meta charset='utf-8'>
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta http-equiv="Content-Language" content="en">
    
    
    <title>GettingAndCleaningData/run_analysis.Rmd at master · benjamin-chan/GettingAndCleaningData · GitHub</title>
    <link rel="search" type="application/opensearchdescription+xml" href="/opensearch.xml" title="GitHub">
    <link rel="fluid-icon" href="https://github.com/fluidicon.png" title="GitHub">
    <link rel="apple-touch-icon" sizes="57x57" href="/apple-touch-icon-114.png">
    <link rel="apple-touch-icon" sizes="114x114" href="/apple-touch-icon-114.png">
    <link rel="apple-touch-icon" sizes="72x72" href="/apple-touch-icon-144.png">
    <link rel="apple-touch-icon" sizes="144x144" href="/apple-touch-icon-144.png">
    <meta property="fb:app_id" content="1401488693436528">

      <meta content="@github" name="twitter:site" /><meta content="summary" name="twitter:card" /><meta content="benjamin-chan/GettingAndCleaningData" name="twitter:title" /><meta content="Contribute to GettingAndCleaningData development by creating an account on GitHub." name="twitter:description" /><meta content="https://avatars1.githubusercontent.com/u/1897044?v=3&amp;s=400" name="twitter:image:src" />
      <meta content="GitHub" property="og:site_name" /><meta content="object" property="og:type" /><meta content="https://avatars1.githubusercontent.com/u/1897044?v=3&amp;s=400" property="og:image" /><meta content="benjamin-chan/GettingAndCleaningData" property="og:title" /><meta content="https://github.com/benjamin-chan/GettingAndCleaningData" property="og:url" /><meta content="Contribute to GettingAndCleaningData development by creating an account on GitHub." property="og:description" />
      <meta name="browser-stats-url" content="https://api.github.com/_private/browser/stats">
    <meta name="browser-errors-url" content="https://api.github.com/_private/browser/errors">
    <link rel="assets" href="https://assets-cdn.github.com/">
    
    <meta name="pjax-timeout" content="1000">
    

    <meta name="msapplication-TileImage" content="/windows-tile.png">
    <meta name="msapplication-TileColor" content="#ffffff">
    <meta name="selected-link" value="repo_source" data-pjax-transient>
      <meta name="google-analytics" content="UA-3769691-2">

    <meta content="collector.githubapp.com" name="octolytics-host" /><meta content="collector-cdn.github.com" name="octolytics-script-host" /><meta content="github" name="octolytics-app-id" /><meta content="C0373626:5678:B0F7FE0:553D6D10" name="octolytics-dimension-request_id" />
    
    <meta content="Rails, view, blob#show" name="analytics-event" />
    <meta class="js-ga-set" name="dimension1" content="Logged Out">
    <meta class="js-ga-set" name="dimension2" content="Header v3">
    <meta name="is-dotcom" content="true">
    <meta name="hostname" content="github.com">
    <meta name="user-login" content="">

    
    <link rel="icon" type="image/x-icon" href="https://assets-cdn.github.com/favicon.ico">


    <meta content="authenticity_token" name="csrf-param" />
<meta content="7RtPvAI1c4ZZORhpeaeyoWA04TTCeZyYPKGZnJgXMglxCSOpclbRtkrW24WGgWUciEdU5dvet1vl96ZvWKEZSw==" name="csrf-token" />

    <link href="https://assets-cdn.github.com/assets/github-99a212f30ce9bafd05712fa4c5c5de4e89c6c27396c34f6458dea3ea2a0b05b0.css" media="all" rel="stylesheet" />
    <link href="https://assets-cdn.github.com/assets/github2-b21c331cc5a9542882fc1f4e2cf08c371d7e52473ffc1017b2b64e3eccc953b8.css" media="all" rel="stylesheet" />
    
    


    <meta http-equiv="x-pjax-version" content="380e0b7c2b581631835a2841991e7107">

      
  <meta name="description" content="Contribute to GettingAndCleaningData development by creating an account on GitHub.">
  <meta name="go-import" content="github.com/benjamin-chan/GettingAndCleaningData git https://github.com/benjamin-chan/GettingAndCleaningData.git">

  <meta content="1897044" name="octolytics-dimension-user_id" /><meta content="benjamin-chan" name="octolytics-dimension-user_login" /><meta content="18577753" name="octolytics-dimension-repository_id" /><meta content="benjamin-chan/GettingAndCleaningData" name="octolytics-dimension-repository_nwo" /><meta content="true" name="octolytics-dimension-repository_public" /><meta content="false" name="octolytics-dimension-repository_is_fork" /><meta content="18577753" name="octolytics-dimension-repository_network_root_id" /><meta content="benjamin-chan/GettingAndCleaningData" name="octolytics-dimension-repository_network_root_nwo" />
  <link href="https://github.com/benjamin-chan/GettingAndCleaningData/commits/master.atom" rel="alternate" title="Recent Commits to GettingAndCleaningData:master" type="application/atom+xml">

  </head>


  <body class="logged_out  env-production windows vis-public page-blob">
    <a href="#start-of-content" tabindex="1" class="accessibility-aid js-skip-to-content">Skip to content</a>
    <div class="wrapper">
      
      
      


        
        <div class="header header-logged-out" role="banner">
  <div class="container clearfix">

    <a class="header-logo-wordmark" href="https://github.com/" data-ga-click="(Logged out) Header, go to homepage, icon:logo-wordmark">
      <span class="mega-octicon octicon-logo-github"></span>
    </a>

    <div class="header-actions" role="navigation">
        <a class="btn btn-primary" href="/join" data-ga-click="(Logged out) Header, clicked Sign up, text:sign-up">Sign up</a>
      <a class="btn" href="/login?return_to=%2Fbenjamin-chan%2FGettingAndCleaningData%2Fblob%2Fmaster%2FProject%2Frun_analysis.Rmd" data-ga-click="(Logged out) Header, clicked Sign in, text:sign-in">Sign in</a>
    </div>

    <div class="site-search repo-scope js-site-search" role="search">
      <form accept-charset="UTF-8" action="/benjamin-chan/GettingAndCleaningData/search" class="js-site-search-form" data-global-search-url="/search" data-repo-search-url="/benjamin-chan/GettingAndCleaningData/search" method="get"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /></div>
  <input type="text"
    class="js-site-search-field is-clearable"
    data-hotkey="s"
    name="q"
    placeholder="Search"
    data-global-scope-placeholder="Search GitHub"
    data-repo-scope-placeholder="Search"
    tabindex="1"
    autocapitalize="off">
  <div class="scope-badge">This repository</div>
</form>
    </div>

      <ul class="header-nav left" role="navigation">
          <li class="header-nav-item">
            <a class="header-nav-link" href="/explore" data-ga-click="(Logged out) Header, go to explore, text:explore">Explore</a>
          </li>
          <li class="header-nav-item">
            <a class="header-nav-link" href="/features" data-ga-click="(Logged out) Header, go to features, text:features">Features</a>
          </li>
          <li class="header-nav-item">
            <a class="header-nav-link" href="https://enterprise.github.com/" data-ga-click="(Logged out) Header, go to enterprise, text:enterprise">Enterprise</a>
          </li>
          <li class="header-nav-item">
            <a class="header-nav-link" href="/blog" data-ga-click="(Logged out) Header, go to blog, text:blog">Blog</a>
          </li>
      </ul>

  </div>
</div>



      <div id="start-of-content" class="accessibility-aid"></div>
          <div class="site" itemscope itemtype="http://schema.org/WebPage">
    <div id="js-flash-container">
      
    </div>
    <div class="pagehead repohead instapaper_ignore readability-menu">
      <div class="container">
        
<ul class="pagehead-actions">

  <li>
      <a href="/login?return_to=%2Fbenjamin-chan%2FGettingAndCleaningData"
    class="btn btn-sm btn-with-count tooltipped tooltipped-n"
    aria-label="You must be signed in to watch a repository" rel="nofollow">
    <span class="octicon octicon-eye"></span>
    Watch
  </a>
  <a class="social-count" href="/benjamin-chan/GettingAndCleaningData/watchers">
    10
  </a>

  </li>

  <li>
      <a href="/login?return_to=%2Fbenjamin-chan%2FGettingAndCleaningData"
    class="btn btn-sm btn-with-count tooltipped tooltipped-n"
    aria-label="You must be signed in to star a repository" rel="nofollow">
    <span class="octicon octicon-star"></span>
    Star
  </a>

    <a class="social-count js-social-count" href="/benjamin-chan/GettingAndCleaningData/stargazers">
      22
    </a>

  </li>

    <li>
      <a href="/login?return_to=%2Fbenjamin-chan%2FGettingAndCleaningData"
        class="btn btn-sm btn-with-count tooltipped tooltipped-n"
        aria-label="You must be signed in to fork a repository" rel="nofollow">
        <span class="octicon octicon-repo-forked"></span>
        Fork
      </a>
      <a href="/benjamin-chan/GettingAndCleaningData/network" class="social-count">
        136
      </a>
    </li>
</ul>

        <h1 itemscope itemtype="http://data-vocabulary.org/Breadcrumb" class="entry-title public">
          <span class="mega-octicon octicon-repo"></span>
          <span class="author"><a href="/benjamin-chan" class="url fn" itemprop="url" rel="author"><span itemprop="title">benjamin-chan</span></a></span><!--
       --><span class="path-divider">/</span><!--
       --><strong><a href="/benjamin-chan/GettingAndCleaningData" class="js-current-repository" data-pjax="#js-repo-pjax-container">GettingAndCleaningData</a></strong>

          <span class="page-context-loader">
            <img alt="" height="16" src="https://assets-cdn.github.com/assets/spinners/octocat-spinner-32-e513294efa576953719e4e2de888dd9cf929b7d62ed8d05f25e731d02452ab6c.gif" width="16" />
          </span>

        </h1>
      </div><!-- /.container -->
    </div><!-- /.repohead -->

    <div class="container">
      <div class="repository-with-sidebar repo-container new-discussion-timeline  ">
        <div class="repository-sidebar clearfix">
            
<nav class="sunken-menu repo-nav js-repo-nav js-sidenav-container-pjax js-octicon-loaders"
     role="navigation"
     data-pjax="#js-repo-pjax-container"
     data-issue-count-url="/benjamin-chan/GettingAndCleaningData/issues/counts">
  <ul class="sunken-menu-group">
    <li class="tooltipped tooltipped-w" aria-label="Code">
      <a href="/benjamin-chan/GettingAndCleaningData" aria-label="Code" class="selected js-selected-navigation-item sunken-menu-item" data-hotkey="g c" data-selected-links="repo_source repo_downloads repo_commits repo_releases repo_tags repo_branches /benjamin-chan/GettingAndCleaningData">
        <span class="octicon octicon-code"></span> <span class="full-word">Code</span>
        <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/assets/spinners/octocat-spinner-32-e513294efa576953719e4e2de888dd9cf929b7d62ed8d05f25e731d02452ab6c.gif" width="16" />
</a>    </li>

      <li class="tooltipped tooltipped-w" aria-label="Issues">
        <a href="/benjamin-chan/GettingAndCleaningData/issues" aria-label="Issues" class="js-selected-navigation-item sunken-menu-item" data-hotkey="g i" data-selected-links="repo_issues repo_labels repo_milestones /benjamin-chan/GettingAndCleaningData/issues">
          <span class="octicon octicon-issue-opened"></span> <span class="full-word">Issues</span>
          <span class="js-issue-replace-counter"></span>
          <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/assets/spinners/octocat-spinner-32-e513294efa576953719e4e2de888dd9cf929b7d62ed8d05f25e731d02452ab6c.gif" width="16" />
</a>      </li>

    <li class="tooltipped tooltipped-w" aria-label="Pull requests">
      <a href="/benjamin-chan/GettingAndCleaningData/pulls" aria-label="Pull requests" class="js-selected-navigation-item sunken-menu-item" data-hotkey="g p" data-selected-links="repo_pulls /benjamin-chan/GettingAndCleaningData/pulls">
          <span class="octicon octicon-git-pull-request"></span> <span class="full-word">Pull requests</span>
          <span class="js-pull-replace-counter"></span>
          <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/assets/spinners/octocat-spinner-32-e513294efa576953719e4e2de888dd9cf929b7d62ed8d05f25e731d02452ab6c.gif" width="16" />
</a>    </li>

  </ul>
  <div class="sunken-menu-separator"></div>
  <ul class="sunken-menu-group">

    <li class="tooltipped tooltipped-w" aria-label="Pulse">
      <a href="/benjamin-chan/GettingAndCleaningData/pulse" aria-label="Pulse" class="js-selected-navigation-item sunken-menu-item" data-selected-links="pulse /benjamin-chan/GettingAndCleaningData/pulse">
        <span class="octicon octicon-pulse"></span> <span class="full-word">Pulse</span>
        <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/assets/spinners/octocat-spinner-32-e513294efa576953719e4e2de888dd9cf929b7d62ed8d05f25e731d02452ab6c.gif" width="16" />
</a>    </li>

    <li class="tooltipped tooltipped-w" aria-label="Graphs">
      <a href="/benjamin-chan/GettingAndCleaningData/graphs" aria-label="Graphs" class="js-selected-navigation-item sunken-menu-item" data-selected-links="repo_graphs repo_contributors /benjamin-chan/GettingAndCleaningData/graphs">
        <span class="octicon octicon-graph"></span> <span class="full-word">Graphs</span>
        <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/assets/spinners/octocat-spinner-32-e513294efa576953719e4e2de888dd9cf929b7d62ed8d05f25e731d02452ab6c.gif" width="16" />
</a>    </li>
  </ul>


</nav>

              <div class="only-with-full-nav">
                  
<div class="clone-url open"
  data-protocol-type="http"
  data-url="/users/set_protocol?protocol_selector=http&amp;protocol_type=clone">
  <h3><span class="text-emphasized">HTTPS</span> clone URL</h3>
  <div class="input-group js-zeroclipboard-container">
    <input type="text" class="input-mini input-monospace js-url-field js-zeroclipboard-target"
           value="https://github.com/benjamin-chan/GettingAndCleaningData.git" readonly="readonly">
    <span class="input-group-button">
      <button aria-label="Copy to clipboard" class="js-zeroclipboard btn btn-sm zeroclipboard-button tooltipped tooltipped-s" data-copied-hint="Copied!" type="button"><span class="octicon octicon-clippy"></span></button>
    </span>
  </div>
</div>

  
<div class="clone-url "
  data-protocol-type="subversion"
  data-url="/users/set_protocol?protocol_selector=subversion&amp;protocol_type=clone">
  <h3><span class="text-emphasized">Subversion</span> checkout URL</h3>
  <div class="input-group js-zeroclipboard-container">
    <input type="text" class="input-mini input-monospace js-url-field js-zeroclipboard-target"
           value="https://github.com/benjamin-chan/GettingAndCleaningData" readonly="readonly">
    <span class="input-group-button">
      <button aria-label="Copy to clipboard" class="js-zeroclipboard btn btn-sm zeroclipboard-button tooltipped tooltipped-s" data-copied-hint="Copied!" type="button"><span class="octicon octicon-clippy"></span></button>
    </span>
  </div>
</div>



<p class="clone-options">You can clone with
  <a href="#" class="js-clone-selector" data-protocol="http">HTTPS</a> or <a href="#" class="js-clone-selector" data-protocol="subversion">Subversion</a>.
  <a href="https://help.github.com/articles/which-remote-url-should-i-use" class="help tooltipped tooltipped-n" aria-label="Get help on which URL is right for you.">
    <span class="octicon octicon-question"></span>
  </a>
</p>


  <a href="https://windows.github.com" class="btn btn-sm sidebar-button" title="Save benjamin-chan/GettingAndCleaningData to your computer and use it in GitHub Desktop." aria-label="Save benjamin-chan/GettingAndCleaningData to your computer and use it in GitHub Desktop.">
    <span class="octicon octicon-device-desktop"></span>
    Clone in Desktop
  </a>


                <a href="/benjamin-chan/GettingAndCleaningData/archive/master.zip"
                   class="btn btn-sm sidebar-button"
                   aria-label="Download the contents of benjamin-chan/GettingAndCleaningData as a zip file"
                   title="Download the contents of benjamin-chan/GettingAndCleaningData as a zip file"
                   rel="nofollow">
                  <span class="octicon octicon-cloud-download"></span>
                  Download ZIP
                </a>
              </div>
        </div><!-- /.repository-sidebar -->

        <div id="js-repo-pjax-container" class="repository-content context-loader-container" data-pjax-container>
          

<a href="/benjamin-chan/GettingAndCleaningData/blob/eb401a34579a545bc64fedd8d410bdf8ecb6f992/Project/run_analysis.Rmd" class="hidden js-permalink-shortcut" data-hotkey="y">Permalink</a>

<!-- blob contrib key: blob_contributors:v21:dc9eeb95f9f93a2f5aa9f22b9c797c16 -->

<div class="file-navigation js-zeroclipboard-container">
  
<div class="select-menu js-menu-container js-select-menu left">
  <span class="btn btn-sm select-menu-button js-menu-target css-truncate" data-hotkey="w"
    data-master-branch="master"
    data-ref="master"
    title="master"
    role="button" aria-label="Switch branches or tags" tabindex="0" aria-haspopup="true">
    <span class="octicon octicon-git-branch"></span>
    <i>branch:</i>
    <span class="js-select-button css-truncate-target">master</span>
  </span>

  <div class="select-menu-modal-holder js-menu-content js-navigation-container" data-pjax aria-hidden="true">

    <div class="select-menu-modal">
      <div class="select-menu-header">
        <span class="select-menu-title">Switch branches/tags</span>
        <span class="octicon octicon-x js-menu-close" role="button" aria-label="Close"></span>
      </div>

      <div class="select-menu-filters">
        <div class="select-menu-text-filter">
          <input type="text" aria-label="Filter branches/tags" id="context-commitish-filter-field" class="js-filterable-field js-navigation-enable" placeholder="Filter branches/tags">
        </div>
        <div class="select-menu-tabs">
          <ul>
            <li class="select-menu-tab">
              <a href="#" data-tab-filter="branches" data-filter-placeholder="Filter branches/tags" class="js-select-menu-tab">Branches</a>
            </li>
            <li class="select-menu-tab">
              <a href="#" data-tab-filter="tags" data-filter-placeholder="Find a tag…" class="js-select-menu-tab">Tags</a>
            </li>
          </ul>
        </div>
      </div>

      <div class="select-menu-list select-menu-tab-bucket js-select-menu-tab-bucket" data-tab-filter="branches">

        <div data-filterable-for="context-commitish-filter-field" data-filterable-type="substring">


            <a class="select-menu-item js-navigation-item js-navigation-open selected"
               href="/benjamin-chan/GettingAndCleaningData/blob/master/Project/run_analysis.Rmd"
               data-name="master"
               data-skip-pjax="true"
               rel="nofollow">
              <span class="select-menu-item-icon octicon octicon-check"></span>
              <span class="select-menu-item-text css-truncate-target" title="master">
                master
              </span>
            </a>
        </div>

          <div class="select-menu-no-results">Nothing to show</div>
      </div>

      <div class="select-menu-list select-menu-tab-bucket js-select-menu-tab-bucket" data-tab-filter="tags">
        <div data-filterable-for="context-commitish-filter-field" data-filterable-type="substring">


        </div>

        <div class="select-menu-no-results">Nothing to show</div>
      </div>

    </div>
  </div>
</div>

  <div class="btn-group right">
    <a href="/benjamin-chan/GettingAndCleaningData/find/master"
          class="js-show-file-finder btn btn-sm empty-icon tooltipped tooltipped-s"
          data-pjax
          data-hotkey="t"
          aria-label="Quickly jump between files">
      <span class="octicon octicon-list-unordered"></span>
    </a>
    <button aria-label="Copy file path to clipboard" class="js-zeroclipboard btn btn-sm zeroclipboard-button tooltipped tooltipped-s" data-copied-hint="Copied!" type="button"><span class="octicon octicon-clippy"></span></button>
  </div>

  <div class="breadcrumb js-zeroclipboard-target">
    <span class='repo-root js-repo-root'><span itemscope="" itemtype="http://data-vocabulary.org/Breadcrumb"><a href="/benjamin-chan/GettingAndCleaningData" class="" data-branch="master" data-direction="back" data-pjax="true" itemscope="url"><span itemprop="title">GettingAndCleaningData</span></a></span></span><span class="separator">/</span><span itemscope="" itemtype="http://data-vocabulary.org/Breadcrumb"><a href="/benjamin-chan/GettingAndCleaningData/tree/master/Project" class="" data-branch="master" data-direction="back" data-pjax="true" itemscope="url"><span itemprop="title">Project</span></a></span><span class="separator">/</span><strong class="final-path">run_analysis.Rmd</strong>
  </div>
</div>


  <div class="commit file-history-tease">
    <div class="file-history-tease-header">
        <img alt="" class="avatar" height="24" src="https://0.gravatar.com/avatar/fccfd78eb90b1591caaa7f6f01bd0fcd?d=https%3A%2F%2Fassets-cdn.github.com%2Fimages%2Fgravatars%2Fgravatar-user-420.png&amp;r=x&amp;s=140" width="24" />
        <span class="author"><span>Benjamin Chan</span></span>
        <time datetime="2014-04-17T16:10:14Z" is="relative-time">Apr 17, 2014</time>
        <div class="commit-title">
            <a href="/benjamin-chan/GettingAndCleaningData/commit/73f0abb7e5bd770a824ee189e21830c7485c5f1a" class="message" data-pjax="true" title="Add codebook.html">Add codebook.html</a>
        </div>
    </div>

    <div class="participation">
      <p class="quickstat">
        <a href="#blob_contributors_box" rel="facebox">
          <strong>1</strong>
           contributor
        </a>
      </p>
      
    </div>
    <div id="blob_contributors_box" style="display:none">
      <h2 class="facebox-header">Users who have contributed to this file</h2>
      <ul class="facebox-user-list">
          <li class="facebox-user-list-item">
            <img alt="@benjamin-chan" data-user="1897044" height="24" src="https://avatars3.githubusercontent.com/u/1897044?v=3&amp;s=48" width="24" />
            <a href="/benjamin-chan">benjamin-chan</a>
          </li>
      </ul>
    </div>
  </div>

<div class="file">
  <div class="file-header">
    <div class="file-actions">

      <div class="btn-group">
        <a href="/benjamin-chan/GettingAndCleaningData/raw/master/Project/run_analysis.Rmd" class="btn btn-sm " id="raw-url">Raw</a>
          <a href="/benjamin-chan/GettingAndCleaningData/blame/master/Project/run_analysis.Rmd" class="btn btn-sm js-update-url-with-hash">Blame</a>
        <a href="/benjamin-chan/GettingAndCleaningData/commits/master/Project/run_analysis.Rmd" class="btn btn-sm " rel="nofollow">History</a>
      </div>

        <a class="octicon-btn tooltipped tooltipped-nw"
           href="https://windows.github.com"
           aria-label="Open this file in GitHub for Windows">
            <span class="octicon octicon-device-desktop"></span>
        </a>

          <button type="button" class="octicon-btn disabled tooltipped tooltipped-n" aria-label="You must be signed in to make or propose changes">
            <span class="octicon octicon-pencil"></span>
          </button>

        <button type="button" class="octicon-btn octicon-btn-danger disabled tooltipped tooltipped-n" aria-label="You must be signed in to make or propose changes">
          <span class="octicon octicon-trashcan"></span>
        </button>
    </div>

    <div class="file-info">
        272 lines (197 sloc)
        <span class="file-info-divider"></span>
      8.925 kb
    </div>
  </div>
    <div id="readme" class="blob instapaper_body">
    <article class="markdown-body entry-content" itemprop="mainContentOfPage"><h1>
<a id="user-content-run_analysis" class="anchor" href="#run_analysis" aria-hidden="true"><span class="octicon octicon-link"></span></a>run_analysis</h1>

<p>Last updated <code>r as.character(Sys.time())</code> using <code>r R.version$version.string</code>.</p>

<h2>
<a id="user-content-instructions-for-project" class="anchor" href="#instructions-for-project" aria-hidden="true"><span class="octicon octicon-link"></span></a>Instructions for project</h2>

<blockquote>
<p>The purpose of this project is to demonstrate your ability to collect, work with, and clean a data set. The goal is to prepare tidy data that can be used for later analysis. You will be graded by your peers on a series of yes/no questions related to the project. You will be required to submit: 1) a tidy data set as described below, 2) a link to a Github repository with your script for performing the analysis, and 3) a code book that describes the variables, the data, and any transformations or work that you performed to clean up the data called CodeBook.md. You should also include a README.md in the repo with your scripts. This repo explains how all of the scripts work and how they are connected.  </p>

<p>One of the most exciting areas in all of data science right now is wearable computing - see for example this article . Companies like Fitbit, Nike, and Jawbone Up are racing to develop the most advanced algorithms to attract new users. The data linked to from the course website represent data collected from the accelerometers from the Samsung Galaxy S smartphone. A full description is available at the site where the data was obtained: </p>

<p><a href="http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones">http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones</a> </p>

<p>Here are the data for the project: </p>

<p><a href="https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip">https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip</a> </p>

<p>You should create one R script called run_analysis.R that does the following. </p>

<ol>
<li>
<strong>DONE</strong> Merges the training and the test sets to create one data set.</li>
<li>
<strong>DONE</strong> Extracts only the measurements on the mean and standard deviation for each measurement.</li>
<li>
<strong>DONE</strong> Uses descriptive activity names to name the activities in the data set.</li>
<li>
<strong>DONE</strong> Appropriately labels the data set with descriptive activity names.</li>
<li>
<strong>DONE</strong> Creates a second, independent tidy data set with the average of each variable for each activity and each subject. </li>
</ol>

<p>Good luck!</p>
</blockquote>

<p><strong>The codebook is at the end of this document.</strong></p>

<h2>
<a id="user-content-preliminaries" class="anchor" href="#preliminaries" aria-hidden="true"><span class="octicon octicon-link"></span></a>Preliminaries</h2>

<p>Load packages.</p>

<div class="highlight highlight-r"><pre><span class="pl-smi">packages</span> <span class="pl-k">&lt;-</span> c(<span class="pl-s"><span class="pl-pds">"</span>data.table<span class="pl-pds">"</span></span>, <span class="pl-s"><span class="pl-pds">"</span>reshape2<span class="pl-pds">"</span></span>)
sapply(<span class="pl-smi">packages</span>, <span class="pl-smi">require</span>, <span class="pl-v">character.only</span><span class="pl-k">=</span><span class="pl-c1">TRUE</span>, <span class="pl-v">quietly</span><span class="pl-k">=</span><span class="pl-c1">TRUE</span>)</pre></div>

<p>Set path.</p>

<div class="highlight highlight-r"><pre><span class="pl-smi">path</span> <span class="pl-k">&lt;-</span> getwd()
<span class="pl-smi">path</span></pre></div>

<h2>
<a id="user-content-get-the-data" class="anchor" href="#get-the-data" aria-hidden="true"><span class="octicon octicon-link"></span></a>Get the data</h2>

<p>Download the file. Put it in the <code>Data</code> folder. <strong>This was already done on 2014-04-11; save time and don't evaluate again.</strong></p>

<pre lang="r,"><code>url &lt;- "https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip"
f &lt;- "Dataset.zip"
if (!file.exists(path)) {dir.create(path)}
download.file(url, file.path(path, f))
</code></pre>

<p>Unzip the file. <strong>This was already done on 2014-04-11; save time and don't evaluate again.</strong></p>

<pre lang="r,"><code>executable &lt;- file.path("C:", "Program Files (x86)", "7-Zip", "7z.exe")
parameters &lt;- "x"
cmd &lt;- paste(paste0("\"", executable, "\""), parameters, paste0("\"", file.path(path, f), "\""))
system(cmd)
</code></pre>

<p>The archive put the files in a folder named <code>UCI HAR Dataset</code>. Set this folder as the input path. List the files here.</p>

<div class="highlight highlight-r"><pre><span class="pl-smi">pathIn</span> <span class="pl-k">&lt;-</span> file.path(<span class="pl-smi">path</span>, <span class="pl-s"><span class="pl-pds">"</span>UCI HAR Dataset<span class="pl-pds">"</span></span>)
list.files(<span class="pl-smi">pathIn</span>, <span class="pl-v">recursive</span><span class="pl-k">=</span><span class="pl-c1">TRUE</span>)</pre></div>

<p><strong>See the <code>README.txt</code> file in <code>r path</code> for detailed information on the dataset.</strong></p>

<p>For the purposes of this project, the files in the <code>Inertial Signals</code> folders are not used.</p>

<h2>
<a id="user-content-read-the-files" class="anchor" href="#read-the-files" aria-hidden="true"><span class="octicon octicon-link"></span></a>Read the files</h2>

<p>Read the subject files.</p>

<div class="highlight highlight-r"><pre><span class="pl-smi">dtSubjectTrain</span> <span class="pl-k">&lt;-</span> fread(file.path(<span class="pl-smi">pathIn</span>, <span class="pl-s"><span class="pl-pds">"</span>train<span class="pl-pds">"</span></span>, <span class="pl-s"><span class="pl-pds">"</span>subject_train.txt<span class="pl-pds">"</span></span>))
<span class="pl-smi">dtSubjectTest</span>  <span class="pl-k">&lt;-</span> fread(file.path(<span class="pl-smi">pathIn</span>, <span class="pl-s"><span class="pl-pds">"</span>test<span class="pl-pds">"</span></span> , <span class="pl-s"><span class="pl-pds">"</span>subject_test.txt<span class="pl-pds">"</span></span> ))</pre></div>

<p>Read the activity files. For some reason, these are called <em>label</em> files in the <code>README.txt</code> documentation.</p>

<div class="highlight highlight-r"><pre><span class="pl-smi">dtActivityTrain</span> <span class="pl-k">&lt;-</span> fread(file.path(<span class="pl-smi">pathIn</span>, <span class="pl-s"><span class="pl-pds">"</span>train<span class="pl-pds">"</span></span>, <span class="pl-s"><span class="pl-pds">"</span>Y_train.txt<span class="pl-pds">"</span></span>))
<span class="pl-smi">dtActivityTest</span>  <span class="pl-k">&lt;-</span> fread(file.path(<span class="pl-smi">pathIn</span>, <span class="pl-s"><span class="pl-pds">"</span>test<span class="pl-pds">"</span></span> , <span class="pl-s"><span class="pl-pds">"</span>Y_test.txt<span class="pl-pds">"</span></span> ))</pre></div>

<p>Read the data files. <code>fread</code> seems to be giving me some trouble reading files. Using a helper function, read the file with <code>read.table</code> instead, then convert the resulting data frame to a data table. Return the data table.</p>

<div class="highlight highlight-r"><pre><span class="pl-en">fileToDataTable</span> <span class="pl-k">&lt;-</span> <span class="pl-k">function</span> (<span class="pl-smi">f</span>) {
    <span class="pl-smi">df</span> <span class="pl-k">&lt;-</span> read.table(<span class="pl-smi">f</span>)
    <span class="pl-smi">dt</span> <span class="pl-k">&lt;-</span> data.table(<span class="pl-smi">df</span>)
}
<span class="pl-smi">dtTrain</span> <span class="pl-k">&lt;-</span> fileToDataTable(file.path(<span class="pl-smi">pathIn</span>, <span class="pl-s"><span class="pl-pds">"</span>train<span class="pl-pds">"</span></span>, <span class="pl-s"><span class="pl-pds">"</span>X_train.txt<span class="pl-pds">"</span></span>))
<span class="pl-smi">dtTest</span>  <span class="pl-k">&lt;-</span> fileToDataTable(file.path(<span class="pl-smi">pathIn</span>, <span class="pl-s"><span class="pl-pds">"</span>test<span class="pl-pds">"</span></span> , <span class="pl-s"><span class="pl-pds">"</span>X_test.txt<span class="pl-pds">"</span></span> ))</pre></div>

<h2>
<a id="user-content-merge-the-training-and-the-test-sets" class="anchor" href="#merge-the-training-and-the-test-sets" aria-hidden="true"><span class="octicon octicon-link"></span></a>Merge the training and the test sets</h2>

<p>Concatenate the data tables.</p>

<div class="highlight highlight-r"><pre><span class="pl-smi">dtSubject</span> <span class="pl-k">&lt;-</span> rbind(<span class="pl-smi">dtSubjectTrain</span>, <span class="pl-smi">dtSubjectTest</span>)
setnames(<span class="pl-smi">dtSubject</span>, <span class="pl-s"><span class="pl-pds">"</span>V1<span class="pl-pds">"</span></span>, <span class="pl-s"><span class="pl-pds">"</span>subject<span class="pl-pds">"</span></span>)
<span class="pl-smi">dtActivity</span> <span class="pl-k">&lt;-</span> rbind(<span class="pl-smi">dtActivityTrain</span>, <span class="pl-smi">dtActivityTest</span>)
setnames(<span class="pl-smi">dtActivity</span>, <span class="pl-s"><span class="pl-pds">"</span>V1<span class="pl-pds">"</span></span>, <span class="pl-s"><span class="pl-pds">"</span>activityNum<span class="pl-pds">"</span></span>)
<span class="pl-smi">dt</span> <span class="pl-k">&lt;-</span> rbind(<span class="pl-smi">dtTrain</span>, <span class="pl-smi">dtTest</span>)</pre></div>

<p>Merge columns.</p>

<div class="highlight highlight-r"><pre><span class="pl-smi">dtSubject</span> <span class="pl-k">&lt;-</span> cbind(<span class="pl-smi">dtSubject</span>, <span class="pl-smi">dtActivity</span>)
<span class="pl-smi">dt</span> <span class="pl-k">&lt;-</span> cbind(<span class="pl-smi">dtSubject</span>, <span class="pl-smi">dt</span>)</pre></div>

<p>Set key.</p>

<div class="highlight highlight-r"><pre>setkey(<span class="pl-smi">dt</span>, <span class="pl-smi">subject</span>, <span class="pl-smi">activityNum</span>)</pre></div>

<h2>
<a id="user-content-extract-only-the-mean-and-standard-deviation" class="anchor" href="#extract-only-the-mean-and-standard-deviation" aria-hidden="true"><span class="octicon octicon-link"></span></a>Extract only the mean and standard deviation</h2>

<p>Read the <code>features.txt</code> file. This tells which variables in <code>dt</code> are measurements for the mean and standard deviation.</p>

<div class="highlight highlight-r"><pre><span class="pl-smi">dtFeatures</span> <span class="pl-k">&lt;-</span> fread(file.path(<span class="pl-smi">pathIn</span>, <span class="pl-s"><span class="pl-pds">"</span>features.txt<span class="pl-pds">"</span></span>))
setnames(<span class="pl-smi">dtFeatures</span>, names(<span class="pl-smi">dtFeatures</span>), c(<span class="pl-s"><span class="pl-pds">"</span>featureNum<span class="pl-pds">"</span></span>, <span class="pl-s"><span class="pl-pds">"</span>featureName<span class="pl-pds">"</span></span>))</pre></div>

<p>Subset only measurements for the mean and standard deviation.</p>

<div class="highlight highlight-r"><pre><span class="pl-smi">dtFeatures</span> <span class="pl-k">&lt;-</span> <span class="pl-smi">dtFeatures</span>[grepl(<span class="pl-s"><span class="pl-pds">"</span>mean<span class="pl-cce">\\</span>(<span class="pl-cce">\\</span>)|std<span class="pl-cce">\\</span>(<span class="pl-cce">\\</span>)<span class="pl-pds">"</span></span>, <span class="pl-smi">featureName</span>)]</pre></div>

<p>Convert the column numbers to a vector of variable names matching columns in <code>dt</code>.</p>

<div class="highlight highlight-r"><pre><span class="pl-smi">dtFeatures</span><span class="pl-k">$</span><span class="pl-smi">featureCode</span> <span class="pl-k">&lt;-</span> <span class="pl-smi">dtFeatures</span>[, paste0(<span class="pl-s"><span class="pl-pds">"</span>V<span class="pl-pds">"</span></span>, <span class="pl-smi">featureNum</span>)]
head(<span class="pl-smi">dtFeatures</span>)
<span class="pl-smi">dtFeatures</span><span class="pl-k">$</span><span class="pl-smi">featureCode</span></pre></div>

<p>Subset these variables using variable names.</p>

<div class="highlight highlight-r"><pre><span class="pl-smi">select</span> <span class="pl-k">&lt;-</span> c(key(<span class="pl-smi">dt</span>), <span class="pl-smi">dtFeatures</span><span class="pl-k">$</span><span class="pl-smi">featureCode</span>)
<span class="pl-smi">dt</span> <span class="pl-k">&lt;-</span> <span class="pl-smi">dt</span>[, <span class="pl-smi">select</span>, <span class="pl-v">with</span><span class="pl-k">=</span><span class="pl-c1">FALSE</span>]</pre></div>

<h2>
<a id="user-content-use-descriptive-activity-names" class="anchor" href="#use-descriptive-activity-names" aria-hidden="true"><span class="octicon octicon-link"></span></a>Use descriptive activity names</h2>

<p>Read <code>activity_labels.txt</code> file. This will be used to add descriptive names to the activities.</p>

<div class="highlight highlight-r"><pre><span class="pl-smi">dtActivityNames</span> <span class="pl-k">&lt;-</span> fread(file.path(<span class="pl-smi">pathIn</span>, <span class="pl-s"><span class="pl-pds">"</span>activity_labels.txt<span class="pl-pds">"</span></span>))
setnames(<span class="pl-smi">dtActivityNames</span>, names(<span class="pl-smi">dtActivityNames</span>), c(<span class="pl-s"><span class="pl-pds">"</span>activityNum<span class="pl-pds">"</span></span>, <span class="pl-s"><span class="pl-pds">"</span>activityName<span class="pl-pds">"</span></span>))</pre></div>

<h2>
<a id="user-content-label-with-descriptive-activity-names" class="anchor" href="#label-with-descriptive-activity-names" aria-hidden="true"><span class="octicon octicon-link"></span></a>Label with descriptive activity names</h2>

<p>Merge activity labels.</p>

<div class="highlight highlight-r"><pre><span class="pl-smi">dt</span> <span class="pl-k">&lt;-</span> merge(<span class="pl-smi">dt</span>, <span class="pl-smi">dtActivityNames</span>, <span class="pl-v">by</span><span class="pl-k">=</span><span class="pl-s"><span class="pl-pds">"</span>activityNum<span class="pl-pds">"</span></span>, <span class="pl-v">all.x</span><span class="pl-k">=</span><span class="pl-c1">TRUE</span>)</pre></div>

<p>Add <code>activityName</code> as a key.</p>

<div class="highlight highlight-r"><pre>setkey(<span class="pl-smi">dt</span>, <span class="pl-smi">subject</span>, <span class="pl-smi">activityNum</span>, <span class="pl-smi">activityName</span>)</pre></div>

<p>Melt the data table to reshape it from a short and wide format to a tall and narrow format.</p>

<div class="highlight highlight-r"><pre><span class="pl-smi">dt</span> <span class="pl-k">&lt;-</span> data.table(melt(<span class="pl-smi">dt</span>, key(<span class="pl-smi">dt</span>), <span class="pl-v">variable.name</span><span class="pl-k">=</span><span class="pl-s"><span class="pl-pds">"</span>featureCode<span class="pl-pds">"</span></span>))</pre></div>

<p>Merge activity name.</p>

<div class="highlight highlight-r"><pre><span class="pl-smi">dt</span> <span class="pl-k">&lt;-</span> merge(<span class="pl-smi">dt</span>, <span class="pl-smi">dtFeatures</span>[, <span class="pl-k">list</span>(<span class="pl-smi">featureNum</span>, <span class="pl-smi">featureCode</span>, <span class="pl-smi">featureName</span>)], <span class="pl-v">by</span><span class="pl-k">=</span><span class="pl-s"><span class="pl-pds">"</span>featureCode<span class="pl-pds">"</span></span>, <span class="pl-v">all.x</span><span class="pl-k">=</span><span class="pl-c1">TRUE</span>)</pre></div>

<p>Create a new variable, <code>activity</code> that is equivalent to <code>activityName</code> as a factor class.
Create a new variable, <code>feature</code> that is equivalent to <code>featureName</code> as a factor class.</p>

<div class="highlight highlight-r"><pre><span class="pl-smi">dt</span><span class="pl-k">$</span><span class="pl-smi">activity</span> <span class="pl-k">&lt;-</span> <span class="pl-k">factor</span>(<span class="pl-smi">dt</span><span class="pl-k">$</span><span class="pl-smi">activityName</span>)
<span class="pl-smi">dt</span><span class="pl-k">$</span><span class="pl-smi">feature</span> <span class="pl-k">&lt;-</span> <span class="pl-k">factor</span>(<span class="pl-smi">dt</span><span class="pl-k">$</span><span class="pl-smi">featureName</span>)</pre></div>

<p>Seperate features from <code>featureName</code> using the helper function <code>grepthis</code>.</p>

<div class="highlight highlight-r"><pre><span class="pl-en">grepthis</span> <span class="pl-k">&lt;-</span> <span class="pl-k">function</span> (<span class="pl-smi">regex</span>) {
  grepl(<span class="pl-smi">regex</span>, <span class="pl-smi">dt</span><span class="pl-k">$</span><span class="pl-smi">feature</span>)
}
<span class="pl-c">## Features with 2 categories</span>
<span class="pl-smi">n</span> <span class="pl-k">&lt;-</span> <span class="pl-c1">2</span>
<span class="pl-smi">y</span> <span class="pl-k">&lt;-</span> <span class="pl-k">matrix</span>(seq(<span class="pl-c1">1</span>, <span class="pl-smi">n</span>), <span class="pl-v">nrow</span><span class="pl-k">=</span><span class="pl-smi">n</span>)
<span class="pl-smi">x</span> <span class="pl-k">&lt;-</span> <span class="pl-k">matrix</span>(c(grepthis(<span class="pl-s"><span class="pl-pds">"</span>^t<span class="pl-pds">"</span></span>), grepthis(<span class="pl-s"><span class="pl-pds">"</span>^f<span class="pl-pds">"</span></span>)), <span class="pl-v">ncol</span><span class="pl-k">=</span>nrow(<span class="pl-smi">y</span>))
<span class="pl-smi">dt</span><span class="pl-k">$</span><span class="pl-smi">featDomain</span> <span class="pl-k">&lt;-</span> <span class="pl-k">factor</span>(<span class="pl-smi">x</span> <span class="pl-k">%*%</span> <span class="pl-smi">y</span>, <span class="pl-v">labels</span><span class="pl-k">=</span>c(<span class="pl-s"><span class="pl-pds">"</span>Time<span class="pl-pds">"</span></span>, <span class="pl-s"><span class="pl-pds">"</span>Freq<span class="pl-pds">"</span></span>))
<span class="pl-smi">x</span> <span class="pl-k">&lt;-</span> <span class="pl-k">matrix</span>(c(grepthis(<span class="pl-s"><span class="pl-pds">"</span>Acc<span class="pl-pds">"</span></span>), grepthis(<span class="pl-s"><span class="pl-pds">"</span>Gyro<span class="pl-pds">"</span></span>)), <span class="pl-v">ncol</span><span class="pl-k">=</span>nrow(<span class="pl-smi">y</span>))
<span class="pl-smi">dt</span><span class="pl-k">$</span><span class="pl-smi">featInstrument</span> <span class="pl-k">&lt;-</span> <span class="pl-k">factor</span>(<span class="pl-smi">x</span> <span class="pl-k">%*%</span> <span class="pl-smi">y</span>, <span class="pl-v">labels</span><span class="pl-k">=</span>c(<span class="pl-s"><span class="pl-pds">"</span>Accelerometer<span class="pl-pds">"</span></span>, <span class="pl-s"><span class="pl-pds">"</span>Gyroscope<span class="pl-pds">"</span></span>))
<span class="pl-smi">x</span> <span class="pl-k">&lt;-</span> <span class="pl-k">matrix</span>(c(grepthis(<span class="pl-s"><span class="pl-pds">"</span>BodyAcc<span class="pl-pds">"</span></span>), grepthis(<span class="pl-s"><span class="pl-pds">"</span>GravityAcc<span class="pl-pds">"</span></span>)), <span class="pl-v">ncol</span><span class="pl-k">=</span>nrow(<span class="pl-smi">y</span>))
<span class="pl-smi">dt</span><span class="pl-k">$</span><span class="pl-smi">featAcceleration</span> <span class="pl-k">&lt;-</span> <span class="pl-k">factor</span>(<span class="pl-smi">x</span> <span class="pl-k">%*%</span> <span class="pl-smi">y</span>, <span class="pl-v">labels</span><span class="pl-k">=</span>c(<span class="pl-c1">NA</span>, <span class="pl-s"><span class="pl-pds">"</span>Body<span class="pl-pds">"</span></span>, <span class="pl-s"><span class="pl-pds">"</span>Gravity<span class="pl-pds">"</span></span>))
<span class="pl-smi">x</span> <span class="pl-k">&lt;-</span> <span class="pl-k">matrix</span>(c(grepthis(<span class="pl-s"><span class="pl-pds">"</span>mean()<span class="pl-pds">"</span></span>), grepthis(<span class="pl-s"><span class="pl-pds">"</span>std()<span class="pl-pds">"</span></span>)), <span class="pl-v">ncol</span><span class="pl-k">=</span>nrow(<span class="pl-smi">y</span>))
<span class="pl-smi">dt</span><span class="pl-k">$</span><span class="pl-smi">featVariable</span> <span class="pl-k">&lt;-</span> <span class="pl-k">factor</span>(<span class="pl-smi">x</span> <span class="pl-k">%*%</span> <span class="pl-smi">y</span>, <span class="pl-v">labels</span><span class="pl-k">=</span>c(<span class="pl-s"><span class="pl-pds">"</span>Mean<span class="pl-pds">"</span></span>, <span class="pl-s"><span class="pl-pds">"</span>SD<span class="pl-pds">"</span></span>))
<span class="pl-c">## Features with 1 category</span>
<span class="pl-smi">dt</span><span class="pl-k">$</span><span class="pl-smi">featJerk</span> <span class="pl-k">&lt;-</span> <span class="pl-k">factor</span>(grepthis(<span class="pl-s"><span class="pl-pds">"</span>Jerk<span class="pl-pds">"</span></span>), <span class="pl-v">labels</span><span class="pl-k">=</span>c(<span class="pl-c1">NA</span>, <span class="pl-s"><span class="pl-pds">"</span>Jerk<span class="pl-pds">"</span></span>))
<span class="pl-smi">dt</span><span class="pl-k">$</span><span class="pl-smi">featMagnitude</span> <span class="pl-k">&lt;-</span> <span class="pl-k">factor</span>(grepthis(<span class="pl-s"><span class="pl-pds">"</span>Mag<span class="pl-pds">"</span></span>), <span class="pl-v">labels</span><span class="pl-k">=</span>c(<span class="pl-c1">NA</span>, <span class="pl-s"><span class="pl-pds">"</span>Magnitude<span class="pl-pds">"</span></span>))
<span class="pl-c">## Features with 3 categories</span>
<span class="pl-smi">n</span> <span class="pl-k">&lt;-</span> <span class="pl-c1">3</span>
<span class="pl-smi">y</span> <span class="pl-k">&lt;-</span> <span class="pl-k">matrix</span>(seq(<span class="pl-c1">1</span>, <span class="pl-smi">n</span>), <span class="pl-v">nrow</span><span class="pl-k">=</span><span class="pl-smi">n</span>)
<span class="pl-smi">x</span> <span class="pl-k">&lt;-</span> <span class="pl-k">matrix</span>(c(grepthis(<span class="pl-s"><span class="pl-pds">"</span>-X<span class="pl-pds">"</span></span>), grepthis(<span class="pl-s"><span class="pl-pds">"</span>-Y<span class="pl-pds">"</span></span>), grepthis(<span class="pl-s"><span class="pl-pds">"</span>-Z<span class="pl-pds">"</span></span>)), <span class="pl-v">ncol</span><span class="pl-k">=</span>nrow(<span class="pl-smi">y</span>))
<span class="pl-smi">dt</span><span class="pl-k">$</span><span class="pl-smi">featAxis</span> <span class="pl-k">&lt;-</span> <span class="pl-k">factor</span>(<span class="pl-smi">x</span> <span class="pl-k">%*%</span> <span class="pl-smi">y</span>, <span class="pl-v">labels</span><span class="pl-k">=</span>c(<span class="pl-c1">NA</span>, <span class="pl-s"><span class="pl-pds">"</span>X<span class="pl-pds">"</span></span>, <span class="pl-s"><span class="pl-pds">"</span>Y<span class="pl-pds">"</span></span>, <span class="pl-s"><span class="pl-pds">"</span>Z<span class="pl-pds">"</span></span>))</pre></div>

<p>Check to make sure all possible combinations of <code>feature</code> are accounted for by all possible combinations of the factor class variables.</p>

<div class="highlight highlight-r"><pre><span class="pl-smi">r1</span> <span class="pl-k">&lt;-</span> nrow(<span class="pl-smi">dt</span>[, .<span class="pl-smi">N</span>, <span class="pl-v">by</span><span class="pl-k">=</span>c(<span class="pl-s"><span class="pl-pds">"</span>feature<span class="pl-pds">"</span></span>)])
<span class="pl-smi">r2</span> <span class="pl-k">&lt;-</span> nrow(<span class="pl-smi">dt</span>[, .<span class="pl-smi">N</span>, <span class="pl-v">by</span><span class="pl-k">=</span>c(<span class="pl-s"><span class="pl-pds">"</span>featDomain<span class="pl-pds">"</span></span>, <span class="pl-s"><span class="pl-pds">"</span>featAcceleration<span class="pl-pds">"</span></span>, <span class="pl-s"><span class="pl-pds">"</span>featInstrument<span class="pl-pds">"</span></span>, <span class="pl-s"><span class="pl-pds">"</span>featJerk<span class="pl-pds">"</span></span>, <span class="pl-s"><span class="pl-pds">"</span>featMagnitude<span class="pl-pds">"</span></span>, <span class="pl-s"><span class="pl-pds">"</span>featVariable<span class="pl-pds">"</span></span>, <span class="pl-s"><span class="pl-pds">"</span>featAxis<span class="pl-pds">"</span></span>)])
<span class="pl-smi">r1</span> <span class="pl-k">==</span> <span class="pl-smi">r2</span></pre></div>

<p>Yes, I accounted for all possible combinations. <code>feature</code> is now redundant.</p>

<h2>
<a id="user-content-create-a-tidy-data-set" class="anchor" href="#create-a-tidy-data-set" aria-hidden="true"><span class="octicon octicon-link"></span></a>Create a tidy data set</h2>

<p>Create a data set with the average of each variable for each activity and each subject.</p>

<div class="highlight highlight-r"><pre>setkey(<span class="pl-smi">dt</span>, <span class="pl-smi">subject</span>, <span class="pl-smi">activity</span>, <span class="pl-smi">featDomain</span>, <span class="pl-smi">featAcceleration</span>, <span class="pl-smi">featInstrument</span>, <span class="pl-smi">featJerk</span>, <span class="pl-smi">featMagnitude</span>, <span class="pl-smi">featVariable</span>, <span class="pl-smi">featAxis</span>)
<span class="pl-smi">dtTidy</span> <span class="pl-k">&lt;-</span> <span class="pl-smi">dt</span>[, <span class="pl-k">list</span>(<span class="pl-v">count</span> <span class="pl-k">=</span> .<span class="pl-smi">N</span>, <span class="pl-v">average</span> <span class="pl-k">=</span> mean(<span class="pl-smi">value</span>)), <span class="pl-v">by</span><span class="pl-k">=</span>key(<span class="pl-smi">dt</span>)]</pre></div>

<p>Make codebook.</p>

<div class="highlight highlight-r"><pre>knit(<span class="pl-s"><span class="pl-pds">"</span>makeCodebook.Rmd<span class="pl-pds">"</span></span>, <span class="pl-v">output</span><span class="pl-k">=</span><span class="pl-s"><span class="pl-pds">"</span>codebook.md<span class="pl-pds">"</span></span>, <span class="pl-v">encoding</span><span class="pl-k">=</span><span class="pl-s"><span class="pl-pds">"</span>ISO8859-1<span class="pl-pds">"</span></span>, <span class="pl-v">quiet</span><span class="pl-k">=</span><span class="pl-c1">TRUE</span>)
markdownToHTML(<span class="pl-s"><span class="pl-pds">"</span>codebook.md<span class="pl-pds">"</span></span>, <span class="pl-s"><span class="pl-pds">"</span>codebook.html<span class="pl-pds">"</span></span>)</pre></div>
</article>
  </div>

</div>

<a href="#jump-to-line" rel="facebox[.linejump]" data-hotkey="l" style="display:none">Jump to Line</a>
<div id="jump-to-line" style="display:none">
  <form accept-charset="UTF-8" action="" class="js-jump-to-line-form" method="get"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /></div>
    <input class="linejump-input js-jump-to-line-field" type="text" placeholder="Jump to line&hellip;" autofocus>
    <button type="submit" class="btn">Go</button>
</form></div>

        </div>

      </div><!-- /.repo-container -->
      <div class="modal-backdrop"></div>
    </div><!-- /.container -->
  </div><!-- /.site -->


    </div><!-- /.wrapper -->

      <div class="container">
  <div class="site-footer" role="contentinfo">
    <ul class="site-footer-links right">
        <li><a href="https://status.github.com/" data-ga-click="Footer, go to status, text:status">Status</a></li>
      <li><a href="https://developer.github.com" data-ga-click="Footer, go to api, text:api">API</a></li>
      <li><a href="https://training.github.com" data-ga-click="Footer, go to training, text:training">Training</a></li>
      <li><a href="https://shop.github.com" data-ga-click="Footer, go to shop, text:shop">Shop</a></li>
        <li><a href="https://github.com/blog" data-ga-click="Footer, go to blog, text:blog">Blog</a></li>
        <li><a href="https://github.com/about" data-ga-click="Footer, go to about, text:about">About</a></li>

    </ul>

    <a href="https://github.com" aria-label="Homepage">
      <span class="mega-octicon octicon-mark-github" title="GitHub"></span>
</a>
    <ul class="site-footer-links">
      <li>&copy; 2015 <span title="0.02910s from github-fe119-cp1-prd.iad.github.net">GitHub</span>, Inc.</li>
        <li><a href="https://github.com/site/terms" data-ga-click="Footer, go to terms, text:terms">Terms</a></li>
        <li><a href="https://github.com/site/privacy" data-ga-click="Footer, go to privacy, text:privacy">Privacy</a></li>
        <li><a href="https://github.com/security" data-ga-click="Footer, go to security, text:security">Security</a></li>
        <li><a href="https://github.com/contact" data-ga-click="Footer, go to contact, text:contact">Contact</a></li>
    </ul>
  </div>
</div>


    <div class="fullscreen-overlay js-fullscreen-overlay" id="fullscreen_overlay">
  <div class="fullscreen-container js-suggester-container">
    <div class="textarea-wrap">
      <textarea name="fullscreen-contents" id="fullscreen-contents" class="fullscreen-contents js-fullscreen-contents" placeholder=""></textarea>
      <div class="suggester-container">
        <div class="suggester fullscreen-suggester js-suggester js-navigation-container"></div>
      </div>
    </div>
  </div>
  <div class="fullscreen-sidebar">
    <a href="#" class="exit-fullscreen js-exit-fullscreen tooltipped tooltipped-w" aria-label="Exit Zen Mode">
      <span class="mega-octicon octicon-screen-normal"></span>
    </a>
    <a href="#" class="theme-switcher js-theme-switcher tooltipped tooltipped-w"
      aria-label="Switch themes">
      <span class="octicon octicon-color-mode"></span>
    </a>
  </div>
</div>



    
    

    <div id="ajax-error-message" class="flash flash-error">
      <span class="octicon octicon-alert"></span>
      <a href="#" class="octicon octicon-x flash-close js-ajax-error-dismiss" aria-label="Dismiss error"></a>
      Something went wrong with that request. Please try again.
    </div>


      <script crossorigin="anonymous" src="https://assets-cdn.github.com/assets/frameworks-2c8ae50712a47d2b83d740cb875d55cdbbb3fdbccf303951cc6b7e63731e0c38.js"></script>
      <script async="async" crossorigin="anonymous" src="https://assets-cdn.github.com/assets/github-fe1102a627c0f0eb4c8ccd94ee4ecb4ea91eb19e1ea462b1d6fe0435bb27e366.js"></script>
      
      


  </body>
</html>

