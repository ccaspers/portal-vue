# PortalVue

> A Portal Component for Vuejs, to render DOM outside of a component, anywhere in the document.

## This is the README of the 2.0.0-beta `next`-branch

<p style="tex-align: center">
  <img src="http://linusborg.github.io/portal-vue/assets/logo.png" alt="PortalVue Logo">
</p>

> Install with `npm install portal-vue`

For more detailed documentation and additional Information, please visit <a href="https://portal-vue-next-preview.netlify.com/">the docs for this beta</a>

## Installation

```bash
npm i portal-vue@next

# or

yarn add portal-vue@nxt
```

```javascript
import PortalVue from 'portal-vue'
Vue.use(PortalVue)
```

## Usage

```html
<portal to="destination">
  <p>This slot content will be rendered wherever the <portal-target> with name 'destination'
    is  located.</p>
</portal>

<portal-target name="destination">
  <!--
  This component can be located anwhere in your App.
  The slot content of the above portal component will be rendered here.
  -->
</portal-target>
```

## Nuxt module

Add `portal-vue/nuxt` to modules section of `nuxt.config.js`

```javascript
{
  modules: ['portal-vue/nuxt']
}
```
