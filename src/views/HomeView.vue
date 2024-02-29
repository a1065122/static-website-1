<script>
export default {
  data() {
    return {
      a: 1,
      isMounted: true
    }
  },
  beforeCreate() {
    console.log('Hook: beforeCreate');
    console.log(` this.a: ${this.a}`);
    console.log();
  },
  created() {
    console.log('Hook: created');
    console.log(123);
  },
  beforeMount() {
    console.log('Hook: beforeMount');
    console.log();
  },
  mounted() {
    console.log('Hook: mounted');
    console.log();
  },
  beforeUpdate() {
    console.log('Hook: beforeUpdate');
    console.log(` this.a: ${this.a}`);
    console.log();
  },
  updated() {
    console.log('Hook: updated');
    console.log();
  },
  beforeUnmount() {
    console.log('Hook: beforeDestroy');
    console.log();
  },
  unmounted() {
    console.log('Hook: destroyed');
    console.log();
  },
}
</script>

<template>
  <main class="">
  <div class="bg-white text-black pl-2 font-bold rounded-sm mb-3">
    {{a}}
  </div>
  <button class="w-30 p-2 rounded-md bg-sky-600" @click="a++">點我增加a數值</button>

  </main>
</template>
