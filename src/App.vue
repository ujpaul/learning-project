<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <MyComponent type="text" name="Maniriho Edouard" />
  <MyComponent type="password" name="Karera Hassan" />
  <MyComponent type="email" name="Arinatwe Joshua" />
  <MyComponent type="time" name="Umutoni Solange" />
  <DataTable :headers="tableHeaders" :items="tableData"></DataTable>
</template>

<script>
import MyComponent from "./views/MyComponent.vue";
import { DataTable } from "vuetify";
const display = (name) => {
  console.log("Hello", name);
};
console.log(display("Paul"));
console.log(display("Paul"));
console.log(display("Cyntia"));
export default {
  name: "App",
  components: {
    MyComponent,
    DataTable,
  },
  data() {
    return {
      tableData: [
        { name: "John", age: 25 },
        { name: "Jane", age: 30 },
        { name: "Bob", age: 40 },
      ],
      tableHeaders: [
        { text: "Name", value: "name" },
        { text: "Age", value: "age" },
      ],
    };
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
