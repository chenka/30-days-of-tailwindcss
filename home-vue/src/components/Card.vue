<template>
  <div>
    <div>
      <img :src="img" :alt="imgAlt" class="object-cover rounded-lg" style="height: 256px" />
    </div>
    <div class="mt-3 font-bold">{{title}}</div>
  </div>
</template>

<script>
export default {
  name: "Card",
  props: ["img", "imgAlt", "title"]
};
</script>
  
