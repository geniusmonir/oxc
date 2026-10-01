# edge-cases/xxx-in-md/css-top-level-declaration.md

## Option 1

`````json
{"printWidth":80}
`````

### Diff

`````diff
===================================================================
--- prettier
+++ oxfmt
@@ -1,3 +1,3 @@
 ```css
-background-image: url("a.png");
+background-image:   url("a.png");
 ```

`````

### Actual (oxfmt)

`````md
```css
background-image:   url("a.png");
```

`````

### Expected (prettier)

`````md
```css
background-image: url("a.png");
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
@@ -1,3 +1,3 @@
 ```css
-background-image: url("a.png");
+background-image:   url("a.png");
 ```

`````

### Actual (oxfmt)

`````md
```css
background-image:   url("a.png");
```

`````

### Expected (prettier)

`````md
```css
background-image: url("a.png");
```

`````
