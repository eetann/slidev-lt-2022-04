<script setup lang="ts">
interface Props {
  help_key?: string;
}
const props = withDefaults(defineProps<Props>(), {
  help_key: "?",
});
</script>

<template>
  <div class="slidev-layout">
    <!-- 縦に要素を並べる -->
    <div class="h-full flex flex-col">
      <slot name="title" />

      <!-- 2列 -->
      <div class="grid grid-cols-2">
        <MyKbd keybind="j" height="12" textSize="text-3xl">
          ：
          <slot name="j_feature" />
        </MyKbd>

        <MyKbd keybind="k" height="12" textSize="text-3xl">
          ：
          <slot name="k_feature" />
        </MyKbd>
      </div>

      <!-- 下寄せ かつ 左右の端に要素を並べる -->
      <div class="mt-auto flex justify-between">
        <slot />

        <!-- 縦に要素を並べる -->
        <div class="flex flex-col">
          <!-- 上下中央 -->
          <div class="my-auto">
            <slot name="description" />
          </div>

          <!-- 横に要素を並べる -->
          <div class="flex items-center bg-lime-300 h-12 p-4">
            <MyKbd
              v-bind:keybind="props.help_key"
              height="8"
              textSize="text-xl"
            >
              ：
              <slot name="help_description"> ショートカットのヘルプ </slot>
            </MyKbd>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
