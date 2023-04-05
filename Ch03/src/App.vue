<template>
  <h3>Ch03.Component 실습</h3>

  <h4>1)컴포넌트 기본</h4>
  <Component1></Component1>
  <Component2 />
  <Component3 />
  <hr />

  <h4>2)Options API</h4>
  <ApiComponent1 />
  <ApiComponent2 />
  <ApiComponent3 />
  <ApiComponent4 />
  <hr />

  <h4>3)컴포넌트 통신</h4>
  <UComponent1 :name="name" />
  <UComponent1 :name="name" :age="age" />

  <hr />

  <h4>4)컴포넌트 생명주기</h4>
  <hr />
</template>

<script>
import Component1 from "./components/sub1/Component1.vue";
import Component2 from "./components/sub1/Component2.vue";
import Component3 from "./components/sub1/Component3.vue";
import ApiComponent1 from "./components/sub2/ApiComponent1.vue";
import ApiComponent2 from "./components/sub2/ApiComponent2.vue";
import ApiComponent3 from "./components/sub2/ApiComponent3.vue";
import ApiComponent4 from "./components/sub2/ApiComponent4.vue";
import UComponent1 from "./components/sub3/UComponent1.vue";

export default {
  name: "App",
  data() {
    return {
      name: "홍길동",
      age: 21,
    };
  },
  components: {
    Component1,
    Component2,
    Component3,
    ApiComponent1,
    ApiComponent2,
    ApiComponent3,
    ApiComponent4,
    UComponent1,
  },
};
</script>
