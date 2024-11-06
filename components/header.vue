<template>
  <div class="flex justify-center p-4">
    <nav class="flex justify-between container items-end">
      <div>
        <div class="text-2xl font-medium uno">
          <router-link to="/">Rituparna W</router-link>
        </div>
      </div>
      <div class="flex sm:gap-8 gap-4 font-medium">
        <div class="uno">
          <router-link to="/">About</router-link>
        </div>
        <div class="uno">
          <router-link to="/">Projects</router-link>
        </div>
        <div class="uno">
          <a href="/assets/resume.pdf">Resume</a>
        </div>
      </div>
    </nav>
  </div>
</template>

<style>
.uno > a {
  position: relative;
  color: #000;
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