<template>
  <h4>로그인 성공</h4>
  <p>
    XXX 님 반갑습니다.
    <a href="#" @click.prevent="logout">로그아웃</a>
  </p>
</template>
<script setup>
import { useRouter } from "vue-router";

const router = useRouter();

const logout = () => {
  localStorage.removeItem("accessToken");
  router.push("/jwt/login");
};
</script>
<style scoped></style>
