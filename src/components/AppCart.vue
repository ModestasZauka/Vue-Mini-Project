<template>
  <div>
    <div class="box">
      <img v-if="photo" :src="photo" alt="photo of a project" />
      <h4 v-if="projectName">{{ projectName }}</h4>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppCart",
  props: {
    photo: {
      type: String,
      default: null
    },
    projectName: {
      type: String,
      default: null
    }
  }
};
</script>

<style lang = "scss" >
.box {
  display: flex;
  width: 290px;
  height: 373px;
  background-color: #3252e5;
  flex-direction: column;
  img {
    margin: 0 auto;
    margin-top: 20px;
    height: 256px;
    width: 242px;
  }
  h4 {
    margin: 24px;
    color: #fff;
  }
}
</style>