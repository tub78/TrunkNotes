Title: Special:Header
Timestamp: 2011-10-07 23:49:33 +0000
Created: 2011-04-18 16:56:29 +0000
Last Accessed: 2011-10-07 23:47:14 +0000
Times Accessed: 40
Tags: Javascript, TrunkNotes, Css
Metadata: 

<!-- not required by TN
<html>
<head> -->
<!-- TITLE -->
<!-- not required by TN -->

<!-- Stylesheet: Homepage -->
{{stylesheet Snippet_csscombined}}

<!-- MATHJAX hosted CDN.MATHJAX.ORG -->
<!-- <script type='text/javascript' src='http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS_HTML'> MathJax.Hub.Config({ extensions: ["tex2jax.js","MathMenu.js","MathZoom.js"], jax: ["input/TeX","output/HTML-CSS"], tex2jax: {inlineMath: [["\\(","\\)"]]}, TeX: { extensions: ["AMSmath.js","AMSsymbols.js","noErrors.js","noUndefined.js"] } }); </script> -->


<!-- Additional stylesheets not supported by TN !? -->
<!-- SYNTAXHIGHLIGHTER: LOCAL, DROPBOX, & ALEXGORBATCHEV sources -->
<!-- <link href="styles/shCore.css" rel="stylesheet" type="text/css" /> <link href="styles/shThemeDefault.css" rel="stylesheet" type="text/css" /> <script type="text/javascript" src="scripts/shCore.js"></script> -->
<!-- <link href="http://dl.dropbox.com/u/1603420/SyntaxHighlighter/styles/shCore.css" rel="stylesheet" type="text/css" /> <link href="http://dl.dropbox.com/u/1603420/SyntaxHighlighter/styles/shThemeDefault.css" rel="stylesheet" type="text/css" /> <script type="text/javascript" src="http://dl.dropbox.com/u/1603420/SyntaxHighlighter/scripts/shCore.js"></script> -->
<!-- <link href="http://alexgorbatchev.com/pub/sh/current/styles/shCore.css" rel="stylesheet" type="text/css" /> <link href="http://alexgorbatchev.com/pub/sh/current/styles/shThemeDefault.css" rel="stylesheet" type="text/css" /> <script type="text/javascript" src="http://alexgorbatchev.com/pub/sh/current/scripts/shCore.js"></script> -->

<!-- GOOGLEAPIS hosted JQUERY.MIN -->
<!-- <script type="text/javascript" src="http://ajax.googleapis.com/ajax/libs/jquery/1.4.2/jquery.min.js"></script> -->

<!-- GITHUB hosted JQUERY.COOKIE.JS -->
<!-- <script type="text/javascript" src="https://raw.github.com/carhartl/jquery-cookie/master/jquery.cookie.js"></script> -->


<!-- DAYTIME/NIGHTTIME JAVASCRIPT -->
<script language="javascript">//<![CDATA[ 
  $(document).ready(function(){
    // Display day mode between 7am and 8pm
    var currentTime = new Date().getHours();
    var daytime_selected = (7 <= currentTime && currentTime < 19) ? 'yes' : 'no';
    daytime_selected = $.cookie('tub78_daytime_selected') || daytime_selected;
    if (daytime_selected == 'yes') {
      $(".title,.todoaction,.ideaaction,.bugaction,.doneaction,body,h1,h2,h3,h4,h5,h6,a,a.missing-wiki-link,th,blockquote,code").addClass("day");
    } else {
      $(".title,.todoaction,.ideaaction,.bugaction,.doneaction,body,h1,h2,h3,h4,h5,h6,a,a.missing-wiki-link,th,blockquote,code").addClass("night");
    }
    $.cookie('tub78_daytime_selected', daytime_selected, { expires: 1, path: '/' });
    $("button#daynight").click(function(){
      $(".title,.todoaction,.ideaaction,.bugaction,.doneaction,body,h1,h2,h3,h4,h5,h6,a,a.missing-wiki-link,th,blockquote,code").toggleClass("day");
      $(".title,.todoaction,.ideaaction,.bugaction .doneaction,body,h1,h2,h3,h4,h5,h6,a,a.missing-wiki-link,th,blockquote,code").toggleClass("night");
      var daytime_selected = $.cookie('tub78_daytime_selected') || 'yes';
      $.cookie('tub78_daytime_selected', (daytime_selected == 'yes') ? 'no' : 'yes', { expires: 1, path: '/' });
    });

    /* Hide first unordered list (toc) if hdrcontents is hidden */
    /* .. does not work b/c toc is not instantiated yet */
    /*
    if ($("div.hdrcontents:visible").size() == 0) {
        $("div.hdrcontents").before($("ul:first").text());
        $("div.hdrcontents").after($("div.hdrcontents:visible").size() + " " + $("div.hdrcontents:hidden").size());
        $("ul:first").hide();
    }
    */

    $("button#hdrcontents").click(function(){
        $("div.hdrcontents").toggle();
        /* ALSO: toggle first unordered list */
        $("ul:first").toggle();
    });

    $("button#hdrtags").click(function(){
        $("div.hdrtags").toggle();
    });

    $("button#hdrbacklinks").click(function(){
        $("div.hdrbacklinks").toggle();
    });

    $("button#hdrrelated").click(function(){
        $("div.hdrrelated").toggle();
    });

    $("button#hdrhistory").click(function(){
        $("div.hdrhistory").toggle();
    });

  });
  //]]></script>
<!-- END HEADER / START BODY -->
<!-- not required by TN
</head>
<body> -->

<!--
BUTTONS [[Snippet_cssincl]] [[Snippet_cssday]] [[Snippet_cssnight]] [[Snippet_csscombined]] [Blogger style-combined.css]
-->
<div class="inline">
<button id="daynight">Day/Night</button>
<button id="hdrcontents">Contents</button>
<button id="hdrtags">Tags</button>
<button id="hdrbacklinks">Backlinks</button>
<button id="hdrrelated">Related</button>
<button id="hdrhistory">History</button>
<span class="tiny">[[About-This-Blog|About]]</span>
</div>



<!-- CONTENTS -->
>%hdrcontents%
># Contents #
{{toc}}

<!-- TAGS -->
>%hdrtags%
>## Tags ##
>{{tags}}

<!-- BACKLINKS -->
>%hdrbacklinks%
>## Backlinks ##
>{{backlinks}}

<!-- HISTORY
>%hdrhistory%
>## History
>{{history 6}} -->

<!-- BODY -->
<!-- not required by TN
<?theme body?>
-->

<!-- END BODY -->
<!-- not required by TN
</body>
</html>
-->

