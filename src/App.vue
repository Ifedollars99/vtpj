<template>
  <div class="min-h-screen flex">
    <!-- Sidebar -->
    <aside
      :class="[
        'fixed inset-y-0 left-0 w-64 bg-gray-900 text-gray-300 transform transition-transform duration-300 ease-in-out',
        sidebarOpen ? 'translate-x-0' : '-translate-x-full',
        'md:translate-x-0' // Ensures sidebar is always visible on larger screens
      ]"
    >
      <div class="p-4">
        <!-- Profile Section -->
        <div class="flex flex-col items-center">
          <img
            src="https://cdn.dribbble.com/userupload/16915703/file/original-d4f59f0b0791f2ba9ed681a4094fc861.png?resize=752x564"
            alt="Profile"
            class="rounded-full w-24 h-24"
          />
          <h2 class="text-white mt-4 text-lg font-semibold">HAMZAH TAOFEEQ</h2>
        </div>

        <!-- Navigation Links -->
        <nav class="mt-8 space-y-8 text-2xl">
          <a href="#home" class="hover:text-white">
            <i class="bi bi-house mr-3 "></i> Home
          </a>
          <a href="#about" class="block hover:text-white">
            <i class="bi bi-file-person mr-3"></i> About
          </a>
          <a href="#resume" class="block hover:text-white">
            <i class="bi bi-journal-bookmark mr-3"></i> Resume
          </a>
          <a href="#services" class="block hover:text-white">
            <i class="bi bi-hdd-stack mr-3"></i> Services
          </a>
          <a href="#contact" class="block hover:text-white">
            <i class="bi bi-envelope-heart mr-3"></i>Contact
          </a>
        </nav>
      </div>
    </aside>

    <!-- Main Content -->
    <div class="flex-1 flex flex-col">
      <!-- Mobile Header with Hamburger Icon -->
      <header class="p-4 bg-gray-900 text-white flex justify-between items-center md:hidden">
        <button @click="toggleSidebar">
          <i class="bi bi-list text-xl"></i> <!-- Hamburger Menu Icon -->
        </button>
        <h1 class="text-lg">HAMZAH TAOFEEQ</h1>
      </header>

      <!-- Main Section with Image and Text -->
      <main>
      <video class="home flex-1 bg-cover bg-center text-white flex items-center justify-center p-4" id="home"
      autoplay 
      loop 
      muted 
      playsinline >
    <source src="https://cdn.dribbble.com/users/1342032/screenshots/9534052/media/a1854b0b345c111867909c77cf08883a.mp4" type="video/mp4" />
    Your browser does not support the video tag.
  </video>
      </main>
      <!-- About section -->
      <div class="ml-10 md:ml-72 px-4 mt-7">
          <h1 class="about text-4xl  font-bold text-gray-800" id="about" >ABOUT</h1>
          <div class="border-b-4 border-blue-600 w-32 mt-2" ></div>
          <p class="mt-4 text-lg">I'm web developer!
            I am a skilled web developer with two years of experience in creating innovative and user-friendly web applications. 
            I have a strong foundation in [HTML, CSS, JavaScript] and am proficient in using popular frameworks like [Vue, Tailwind, Bootstrap].
        Throughout my career, I have successfully developed so a few good projct, demonstrating my ability to deliver high-quality web solutions. 
            I am passionate about staying up-to-date with the latest web development trends and technologies.
          </p>
          <!-- web Section -->
            <div class="mt-7" >
              <h1 class="text-4xl  font-bold text-gray-800"  >WEB DEVELOPER</h1>
              <p class="text-lg" >A dedicated and proficient developer and technical writer,always ready to meet the 
                neccessary demand from my clients.</p>
                <div class="grid grid-cols-1 md:grid md:grid-cols-2" >
                  <div class="flex flex-row space-x-3" >
                    <i class="bi bi-chevron-double-right text-lg text-blue-600"></i>
                    <p class="text-lg font-bold">Birthday:</p>
                    <p class="text-lg" >24th, March, 2006</p>
                  </div>
                  <div class="flex flex-row space-x-3" >
                    <i class="bi bi-chevron-double-right text-lg text-blue-600"></i>
                    <p class="text-lg font-bold">loaction:</p>
                    <p class="text-lg" >riyadh</p>
                  </div>
                  <div class="flex flex-row space-x-3" >
                    <i class="bi bi-chevron-double-right text-lg text-blue-600"></i>
                    <p class="text-lg font-bold">Phone:</p>
                    <p class="text-lg" >08137628419</p>
                  </div>
                  <div class="flex flex-row space-x-3" >
                    <i class="bi bi-chevron-double-right text-lg text-blue-600"></i>
                    <p class="text-lg font-bold">Degree:</p>
                    <p class="text-lg" >Bsc, computer science</p>
                  </div>
                  <div class="flex flex-row space-x-3" >
                    <i class="bi bi-chevron-double-right text-lg text-blue-600"></i>
                    <p class="text-lg font-bold">Email:</p>
                    <p class="text-lg" >taofeeqifedollar <br> @gmail.com</p>
                  </div>
                  <div class="flex flex-row space-x-3" >
                    <i class="bi bi-chevron-double-right text-lg text-blue-600"></i>
                    <p class="text-lg font-bold">Age:</p>
                    <p class="text-lg" >18</p>
                  </div>
                  <div class="flex flex-row space-x-3" >
                    <i class="bi bi-chevron-double-right text-lg text-blue-600"></i>
                    <p class="text-lg font-bold">Freelance:</p>
                    <p class="text-lg" >Available</p>
                  </div>
                </div>
                <p class="mt-5 text-lg" >A dedicated and proficient developer and technical writer,always ready to meet the neccessary demand from my clients</p>
            </div>
            <!-- emoji Section -->
            <div class="grid grid-cols-1 mt-5 md:grid md:grid-cols-3" >
              <div class="flex flex-row gap-3" >
                <i class="bi bi-emoji-smile text-5xl text-blue-600"></i>
                <div class="flex flex-col" >
                <p class="text-5xl font-bold" >20</p>
                <p>Happy clients...... always happy to help</p>
              </div>
              </div>
              <div class="flex flex-row gap-3 md:ml-5" >
                <i class="bi bi-kanban text-5xl text-blue-600"></i>
                <div class="flex flex-col" >
                <p class="text-5xl font-bold" >15</p>
                <p>Projects dedicated to work</p>
              </div>
              </div>
              <div class="flex flex-row gap-3 md:ml-5" >
                <i class="bi bi-headset text-5xl text-blue-600"></i>
                <div class="flex flex-col" >
                <p class="text-5xl font-bold" >10</p>
                <p>Hours of support working with good group</p>
              </div>
              </div>
              <div class="flex flex-row gap-3 md:ml-5" >
                <i class="bi bi-person-lines-fill text-5xl text-blue-600"></i>
                <div class="flex flex-col" >
                <p class="text-5xl font-bold" >5</p>
                <p>Hard Workers Great Workers</p>
              </div>
              </div>
            </div> 
        </div> 
        <!-- skill Section -->
       
        <div class="bg-blue-100 mt-10 w-auto h-[400px]" >
          <div class="ml-10 md:ml-72 px-4" >
          <h1 class="text-4xl  font-bold text-gray-800 mt-5">SKILL</h1>
          <div class="border-b-4 border-blue-600 w-28 mt-2" ></div>
          <p class="mt-3" >the level of my skill as a frontend developer</p>
          <div class="p-6">
  <!-- Skill Bars Wrapper -->
  <div class="grid grid-cols-2 gap-4">
    <!-- HTML Skill Bar -->
    <div>
      <div class="flex justify-between text-sm font-bold mb-1">
        <span>HTML</span>
        <span>100%</span>
      </div>
      <div class="w-full bg-gray-300 h-2 rounded">
        <div class="bg-blue-500 h-full rounded" style="width: 100%"></div>
      </div>
    </div>

    <!-- React Skill Bar -->
    <div>
      <div class="flex justify-between text-sm font-bold mb-1">
        <span>TAILWIND</span>
        <span>100%</span>
      </div>
      <div class="w-full bg-gray-300 h-2 rounded">
        <div class="bg-blue-500 h-full rounded" style="width: 100%"></div>
      </div>
    </div>

    <!-- CSS Skill Bar -->
    <div>
      <div class="flex justify-between text-sm font-bold mb-1">
        <span>BOOTSTRAP</span>
        <span>90%</span>
      </div>
      <div class="w-full bg-gray-300 h-2 rounded">
        <div class="bg-blue-500 h-full rounded" style="width: 90%"></div>
      </div>
    </div>

    <!-- Technical Writing Skill Bar -->
    <div>
      <div class="flex justify-between text-sm font-bold mb-1">
        <span>CSS</span>
        <span>90%</span>
      </div>
      <div class="w-full bg-gray-300 h-2 rounded">
        <div class="bg-blue-500 h-full rounded" style="width: 90%"></div>
      </div>
    </div>

    <!-- JavaScript Skill Bar -->
    <div>
      <div class="flex justify-between text-sm font-bold mb-1">
        <span>JAVASCRIPT</span>
        <span>75%</span>
      </div>
      <div class="w-full bg-gray-300 h-2 rounded">
        <div class="bg-blue-500 h-full rounded" style="width: 75%"></div>
      </div>
    </div>

    <!-- Tailwind Skill Bar -->
    <div>
      <div class="flex justify-between text-sm font-bold mb-1">
        <span>VUE</span>
        <span>85%</span>
      </div>
      <div class="w-full bg-gray-300 h-2 rounded">
        <div class="bg-blue-500 h-full rounded" style="width: 85%"></div>
      </div>
    </div>
    </div>
    <div>
    </div>
  </div>
</div>
<!-- resume Section -->
<div class="ml-10 md:ml-72 px-4 mt-10" >
<h1 class="resume text-4xl  font-bold text-gray-800 mt-28" id="resume">RESUME</h1>
      <div class="border-b-4 border-blue-600 w-40 mt-2" ></div>
      <p class="mt-5" >I am a skilled web developer with two years of experience in creating innovative and user-friendly web applications. 
        I have a strong foundation in [HTML, CSS, JavaScript] and am proficient in using popular frameworks like [Vue, Tailwind, Bootstrap]. 
        Throughout my career, I have successfully developed so many good projects, demonstrating my ability to deliver high-quality web solutions. 
        I am passionate about staying up-to-date with the latest web development trends and technologies.</p>
    </div>

    <!-- summary Section -->
    <div class="ml-10 md:ml-72 px-6 mt-32 md:grid md:grid-cols-2 md:space-x-5" >
  <!-- Education Section -->
  <div class="">
    <h2 class="text-xl font-bold uppercase mb-4">Education</h2>
    <div class="relative">
      <!-- Blue Line -->
      <div class="absolute left-1 top-0 h-full w-1 bg-blue-500"></div>
      
      <!-- Timeline Item 1 -->
      <div class="flex items-start mb-8">
        <div class="w-4 h-4 bg-white border-2 border-blue-500 rounded-full mt-1.5 relative z-10"></div>
        <div class="ml-6">
          <h3 class="font-bold">Secondary school Certificate</h3>
          <p class="text-sm text-gray-600">2008-2022</p>
          <p class="italic text-gray-700">Grait international college</p>
          <p>Best student of the year doing great .. in being creative</p>
        </div>
      </div>

      <!-- Timeline Item 2 -->
      <div class="flex items-start mb-8">
        <div class="w-4 h-4 bg-white border-2 border-blue-500 rounded-full mt-1.5 relative z-10"></div>
        <div class="ml-6">
          <h3 class="font-bold">O'Level Certificate</h3>
          <p class="text-sm text-gray-600">2020 - 2022</p>
          <p class="italic text-gray-700">Grait international college</p>
          <p>Best in technical writing and fluent English speaking</p>
        </div>
      </div>
    </div>
  </div>

  <!-- Experience Section -->
  <div>
    <h2 class="text-xl font-bold uppercase mb-4">Experience</h2>

    <!-- Timeline Wrapper with Blue Line -->
    <div class="relative">
      <!-- Blue Line -->
      <div class="absolute left-1 top-0 h-full w-1 bg-blue-500"></div>

      <!-- Experience Item 2 -->
      <div class="flex items-start mb-8">
        <div class="w-4 h-4 bg-white border-2 border-blue-500 rounded-full mt-1.5 relative z-10"></div>
        <div class="ml-6">
          <h3 class="font-bold">Web Developer</h3>
          <p class="text-sm text-gray-600">2024 August - Present</p>
          <p class="italic text-gray-700">TechHub, oxbridge schools Tech Hub</p>
          <ul class="list-disc ml-5 text-gray-700">
            <li>Developed numerous websites (eCommerce,  exams website, etc.)</li>
            <li>Managed up to 5 projects or tasks at a time under pressure</li>
            <li>Recommended and consulted with clients on the most appropriate web development</li>
          </ul>
        </div>
  </div>
</div>
</div>
</div>
<!-- services section -->
<div class="ml-10 md:ml-72 px-4 mt-10" >
  <h1 class="services text-4xl  font-bold text-gray-800 mt-28" id="services">SERVICES</h1>
      <div class="border-b-4 border-blue-600 w-40 mt-2" ></div>
      <p class="mt-3" >A dedicated and proficient developer and technical writer,always ready to meet
         the neccessary demand from my clients</p>
      <div class="mt-10 grid grid-cols-1 md:grid md:grid-cols-3 gap-9" >
        <div class="flex flex-row gap-3" >
          <div class="bg-blue-500 w-32 h-16"><i class="bi bi-hurricane text-4xl text-white flex justify-center items-center pt-3"></i></div>
          <div class="flex flex-col" >
            <h1 class="text-2xl font-bold hover:text-blue-500" >Web development</h1>
            <p>Building an interactive and engaging webites that suits our clients desires</p>
          </div>
        </div>
        <div class="flex flex-row gap-3" >
          <div class="bg-blue-500 w-24 h-16"><i class="bi bi-pen text-4xl flex justify-center items-center pt-3 text-white"></i></div>
          <div class="flex flex-col" >
            <h1 class="text-2xl font-bold hover:text-blue-500" >Technical Writing</h1>
            <p>Give details to every single steps in building websites</p>
          </div>
        </div>
        <div class="flex flex-row gap-3" >
          <div class="bg-blue-500 w-16 h-16"><i class="bi bi-train-freight-front text-white text-4xl flex justify-center items-center pt-3"></i></div>
          <div class="flex flex-col" >
            <h1 class="text-2xl font-bold hover:text-blue-500" >Freelance</h1>
            <p>Open for freelance jobs</p>
          </div>
        </div>
        <div class="flex flex-row gap-3" >
          <div class="bg-blue-500 w-20 h-16"><i class="bi bi-snow text-white text-4xl flex justify-center items-center pt-3"></i></div>
          <div class="flex flex-col" >
            <h1 class="text-2xl font-bold hover:text-blue-500" >Consultation</h1>
            <p>Maximum attention always assured</p>
          </div>
        </div>
        <div class="flex flex-row gap-3" >
          <div class="bg-blue-500 w-24 h-16"><i class="bi bi-kanban text-white text-4xl flex justify-center items-center pt-3"></i></div>
          <div class="flex flex-col" >
            <h1 class="text-2xl font-bold hover:text-blue-500" >Problem Solving</h1>
            <p>Always willing to break down the complex works</p>
          </div>
        </div>
        <div class="flex flex-row gap-3" >
          <div class="bg-blue-500 w-24 h-16"><i class="bi bi-person-lines-fill text-4xl flex justify-center pt-3 text-white  "></i></div>
          <div class="flex flex-col" >
            <h1 class="text-2xl font-bold hover:text-blue-500" >Fluent Communication</h1>
            <p>Making it very easy for our client to relate with us</p>
          </div>
        </div>
    
      </div>
</div>
<!-- contact section -->
<div class="ml-10 md:ml-72 px-4 mt-10" >
  <h1 class="contact text-4xl  font-bold text-gray-800 mt-28" id="contact">CONTACT</h1>
      <div class="border-b-4 border-blue-600 w-40 mt-2" ></div>
       <p class="mt-3" >I will always love to get your feedback in other for me to relate very well</p>
       <!-- box section -->
       <div data-aos="zoom-in">
       <div class="flex justify-center" >
       <div class=" md:flex md:justify-center pl-10 md:pl-0 mt-10 shadow-lg bg-white w-[1200px] h-[1000px] md:h-[700px]">
        <div class="mt-7 grid grid-cols-1 md:grid md:grid-cols-2 gap-36 " >
          <div class="flex flex-col " >
        <h1>Your Name</h1>
        <input type="text" class="bg-white text-black border-2 border-gray-500 hover:border-blue-600
        p-2 rounded h-14 w-96 mt-3" >
      </div>
      <div class="flex flex-col -mt-28 md:mt-0" >
        <h1>Your Email</h1>
        <input type="text" class="bg-white text-black border-2 border-gray-500 hover:border-blue-600
        p-2 rounded h-14 mt-3 w-96" >
      </div>
      <div class="-mt-36 flex flex-col" >
        <h1>Subject</h1>
        <input type="text" class="bg-white text-black border-2 border-gray-500 hover:border-blue-600
        p-2 rounded h-14 mt-3 w-[500px]" >
        <h1 class="mt-10" >Message</h1>
        <input type="text" class="bg-white text-black border-2 border-gray-500 hover:border-blue-600
        p-2 rounded h-40 mt-3 w-[500px]" >
      </div>
       </div>
      </div>
       </div>
       </div>
</div> 
<!-- with section -->
<div class="bg-blue-100 h-[200px] flex justify-center items-center" >
<h1 class="md:text-2xl text-lg" >@code_with_Taofeeq</h1>
</div>
<!-- ending -->
            </div>
    </div>

    <!-- Overlay for Mobile Sidebar -->
    <div
      v-if="sidebarOpen"
      class="fixed inset-0 bg-black opacity-50 md:hidden"
      @click="toggleSidebar"
    ></div>
  </div>
</template>

<script>
import { onMounted } from 'vue';
import AOS from 'aos';
import 'aos/dist/aos.css';
export default {
  data() {
    return {
      sidebarOpen: false, // Sidebar state
    };
  },
  methods: {
    toggleSidebar() {
      this.sidebarOpen = !this.sidebarOpen; // Toggles sidebar
    },
  },
  setup() {
    onMounted(() => {
      AOS.init();
    });
  }
};
</script>

<style scoped>
/* You can add any additional styles here */
html {
    scroll-behavior: smooth;
}

</style>