# CSS Global Reset

CSS Global Reset reset.css link to copy :-

<a href="https://raw.githubusercontent.com/mustafaabobakr/CSS-Global-Reset/master/reset.css" download>reset.css</a>

```html
<link rel="stylesheet" href="https://raw.githubusercontent.com/mustafaabobakr/CSS-Global-Reset/master/reset.css" />
```

![preview pic](https://github.com/mostafaabobakr7/CSS-Global-Reset/blob/master/reset%20css.jpg)

```
reset.css
```

```css
:root {
	--scrollbar-width: 7px;
	--scrollbar-radius: 16px;
	--scrollbar-bg: #fff;
	--scrollbar-thumb: #babac0;
	--scrollbar-thumb-hover: #a0a0a5;
	--scrollbar-thumb-active: #7f7f85;
	--scrollbar-track: #f4f4f4;
	--scrollbar-track-hover: #e4e4e4;
	--scrollbar-track-active: #d4d4d4;

	--selection-bg: #02124e;
	--selection-color: #fff;

	--mark-bg: yellow;
	--mark-color: black;
	--blockquote-bg: #f9f9f9;
	--blockquote-border: 10px solid #ccc;
	--blockquote-color: #ccc;
}
*,
*::after,
*::before {
	margin: 0;
	padding: 0;
	border: 0 solid transparent;
	-webkit-box-sizing: inherit;
	box-sizing: inherit;
	background-repeat: no-repeat;
	overflow-wrap: break-word;
	word-wrap: break-word;
	word-break: break-word;
	-webkit-font-smoothing: antialiased;
}

::-webkit-scrollbar {
	background-color: var(--scrollbar-bg)
	width: var(--scrollbar-width);
}
::-webkit-scrollbar-track {
	background-color: var(--scrollbar-track);
}
::-webkit-scrollbar-track:hover {
	background-color: var(--scrollbar-track-hover);
}
::-webkit-scrollbar-thumb {
	background-color: var(--scrollbar-thumb);
	border-radius: var(--scrollbar-radius);
	border: 1px solid var(--scrollbar-bg);
}
::-webkit-scrollbar-thumb:hover {
	background-color: var(--scrollbar-thumb-hover);
	border: 1px solid var(--scrollbar-bg);
}
::-webkit-scrollbar-button {
	display: none;
}

::-moz-selection {
	color: var(--selection-bg);
	background: var(--selection-color);
}

::selection {
	color: var(--selection-bg);
	background: var(--selection-color);
}
html {
	scroll-behavior: smooth;
}

body {
	cursor: default;
	margin: 0 !important;
	padding: 0 !important;
	-webkit-box-sizing: border-box;
	box-sizing: border-box;
	print-color-adjust: exact !important;
	-webkit-print-color-adjust: exact !important;
	-webkit-text-size-adjust: 100%;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
	scroll-behavior: smooth;
	text-rendering: optimizeSpeed;
}

html,
body,
#root {
	min-block-size: 100vh;
}

body.modal-open {
	/* when modal opens body:scroll disappear tat leads to width of scroll=0 so body width expand */
	overflow: visible;
}

main {
	min-block-size: 50vh;
}

ul li {
	list-style: none;
}

a {
	cursor: pointer;
	display: inline-flex;
	text-decoration: none !important;
}

a:not([class]) {
	text-decoration-skip-ink: auto;
}
a > * {
	/* for icons inside links when dealing with Event in JS */
	pointer-events: none;
}

picture,
img {
	-o-object-fit: cover;
	object-fit: cover;
	-webkit-user-select: none;
	-khtml-user-select: none;
	-moz-user-select: none;
	-o-user-select: none;
	-ms-user-select: none;
	user-select: none;
	-webkit-user-drag: none;
	-khtml-user-drag: none;
	-moz-user-drag: none;
	-o-user-drag: none;
	-ms-user-drag: none;
	user-drag: none;

	display: block;
	max-inline-size: 100%;
	/* https://x.com/csswizardry/status/1717841334462005661 */
	block-size: auto;
	vertical-align: middle;
	font-style: italic;
	background-repeat: no-repeat;
	background-size: cover;
	shape-margin: 0.75rem;
}

audio,
canvas,
embed,
iframe,
img,
object,
svg,
video {
	display: block;
	vertical-align: middle;
}

section,
article,
aside {
	display: flex;
	inline-size: 100%;
}

[hidden] {
	display: none !important;
}
[disabled],
.disabled {
	cursor: not-allowed !important;
	pointer-events: none !important;
	opacity: 0.5;
}

[type="text"],
[type="password"],
[type="email"],
[type="search"],
[type="url"],
[title="tel"],
[title="number"],
[title="time"],
[title="date"],
[title="datetime"],
[title="datetime-local"],
[title="month"],
[title="week"],
[title="image"],
[title="file"],
[type="button"],
[type="reset"],
[type="submit"],
button,
select,
textarea {
	font-family: inherit;
	color: inherit;
}

.btn,
[type="button"],
[type="reset"],
[type="submit"],
button {
	-webkit-appearance: button;
	border: none;
	cursor: pointer;
	display: inline-flex;
	justify-content: center;
	align-items: center;
}

.btn i,
.btn span,
[type="button"] i,
[type="button"] span,
[type="reset"] i,
[type="reset"] span,
[type="submit"] i,
[type="submit"] span,
button i,
button span {
	pointer-events: none;
}

input[type="search"] {
	-webkit-appearance: textfield;
	outline-offset: -2px;
}

::-webkit-file-upload-button {
	-webkit-appearance: button;
	font-family: inherit;
}
option[value=""][disabled],
option.placeholder {
	display: none;
}

mark {
	background-color: var(--mark-bg);
	color: var(--mark-color);
}

blockquote {
	margin: 1.5em 0;
	padding: 0.5em 10px;
	position: relative;
	font-style: italic;
	background: var(--blockquote-bg);
	border-inline-start: var(--blockquote-border);
}
blockquote::before,
blockquote::after {
	color: var(--blockquote-color);
	font-size: 4em;
	line-height: 0.1em;
	vertical-align: -0.4em;
}

blockquote::before {
	content: open-quote;
}

blockquote::after {
	content: close-quote;
}

```
