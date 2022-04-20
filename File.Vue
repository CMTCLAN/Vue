<template>
  <div id="app">
    <CodeInput :loading="false" class="input" v-on:change="onChange" v-on:complete="onComplete" />
  </div>
</template>
 
<script>
import CodeInput from "vue-verification-code-input";
 
export default {
  name: "app",
  components: {
    CodeInput
  },
  methods: {
    onChange(v) {
      console.log("onChange ", v);
    },
    onComplete(v) {
      console.log("onComplete ", v);
    }
  }
};
</script>
