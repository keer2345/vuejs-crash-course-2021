<template>
  <header>
    <h1>{{ title }}</h1>
    <Button
      v-show="homePage"
      @btn-click="$emit('toggle-add-task')"
      :text="showAddTask ? 'Hide' : 'Add Task'"
      :color="showAddTask ? 'red' : 'green'"
    />
    <!-- <Button text="Update" color="blue" /> -->
    <!-- <Button text="Delete" color="red" /> -->
  </header>
</template>

<script>
import Button from "./Button";

export default {
  name: "Header",
  props: {
    title: {
      type: String,
    },
    showAddTask: {
      type: Boolean
    }
  },
  components: {
    Button,
  },
  computed: {
    homePage () {
      if (this.$route.path === '/') {
        return true
      } else {
        return false
      }
    }
  }
};
</script>
<style>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
}
</style>
