<template>
  <header>
    <h2>{{ title }}</h2>
    <Button text="Add Task" color="green" />
  </header>
</template>

<script>
import MyButton from "./MyButton";
export default {
  name: "Header",
  props: ["title"],

  components: {
    Button: MyButton,
  },
};
</script>

<style scoped>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
}
</style>