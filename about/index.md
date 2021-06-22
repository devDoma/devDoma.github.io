---
layout: page
title: About the Theme
tags: [about, Jekyll, theme, moon]
date: 2016-03-21
comments: false
---

<html><head><meta http-equiv="Content-Type" content="text/html; charset=utf-8"/><title>정형식 (Hyung Sik Jeong)</title><style>
/* cspell:disable-file */
/* webkit printing magic: print all background colors */
html {
	-webkit-print-color-adjust: exact;
}
* {
	box-sizing: border-box;
	-webkit-print-color-adjust: exact;
}

html,
body {
	margin: 0;
	padding: 0;
}
@media only screen {
	body {
		margin: 2em auto;
		max-width: 900px;
		color: rgb(55, 53, 47);
	}
}

body {
	line-height: 1.5;
	white-space: pre-wrap;
}

a,
a.visited {
	color: inherit;
	text-decoration: underline;
}

.pdf-relative-link-path {
	font-size: 80%;
	color: #444;
}

h1,
h2,
h3 {
	letter-spacing: -0.01em;
	line-height: 1.2;
	font-weight: 600;
	margin-bottom: 0;
}

.page-title {
	font-size: 2.5rem;
	font-weight: 700;
	margin-top: 0;
	margin-bottom: 0.75em;
}

h1 {
	font-size: 1.875rem;
	margin-top: 1.875rem;
}

h2 {
	font-size: 1.5rem;
	margin-top: 1.5rem;
}

h3 {
	font-size: 1.25rem;
	margin-top: 1.25rem;
}

.source {
	border: 1px solid #ddd;
	border-radius: 3px;
	padding: 1.5em;
	word-break: break-all;
}

.callout {
	border-radius: 3px;
	padding: 1rem;
}

figure {
	margin: 1.25em 0;
	page-break-inside: avoid;
}

figcaption {
	opacity: 0.5;
	font-size: 85%;
	margin-top: 0.5em;
}

mark {
	background-color: transparent;
}

.indented {
	padding-left: 1.5em;
}

hr {
	background: transparent;
	display: block;
	width: 100%;
	height: 1px;
	visibility: visible;
	border: none;
	border-bottom: 1px solid rgba(55, 53, 47, 0.09);
}

img {
	max-width: 100%;
}

@media only print {
	img {
		max-height: 100vh;
		object-fit: contain;
	}
}

@page {
	margin: 1in;
}

.collection-content {
	font-size: 0.875rem;
}

.column-list {
	display: flex;
	justify-content: space-between;
}

.column {
	padding: 0 1em;
}

.column:first-child {
	padding-left: 0;
}

.column:last-child {
	padding-right: 0;
}

.table_of_contents-item {
	display: block;
	font-size: 0.875rem;
	line-height: 1.3;
	padding: 0.125rem;
}

.table_of_contents-indent-1 {
	margin-left: 1.5rem;
}

.table_of_contents-indent-2 {
	margin-left: 3rem;
}

.table_of_contents-indent-3 {
	margin-left: 4.5rem;
}

.table_of_contents-link {
	text-decoration: none;
	opacity: 0.7;
	border-bottom: 1px solid rgba(55, 53, 47, 0.18);
}

table,
th,
td {
	border: 1px solid rgba(55, 53, 47, 0.09);
	border-collapse: collapse;
}

table {
	border-left: none;
	border-right: none;
}

th,
td {
	font-weight: normal;
	padding: 0.25em 0.5em;
	line-height: 1.5;
	min-height: 1.5em;
	text-align: left;
}

th {
	color: rgba(55, 53, 47, 0.6);
}

ol,
ul {
	margin: 0;
	margin-block-start: 0.6em;
	margin-block-end: 0.6em;
}

li > ol:first-child,
li > ul:first-child {
	margin-block-start: 0.6em;
}

ul > li {
	list-style: disc;
}

ul.to-do-list {
	text-indent: -1.7em;
}

ul.to-do-list > li {
	list-style: none;
}

.to-do-children-checked {
	text-decoration: line-through;
	opacity: 0.375;
}

ul.toggle > li {
	list-style: none;
}

ul {
	padding-inline-start: 1.7em;
}

ul > li {
	padding-left: 0.1em;
}

ol {
	padding-inline-start: 1.6em;
}

ol > li {
	padding-left: 0.2em;
}

.mono ol {
	padding-inline-start: 2em;
}

.mono ol > li {
	text-indent: -0.4em;
}

.toggle {
	padding-inline-start: 0em;
	list-style-type: none;
}

/* Indent toggle children */
.toggle > li > details {
	padding-left: 1.7em;
}

.toggle > li > details > summary {
	margin-left: -1.1em;
}

.selected-value {
	display: inline-block;
	padding: 0 0.5em;
	background: rgba(206, 205, 202, 0.5);
	border-radius: 3px;
	margin-right: 0.5em;
	margin-top: 0.3em;
	margin-bottom: 0.3em;
	white-space: nowrap;
}

.collection-title {
	display: inline-block;
	margin-right: 1em;
}

time {
	opacity: 0.5;
}

.icon {
	display: inline-block;
	max-width: 1.2em;
	max-height: 1.2em;
	text-decoration: none;
	vertical-align: text-bottom;
	margin-right: 0.5em;
}

img.icon {
	border-radius: 3px;
}

.user-icon {
	width: 1.5em;
	height: 1.5em;
	border-radius: 100%;
	margin-right: 0.5rem;
}

.user-icon-inner {
	font-size: 0.8em;
}

.text-icon {
	border: 1px solid #000;
	text-align: center;
}

.page-cover-image {
	display: block;
	object-fit: cover;
	width: 100%;
	height: 30vh;
}

.page-header-icon {
	font-size: 3rem;
	margin-bottom: 1rem;
}

.page-header-icon-with-cover {
	margin-top: -0.72em;
	margin-left: 0.07em;
}

.page-header-icon img {
	border-radius: 3px;
}

.link-to-page {
	margin: 1em 0;
	padding: 0;
	border: none;
	font-weight: 500;
}

p > .user {
	opacity: 0.5;
}

td > .user,
td > time {
	white-space: nowrap;
}

input[type="checkbox"] {
	transform: scale(1.5);
	margin-right: 0.6em;
	vertical-align: middle;
}

p {
	margin-top: 0.5em;
	margin-bottom: 0.5em;
}

.image {
	border: none;
	margin: 1.5em 0;
	padding: 0;
	border-radius: 0;
	text-align: center;
}

.code,
code {
	background: rgba(135, 131, 120, 0.15);
	border-radius: 3px;
	padding: 0.2em 0.4em;
	border-radius: 3px;
	font-size: 85%;
	tab-size: 2;
}

code {
	color: #eb5757;
}

.code {
	padding: 1.5em 1em;
}

.code-wrap {
	white-space: pre-wrap;
	word-break: break-all;
}

.code > code {
	background: none;
	padding: 0;
	font-size: 100%;
	color: inherit;
}

blockquote {
	font-size: 1.25em;
	margin: 1em 0;
	padding-left: 1em;
	border-left: 3px solid rgb(55, 53, 47);
}

.bookmark {
	text-decoration: none;
	max-height: 8em;
	padding: 0;
	display: flex;
	width: 100%;
	align-items: stretch;
}

.bookmark-title {
	font-size: 0.85em;
	overflow: hidden;
	text-overflow: ellipsis;
	height: 1.75em;
	white-space: nowrap;
}

.bookmark-text {
	display: flex;
	flex-direction: column;
}

.bookmark-info {
	flex: 4 1 180px;
	padding: 12px 14px 14px;
	display: flex;
	flex-direction: column;
	justify-content: space-between;
}

.bookmark-image {
	width: 33%;
	flex: 1 1 180px;
	display: block;
	position: relative;
	object-fit: cover;
	border-radius: 1px;
}

.bookmark-description {
	color: rgba(55, 53, 47, 0.6);
	font-size: 0.75em;
	overflow: hidden;
	max-height: 4.5em;
	word-break: break-word;
}

.bookmark-href {
	font-size: 0.75em;
	margin-top: 0.25em;
}

.sans { font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol"; }
.code { font-family: "SFMono-Regular", Consolas, "Liberation Mono", Menlo, Courier, monospace; }
.serif { font-family: Lyon-Text, Georgia, YuMincho, "Yu Mincho", "Hiragino Mincho ProN", "Hiragino Mincho Pro", "Songti TC", "Songti SC", "SimSun", "Nanum Myeongjo", NanumMyeongjo, Batang, serif; }
.mono { font-family: iawriter-mono, Nitti, Menlo, Courier, monospace; }
.pdf .sans { font-family: Inter, -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol", 'Twemoji', 'Noto Color Emoji', 'Noto Sans CJK SC', 'Noto Sans CJK KR'; }

.pdf .code { font-family: Source Code Pro, "SFMono-Regular", Consolas, "Liberation Mono", Menlo, Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK SC', 'Noto Sans Mono CJK KR'; }

.pdf .serif { font-family: PT Serif, Lyon-Text, Georgia, YuMincho, "Yu Mincho", "Hiragino Mincho ProN", "Hiragino Mincho Pro", "Songti TC", "Songti SC", "SimSun", "Nanum Myeongjo", NanumMyeongjo, Batang, serif, 'Twemoji', 'Noto Color Emoji', 'Noto Sans CJK SC', 'Noto Sans CJK KR'; }

.pdf .mono { font-family: PT Mono, iawriter-mono, Nitti, Menlo, Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK SC', 'Noto Sans Mono CJK KR'; }

.highlight-default {
}
.highlight-gray {
	color: rgb(155,154,151);
}
.highlight-brown {
	color: rgb(100,71,58);
}
.highlight-orange {
	color: rgb(217,115,13);
}
.highlight-yellow {
	color: rgb(223,171,1);
}
.highlight-teal {
	color: rgb(15,123,108);
}
.highlight-blue {
	color: rgb(11,110,153);
}
.highlight-purple {
	color: rgb(105,64,165);
}
.highlight-pink {
	color: rgb(173,26,114);
}
.highlight-red {
	color: rgb(224,62,62);
}
.highlight-gray_background {
	background: rgb(235,236,237);
}
.highlight-brown_background {
	background: rgb(233,229,227);
}
.highlight-orange_background {
	background: rgb(250,235,221);
}
.highlight-yellow_background {
	background: rgb(251,243,219);
}
.highlight-teal_background {
	background: rgb(221,237,234);
}
.highlight-blue_background {
	background: rgb(221,235,241);
}
.highlight-purple_background {
	background: rgb(234,228,242);
}
.highlight-pink_background {
	background: rgb(244,223,235);
}
.highlight-red_background {
	background: rgb(251,228,228);
}
.block-color-default {
	color: inherit;
	fill: inherit;
}
.block-color-gray {
	color: rgba(55, 53, 47, 0.6);
	fill: rgba(55, 53, 47, 0.6);
}
.block-color-brown {
	color: rgb(100,71,58);
	fill: rgb(100,71,58);
}
.block-color-orange {
	color: rgb(217,115,13);
	fill: rgb(217,115,13);
}
.block-color-yellow {
	color: rgb(223,171,1);
	fill: rgb(223,171,1);
}
.block-color-teal {
	color: rgb(15,123,108);
	fill: rgb(15,123,108);
}
.block-color-blue {
	color: rgb(11,110,153);
	fill: rgb(11,110,153);
}
.block-color-purple {
	color: rgb(105,64,165);
	fill: rgb(105,64,165);
}
.block-color-pink {
	color: rgb(173,26,114);
	fill: rgb(173,26,114);
}
.block-color-red {
	color: rgb(224,62,62);
	fill: rgb(224,62,62);
}
.block-color-gray_background {
	background: rgb(235,236,237);
}
.block-color-brown_background {
	background: rgb(233,229,227);
}
.block-color-orange_background {
	background: rgb(250,235,221);
}
.block-color-yellow_background {
	background: rgb(251,243,219);
}
.block-color-teal_background {
	background: rgb(221,237,234);
}
.block-color-blue_background {
	background: rgb(221,235,241);
}
.block-color-purple_background {
	background: rgb(234,228,242);
}
.block-color-pink_background {
	background: rgb(244,223,235);
}
.block-color-red_background {
	background: rgb(251,228,228);
}
.select-value-color-default { background-color: rgba(206,205,202,0.5); }
.select-value-color-gray { background-color: rgba(155,154,151, 0.4); }
.select-value-color-brown { background-color: rgba(140,46,0,0.2); }
.select-value-color-orange { background-color: rgba(245,93,0,0.2); }
.select-value-color-yellow { background-color: rgba(233,168,0,0.2); }
.select-value-color-green { background-color: rgba(0,135,107,0.2); }
.select-value-color-blue { background-color: rgba(0,120,223,0.2); }
.select-value-color-purple { background-color: rgba(103,36,222,0.2); }
.select-value-color-pink { background-color: rgba(221,0,129,0.2); }
.select-value-color-red { background-color: rgba(255,0,26,0.2); }

.checkbox {
	display: inline-flex;
	vertical-align: text-bottom;
	width: 16;
	height: 16;
	background-size: 16px;
	margin-left: 2px;
	margin-right: 5px;
}

.checkbox-on {
	background-image: url("data:image/svg+xml;charset=UTF-8,%3Csvg%20width%3D%2216%22%20height%3D%2216%22%20viewBox%3D%220%200%2016%2016%22%20fill%3D%22none%22%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%3E%0A%3Crect%20width%3D%2216%22%20height%3D%2216%22%20fill%3D%22%2358A9D7%22%2F%3E%0A%3Cpath%20d%3D%22M6.71429%2012.2852L14%204.9995L12.7143%203.71436L6.71429%209.71378L3.28571%206.2831L2%207.57092L6.71429%2012.2852Z%22%20fill%3D%22white%22%2F%3E%0A%3C%2Fsvg%3E");
}

.checkbox-off {
	background-image: url("data:image/svg+xml;charset=UTF-8,%3Csvg%20width%3D%2216%22%20height%3D%2216%22%20viewBox%3D%220%200%2016%2016%22%20fill%3D%22none%22%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%3E%0A%3Crect%20x%3D%220.75%22%20y%3D%220.75%22%20width%3D%2214.5%22%20height%3D%2214.5%22%20fill%3D%22white%22%20stroke%3D%22%2336352F%22%20stroke-width%3D%221.5%22%2F%3E%0A%3C%2Fsvg%3E");
}
	
</style></head><body><article id="29b27bdd-4ce9-402e-a742-b3e971ccf684" class="page sans"><header><div class="page-header-icon undefined"><img class="icon" src="%E1%84%8C%E1%85%A5%E1%86%BC%E1%84%92%E1%85%A7%E1%86%BC%E1%84%89%E1%85%B5%E1%86%A8%20(Hyung%20Sik%20Jeong)%2029b27bdd4ce9402ea742b3e971ccf684/20210108_201625.png"/></div><h1 class="page-title">정형식 (Hyung Sik Jeong)</h1></header><div class="page-body"><h2 id="9ab57fd6-d4c0-4a02-af66-167df7f2339b" class="">세계를 바라보는 모바일 개발자 </h2><p id="00a947c0-61a6-42a4-a7c5-744c70ee5d5b" class="">안녕하세요! 열린 마음의 개발 경력 4년차에 들어선 풀스택 지향 개발자입니다. 한국을 베이스 캠프 삼아 17개국을 여행, 단기 거주했으며 새로운 환경에 처하는 것을 사랑합니다 😎</p><p id="f5203f76-8415-4482-afa6-636b24e1ba7b" class="">🇨🇳🇯🇵🇵🇭🇲🇾🇬🇧🇩🇪🇫🇷🇦🇹🇨🇿🇭🇺🇮🇹🇧🇪🇳🇱🇨🇱🇦🇷🇵🇪🇺🇸</p><p id="94eda4b8-4173-4196-9918-91c13dc4194e" class="">
</p><p id="16f905ec-1c35-4f5a-858a-eefe89980944" class="">안드로이드 개발을 주로 하고 있지만 php, mysql 등 서버 측 언어에도 익숙합니다.</p><p id="9113860c-d93b-44d0-b7bc-907c7d848074" class="">어플리케이션 개발, 운영에 필요한 기술 등에 익숙하며 새로운 기술을 받아들이는데 거부감이 없습니다. 현재 코틀린과 자바로 작업하며, 따로 플러터를 공부 중입니다.</p><p id="386bf145-161c-454e-af17-c5319ab95a5e" class="">웹개발도 가능하고 웹뷰로 서비스 운영해본 경험이 있습니다.</p><p id="6365b730-f9d7-479c-ae84-d46f107ec088" class="">스타트업에서 글로벌 유저를 타게팅한 웹사이트, 안드로이드 어플리케이션을 기획 단계부터 참여, 개발한 경험이 있으며, 디자이너, 개발자, 기획자와의 원활한 의사소통을 자신합니다.</p><h3 id="19168c79-9cc9-4fcc-a804-be286184929a" class="">👨‍💻 Career</h3><ul id="db0204ce-b48e-4002-8c39-99f50043073b" class="bulleted-list"><li>dico ( 2018.01.01 ~ 2019.01.31)<ul id="8d39b7e2-c5c0-4054-a901-cc07d39fd603" class="bulleted-list"><li>마지막 3개월은 칠레에서 현지인과 영어로 업무</li></ul></li></ul><ul id="897dc5a5-d7a1-40ae-8eed-106bcec988f1" class="bulleted-list"><li>프리랜서(2019.02.26~ 2019.12.31)<ul id="2f7a98cb-6e25-4309-8016-e2cfa215f288" class="bulleted-list"><li>기 개발된 해외 몰 안내앱 등 안드로이드 3종 앱 수정<ul id="5529bd43-daed-44b9-887c-f289dff46d6d" class="bulleted-list"><li>약 5년 전에 개발된 코드 라이브러리 최신화 및 빌드 가능하도록 오류 수정</li></ul></li></ul><ul id="c77ddb1c-852c-43dc-8580-d0ff06f8fe0a" class="bulleted-list"><li>중년 타겟팅 소개팅 어플 자기야 디자인 변경 및 기능 추가</li></ul></li></ul><ul id="c5fe4a2a-5570-4d8c-861b-68b285a9dd38" class="bulleted-list"><li>(주)상현  ( 2020.01.01 ~2020.12.28 )<ul id="7c0a6a43-fed7-4758-9c6c-a6771435227f" class="bulleted-list"><li>기존 외주 클라이언트사</li></ul></li></ul><ul id="10f30acf-9562-4d76-b11c-f02bcd1a56a3" class="bulleted-list"><li>이수시스템(2021.03~07)<ul id="89ee1a09-f43d-47da-b238-41b989e78587" class="bulleted-list"><li>SK케미칼 통합바코드 시스템 구축<ul id="4479ac23-0fa0-43e1-8f09-093f7e1374b5" class="bulleted-list"><li>100페이지 분량의 화면 개발, api 연동</li></ul><ul id="194e5355-e44c-4885-933d-2aa8a5915c3e" class="bulleted-list"><li>mvvm패턴, databinding, livedata, retrofit2 사용</li></ul></li></ul></li></ul><h3 id="7679cdb4-9158-44e5-9f99-c8b1e1b8f9cb" class="">🏆 Prize</h3><ul id="88ebeb68-873c-43ca-84e6-7899c9c794d3" class="bulleted-list"><li>2014 대한전기학회 하계학술대회 미니드론 자율비행 경진대회 금상 수상<ul id="e2f0c42e-e2ff-48aa-ab9f-823a284562b8" class="bulleted-list"><li><a href="http://www.konkuk.ac.kr/do/MessageBoard/ArticleRead.do?forum=people&amp;sort=6&amp;id=5b0f4fa">http://www.konkuk.ac.kr/do/MessageBoard/ArticleRead.do?forum=people&amp;sort=6&amp;id=5b0f4fa</a></li></ul></li></ul><hr id="da2b1386-bf48-4028-b7ab-07c48b8dbd69"/><h2 id="9dd9d48d-9ce5-4333-ae83-3d80843850d3" class="">📚 Stack</h2><p id="4bd5f94e-e224-4aa3-8011-c8832ff3de36" class="">다룰 수 있는 기술/언어/프레임워크들입니다.</p><ul id="63e54932-636d-4d05-aab9-bd6670288801" class="bulleted-list"><li>Java</li></ul><ul id="fb86a378-8050-47ad-b77d-5d2ade357724" class="bulleted-list"><li>Kotlin</li></ul><ul id="c9b802fb-61ab-433f-99af-11fd2d695bc0" class="bulleted-list"><li>Android Studio<ul id="6092e1de-25e5-4b4a-98c0-df59e85b7208" class="bulleted-list"><li>databinding</li></ul><ul id="6bd17bda-98f8-46ae-a45d-119b90d016d8" class="bulleted-list"><li>retrofit2</li></ul><ul id="74180a15-bf9b-4183-9e58-0b150f8b0722" class="bulleted-list"><li>LiveData</li></ul><ul id="46557c4b-1ac1-40ae-9bba-67f167f3756f" class="bulleted-list"><li>sqlite, Room</li></ul></li></ul><ul id="df2cfb4e-9744-4a66-a798-e4cccc3aeafc" class="bulleted-list"><li>MVC, MVVM design pattern</li></ul><ul id="5ca2967a-cfa3-436a-b8fe-91159b787723" class="bulleted-list"><li>Mysql</li></ul><ul id="ac4be0ef-3c6a-49f1-ae61-50ef93a9013c" class="bulleted-list"><li>HTML/CSS</li></ul><ul id="82bf1c17-c168-449c-b0e0-caa624bb18b2" class="bulleted-list"><li>JavaScript</li></ul><ul id="9b7cd6ab-b85b-4748-bc5d-cd97f0e9b73e" class="bulleted-list"><li>php</li></ul><ul id="14bf7f3d-b21b-4150-823e-c96570217ee9" class="bulleted-list"><li>CodeIgniter</li></ul><ul id="7bc0affd-f8c6-48dd-8fc4-9056cb6bbe78" class="bulleted-list"><li>Bootstrap</li></ul><ul id="25e9d70f-454f-42f1-9787-09fb6fff3620" class="bulleted-list"><li>FCM</li></ul><ul id="e60db452-6b3b-4695-a1bc-b4f6be17fe41" class="bulleted-list"><li>AWS</li></ul><ul id="377231b8-26e1-4723-b403-d863b6abd404" class="bulleted-list"><li>Google Analytics</li></ul><hr id="2aa46bb6-ce45-4ff4-86bb-bda22907617b"/><h2 id="c958300e-5937-498b-9153-4d57c5237997" class="">🌎 Project</h2><p id="f93e5239-a37f-4d50-8f31-462b26b3f43a" class="">제가 진행한 토이 프로젝트 및 회사 프로젝트입니다.</p><h3 id="6b547e25-c16f-42f1-9105-36b84bd059f5" class="">개인</h3><figure id="9b2a763a-85ef-4e6e-adc1-8af0736d5f51" class="link-to-page"><a href="https://www.notion.so/9b2a763a85ef4e6eadc18af0736d5f51"><span class="icon">🧳</span>여행일기</a></figure><figure id="099261e7-3686-4b62-8882-e35090664a2d" class="link-to-page"><a href="https://www.notion.so/099261e736864b628882e35090664a2d"><span class="icon">✝️</span>문단암송</a></figure><p id="8a8f170a-b81a-4168-8432-a7de91cbce39" class="">
</p><h3 id="26e18613-0be7-4eec-889b-e1381a78ff63" class="">회사</h3><figure id="18f1f47b-27ff-40cd-a40e-6c94dc3ccf0f" class="link-to-page"><a href="https://www.notion.so/DICO-18f1f47b27ff40cda40e6c94dc3ccf0f"><span class="icon">🇪🇸</span>DICO</a></figure><figure id="cecf88d4-f69e-4560-94f5-eb8fc23cb32c" class="link-to-page"><a href="https://www.notion.so/cecf88d4f69e456094f5eb8fc23cb32c"><span class="icon">😍</span>자기야</a></figure><h2 id="4e59cc4c-e6d9-4a4b-852a-618990c74a73" class="">👨🏼‍🎓Graduation Project</h2><p id="270dd590-1839-465d-8b71-06fd3b5bd5b0" class="">졸업작품으로 PID 적응 제어 기법을 적용한 고속 라인트레이서를 개발 하였습니다. 졸업 논문을 쓰기 위한 프로젝트로 학부 과정에서 배운 제어공학이나 회로이론 등 이론의 영역에 있던 지식들을 적용해 볼 수 있었습니다.</p><h3 id="42845db4-c6df-4920-ba41-a114e36d25bb" class=""><strong>맡은 역할</strong></h3><ul id="a0653d52-93d0-4cf3-8ef1-38652bac63e3" class="bulleted-list"><li>모터 드라이브 하드웨어 디버깅 및 수정</li></ul><ul id="1ea44798-fe2b-498d-8061-d0f7a33f8644" class="bulleted-list"><li>센서부 설계 및 납땜</li></ul><ul id="30095aea-e6ce-4fbe-a4e5-4646a8c1ae5c" class="bulleted-list"><li>적응 PID 제어 알고리즘 프로그래밍</li></ul><ul id="71b6af85-1e94-4936-80c8-fb9eb686edbf" class="bulleted-list"><li>주행 관련 수식 계산</li></ul><ul id="d79e4863-5c64-4bcc-949f-f1b286320acf" class="bulleted-list"><li>관련 논문 검색 및 부품 주문</li></ul><p id="99307f7a-ee57-4400-be6e-280b7924d547" class=""><a href="https://drive.google.com/open?id=1phR6k1FN-pGBf93MMg_kPwqi7U0BgAaX">영상 링크</a></p><h3 id="94d28a9a-adec-4026-add6-c9054cdade5b" class=""><a href="mailto:leegun2003@gmail.com">📧 devDoma</a><a href="mailto:devdoma3904@gmail.com">3904@gmail.com</a></h3><p id="487e8242-8c04-47f2-9a0d-1d9ab9fa23cf" class="">
</p></div></article></body></html>
