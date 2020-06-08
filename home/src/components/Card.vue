<template>
  <a :href="href">
    <div>
      <img
        :src="img"
        :alt="imgAlt"
        class="object-cover rounded-lg w-full"
        style="height: 256px"
      />
    </div>
    <div class="flex justify-between mt-3 ">
      <div class="font-bold">{{ title }}</div>
      <div class="opacity-50 font-bold">day {{ day }}</div>
    </div>
  </a>
</template>

<script>
export default {
  name: "Card",
  props: ["img", "imgAlt", "title", "day", "href"],
}
</script>
