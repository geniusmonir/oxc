# externals/prettier/markdown/code/mdn-import.md

## Option 1

`````json
{"printWidth":80}
`````

### Diff

`````diff
===================================================================
--- prettier
+++ oxfmt
@@ -1,7 +1,7 @@
 ```css
 @import url("gridy.css") supports(display: grid) screen and (max-width: 400px);
-@import url("flexy.css") supports(not (display: grid) and (display: flex))
-  screen and (max-width: 400px);
+@import url("flexy.css") supports(not(display: grid) and (display: flex)) screen
+  and (max-width: 400px);
 @import url("whatever.css")
-supports((selector(h2 > p)) and (font-tech(color-COLRv1)));
+  supports((selector(h2 > p)) and (font-tech(color-COLRv1)));
 ```

`````

### Actual (oxfmt)

`````md
```css
@import url("gridy.css") supports(display: grid) screen and (max-width: 400px);
@import url("flexy.css") supports(not(display: grid) and (display: flex)) screen
  and (max-width: 400px);
@import url("whatever.css")
  supports((selector(h2 > p)) and (font-tech(color-COLRv1)));
```

`````

### Expected (prettier)

`````md
```css
@import url("gridy.css") supports(display: grid) screen and (max-width: 400px);
@import url("flexy.css") supports(not (display: grid) and (display: flex))
  screen and (max-width: 400px);
@import url("whatever.css")
supports((selector(h2 > p)) and (font-tech(color-COLRv1)));
```

`````

## Option 2

`````json
{"printWidth":100,"proseWrap":"always"}
`````

### Diff

`````diff
===================================================================
--- prettier
+++ oxfmt
@@ -1,6 +1,6 @@
 ```css
 @import url("gridy.css") supports(display: grid) screen and (max-width: 400px);
-@import url("flexy.css") supports(not (display: grid) and (display: flex)) screen and
+@import url("flexy.css") supports(not(display: grid) and (display: flex)) screen and
   (max-width: 400px);
 @import url("whatever.css") supports((selector(h2 > p)) and (font-tech(color-COLRv1)));
 ```

`````

### Actual (oxfmt)

`````md
```css
@import url("gridy.css") supports(display: grid) screen and (max-width: 400px);
@import url("flexy.css") supports(not(display: grid) and (display: flex)) screen and
  (max-width: 400px);
@import url("whatever.css") supports((selector(h2 > p)) and (font-tech(color-COLRv1)));
```

`````

### Expected (prettier)

`````md
```css
@import url("gridy.css") supports(display: grid) screen and (max-width: 400px);
@import url("flexy.css") supports(not (display: grid) and (display: flex)) screen and
  (max-width: 400px);
@import url("whatever.css") supports((selector(h2 > p)) and (font-tech(color-COLRv1)));
```

`````
