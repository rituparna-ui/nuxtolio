<template>
  <div class="h-full flex flex-col bg-[#fafafa]" id="particles-js">
    <NuxtParticles id="tsparticles" url="/particles.json"> </NuxtParticles>
    <Header />
    <div class="flex-grow">
      <slot />
    </div>
    <Footer />
  </div>
</template>

<script>
import Header from "./../components/header.vue";
import Footer from "./../components/footer.vue";

export default {
  components: {
    Header,
    Footer,
  },
};
</script>
