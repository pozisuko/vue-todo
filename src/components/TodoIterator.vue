<template>
  <v-container fluid grid-list-md>
    <v-form @submit.prevent="addTodo">
      <v-text-field v-model="title" @submit.prevent="addTodo" label="Add your todo" required></v-text-field>
    </v-form>
    <v-spacer></v-spacer>
    <v-card>
      <TodoItem v-for="item in items" :key="item.title" :title="item.title">{{ item.title }}</TodoItem>
    </v-card>
  </v-container>
</template>

<script>
import TodoItem from "./TodoItem";
export default {
  components: {
    TodoItem
  },
  data() {
    return {
      title: "",
      items: []
    };
  },
  methods: {
    addTodo() {
      if (this.title != "") {
        this.items.push({
          title: this.title
        });
        this.title = "";
      }
    }
  }
};
</script>