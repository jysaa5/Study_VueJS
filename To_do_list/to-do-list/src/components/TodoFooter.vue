<template>
  <div class="clearAllContainer">
    <span class="clearAllBtn" @click="clearTodo">Clear All</span>
  </div>
</template>
<script>
// 할 일 모두 삭제
export default {
  methods: {
    clearTodo() {
      // localStorage.clear();
      this.$emit("removeAll");
    },
  },
};
</script>
<style scoped>
.clearAllContainer {
  width: 8.5rem;
  height: 50px;
  line-height: 50px;
  background-color: white;
  border-radius: 5px;
  margin: 0 auto;
}

.clearAllBtn {
  color: #e20303;
  display: black;
}
</style>
