<template>
  <h4>User1 목록</h4>
  <table border="1">
    <tr>
      <th>아이디</th>
      <th>이름</th>
      <th>휴대폰</th>
      <th>나이</th>
      <th>관리</th>
    </tr>
    <tr>
      <td>a101</td>
      <td>홍길동</td>
      <td>010-1212-1001</td>
      <td>22</td>
      <td>
        <a href="#">수정</a>
        <a href="#">삭제</a>
      </td>
    </tr>
  </table>
</template>
<script setup>
import axios from "axios";
import { onBeforeMount } from "vue";

onBeforeMount(() => {
  axios
    .get("http://localhost:8080/Ch09/user1s")
    .then((response) => {
      console.log(response);
    })
    .catch((error) => {
      console.log(error);
    });
});
</script>
<style scoped></style>
