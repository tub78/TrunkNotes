Title: Snippet_csscombined
Timestamp: 2012-04-21 20:56:16 +0000
Created: 2011-03-27 03:31:28 +0000
Last Accessed: 2011-07-17 02:26:39 +0000
Times Accessed: 7
Tags: TrunkNotes, Html
Metadata: 

/* was TN:Stylesheet:Day */
#info {
    font: medium Arial;
    background: #CFCFCF;
    font-size: 12px;
    padding-left: 4px;
    margin-bottom: 0px;
    padding-top: 2px;
    padding-bottom: 2px;
    height: 14px;
}

#contents {
    margin-top: 0px;
    padding-left: 8px;
    padding-right: 8px;
}
html {
    -webkit-text-size-adjust: none;
}

/*
Action Items
*/
.action {
    /* display: inline-block; */
    display: none;
    font-weight: bold;
    padding-left: 0.5em;
    padding-right: 0.5em;
}
.todoaction {
    color: #FF0000;
}
.todoaction.day {
    background-color: #DDDDDD;
}
.todoaction.night {
    background-color: #292929;
}
.ideaaction {
    color: #FF7F00;
}
.ideaaction.day {
    background-color: #DDDDDD;
}
.ideaaction.night {
    background-color: #292929;
}
.bugaction {
    color: #00FF00;
}
.bugaction.day {
    background-color: #DDDDDD;
}
.bugaction.night {
    background-color: #292929;
}
.doneaction {
    color: #FF7FFF;
}
.doneaction.day {
    background-color: #DDDDDD;
}
.doneaction.night {
    background-color: #292929;
}

/*
Classes
*/

.toc li {
    list-style-type: none;
}
.todo {
    font-weight: bold;
    background-color: #F0ECE8;
    color: #A03020;
}
.justleft {
    text-align: left;
}
.justright {
    text-align: right;
}
.justcenter {
    text-align: center;
}
.center {
    margin-left: auto;
    margin-right: auto;
}
.highlight {
    background-color: yellow;
}

.highlight-selected {
    background-color: red;
}
.tiny {
    font-size: 0.5em;
    /* font-size: 10px; */
}

/* divflash style */
.divflash {
    display: none;
}
/* divnotflash style */
.divnotflash {
}
/* tabbar list style */
.tabbar li {
    display: inline;
    list-style-type: none;
    padding-right: 20px;
}
/* inline */
.inline p {
    display: inline;
    list-style-type: none;
    padding-right: 20px;
}
/* special header styles */
.hdrcontents {
    /* display: none; */
}
.hdrtags {
    display: none;
}
.hdrtags li {
    display: inline;
    list-style-type: none;
    padding-right: 20px;
}
.hdrbacklinks {
    display: none;
}
.hdrbacklinks li {
    display: inline;
    list-style-type: none;
    padding-right: 20px;
}
.hdrrelated {
    display: none;
}
.hdrrelated li {
    display: inline;
    list-style-type: none;
    padding-right: 20px;
}


/*
 * Default tag style
 * margin: top right btm left
 * margin: 0em;
 * margin: 1em 2em 1em 2em;

 * font-family: 'Trebuchet MS',Trebuchet,Verdana,sans-serif;
 * font-size: 100%;
 * line-height: 150%;

 * font-family: "Consolas", "Bitstream Vera Sans Mono", "Courier New", Courier;
 * font-size: 100%;
 * line-height: 125%;

 * font: medium Arial;
 */
body {
    margin: 0em;
    font-family: helvetica,arial,freesans,clean,sans-serif;
    font-size: 16px;
    /* line-height: 1.5em; */
    background-repeat: repeat-x;
    background-attachment: fixed;
}
body.day {
    color: #657B83;
    background-color: #FDF6E3;
}
body.night {
    color: #839496;
    background-color: #002B36;
}


/*
 * font-family: Tahoma, sans-serif;
 * font: Arial;

 * font-family: 'Trebuchet MS',Trebuchet,Verdana,sans-serif;
 * font-family: "Consolas", "Bitstream Vera Sans Mono", "Courier New", Courier;
 */
h1, h2, h3, h4, h5, h6 {
    font-family: helvetica,arial,freesans,clean,sans-serif;
    margin-top: 1.5em;
    margin-bottom: 0.5em;
}
/* font-family: Trebuchet MS, serif; */
/* font-weight: bold; */
h1 {
    font-size: 1.8em;
}
h1.day {
    color: #DC322F;
}
h1.night {
    color: #D33682;
}
h2 {
    font-size: 1.5em;
}
h2.day {
    color: #268BD2;
}
h2.night {
    color: #B58900;
}
h3 {
    font-size: 1.3em;
}
h3.day {
    color: #2AA198;
}
h3.night {
    color: #859900;
}
h4 {
    font-size: 1.2em;
}
h4.day {
    color: #859900;
}
h4.night {
    color: #2AA198;
}
h5 {
    font-size: 1.1em;
}
h5.day {
    color: #B58900;
}
h5.night {
    color: #268BD2;
}
h6 {
    font-size: 1.0em;
}
h6.day {
    color: #D33682;
}
h6.night {
    color: #DC322F;
}
a {
    text-decoration: none;
    border-bottom: 1px dotted;
    color: #6C71C4;
}
a.day {
    /* color: #0000FF; */
    /* color: #CB4B16 */
    /* color: #6C71C4; */
}
a.night {
    /* color: #63B8FF; */
    /* color: #6C71C4; */
}
a.wiki-link {
    text-decoration: underline;
    border-bottom: none;
}
a.missing-wiki-link {
}
a.missing-wiki-link.day {
    color: red;
}
a.missing-wiki-link.night {
    color: green;
}
p, pre, blockquote, table, ul, ol, dl {
    margin-top: 1em;
    margin-bottom: 1em;
}
ul ul, ul ol, ol ol, ol ul {
    margin-top: 0.5em;
    margin-bottom: 0.5em;
}
/* 
ul ul li, ul ol li, ol ol li, ol ul li {
    padding: 0.1em;
}
*/
table {
    margin: 1em;
    /* padding: 1em; */
    border-collapse: collapse;
    width: 90%;
}
thead {
    background: #CCCCCC;
}

th, td {
    border: 1px solid #CCCCCC;
    padding: 0.3em;
}
th {
}
th.day {
    background-color: #F0F0F0;
}
th.night {
    background-color: #555555;
}
li {
    /* padding: 0.3em; */
    margin: 0.3em auto;
}
ul {
    margin-left: 2em;
    padding-left: 0.5em;
}
dt {
    font-weight: bold;
}
img {
    border: none;
}
pre {
    /* border-left: 1px solid #CCCCCC; */
    /* margin-left: 2em; */
    padding-left: 0.5em;
    padding-right: 0.5em;
    /* background: */
}
blockquote {
    padding: 0.4em;
}
blockquote.day {
    background-color: #F6F5EB;
}
blockquote.night {
    background-color: #30302E;
}
hr {
    border: none;
    border-top: 1px solid #CCCCCC;
    width: 100%;
}
del {
    text-decoration: line-through;
    color: #777777;
}
code {
    padding: 0px 3px 0px;
    display: inline-block;
}
code.day {
    color: #0000FF;
    background-color: #DDDDDD;
}
code.night {
    color: #FFFFFF;
    background-color: #555555;
}

/* daynight button ================================================ */

button#daynight, button#hdrcontents, button#hdrtags, button#hdrbacklinks, button#hdrrelated {
	  float:right;
    vertical-align:bottom;
  	padding: 3px 6px;
  	margin: 2px;
  	background: #eee;
  	color:#005F6B;
  	border-radius: 3px;
    border: 0px;
    border-bottom: 1px dotted;
  	text-decoration:none;
}

.header {
    margin: 1em 0em 1em 0em;
}
.title {
    font-family: helvetica,arial,freesans,clean,sans-serif;
    /* font-size: 2.4em; */
    font-size: 1.2em;
    /* line-height: 1.5em; */
}
.title.day {
    color: #657B83;
    background-color: #FDF6E3;
}
.title.night {
    color: #839496;
    background-color: #002B36;
}



