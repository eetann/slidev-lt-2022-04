<script setup lang="ts">
import { computed } from "@vue/reactivity";
const props = defineProps<{
  height: number;
  width?: number;
  keybind: string;
  textSize: string;
}>();

const keyClass = computed(() => {
  let width = props.width;
  if (!width) {
    width = props.height;
  }
  return `bg-yellow-300 text-center leading-${props.height} h-${props.height} w-${width}`;
});

const textClass = computed(() => {
  return `flex items-center ${props.textSize}`;
});
</script>

<template>
  <div v-bind:class="textClass">
    <div v-bind:class="keyClass">
      {{ props.keybind }}
    </div>
    <slot />
  </div>
</template>
