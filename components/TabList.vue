<template>
  <div>
    <div>
      <slot name="icon">
        <carbon-pen text-orange-400 />
      </slot>
      <span ml-2>{{ title }}</span>
    </div>
    <ul>
      <li v-for="item in list" :key="item">{{ item }}</li>
    </ul>
  </div>
</template>

<script setup>
defineProps({
  list: Array,
  title: String,
})
</script>