# Iconpicker for Bootstrap 5

### Usage

**1** - Just download the git repo and get file under dist directory and import it:

```
<script src="/path/to/biconpicker.js"></script>
```

**2** - Install via **npm**

```
npm i biconpicker

import Biconpicker from 'biconpicker'
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
});
```

**You can check the example folder for demonstration**
