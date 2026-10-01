# externals/prettier/markdown/code/mdn-grid-auto-columns.md

## Option 1

`````json
{"printWidth":80}
`````

### Diff

`````diff
===================================================================
--- prettier
+++ oxfmt
@@ -1,10 +1,10 @@
 ```css
+
 /* multiple track-size values */
 grid-auto-columns: min-content max-content auto;
 grid-auto-columns: 100px 150px 390px;
 grid-auto-columns: 10% 33.3%;
 grid-auto-columns: 0.5fr 3fr 1fr;
-grid-auto-columns: minmax(100px, auto) minmax(max-content, 2fr)
-  minmax(20%, 80vmax);
-grid-auto-columns: 100px minmax(100px, auto) 10% 0.5fr fit-content(400px);
+grid-auto-columns: minmax(100px, auto)    minmax(max-content, 2fr) minmax(20%, 80vmax);
+grid-auto-columns: 100px minmax(100px, auto)        10% 0.5fr fit-content(400px);
 ```

`````

### Actual (oxfmt)

`````md
```css

/* multiple track-size values */
grid-auto-columns: min-content max-content auto;
grid-auto-columns: 100px 150px 390px;
grid-auto-columns: 10% 33.3%;
grid-auto-columns: 0.5fr 3fr 1fr;
grid-auto-columns: minmax(100px, auto)    minmax(max-content, 2fr) minmax(20%, 80vmax);
grid-auto-columns: 100px minmax(100px, auto)        10% 0.5fr fit-content(400px);
```

`````

### Expected (prettier)

`````md
```css
/* multiple track-size values */
grid-auto-columns: min-content max-content auto;
grid-auto-columns: 100px 150px 390px;
grid-auto-columns: 10% 33.3%;
grid-auto-columns: 0.5fr 3fr 1fr;
grid-auto-columns: minmax(100px, auto) minmax(max-content, 2fr)
  minmax(20%, 80vmax);
grid-auto-columns: 100px minmax(100px, auto) 10% 0.5fr fit-content(400px);
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
@@ -1,9 +1,10 @@
 ```css
+
 /* multiple track-size values */
 grid-auto-columns: min-content max-content auto;
 grid-auto-columns: 100px 150px 390px;
 grid-auto-columns: 10% 33.3%;
 grid-auto-columns: 0.5fr 3fr 1fr;
-grid-auto-columns: minmax(100px, auto) minmax(max-content, 2fr) minmax(20%, 80vmax);
-grid-auto-columns: 100px minmax(100px, auto) 10% 0.5fr fit-content(400px);
+grid-auto-columns: minmax(100px, auto)    minmax(max-content, 2fr) minmax(20%, 80vmax);
+grid-auto-columns: 100px minmax(100px, auto)        10% 0.5fr fit-content(400px);
 ```

`````

### Actual (oxfmt)

`````md
```css

/* multiple track-size values */
grid-auto-columns: min-content max-content auto;
grid-auto-columns: 100px 150px 390px;
grid-auto-columns: 10% 33.3%;
grid-auto-columns: 0.5fr 3fr 1fr;
grid-auto-columns: minmax(100px, auto)    minmax(max-content, 2fr) minmax(20%, 80vmax);
grid-auto-columns: 100px minmax(100px, auto)        10% 0.5fr fit-content(400px);
```

`````

### Expected (prettier)

`````md
```css
/* multiple track-size values */
grid-auto-columns: min-content max-content auto;
grid-auto-columns: 100px 150px 390px;
grid-auto-columns: 10% 33.3%;
grid-auto-columns: 0.5fr 3fr 1fr;
grid-auto-columns: minmax(100px, auto) minmax(max-content, 2fr) minmax(20%, 80vmax);
grid-auto-columns: 100px minmax(100px, auto) 10% 0.5fr fit-content(400px);
```

`````
