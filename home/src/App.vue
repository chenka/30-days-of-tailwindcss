<template>
<body class="antialiased" style="font-family: 'Roboto', sans-serif;">
  <div class="px-10 py-20">
    <div class="mb-10 text-center">
      <div class="text-4xl font-black font">30 Days of Tailwind CSS</div>
      <div class="text-lg">My project made in 30 days</div>
    </div>
    <div
      class="grid grid-flow-row grid-cols-1 sm:grid-cols-2 md:grid-cols-3 xl:grid-cols-4 gap-10 sm:gap-12 sm:w-full w-408 mx-auto"
    >
      <div v-for="(card,index) in cards" :key="card.title">
        <Card
          :img="card.img"
          :imgAlt="card.title"
          :title="card.title"
          :href="card.href"
          :day="index+1"
        />
      </div>
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
  },
  data: () => {
    return {
      cards: [
        {
          img: "images/day-1.png",
          title: "Statistics",
          href: "ui/day-1/public/index.html"
        },
        {
          img: "images/day-4.png",
          title: "File Manager - Cloud Storage",
          href: "ui/day-2/public/index.html"
        }
      ]
    };
  }
};
</script>

<style src="./assets/tailwind.css">
