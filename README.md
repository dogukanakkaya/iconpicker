# Iconpicker for Bootstrap 5

### Usage

**1** - Via **cdn**

```js
<script src="https://unpkg.com/codethereal-iconpicker@1.2.1/dist/iconpicker.js"></script>
```

**2** - Via **npm**

```
npm i codethereal-iconpicker
```

```js
import Iconpicker from 'codethereal-iconpicker'
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
(async () => {
    const response = await fetch('https://unpkg.com/codethereal-iconpicker@1.2.1/dist/iconsets/bootstrap5.json')
    const result = await response.json()

    const iconpicker = new Iconpicker(document.querySelector(".iconpicker"), {
        icons: result,
        showSelectedIn: document.querySelector(".selected-icon"),
        searchable: true,
        selectedClass: "selected",
        containerClass: "my-picker",
        hideOnSelect: true,
        fade: true,
        defaultValue: 'bi-alarm',
        valueFormat: val => `bi ${val}`
    });

    iconpicker.set() // Set as empty
    iconpicker.set('bi-alarm') // Reset with a value
})()
```

**Use with font awesome**
```js
(async () => {
  const response = await fetch('https://unpkg.com/codethereal-iconpicker@1.2.1/dist/iconsets/fontawesome4.json')
  const result = await response.json()

  new Iconpicker(document.querySelector(".iconpicker"), {
    icons: result,
    valueFormat: val => `fa ${val}`
  })
})()
```
