<script lang="ts" setup>
useHead({
  bodyAttrs: {
    class: 'bg-cyan-300'
  }
})
</script>
<template>
  <div class="p-6">
    <div
      class="max-w-[900px] w-full border-dashed border-2 border-cyan-400 rounded-md p-4 text-lg font-medium text-center transition bg-cyan-200 cursor-pointer"
    >
      <FileDialog />
    </div>
    <div class="mt-4">
      <div class="text-cyan-700 text-lg">
        Preview
      </div>
    </div>
  </div>
</template>
<style scoped lang="css"></style>
