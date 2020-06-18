<template>
  <h1>{{ msg }}</h1>
  <button @click="count++">count is: {{ count }}</button>
  <p v-text="name"></p>
</template>

<script>
import { reactive, ref } from "vue";
export default {
  name: "HelloWorld",
  props: {
    msg: String
  },
  data() {
    return {
      count: 0
    };
  },
  setup() {
    let name = ref("zhangsan");

    return {
      name
    };
  }
};
</script>
