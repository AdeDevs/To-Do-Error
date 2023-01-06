<template>
  <div>
    <Head title="Task Tracker" />
    <Tasks :tasks="tasks" />
  </div>
</template>

<script>
import MyHeader from "./MyHeader.vue";
import MyButton from "./MyButton";
import Tasks from "./Tasks";

export default {
  components: {
    Head: MyHeader,
    Tasks,
  },
  data() {
    return {
      tasks: [],
    };
  },
  created() {
    this.tasks = [
      {
        id: 1,
        text: "Push Code To Github",
        day: "January 5 at 19:00",
        reminder: true,
      },
      {
        id: 2,
        text: "Gaming Session",
        day: "January 5 at 21:00",
        reminder: true,
      },
      {
        id: 3,
        text: "Dinner",
        day: "January 5 at 22:00",
        reminder: false,
      },
    ];
  },
};
</script>

<style>
</style>