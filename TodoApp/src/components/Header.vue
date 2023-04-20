<template>
  <header>
    <div>
      <input type="text" placeholder="할일을 입력하세요." />
      <button>등록</button>
    </div>
  </header>
</template>
<script>
export default {
  name: "Header",
  setup() {
    return {};
  },
};
</script>

<style scoped>
header {
  width: 100%;
  height: 60px;
  background-color: white;
  padding: 10px;
  box-sizing: border-box;
}
header > div {
  position: relative;
  width: 100%;
  height: 100%;
  box-sizing: border-box;
}
header > div > input {
  width: 100%;
  height: 100%;
  padding: 6px;
  box-sizing: border-box;
  border: none;
  outline: none;
}
header > div > button {
  position: absolute;
  right: 0;
  top: 0;
  width: 40px;
  height: 40px;
  border: none;
  background-color: #44ba81;
  color: white;
}
</style>
