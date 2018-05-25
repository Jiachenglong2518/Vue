<template>
  <div class='test1'>
    <h1 class='a' v-on:click='alert1'>{{msg}}</h1>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'HelloWorld! My name is Jiachenglong'
    }
  },
  created: function () {
    console.log(1)
    console.log(this.msg)
  },
  mounted: function () {
    console.log(window)
  },
  methods: {
    alert1: function () {
      alert(1)
    }
  }
}
</script>

<style scoped lang='less'>
    .test1{
        .a{
            color: red;
        }
   }
</style>
