# jp-split

A small and understandable split view witch supports both horizontal and vertical splittings.

## Install

```
npm install @satachito/jp-split --save
```

## HTML

Include jp-split.js at the very bottom of the <body> tag.

```
---------------- BarH
<style>
#BarH {
;	height			: 200px
}
#BarH > div {
;	background		: grey
;	cursor			: col-resize
}
</style>
<jp-split-h id=BarH grid-template="1fr 4px 1fr">
	<textarea></textarea>
	<div></div>
	<textarea></textarea>
</jp-split-h>

<script>
Array.from( document.getElementsByTagName( 'textarea' ) ).forEach(
	$ => $.textContent = 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.'
)
</script>
<script src=node-modules/@satachito/jp-split.js></script>
```

