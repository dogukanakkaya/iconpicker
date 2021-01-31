# Iconpicker for Bootstrap 5 (Also you can use it with fontawesome of any other using valueFormat option)

### Usage

**1** - Via **cdn** (latest)

```js
<script src="http://cdn.codethereal.com/iconpicker/dist/iconpicker.js"></script>
```

**2** - Via **npm**

```
npm i biconpicker
```

```js
import Iconpicker from 'iconpicker'
```

**3** - Or just download the git repo and get file under dist directory and import it

```js
<script src="/path/to/iconpicker.js"></script>
```


```js
new Iconpicker(document.querySelector(".iconpicker"));
new Iconpicker(document.querySelector(".iconpicker"), options);
document.querySelectorAll('.iconpicker').forEach(picker => new Iconpicker(picker))
```


**Options**
```js
new Iconpicker(document.querySelector(".iconpicker"), {
  //icons: [], // default: all of the icons (icon set if you want to use only some of them)
  showSelectedIn: document.querySelector(".selected-icon"), // default: none (element to show selected icon)
  searchable: true, // default: true (use the input as a search box)
  selectedClass: "selected", // default: true (selected icon class)
  containerClass: "my-picker", // default: (container class of biconpicker)
  hideOnSelect: true, // default true (hides the dropdown on select)
  fade: true, // default: false (fade animation)
  defaultValue: 'bi-alarm', // default: (default value)
  valueFormat: val => `bi ${val}` // default: bi ${val} (format the value instead of prefix in previous versions)
});
```

**Use with font awesome**
```js
new Iconpicker(document.querySelector(".iconpicker"), {
  icons: ['fa-times', 'fa-check'],
  valueFormat: val => `fa ${val}`
```

![iconpicker](http://cdn.codethereal.com/iconpicker/demo.png)
