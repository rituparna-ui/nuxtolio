<template>
  <div class="flex justify-center p-4">
    <nav class="flex justify-between container items-end">
      <div>
        <h1 class="text-2xl font-medium uno">
          <router-link to="/">Rituparna W</router-link>
        </h1>
      </div>
      <div class="flex sm:gap-8 gap-4 font-medium">
        <h2 class="uno">
          <router-link to="/about">About</router-link>
        </h2>
        <h2 class="uno">
          <router-link to="/projects">Projects</router-link>
        </h2>
        <h2 class="uno">
          <a href="/assets/resume.pdf">Resume</a>
        </h2>
      </div>
    </nav>
  </div>
</template>

<style>
.uno > a {
  position: relative;
  color: #222222;
  text-decoration: none;
}

.uno > a:hover {
  color: #000;
}

.uno > a:before {
  content: "";
  position: absolute;
  width: 100%;
  height: 2px;
  bottom: -8px;
  left: 0;
  background-color: #000;
  visibility: hidden;
  -webkit-transform: scaleX(0);
  transform: scaleX(0);
  -webkit-transition: all 0.3s ease-in-out 0s;
  transition: all 0.3s ease-in-out 0s;
}

.uno > a:hover:before {
  visibility: visible;
  -webkit-transform: scaleX(1);
  transform: scaleX(1);
}
</style>