<template>
  <div class="parent">
    <div class="overlay">{{title}}</div>
    <img
    class="child"
    :src="imgSrc"
    v-on:mouseover="mouseOver"
    v-on:mouseout="mouseOver"
    :class="[{on:active, off:!active}]"
    >
</div >
</template>

<script>
export default {
  props: ['imgSrc', 'title'],
  data () {
    return {
      active: false
    }
  },
  methods: {
    mouseOver: function () {
      this.active = !this.active
      // console.log('flag' + this.active)
    }
  }
}
</script>

<style scoped>
.on {
  -ms-transform: scale(1.2); /* IE 9 */
  -webkit-transform: scale(1.2); /* Safari 3-8 */
  transform: scale(1.2);
}
.off {width: 100%;}
.parent{
  width: 100%;
  overflow: hidden;
  position: relative
}
.child{
  width: 100%;
  transition: transform .2s;
  cursor: pointer;
}
.overlay{
  background-color: rgb(50,54,67,0.7);
  width:100%;
  height: 30px;
  position: absolute;
  bottom: 0;
  right: 0;
  text-align: center;
  color: #fff;
  font-size: 17px;
  z-index: 1;
  cursor: pointer;
}
</style>
