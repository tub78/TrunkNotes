Title: Snippet_csscombined
Timestamp: 2011-07-17 02:26:35 +0000
Created: 2011-03-27 03:31:28 +0000
Last Accessed: 2011-07-17 02:26:39 +0000
Times Accessed: 7
Tags: Html, TrunkNotes
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
.hdrhistory {
    display: none;
}
.hdrhistory li {
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
 */
body {
    margin: 0em;
    font: medium Arial;
    font-size: 16px;
    /* line-height: 130%; */
    background-repeat: repeat-x;
    background-attachment: fixed;
}
body.day {
    color: #000000;
    background-color: #FFFFFF;
}
body.night {
    color: #AAAAAA;
    background-color: #191919;
}

/* font-family: Tahoma, sans-serif; */
h1, h2, h3, h4, h5, h6 {
    font: Arial;
    margin-top: 1.5em;
    margin-bottom: 0.5em;
}
/* font-family: Trebuchet MS, serif; */
/* font-weight: bold; */
h1 {
    font-size: 1.8em;
}
h1.day {
    color: #AA5873;
}
h1.night {
    color: #E08089;
}
h2 {
    font-size: 1.5em;
}
h2.day {
    color: #50705C;
}
h2.night {
    color: #80E089;
}
h3 {
    font-size: 1.3em;
}
h3.day {
    color: #1030A0;
}
h3.night {
    color: #4D89E0;
}
h4 {
    font-size: 1.2em;
}
h4.day {
    color: #103064;
}
h4.night {
    color: #C0C0F0;
}
h5 {
    font-size: 1.1em;
}
h5.day {
    color: #50506E;
}
h5.night {
    color: #E0E0E4;
}
h6 {
    font-size: 1.0em;
}
h6.day {
    color: #636363;
}
h6.night {
    color: #F0F0EC;
}
a {
    text-decoration: none;
    border-bottom: 1px dotted;
}
a.day {
    color: #0000FF;
}
a.night {
    color: #63B8FF;
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
    border-left: 1px solid #CCCCCC;
    margin-left: 2em;
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
    background-color: #302E2E;
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
    display: inline-block;
    padding-left: 0.5em;
    padding-right: 0.5em;
}
code.day {
    color: #0000FF;
    background-color: #DDDDDD;
}
code.night {
    color: #FFFFFF;
    background-color: #555555;
}


