<template>
    <div>
        <base-header />
        <slot></slot>
        <base-footer />
  </div>
</template>

<script>
  import BaseHeader from './BaseHeader.vue'
  import BaseFooter from './BaseFooter.vue'
  

export default {
  name: 'App',
  components: {
    BaseHeader,
    BaseFooter
  }
}
</script>
