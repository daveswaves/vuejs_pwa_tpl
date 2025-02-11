# Vue JS PWA (Progressive Web App) Template

## Clones a blank Vue JS template, pre installed with the following:

```json
axios
pinia
vue-router
autoprefixer
postcss
tailwindcss
```

## App.vue

Imports `RouterLink` & `RouterView` from `vue-router`.

RouterLink is used to navigate to `HomeView` or `AboutView`.

<RouterView /> (built-in component from Vue Router) dynamically renders the matched component based on the current route.

The main `template` `div` tag uses the following Tailwind classes for darkMode:

```html
<template>
  <div class="min-h-screen bg-white text-black dark:bg-gray-900 dark:text-white">
```
Note:  
The `tailwind.config.js` file needs to include `darkMode: "class"` for this to work (see `tailwind.config.js` section below).  
`index.html` also requires the following:
```html
<body class="dark">
```

## router/index.js

Imports views/HomeView.vue and views/AboutView.vue components.

Passes 'msg' prop to the HomeView component.

## views/HomeView.vue

```html
<!-- Receives prop from router script. -->
<script setup>
defineProps({
  msg: {
    type: String,
    required: true,
  },
})
</script>

<template>
  ...
    <!-- Display 'msg' prop -->
    {{ msg }}
  ...
</template>
```

## tailwind.config.js

```js
// Includes darkMode: "class"
export default {
  darkMode: "class",
  ...
```
