<template>
  <h4>로그인 성공</h4>
  <p>
    {{ user }} 님 반갑습니다.
    <a href="#" @click.prevent="logout">로그아웃</a>
  </p>
</template>
<script setup>
import { useRouter } from "vue-router";
import { useStore } from "vuex";

const store = useStore();
const router = useRouter();

const user = store.getters.getUser;
console.log(JSON.stringify(user));

const logout = () => {
  localStorage.removeItem("accessToken");
  router.push("/jwt/login");
};
</script>
<style scoped></style>
