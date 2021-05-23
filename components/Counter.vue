<template>
  <div>
    <h1>{{ title }}</h1>
    <div>
      counter: {{ $store.state.counter.counter }}
      <button @click="$store.commit('counter/countUp')">+1</button>
      <button @click="$store.commit('counter/reset')">reset</button>
    </div>
  </div>
</template>

<script>
export default {
  data: function () {
    return {
      title: "Counter App",
    };
  },
};
</script>
