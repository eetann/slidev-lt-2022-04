---
theme: seriph
fonts:
  sans: "HiraMaruProN-W4"
---

# この世、
# ショートカットキー
# 多すぎ

## えーたん

---
layout: center
---

# 一日どれくらい スクロール していますか？

---
layout: center
---

# ブラウザ や テキストエディタ で、
# 一日どれくらい "移動" していますか？

---
layout: center
---

<!-- Markdown記法で画像 -->
![mouse](/computer_mouse_top.png)

---
layout: center
---

<!-- imgタグで画像 -->
<img class="h-80" src="/trackpad.jpg">

---
layout: center
---

<img class="h-80" src="/cursor-keys.jpg">

---
layout: center
---

# ホームポジションをなるべく崩さずにできる？

<img class="h-80 mx-auto" src="/keyboard_typing.png">

---
layout: center
---

# ショートカットキーはあるけど

<img class="h-64 mx-auto" src="/computer_keyboard_black.png">

---
layout: center
---

# この世、ショートカットキー多すぎ

<div class="text-2xl">
  全部は覚えられない、、、
</div>

<div class="flex">
  <img class="h-72" src="/pien.png">
  <img class="h-72" src="/many-shortcut-key.png">
</div>

---
layout: center
---

<div class="text-7xl">
  提案！
</div>

---
layout: center
---

<div class="text-7xl flex items-center space-x-5">
  <div class="bg-yellow-300 text-center leading-32 h-32 w-24">j</div>
  <div class="bg-yellow-300 text-center leading-32 h-32 w-24">k</div>
  <p>をセットで覚える</p>
</div>

---

<div class="h-full flex flex-col">

# Google Calendar

<div class="flex-grow text-3xl grid grid-cols-2">
  <div class="flex items-center">
    <div class="bg-yellow-300 text-center leading-12 h-12 w-12">j</div>
    ：次の期間
  </div>
  <div class="flex items-center">
    <div class="bg-yellow-300 text-center leading-12 h-12 w-12">k</div>
    ：前の期間
  </div>
</div>

  <div class="self-end flex items-center bg-lime-300 h-12 p-4">
    <div class="bg-yellow-300 text-center leading-8 h-8 w-8">？</div>
    ：ショートカットのヘルプ
  </div>
</div>

---
layout: two-col-with-gif
---
::title::
# Google Calendar

::j_feature::
次の日

::k_feature::
前の日

::description::
<MyKbd keybind="d" height=12 textSize="text-3xl">
：[日]ビュー
</MyKbd>

::default::
<img class="h-88" src="/google-calendar.gif">

---
layout: two-col-with-gif
---
::title::
# Google Calendar

::j_feature::
次の月

::k_feature::
前の月

::description::
<MyKbd keybind="m" height=12 textSize="text-3xl">
：[月]ビュー
</MyKbd>

::default::
<img class="h-88" src="/google-calendar-month-jk.gif">

---
layout: two-col-with-gif
---
::title::
# Gmail

::j_feature::
古いスレッド

::k_feature::
新しいスレッド

::default::
<img class="h-80" src="/gmail-jk-mosaic.gif">

---
layout: two-col-with-gif
---
::title::
# Google Drive

::j_feature::
下のアイテムを選択

::k_feature::
上のアイテムを選択

::default::
<img class="h-80" src="/google-drive-jk.gif">

---
layout: two-col-with-gif
---
::title::
# GitHub

::j_feature::
下を選択

::k_feature::
上を選択

::default::
<img class="h-80" src="/github-jk.gif">

---
layout: two-col-with-gif
help_key: ":h"
---
::title::
# vi / Vim / Neovim (テキストエディタ)

::j_feature::
下に移動

::k_feature::
上に移動

::default::
<img class="h-80" src="/vim-jk.gif">

::help_description::
ヘルプ

---
layout: center
---

<div class="text-6xl">
  <div class="flex space-x-5 items-center mb-20">
    <MyKbd keybind="←h" :height="20" :width="30" textSize="text-6xl" />
    <div class="mt-20">
      <MyKbd keybind="j" :height="20" textSize="text-6xl" />
      <MyKbd keybind="↓" :height="20" textSize="text-6xl" />
    </div>
    <div class="mb-20">
      <MyKbd keybind="↑" :height="20" textSize="text-6xl" />
      <MyKbd keybind="k" :height="20" textSize="text-6xl" />
    </div>
    <MyKbd keybind="l→" :height="20" :width="30" textSize="text-6xl" />
    <p>は</p>
  </div>
  <div>移動だけではない！</div>
</div>

---

水平線テスト `***`

***

水平線テスト `___` アンダースコア3つ

___

以下のコードは公式ドキュメントのexampleを加工したもの

```ts
function add(
  a: Ref<number> | number,
  b: Ref<number> | number
) {
  return computed(() => unref(a) + unref(b))
}
```

```ts {2-3}
function add(
  a: Ref<number> | number,
  b: Ref<number> | number
) {
  return computed(() => unref(a) + unref(b))
}
```

---

# h1タグ。Windi CSS では text-4xl です
## h2タグ。Windi CSS では text-3xl です
### h3タグ。Windi CSS では text-2xl です
#### h4タグ。Windi CSS では text-xl です
##### h5タグ。Windi CSS では text-base です
###### h6タグ。Windi CSS では text-sm です

<!-- これはただのコメントで、ノートにはならない -->

本文はpタグになります。  
このページは layout で使用されるクラス `slidev-layout`の使用例です。

* リストの要素1
  * リスト入れ子
* リストの要素2

<kbd>j</kbd>, <kbd>k</kbd>  
`kbd`タグ使える


<!--
各スライドの最後のコメントのみノートになる  
asdfdkfjdls<br>
sdjflsdjfs
-->
