# vue-scroll-outside

Vue directive to react on clicks outside an element. Great for closing popovers, menus among other things.

## Install

```
$ npm install --save vue-scroll-outside
```

## Use

```
import Vue from 'vue'
import ScrollOutside from 'vue-scroll-outside'

Vue.directive('scroll-outside', ScrollOutside)
```

```
<script>
  export default {
    methods: {
      scrollEvent (event) {
        console.log('Scroll outside. Event: ', event)
      }
    }
  }
</script>

<template>
  <div v-click-outside="scrollEvent"></div>
</template>
```
