<template>
  <div class="loader">
<!--    <div class="loader-bar" :style="{ width: progress + '%' }"></div>-->
    <div class="loader-text">{{ progress }}%</div>
  </div>
</template>

<script>
export default {
  name: "LoaderSection",
  props: {
    progress: {
      type: Number,
      required: true
    }
  }
}
</script>

<style scoped>
.loader {
  width: 100%;
  height: 4px;
  /*background-color: #ccc;*/
  position: relative;
}

.loader-bar {
  height: 100%;
  transition: width 0.3s;
}

.loader-text {
  transform: translate(-50%, -50%);
  color:#5d0cc7;
  text-align: center;
  font-size: 78px;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
  text-transform: capitalize;
 }
</style>