<script setup lang="ts">
import backgroundImage from './assets/IMG_4358.jpg'
import ecoimpactlogo from './assets/logos/logo.png'
import meimage from './assets/IMG_4393.jpg'
import ciclogo from './assets/cic.png'

</script>

<template>

  <!-- 🌐 Sticky Navbar -->
  <nav class="fixed top-0 z-50 w-full bg-slate-800/70 backdrop-blur-sm font-mono text-white">
    <div class="max-w-6xl mx-auto px-4 py-3 flex justify-between items-center">
      <h1 class="text-xl font-bold">Ivan R.C.</h1>
      <ul class="flex space-x-6 text-sm font-medium">
        <li><a href="#about" class="hover:underline">About</a></li>
        <li><a href="#project" class="hover:underline">Projects</a></li>
        <li><a href="#skills" class="hover:underline">Skills</a></li>  <!-- Fixed typo -->
        <li><a href="#contact" class="hover:underline">Contact Me</a></li>
      </ul>
    </div>
  </nav>

  <!-- ✅ Background Section -->
  <section id='landing'>
  <div class="pt-20 flex flex-col justify-center items-center h-screen text-center bg-cover bg-center"
       :style="{ backgroundImage: `url(${backgroundImage})` }">
    <h1 class="italic text-center text-7xl font-mono text-white drop-shadow-lg">Ivan Ramos Candelero</h1>
    <h2 class="text-center text-2xl font-mono text-white drop-shadow">I love coding and building projects</h2>
  </div>
</section>

  <section id="about" class="py-16 px-4 bg-gray-100">
    <img :src="meimage" alt="Ivan R.C"
     class="mx-auto rounded-full w-32 h-32 sm:w-40 sm:h-40 md:w-48 md:h-48 object-cover mb-6 shadow-md">

    <h1 class="text-center text-5xl font-mono mb-6">ABOUT ME</h1>
    <p class="text-center text-gray-600 max-w-3xl mx-auto leading-relaxed">
      Hi y'all. My name is Ivan. I'm an IT Support Specialist and up-and-coming junior software developer from a small town in North Carolina.
      I graduated from the University of North Carolina at Greensboro with a Bachelor's degree in Computer Science.
      I love exploring new technologies and building mini projects in my free time.
      I'm also passionate about games—whether it's football (soccer), chess, or video games.
      I enjoy leading teams and having fun while doing serious work.
    </p>
  </section>

  <section id="project" class="py-16 px-4 bg-white">
    <h1 class="text-center text-5xl font-mono mb-1">Projects</h1>
    <div class="mt-16 max-w-6xl mx-auto flex flex-wrap justify-center gap-8">
      
      <div class="w-full md:w-[45%] bg-white p-6 rounded-xl shadow-md">
        <a href="https://github.com/littleivan12/EcoImpact" target="_blank" rel="noopener noreferrer">
          <img :src="ecoimpactlogo" alt="EcoImpact Logo" class="mx-auto object-contain h-48 w-full mb-4">
        </a>
        <h2 class="text-3xl font-semibold text-center font-mono mb-2">EcoImpact</h2>
        <p class="text-center text-gray-600 leading-relaxed">
          EcoImpact is an interactive web application designed to help users explore humanity’s environmental impact across three major domains:
          Air, Water, and Ground. Through data-driven visualizations and simulations, EcoImpact turns climate metrics into compelling
          experiences that inspire sustainable choices.
        </p>
      </div>

      <div class="w-full md:w-[45%] bg-white p-6 rounded-xl shadow-md">
        <a href="https://github.com/glemerich/CIC" target="_blank" rel="noopener noreferrer">
          <img :src="ciclogo" alt="CIC Logo" class="mx-auto object-contain h-48 w-full mb-4">
        </a>
        <h2 class="text-3xl font-semibold text-center font-mono mb-2">Currently In Congress (CIC)</h2>
        <p class="text-center text-gray-600 leading-relaxed">
          Currently In Congress (CIC) is a discussion platform that delivers real-time updates on the 117th U.S. Congress.
          It promotes transparency and combats misinformation by offering unbiased coverage of congressional proceedings.
          Users can explore voting records, participate in discussions, and interact directly with Congress members.
        </p>
      </div>
    </div>
  </section>

  <section id="skills" class="py-16 px-4  bg-gray-100">
    <h1 class="text-center text-5xl font-mono mb-10">Skills & Technologies</h1>
    <div class="max-w-4xl mx-auto grid grid-cols-2 sm:grid-cols-3 md:grid-cols-4 gap-6 text-center">
      <div class="h-40 bg-white p-4 rounded-lg shadow hover:scale-105 transition flex flex-col items-center justify-center">
        <img src="./assets/logos/Spring.png" class="w-12 h-12 mb-2" />
        <span class="text-xl font-semibold text-green-500">SpringBoot</span>
      </div>

      <div class="h-40 bg-white p-4 rounded-lg shadow hover:scale-105 transition flex flex-col items-center justify-center">
        <img src="./assets/logos/Java.png" class="w-12 h-12 mb-2" />
        <span class="text-xl font-semibold text-blue-400">Java</span>
      </div>

      <div class="h-40 bg-white p-4 rounded-lg shadow hover:scale-105 transition flex flex-col items-center justify-center">
        <img src="./assets/logos/Python.png" class="w-12 h-12 mb-2" />
        <span class="text-xl font-semibold text-yellow-500">Python</span>
      </div>

      <div class="h-40 bg-white p-4 rounded-lg shadow hover:scale-105 transition flex flex-col items-center justify-center">
        <img src="./assets/logos/Tailwind CSS.png" class="w-12 h-12 mb-2" />
        <span class="text-xl font-semibold text-blue-400">Tailwind</span>
      </div>

      <div class="h-40 bg-white p-4 rounded-lg shadow hover:scale-105 transition flex flex-col items-center justify-center">
        <img src="./assets/logos/HTML5.png" class="w-12 h-12 mb-2" />
        <span class="text-xl font-semibold text-red-500">HTML5</span>
      </div>

      <div class="h-40 bg-white p-4 rounded-lg shadow hover:scale-105 transition flex flex-col items-center justify-center">
        <img src="./assets/logos/CSS3.png" class="w-12 h-12 mb-2" />
        <span class="text-xl font-semibold text-blue-400">CSS</span>
      </div>

      <div class="h-40 bg-white p-4 rounded-lg shadow hover:scale-105 transition flex flex-col items-center justify-center">
        <img src="./assets/logos/Vue.js.png" class="w-12 h-12 mb-2" />
        <span class="text-xl font-semibold text-green-400">Vue.js</span>
      </div>

      <div class="h-40 bg-white p-4 rounded-lg shadow hover:scale-105 transition flex flex-col items-center justify-center">
        <img src="./assets/logos/React.png" class="w-12 h-12 mb-2" />
        <span class="text-xl font-semibold text-sky-500">React</span>
      </div>

      <div class="h-40 bg-white p-4 rounded-lg shadow hover:scale-105 transition flex flex-col items-center justify-center">
        <img src="./assets/logos/PostgresSQL.png" class="w-12 h-12 mb-2" />
        <span class="text-xl font-semibold text-blue-500">PostgresSQL</span>
      </div>

      <div class="h-40 bg-white p-4 rounded-lg shadow hover:scale-105 transition flex flex-col items-center justify-center">
        <img src="./assets/logos/FastAPI.png" class="w-12 h-12 mb-2" />
        <span class="text-xl font-semibold text-emerald-500">FastAPI</span>
      </div>

      <div class="h-40 bg-white p-4 rounded-lg shadow hover:scale-105 transition flex flex-col items-center justify-center">
        <img src="./assets/logos/D3.js.png" class="w-12 h-12 mb-2" />
        <span class="text-xl font-semibold text-orange-500">D3.js</span>
      </div>

      <div class="h-40 bg-white p-4 rounded-lg shadow hover:scale-105 transition flex flex-col items-center justify-center">
        <img src="./assets/logos/Vite.js.png" class="w-12 h-12 mb-2" />
        <span class="text-xl font-semibold text-violet-500">Vite.js</span>
      </div>
    </div>
  </section>

  <section id="contact" class="py-16 px-4  bg-white">
    <h2 class="text-center text-5xl font-mono mb-1">Contact Me</h2>
    <p class="text-center text-gray-600 max-w-3xl mx-auto leading-relaxed mb-2">
      Feel free to connect with me via the options below:
    </p>
    <div class="max-w-4xl mx-auto grid grid-cols-2 sm:grid-cols-3 md:grid-cols-3 gap-6 text-center">
      <div class="h-40 bg-white p-4 rounded-lg shadow hover:scale-100 transition flex flex-col items-center justify-center">
        <a href="https://github.com/littleivan12" target="_blank" rel="noopener noreferrer">
          <img src="./assets/logos/GitHub.png" class="w-12 h-12 mb-2" />
        </a>
        <span class="text-xl font-semibold ">GitHub</span>
      </div>

      <div class="h-40 bg-white p-4 rounded-lg shadow hover:scale-100 transition flex flex-col items-center justify-center">
        <a href="https://www.linkedin.com/in/ivancand/" target="_blank" rel="noopener noreferrer">
          <img src="./assets/logos/LinkedIn.png" class="w-12 h-12 mb-2" />
        </a>
        <span class="text-xl font-semibold text-blue-500">LinkedIn</span>
      </div>

      <div class="h-40 bg-white p-4 rounded-lg shadow hover:scale-100 transition flex flex-col items-center justify-center">
        <a href="mailto:irctech12@gmail.com">
          <img src="./assets/logos/icons8-email-open-50.png" class="w-12 h-12 mb-2" />
        </a>
        <span class="text-xl font-semibold ">Email</span>
      </div>
    </div>
  </section>

  <!-- 🔚 Footer -->
  <footer class="bg-slate-900 bg-gray-100 text-center py-6">
    <p class="mt-2 text-white">© 2025 Ivan Ramos Candelero — All rights reserved.</p>
  </footer>

</template>

<style>
body {
  font-family: 'Inter', sans-serif;
  -webkit-font-smoothing: antialiased;
  background-color: #f9fafb;
}
</style>
