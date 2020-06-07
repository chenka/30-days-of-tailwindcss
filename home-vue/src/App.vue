<template>
<body class="antialiased" style="font-family: 'Roboto', sans-serif;">
  <div class="px-10 py-20">
    <div class="mb-10 text-center">
      <div class="text-4xl font-black font">30 Days of Tailwind CSS</div>
      <div class="text-lg">My project made in 30 days</div>
    </div>
    <div
      class="grid grid-flow-row grid-cols-1 sm:grid-cols-2 md:grid-cols-3 xl:grid-cols-4 gap-10 sm:gap-8 text-center sm:w-full w-408 mx-auto"
    >
      <Card
        img="/images/day-4.png"
        imgAlt="File Manager - Cloud Storage"
        title="File Manager - Cloud Storage"
      />
      <Card
        img="/images/day-4.png"
        imgAlt="File Manager - Cloud Storage"
        title="File Manager - Cloud Storage"
      />
      <Card
        img="/images/day-4.png"
        imgAlt="File Manager - Cloud Storage"
        title="File Manager - Cloud Storage"
      />
      <Card
        img="/images/day-4.png"
        imgAlt="File Manager - Cloud Storage"
        title="File Manager - Cloud Storage"
      />
    </div>
  </div>
</body>
</template>

<script>
import Card from "@/components/Card";
export default {
  name: "app",
  components: {
    Card
  }
};
</script>

<style src="./assets/tailwind.css">
