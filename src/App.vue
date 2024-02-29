<script>
export default {
  data() {
    return {
      a: 1,
      isMounted: true
    }
  },
}
 
</script>

<template>
  <div class="flex justify-center items-center flex-wrap min-h-[100dvh] bg-black text-white">
    <RouterView v-if="isMounted" />
    <div class="w-full flex justify-center">
      <button class="w-30 p-2 rounded-md bg-sky-600" @click="isMounted = false">點我刪除組件</button>
    </div>
  </div>
  
</template>

<style scoped>
</style>
