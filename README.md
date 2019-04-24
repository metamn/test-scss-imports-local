# Testing SCSS Imports Local

## Defaults

No global imports (Only the framework).
Every file imports the mixins needed.

## CSS file size

### Initial state

Articles added and styled

- `project` has 13 mixins
- `pages/home` has 3 thumbs and 3 full articles
- CSS file size: 63K

```
cs@cs-swift:~/work/test-scss-imports$ ls -alh production/assets/styles/site.min.css
-rw-r--r-- 1 cs cs 63K Apr 24 17:23 production/assets/styles/site.min.css
```

### More articles

- `pages/home` has 7 thumbs and 6 full articles
- CSS file size: 63K

```
cs@cs-swift:~/work/test-scss-imports$ ls -alh production/assets/styles/site.min.css
-rw-r--r-- 1 cs cs 63K Apr 24 17:23 production/assets/styles/site.min.css
```

### Article template

- Added `code/pages/delivering-the-message`
- And the corresponing template: `code/framework/templates/article`
- CSS file size: 90K

```
cs@cs-swift:~/work/test-scss-imports-local$ ls -alh production/assets/styles/site.min.css
-rw-r--r-- 1 cs cs 90K Apr 24 18:33 production/assets/styles/site.min.css
```

### Article template + homepage content

- Homepage content and styling added to Article template
- CSS file size: 148K

```
cs@cs-swift:~/work/test-scss-imports-local$ ls -alh production/assets/styles/site.min.css
-rw-r--r-- 1 cs cs 148K Apr 24 18:51 production/assets/styles/site.min.css
```

### Remove minification

- CSS file size: 467K

```
cs@cs-swift:~/work/test-scss-imports-local$ ls -alh production/assets/styles/site.min.css
-rw-r--r-- 1 cs cs 467K Apr 24 18:56 production/assets/styles/site.min.css
```
