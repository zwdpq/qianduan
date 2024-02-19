<template>
  <div class="demo">
    <h2>學校名稱{{ sName }}</h2>
    <h2>學校地址{{ sAddr }}</h2>
    <button @click="showName">点我提示学校名</button>
  </div>
</template>

<script>
export default Vue.extend({
  name: "School",
  data() {
    return {
      sName: "六中",
      sAddr: "安徽池州",
    };
  },
  methods: {
    showName() {
      alert(this.sName);
    },
  },
});

// export default {

// }
</script>

<style>
.demo {
  background-color: aqua;
}
</style>