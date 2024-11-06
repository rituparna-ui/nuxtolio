<template>
  <div class="h-full flex flex-col bg-[#fafafa]" id="particles-js">
    <NuxtParticles id="tsparticles" url="/particles.json"> </NuxtParticles>
    <Header />
    <div class="flex-grow flex items-center justify-center">
      <div>Projects Page</div>
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
