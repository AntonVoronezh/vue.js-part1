<template lang="pug">
div
    
    h3 внутренний компонент
    h4 {{msg}}
    input(type="text" v-bind="$attrs")
</template>

<script>
export default {
  inheritAttrs: false,
  data() {
    return {
      msg: "-------------p"
    };
  },
  mounted() {
    console.log(this.$attrs);
    
  }
};
</script>