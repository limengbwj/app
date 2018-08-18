```
<template>
    <swipe class="my-swipe">
  <swipe-item class="slide1"></swipe-item>
  <swipe-item class="slide2"></swipe-item>
  <swipe-item class="slide3"></swipe-item>
  <swipe-item class="slide4"></swipe-item>
  <swipe-item class="slide5"></swipe-item>
  <swipe-item class="slide6"></swipe-item>
  <swipe-item class="slide7"></swipe-item>
</swipe>
</template>
<script>
    import 'vue-swipe/dist/vue-swipe.css'
    import { Swipe, SwipeItem } from 'vue-swipe';
    export default{
        created() {
            this.$emit('switchTab','book');
         },
        components: {
            'swipe': Swipe,
            'swipe-item': SwipeItem
        }

    };
</script>

<style lang="scss" scoped>
.my-swipe {
  height: 200px;
  color: #fff;
  font-size: 30px;
  text-align: center;
}

.slide1 {
  background-color: #FFF0AC;
  color: #fff;
}

.slide2 {
  background-color: #FFED97;
  color: #000;
}

.slide3 {
  background-color: #FFE66F;
  color: #fff;
}
.slide4 {
  background-color: #FFE153;
  color: #000;
}
.slide5 {
  background-color: #FFDC35;
  color: #fff;
}
.slide6 {
  background-color: #FFD306;
  color: #000;
}
.slide7 {
  background-color: #EAC100;
  color: #fff;
}
</style>

```
