<template>
  <base-button :buttonText="buttonTextBis"
    :disabled="isPending"
    :class="{buttonprimary: true,common: true}"
    :color="color"
    @click.stop.prevent="handleClick"
  >
    <font-awesome-icon 
      v-if="isPending"
      :icon="['fas', 'circle-notch']"
      pulse
    />
    <slot />
  </base-button>
</template>

<script>
import BaseButton from './BaseButton.vue'

export default {
  name: 'AsyncButton',
  components: { BaseButton },
  inheritAttrs: false,

  props: {
    color: {
      type: String,
      default: 'primary'
    },
    buttonTextBis: {
      type: String,
      default: () => "Label2"
    }
  },

  data () {
    return {
      isPending: false,
      myDelay: 2000
    }
  },

  methods: {
    handleClick () {
      console.log(this.myDelay)
      const myPromise =  new Promise(function(resolve) {
        setTimeout(resolve, 200);
      });
      (this.$attrs.onClick)
      this.isPending = true
      myPromise().finally(() => { this.isPending = false })
    }
  }
}
</script>