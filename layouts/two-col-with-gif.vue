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
      <!-- 1. 見出し -->
      <slot name="title" />

      <!-- 2. 「黄色の背景に文字」+「文字」の組み合わせが左右に並んだもの -->
      <div class="grid grid-cols-2">
        <!-- ショートカットキー 1 -->
        <MyKbd keybind="j" height="12" textSize="text-3xl">
          ：
          <slot name="j_feature" />
        </MyKbd>

        <!-- ショートカットキー 2 -->
        <MyKbd keybind="k" height="12" textSize="text-3xl">
          ：
          <slot name="k_feature" />
        </MyKbd>
      </div>

      <!-- 下寄せ かつ 左右の端に要素を並べる -->
      <div class="mt-auto flex justify-between">
        <!-- 3. GIF -->
        <slot />

        <!-- 縦に要素を並べる -->
        <div class="flex flex-col">
          <!-- 上下中央 -->
          <div class="my-auto">
            <!-- 4. 説明欄 -->
            <!-- ショートカットキー 3 -->
            <slot name="description" />
          </div>

          <!-- 5. ショートカットキーのヘルプ -->
          <!-- 背景緑で中央に配置 -->
          <div class="flex items-center bg-lime-300 h-12 p-4">
            <!-- ショートカットキー 4 -->
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
