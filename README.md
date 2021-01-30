# Iconpicker for Bootstrap 5

### Usage

**1** - Via **cdn** (latest)

```js
<script src="http://cdn.codethereal.com/biconpicker/dist/biconpicker.js"></script>
```

**2** - Via **npm**

```
npm i biconpicker
```

```js
import Biconpicker from 'biconpicker'
```

**3** - Or just download the git repo and get file under dist directory and import it

```js
<script src="/path/to/biconpicker.js"></script>
```


```js
new Biconpicker(document.querySelector(".biconpicker"));
new Biconpicker(document.querySelector(".biconpicker"), options);
document.querySelectorAll('.biconpicker').forEach(picker => new Biconpicker(picker))
```


**Options**
```js
new Biconpicker(document.querySelector(".biconpicker"), {
  prefix: "bi-", // default: bi- (class prefix for selected icon let's say you pass it as 'ds' will return you ds-alarm)
  //icons: [], // default: all of the icons (icon set if you want to use only some of them)
  showSelectedIn: document.querySelector(".selected-bicon"), // default: none (element to show selected icon)
  searchable: true, // default: true (use the input as a search box)
  selectedClass: "selected", // default: true (selected icon class)
  containerClass: "my-picker", // default: (container class of biconpicker)
  hideOnSelect: true // default true (hides the dropdown on select)
});
```

![biconpicker](http://cdn.codethereal.com/biconpicker/demo.png)
