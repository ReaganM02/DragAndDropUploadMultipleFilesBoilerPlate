<script lang="ts" setup>
defineProps<{ fileName: string, fileType: string, url: string }>()
defineEmits<{ (e: 'delete'): void }>()

</script>
<template>
  <div class="flex justify-between items-center mb-2 bg-cyan-200 rounded-md overflow-hidden">
    <div class="flex gap-2">
      <div>
        <img
          :src="url"
          class="w-[60px]"
        >
      </div>
      <div>
        <div class="font-semibold text-cyan-600">
          {{ fileName }}
        </div>
        <div class="text-cyan-700 opacity-50">
          {{ fileType }}
        </div>
      </div>
    </div>
    <div class="pr-4">
      <div
        class="bg-cyan-100 hover:bg-cyan-300 transition w-[35px] h-[35px] grid place-items-center rounded-full cursor-pointer"
        @click="$emit('delete')"
      >
        <TrashIcon class="text-red-400 w-[20px]" />
      </div>
    </div>
  </div>
</template>
<style scoped lang="css"></style>
