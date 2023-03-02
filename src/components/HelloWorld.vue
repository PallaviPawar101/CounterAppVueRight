<template>
  <div>
    <h1>Counter App</h1>
  <p>{{count}}</p>
  <button class="button" @click="decrement">increment</button>
  <button class="button" @click="increment">decrement</button>
</div>
</template>

<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      count: 0
    };
  },
  methods: {
    increment() {
      this.count++;
    },
    decrement() {
      this.count--;
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1,
h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
.button {
  width: 100px;
  height: 40px;
  border: 1px solid blue;
  color: white;
  background: rgb(141, 141, 244);
  cursor: pointer;
}
</style>
