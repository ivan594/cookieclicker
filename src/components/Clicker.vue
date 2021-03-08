<template>
  <div class="clicker">
    <h1 class="title">{{ title }}</h1>
    <span class="toSpan">{{ toSpan }}</span>
    <img @click="onCookieClick" class="cookie" src="../assets/cookie.png">
  </div>
</template>

<script>
export default ({
  name: 'Clicker',
  props: {
    title: {
      type: String,
    },
  },
  data() {
    return {
      counter: 0,
    };
  },
  computed: {
    counterToRender() {
      return `Всего печенек: ${this.counter}`;
    },
    toSpan() {
      return `${this.counterToRender}`;
    },
  },
  methods: {
    onCookieClick() {
      this.counter += 1;
      console.log('+1 печенька');
    },
  },
});  
</script>

<style scoped>
.clicker {
  display: flex;
  flex-direction: column;
  align-items: center;
  
}
.title {
  font-size: 45px;
}

.toSpan{
  margin-bottom: 35px;
}

.cookie {
  height: 200px;
  width: 200px;
  background-color: #fff;
}
</style>