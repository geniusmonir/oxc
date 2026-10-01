# externals/prettier/markdown/code/mdn-background-2.md

## Option 1

`````json
{"printWidth":80}
`````

### Diff

`````diff
===================================================================
--- prettier
+++ oxfmt
@@ -1,5 +1,10 @@
 ```css
-background-image:
-  linear-gradient(to bottom, rgb(255 255 0 / 50%), rgb(0 0 255 / 50%)),
-  url("catfront.png");
+
+
+
+background-image: linear-gradient(
+    to bottom,
+              rgb(255 255 0 / 50%),
+ rgb(0 0 255 / 50%)
+  ), url("catfront.png");
 ```

`````

### Actual (oxfmt)

`````md
```css



background-image: linear-gradient(
    to bottom,
              rgb(255 255 0 / 50%),
 rgb(0 0 255 / 50%)
  ), url("catfront.png");
```

`````

### Expected (prettier)

`````md
```css
background-image:
  linear-gradient(to bottom, rgb(255 255 0 / 50%), rgb(0 0 255 / 50%)),
  url("catfront.png");
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
@@ -1,4 +1,10 @@
 ```css
-background-image:
-  linear-gradient(to bottom, rgb(255 255 0 / 50%), rgb(0 0 255 / 50%)), url("catfront.png");
+
+
+
+background-image: linear-gradient(
+    to bottom,
+              rgb(255 255 0 / 50%),
+ rgb(0 0 255 / 50%)
+  ), url("catfront.png");
 ```

`````

### Actual (oxfmt)

`````md
```css



background-image: linear-gradient(
    to bottom,
              rgb(255 255 0 / 50%),
 rgb(0 0 255 / 50%)
  ), url("catfront.png");
```

`````

### Expected (prettier)

`````md
```css
background-image:
  linear-gradient(to bottom, rgb(255 255 0 / 50%), rgb(0 0 255 / 50%)), url("catfront.png");
```

`````
