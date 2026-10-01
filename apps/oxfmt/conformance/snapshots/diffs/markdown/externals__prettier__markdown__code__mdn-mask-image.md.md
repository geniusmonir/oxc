# externals/prettier/markdown/code/mdn-mask-image.md

## Option 1

`````json
{"printWidth":80}
`````

### Diff

`````diff
===================================================================
--- prettier
+++ oxfmt
@@ -1,5 +1,5 @@
 ```css
+
 /* Multiple values */
-mask-image:
-  image(url(mask.png), skyblue), linear-gradient(rgb(0 0 0 / 100%), transparent);
+mask-image: image(url(mask.png), skyblue),                          linear-gradient(rgb(0 0 0 / 100%), transparent);
 ```

`````

### Actual (oxfmt)

`````md
```css

/* Multiple values */
mask-image: image(url(mask.png), skyblue),                          linear-gradient(rgb(0 0 0 / 100%), transparent);
```

`````

### Expected (prettier)

`````md
```css
/* Multiple values */
mask-image:
  image(url(mask.png), skyblue), linear-gradient(rgb(0 0 0 / 100%), transparent);
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
@@ -1,4 +1,5 @@
 ```css
+
 /* Multiple values */
-mask-image: image(url(mask.png), skyblue), linear-gradient(rgb(0 0 0 / 100%), transparent);
+mask-image: image(url(mask.png), skyblue),                          linear-gradient(rgb(0 0 0 / 100%), transparent);
 ```

`````

### Actual (oxfmt)

`````md
```css

/* Multiple values */
mask-image: image(url(mask.png), skyblue),                          linear-gradient(rgb(0 0 0 / 100%), transparent);
```

`````

### Expected (prettier)

`````md
```css
/* Multiple values */
mask-image: image(url(mask.png), skyblue), linear-gradient(rgb(0 0 0 / 100%), transparent);
```

`````
