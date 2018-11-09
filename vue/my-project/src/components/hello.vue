// hello.vue
<template>
  <div>
      <h2>Hello Vue.js</h2>
      <hr/>
      <p>{{content}}</p>
  </div>
</template>
<script>
export default {
  data() {
    return {
      content: "this is Hello components"
    };
  }
};
</script>

