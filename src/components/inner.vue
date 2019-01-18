<template lang="pug">
div
    
    h3 внутренний компонент
    h4 {{msg}}
    input(type="text" v-bind="$attrs")
    button(
      v-on="$listeners"
    ) click
    br
    br
    br
    div {{formData}}
      br
      input(type="text" v-model="formData.userName")
      span hello
      br
      input(type="checkbox" value="music" v-model="formData.hobby") 
      span music
      input(type="checkbox" value="kino" v-model="formData.hobby") 
      span kino
      br
      input(type="radio" name="payment" value="mastercard"  v-model="formData.payment") 
      span mastercard
      input(type="radio" name="payment" value="visa"  v-model="formData.payment") 
      span visa
      br
      select(v-model="formData.number")
        option(v-for="n in 10" :value="n" ) {{n}}
</template>

<script>
export default {
  inheritAttrs: false,
  data() {
    return {
      msg: "-------------p",
      title: "ss",
      formData: {
        userName: "",
        hobby:[],
        payment: "",
        number: ""
      }
    };
  },
  mounted() {
    console.log(this.$attrs);
    
  }
};
</script>
