Title: Special:Header
Timestamp: 2011-10-07 23:49:33 +0000
Created: 2011-04-18 16:56:29 +0000
Last Accessed: 2011-10-07 23:47:14 +0000
Times Accessed: 40
Tags: Javascript, TrunkNotes, Css
Metadata: 

<pre class="action ideaaction" style="display:none">
@I 2011-03-21     ../TN      [[SpecialHeader]];
@I 2011-03-21     ../Html    [page.theme](file:///Users/stu/Desktop/Dropbox/Documents/TrunkNotes/Html/page.theme)
@I 2011-03-21     ../Blog    [page.theme](file:///Users/stu/Desktop/Dropbox/Documents/TrunkNotes/Blog/page.theme)
@I 2011-03-21     ../Blogger [DesignTemplate.xml](file:///Users/stu/Desktop/Dropbox/Documents/TrunkNotes/Blog/DesignTemplate.xml)
</pre>

<pre class="action bugaction"> 
@B 2011-11-07 MathJax script is not called from TrunkNotes app !!!
@B 2011-03-26 23:32:56 [[TN]]: toc (TN function) is probably javascript, activated via jquery ready() queue executing AFTER personal jquery.ready() calls
</pre>


<!-- TITLE -->
<!-- not required by TN -->

<!-- STYLESHEET -->
{{stylesheet Snippet_csscombined}}

<!-- MATHJAX hosted CDN.MATHJAX.ORG -->
<!-- <script type='text/javascript' src='http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS_HTML'> MathJax.Hub.Config({ extensions: ["tex2jax.js","MathMenu.js","MathZoom.js"], jax: ["input/TeX","output/HTML-CSS"], tex2jax: {inlineMath: [["\\(","\\)"]]}, TeX: { extensions: ["AMSmath.js","AMSsymbols.js","noErrors.js","noUndefined.js"] } }); </script> -->


<!-- SYNTAXHIGHLIGHTER -->
<!-- LOCAL, DROPBOX, ALEXGORBATCHEV -->
<!-- additional stylesheets not supported by TN -->
<!-- <link href="styles/shCore.css" rel="stylesheet" type="text/css" /> <link href="styles/shThemeDefault.css" rel="stylesheet" type="text/css" /> <script type="text/javascript" src="scripts/shCore.js"></script> -->
<!-- <link href="http://dl.dropbox.com/u/1603420/SyntaxHighlighter/styles/shCore.css" rel="stylesheet" type="text/css" /> <link href="http://dl.dropbox.com/u/1603420/SyntaxHighlighter/styles/shThemeDefault.css" rel="stylesheet" type="text/css" /> <script type="text/javascript" src="http://dl.dropbox.com/u/1603420/SyntaxHighlighter/scripts/shCore.js"></script> -->
<!-- <link href="http://alexgorbatchev.com/pub/sh/current/styles/shCore.css" rel="stylesheet" type="text/css" /> <link href="http://alexgorbatchev.com/pub/sh/current/styles/shThemeDefault.css" rel="stylesheet" type="text/css" /> <script type="text/javascript" src="http://alexgorbatchev.com/pub/sh/current/scripts/shCore.js"></script> -->




<!-- DAY/NIGHT, HDRCONTENTS, HDRTAGS, HDRBACKLINKS, HDRRELATED ... JAVASCRIPT -->
<!-- <script type="text/javascript" src="http://ajax.googleapis.com/ajax/libs/jquery/1.4.2/jquery.min.js"></script>  -->
<script language="javascript">//<![CDATA[ 
    $(document).ready(function(){
        // Display day mode between 7am and 8pm
        var currentTime = new Date().getHours();
        if (7 <= currentTime && currentTime < 19) {
            $(".todoaction,.ideaaction,.bugaction,.doneaction,body,h1,h2,h3,h4,h5,h6,a,a.missing-wiki-link,th,blockquote,code").addClass("day");
        } else {
            $(".todoaction,.ideaaction,.bugaction,.doneaction,body,h1,h2,h3,h4,h5,h6,a,a.missing-wiki-link,th,blockquote,code").addClass("night");
        }

        $("button#daynight").click(function(){
            $(".todoaction,.ideaaction,.bugaction,.doneaction,body,h1,h2,h3,h4,h5,h6,a,a.missing-wiki-link,th,blockquote,code").toggleClass("day");
            $(".todoaction,.ideaaction,.bugaction .doneaction,body,h1,h2,h3,h4,h5,h6,a,a.missing-wiki-link,th,blockquote,code").toggleClass("night");
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
<body>
-->

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



<!-- CONTENTS
>%hdrcontents%
># Contents #
{{toc}} -->

<!-- TAGS -->
>%hdrtags%
>## Tags ##
>{{tags}}

<!-- BACKLINKS -->
>%hdrbacklinks%
>## Backlinks ##
>{{backlinks}}

<!-- HISTORY  -->
>%hdrhistory%
>## History
>{{history 6}}

<!-- BODY -->
<!-- not required by TN
<?theme body?>
-->

<!-- END BODY -->
<!-- not required by TN
</body>
</html>
-->

<!--
Log
-->

<pre class="action doneaction"> 
@D 2011-03-27 22:28:26 WORKS! jquery without explicitly including library (b/c it appears to be available on the iPad)
@D 2011-03-20 11:22:31 WORKS!   (JQuery Rules!)   TN, Javascript, Html, SpecialHeader: include FIRST Unordered List - TOC is $(ul:first)
@D 2011-03-20 10:32:37 TN, Javascript, Html: [BUTTONS] for: contents, tags, backlinks, day/night
@D 2011-03-20 00:03:47 Wiki/Blog: customized header information : CSS and Javascript ../TN: [[SpecialHeader]]; ../Html: [page.theme](file:///Users/stu/Desktop/Dropbox/Documents/TrunkNotes/Html/page.theme) ../Blog: [page.theme](file:///Users/stu/Desktop/Dropbox/Documents/TrunkNotes/Blog/page.theme)
@D 2011-03-19 22:56:06 DID NOT WORK: include INLINE<<[[SyntaxHighlighter_shThemeDefaultCss]], [[SyntaxHighlighter_shCoreCss]]
@D 2011-03-19 22:43:49 DID NOT WORK: enclosure / include file, with END-PRE] ... [START-PRE tags, : [[Snippet_javascript]]
@D 2011-03-19 21:30:05 include javascript.txt note in page.theme ... discount theme would complain about TN headers
@D 2011-03-19 23:02:07 using Snippet_csscombined instead of Snippet_cssincl
</pre>

