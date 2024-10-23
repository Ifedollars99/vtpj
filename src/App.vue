<template>
  <nav class="bg-gray-100 p-4 shadow-bottom">
    <div class="container mx-auto flex justify-between items-center">
      <!-- Logo -->
      <a href="#" class="text-blue-800 text-5xl font-semibold no-underline">Fibre</a>

      <!-- Hamburger Menu (Visible on Mobile) -->
      <button @click="toggleMenu" class="text-blue-800 md:hidden text-4xl">
        <i class="bi bi-list"></i>
      </button>

      <!-- Navigation Links (Visible on Desktop) -->
      <ul class="hidden md:flex space-x-6 md:space-x-3 mt-4">
        <li><a href="#" class="text-black md:text-3xl font-bold no-underline">Community</a></li>
        <li><a href="#" class="text-black md:text-3xl no-underline font-bold ">Pricing</a></li>
        <li><a href="#" class="text-black md:text-3xl no-underline font-bold ">features</a></li>
      </ul>
      <div class="flex flex-row gap-3" >
      <button class="md:text-2xl font-bold text-black hidden md:flex mt-6" >Sign In</button>
      <button class="md:text-2xl font-bold  w-32 h-16 text-white bg-blue-700 rounded-xl hidden md:flex justify-center items-center " >Sign Up</button>
    </div>
    </div>
    <div>  
    </div>
  </nav>

  <!-- Sidebar for Mobile -->
  <div :class="menuOpen ? 'translate-x-0' : 'translate-x-full'" class="fixed top-0 right-0 w-2/3 md:w-1/4 h-full bg-gray-200 opacity-50 text-white transition-transform transform z-50 md:hidden">
    <div class="p-4 flex justify-between items-center">
      <span class="text-blue-800 text-4xl font-semibold md:text-2xl">Fibre</span>
      <button @click="toggleMenu" class="text-gray-400">
        <i class="bi bi-x text-7xl text-blue-800"></i>
      </button>
    </div>
    <ul class="p-4">
      <li><a href="#" class=" text-blue-800 hover:text-black text-3xl">Community</a></li>
      <li><a href="#" class=" text-blue-800 hover:text-black text-3xl">Pricing</a></li>
      <li><a href="#" class=" text-blue-800 hover:text-black text-3xl">Features</a></li>
    </ul>
  </div>
  <!-- Overlay when Menu is Open -->
  <div v-if="menuOpen" @click="toggleMenu" class="fixed inset-0 bg-black opacity-50 z-40 md:hidden"></div>
   <!-- images -->

  <div class=" bg-white w-full h-[1050px] md:h-[600px] flex flex-col  md:flex md:flex-row-reverse items-center px-4 mt-5">
    <div>
   <img src="https://cdn.dribbble.com/userupload/8386663/file/original-84c8796fd5fdc73682b46b9dd8a70fcb.jpg?resize=752x536" 
  class="rounded-full lg:h-[400px] lg:w-[400px] h-[300px] w-[300px] md:w-[250px] md:h-[250px] ">
</div> 
    <div class="mt-5 md:mt-0 lg:mt-0" >
      <div class="flex flex-row text-orange-600 gap-3">
      <i class="bi bi-star-fill text-xl"></i>
      <i class="bi bi-star-fill text-xl"></i>
      <i class="bi bi-star-fill text-xl"></i>
      <i class="bi bi-star-fill text-xl"></i>
      <i class="bi bi-star-fill text-xl"></i>
      <div class="text-gray-500" >
        <h1 class=" text-xl font-bold" >Rated 4.8/5 (284 reviews)</h1>
      </div>
    </div>
    <h1 class="text-2xl font-bold  text-black" >Create your porfolio in minutes</h1>
    <h1 class="text-xl text-gray-500" >With fiber you can Setup your own 
      <br> personal portfolio in minutes
      <br>  with dozens of premade beautiful templates.</h1>
      <div class="flex flex-col md:flex md:flex-row items-center gap-24" >
        <a href="wa.me08137628419"
         class="text-2xl  no-underline font-bold w-48 mt-3 h-16
            text-white bg-blue-700 rounded-xl flex justify-center items-center " 
         >Start free trial</a>
        <a href="wa.me08137628419" 
        class=" text-2xl text-blue-600 underline md:mt-5 font-bold -mt-20">View Examples</a>
      </div>
      <div class="mt-3 flex flex-col md:flex md:flex-row gap-1 md:gap-4" >
      <div class="mt-3 flex flex-row gap-2" >
        <i class="bi bi-check-circle-fill text-green-500 text-3xl md:text-4xl"></i>
        <h1 class="text-gray-500 text-3xl md:text-4xl ">No credit card required</h1> 
      </div>
      <div class="mt-3 flex flex-row gap-2" >
        <i class="bi bi-check-circle-fill text-green-500 text-3xl md:text-4xl"></i>
        <h1 class="text-gray-500 text-3xl md:text-4xl ">No credit card required</h1> 
      </div>
    </div>
  </div>
  </div>
  <div data-aos="zoom-in">
  <div class="ml-5 px-4 mt-5" >
    <h1 class="text-blue-800 text-2xl font-bold" >Why fibre</h1>
    <h1 class="text-4xl mt-3 font-bold" >A good portfolio means good employability</h1>
   <div class="flex flex-col mt-10 md:flex md:flex-row gap-5" >
    <div class="md:flex md:flex-col" >
    <i class="bi bi-alarm text-4xl text-blue-600"></i>
    <h1 class="text-black font-bold text-3xl mt-1" >Build in minutes</h1>
    <h1 class="text-xl text-gray-500" >With a selection of premade templates, you can build out a portfolio in less than 10 minutes</h1>
     </div>
     <div class="md:flex md:flex-col" >
    <i class="bi bi-arrow-left-right text-4xl text-blue-600 mt-3"></i>
    <h1 class="text-black font-bold text-3xl mt-1">Add custom CSS</h1>
    <h1 class="text-xl text-gray-500">Customize your personal porfolio even more with the ability to add your own custom CSS styles</h1>
    </div>
    <div class="md:flex md:flex-col" >
    <i class="bi bi-phone-flip text-4xl text-blue-600 mt-3"></i>
    <h1 class="text-black font-bold text-3xl mt-1">Responsive</h1>
    <h1 class="text-xl text-gray-500">ALl fiber templates are fully responsive to ensure the experience is seemless across all devices</h1>
    </div>
  </div>
</div>
<div data-aos="zoom-in">
    <div class="container bg-blue-800 w-[700px] md:h-[500px] h-[600px] rounded-lg mt-5" >
      <h1 class="text-white pt-3 ml-9 text-4xl" >Diversify your portfolio.</h1>
      <h1 class="text-white pt-3 ml-9 text-xl" >Create an even more impressing portfolios by creating case studies for your projects. simply follow our step by step guide</h1>
      <a href="wa.me08137628419" class="text-xl md:text-4xl no-underline font-bold w-52 ml-9 md:w-72 mt-3 h-16 md:h-16 text-blue-800 bg-white rounded-lg flex justify-center items-center " >Start free trial</a>
    <img src="https://cdn.dribbble.com/userupload/10740100/file/original-8e94725341c91ba8184bbdb21b6adc71.png?resize=1600x1200"
     class="w-[250px] ml-[30px] h-[215px] lg:w-[450px] md:w-[450px] md:mt-8 md:h-[260px] lg:h-[300px] md:ml-[200px] lg:ml-[500px] mt-6 lg:mt-0">
   </div>
  </div>
</div>
<div data-aos="zoom-in">
  <div class="md:flex md:flex-row gap-20 mt-16 px-20 lg:-ml-10 md:ml-10 md:justify-center " >
  <div class="mt-10 flex flex-col  items-center" >
    <div class="border-2 md:-ml-3 lg:ml-10 border-gray-500 w-72 h-72 md:w-[300px] md:h-[450px] lg:w-[450px] lg:h-[400px] rounded-lg px-4" >
      <div class="flex flex-row" >
      <img src="https://cdn.dribbble.com/userupload/16216368/file/original-74a100b764fc01baa9e42baf4c5b7e45.png?resize=752x564"
      class="h-[100px] w-[100px] rounded-full" >
      <div>
      <h1 class="text-blue-800 md:text-4xl text-3xl" >wayne</h1>
      <h1 class="text-xl  md:text-2xl" >100k in revenue</h1>
    </div>
    </div>
    <div>
      <h1 class="text-gray-500 text-sm lg:text-2xl md:text-xl" > setting up my porfolio with fibre took me not more than 10minutes. since then my portfolio has attracted a lot of clients and made over $100k</h1>
      <div class="md:ml-10  border-2 border-gray-500 w-60 h-11 rounded-lg px-4 mt-4 flex justify-center items-center lg:w-[350px] lg:h-[50px] md:w-[200px] md:h-[80px]" >
        <h1 class="text-lg text-blue-800 font-bold lg:text-2xl md:text-xl" >View Wayne porfolio</h1>
      </div>
    </div>
    </div>
  </div>
  <div class="mt-10 flex flex-col  items-center" >
    <div class="border-2 border-gray-500 w-72 h-72 rounded-lg px-4 md:w-[300px] md:h-[450px] lg:w-[450px] lg:h-[400px]" >
      <div class="flex flex-row" >
      <img src="https://cdn.dribbble.com/userupload/16448774/file/original-a088bc300823204bd1a5240d4e722a00.png?resize=752x564"
      class="h-[100px] w-[100px] rounded-full  mt-3" >
      <div class="ml-5" >
      <h1 class="text-blue-800  lg:text-6xl md:text-3xl" >Matthew</h1>
      <h1 class="text-xl md:text-2xl" >20k in revenue</h1>
    </div>
    </div>
    <div>
      <h1 class="text-gray-500 text-sm lg:text-2xl md:text-xl" > I have been getting A LOT of leads ever since I used Fiber's premade templates, now I just need to work on my case studies and I'll be ready to go!</h1>
      <div class=" md:ml-10 border-2 border-gray-500 w-60 h-11 rounded-lg px-4 mt-2 flex justify-center items-center lg:w-[350px] lg:h-[50px] md:w-[200px] md:h-[80px]" >
        <h1 class="text-lg text-blue-800 font-bold lg:text-2xl md:text-xl" >View Matt porfolio</h1>
      </div>
    </div>
    </div>
  </div>
</div>
</div>
<div data-aos="zoom-in">
<div class="bg-gray-100 h-[800px] md:h-[500px] shadow-top mt-28 grid grid-cols-2 gap-10 md:grid md:grid-cols-4 px-4" >
  <div class="flex flex-col gap-2" >
    <h1>Fibre</h1>
    <h1 class="text-lg" >With fibre you can set up your own personal portfolio in minutes with dozens of premade, beautiful templates.</h1>
  </div>
  <div class="flex flex-col gap-2" >
    <h1>Sitemap</h1>
    <h1 class="text-lg" >Homepage</h1>
    <h1 class="text-lg" >Testimonials</h1>
    <h1 class="text-lg" >Pricing</h1>
    <h1 class="text-lg" >Features</h1>
  </div>
  <div class="flex flex-col gap-2" >
    <h1>Resources</h1>
    <h1 class="text-lg" > Support</h1>
    <h1 class="text-lg" > Contact</h1>
    <h1 class="text-lg" > FAQ </h1>
  </div>
  <div class="flex flex-col gap-2" >
    <h1>Company</h1>
    <h1 class="text-lg" >About</h1>
    <h1 class="text-lg" >Customers</h1>
    <h1 class="text-lg" > Blog</h1>
  </div>
  <div class="flex flex-col gap-2" >
    <h1>Portfolio</h1>
    <h1 class="text-lg" >wayne</h1>
    <h1 class="text-lg" >Matthew</h1>
  </div>
</div>
</div>
</template>

<script>
import AOS from 'aos';
import 'aos/dist/aos.css';

export default {
  data () {
    return {
      menuOpen: false,
    };
  },
  methods: {
    toggleMenu() {
      this.menuOpen = !this.menuOpen;
    },
  },
  mounted() {
    AOS.init();
  }
};
</script>

<style>
  .shadow-bottom {
    @apply shadow-none; /* Ensure no default shadow */
    box-shadow: 0 10px 15px rgba(0, 0, 0, 0.3);
  }
  .shadow-top {
    @apply shadow-none; /* Ensure no default shadow */
    box-shadow: 0 -10px 15px rgba(0, 0, 0, 0.3);
  }
 

</style>
