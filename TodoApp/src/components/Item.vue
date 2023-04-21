<template>
  <li>
    <i class="fa fa-check" aria-hidden="true"></i>
    <span>{{ todo }}</span>
    <button>삭제</button>
  </li>
</template>
<script>
export default {
  name: "Item",
  props: {
    todo: String,
  },
  setup(props) {
    const todo = props.todo;

    return { todo };
  },
};
</script>

<style scoped></style>
