<script>

export default {
  data() {
    return {
      activeTab: 1,
      tech: [
        {
          id: 1,
          name: 'HTML',
          imageUrl: 'https://cdn-icons-png.flaticon.com/512/1051/1051277.png',
          status: 'Advanced'
        },
        {
          id: 2,
          name: 'CSS',
          imageUrl: 'https://cdn-icons-png.flaticon.com/512/732/732190.png',
          status: 'Advanced'
        },
        {
          id: 3,
          name: 'PHP',
          imageUrl: 'https://cdn.iconscout.com/icon/free/png-256/free-php-2038871-1720084.png',
          status: 'Beginner'
        },
        {
          id: 4,
          name: 'Javascript',
          imageUrl: 'https://cdn.icon-icons.com/icons2/2415/PNG/512/javascript_original_logo_icon_146455.png',
          status: 'Advance'
        },
        {
          id: 5,
          name: 'Laravel',
          imageUrl: 'https://cdn.worldvectorlogo.com/logos/laravel-2.svg',
          status: 'Beginner'
        },
        {
          id: 6,
          name: 'VueJS',
          imageUrl: 'https://cdn.iconscout.com/icon/free/png-256/free-vue-282497.png?f=webp',
          status: 'Intermediate'
        },
        {
          id: 7,
          name: 'Tailwind',
          imageUrl: 'https://upload.wikimedia.org/wikipedia/commons/d/d5/Tailwind_CSS_Logo.svg',
          status: 'Intermediate'
        },
        {
          id: 12,
          name: 'ReactJS',
          imageUrl: 'https://cdn4.iconfinder.com/data/icons/logos-3/600/React.js_logo-512.png',
          status: 'Beginner'
        }
      ],
      tools: [
        {
          id: 1,
          name: 'Git',
          imageUrl: 'https://git-scm.com/images/logos/downloads/Git-Icon-1788C.png',
          status: 'Version Control'
        },
        {
          id: 2,
          name: 'GitHub',
          imageUrl: 'https://cdn-icons-png.flaticon.com/512/25/25231.png',
          status: 'Git Hosting'
        },
        {
          id: 3,
          name: 'NPM',
          imageUrl: 'https://cdn.iconscout.com/icon/free/png-256/free-npm-3-1175132.png',
          status: 'Package Manager'
        },
        {
          id: 4,
          name: 'MySQL',
          imageUrl: 'https://cdn-icons-png.flaticon.com/512/5968/5968313.png',
          status: 'Database'
        },
      ],
      workExperience: [
        {
          id: 1,
          title: "Frontend Engineer",
          desc: "Create and developed web-based platforms using various Frameworks.",
          className: "md:col-span-2",
          thumbnail: "/img/exp1.svg"
        },
        {
          id: 2,
          title: "Mobile App Dev",
          desc: "Designed and developed mobile app for both iOS & Android platforms.",
          className: "md:col-span-2",
          thumbnail: "/img/exp2.svg"
        },
        {
          id: 3,
          title: "Web Design",
          desc: "Building creative ideas in designing a website following the latest trends.",
          className: "md:col-span-2",
          thumbnail: "/img/exp3.svg"
        },
        {
          id: 4,
          title: "Backend Engineer",
          desc: "Developing and maintaining behind the scenes development to keep it running.",
          className: "md:col-span-2",
          thumbnail: "/img/exp4.svg"
        }
      ]
    };
  }
}

</script>
<template>
  <div
    class="bg-[#1e1e1f] px-5 py-5 md:px-12 md:py-10 text-left border border-[#383838] rounded-3xl text-amber-50 mx-3 mb-5">
    <article data-page="about">

      <header>
        <div class="text-2xl font-bold text-white mb-5 fadein-bot title-section flex items-center">
          About Me &nbsp;
          <div class="h-[1px] w-32 bg-amber-200 md:w-96 aos-init aos-animate" data-aos="zoom-in-left"
            data-aos-duration="600"></div>
        </div>
      </header>

      <section
        class="text-sm md:text-lg text-justify flex flex-col gap-4 md:flex-row md:gap-8 md:justify-left md:items-center">
        <div class="flex justify-center">
          <img class="w-9/12 rounded-full mb-3 fadein-up"
            src="https://i1.sndcdn.com/avatars-YJbqX8KrsmnEZXgD-IuQVeA-t500x500.jpg" alt="Foto">
        </div>
        <div class="md:w-7/12">
          <p class="mb-3 md:mb-7 fadein-left fadeins-1">
            &nbsp; &nbsp; &nbsp; Hi everyone! My name is Azhar Khairu Hafidz. I'm a web developer from Medan, North
            Sumatra. I
            Previously I was an ordinary student at MAN INSAN CENDEKIA, but after joining an organization at school, I
            became interested in the technology field after entering the Secretariat and Logistics division. My
            experience in the technology field began when I held a big event website held directly by my old school. Now
            my interest in the technology field is getting bigger, now, I am at Telkom University. My ultimate goal is to become a Web Developer or more precisely a Full-Stack
            developer. in my opinion, creating programs is not just a job, but also an art that
            has
            aesthetic value
          </p>
        </div>

      </section>

    </article>
  </div>
  <div
    class="bg-[#1e1e1f] px-5 py-5 md:px-12 md:py-10 text-left border border-[#383838] rounded-3xl text-amber-50 mx-3 mb-5">
    <article data-page="resume">
      <header>
        <div class="text-2xl font-bold text-white mb-5 fadein-bot title-section flex items-center">
          Resume &nbsp;
          <div class="h-[1px] w-32 bg-amber-200 md:w-96 aos-init aos-animate" data-aos="zoom-in-left"
            data-aos-duration="600"></div>
        </div>
      </header>

      <div class="max-w-3xl mx-auto">
        <div class="space-y-12">
          <!-- Education Section -->
          <div class="space-y-6">
            <div class="flex items-center gap-3 mb-6 justify-center">
              <span class="text-amber-200">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24"
                  stroke="currentColor">
                  <path d="M12 14l9-5-9-5-9 5 9 5z" />
                  <path
                    d="M12 14l6.16-3.422a12.083 12.083 0 01.665 6.479A11.952 11.952 0 0012 20.055a11.952 11.952 0 00-6.824-2.998 12.078 12.078 0 01.665-6.479L12 14z" />
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 14l9-5-9-5-9 5 9 5z" />
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 20v-6" />
                </svg>
              </span>
              <h3 class="text-xl font-bold text-amber-200">Education</h3>
            </div>

            <div class="space-y-6">
              <div
                class="relative pl-6 before:absolute before:left-0 before:h-full before:w-[2px] before:bg-amber-200 before:content-[''] hover:transform hover:translate-x-2 transition-transform duration-300">
                <h4 class="text-lg font-semibold">Telkom University</h4>
                <p class="text-amber-200/80 text-sm font-medium mb-1">2024 — Present</p>
                <p class="text-gray-400">Sistem Informasi Kota Cerdas.</p>
              </div>

              <div
                class="relative pl-6 before:absolute before:left-0 before:h-full before:w-[2px] before:bg-amber-200 before:content-[''] hover:transform hover:translate-x-2 transition-transform duration-300">
                <h4 class="text-lg font-semibold">MAN INSAN CENDEKIA</h4>
                <p class="text-amber-200/80 text-sm font-medium mb-1">2021 — 2024</p>
                <p class="text-gray-400">MIPA.</p>
              </div>

              <div
                class="relative pl-6 before:absolute before:left-0 before:h-full before:w-[2px] before:bg-amber-200 before:content-[''] hover:transform hover:translate-x-2 transition-transform duration-300">
                <h4 class="text-lg font-semibold">SMPN 4 PERCONTOHAN</h4>
                <p class="text-amber-200/80 text-sm font-medium mb-1">2018 — 2021</p>
                <p class="text-gray-400">IPA.</p>
              </div>
            </div>
          </div>

          <!-- Experience Section -->
          <div class="space-y-6">
            <div class="flex items-center gap-3 mb-6 justify-center">
              <span class="text-amber-200">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24"
                  stroke="currentColor">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                    d="M21 13.255A23.931 23.931 0 0112 15c-3.183 0-6.22-.62-9-1.745M16 6V4a2 2 0 00-2-2h-4a2 2 0 00-2 2v2m4 6h.01M5 20h14a2 2 0 002-2V8a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" />
                </svg>
              </span>
              <h3 class="text-xl font-bold text-amber-200">Experience</h3>
            </div>

            <div class="space-y-6">
              <div
                class="relative pl-6 before:absolute before:left-0 before:h-full before:w-[2px] before:bg-amber-200 before:content-[''] hover:transform hover:translate-x-2 transition-transform duration-300">
                <h4 class="text-lg font-semibold">AWS Back-End Academy</h4>
                <p class="text-amber-200/80 text-sm font-medium mb-1">2024 — Present</p>
                <p class="text-gray-400">Dicoding Indonesia.</p>
              </div>

              <div
                class="relative pl-6 before:absolute before:left-0 before:h-full before:w-[2px] before:bg-amber-200 before:content-[''] hover:transform hover:translate-x-2 transition-transform duration-300">
                <h4 class="text-lg font-semibold">IDCamp 2024</h4>
                <p class="text-amber-200/80 text-sm font-medium mb-1">2024 — Present</p>
                <p class="text-gray-400">Dicoding Indonesia.</p>
              </div>

              <div
                class="relative pl-6 before:absolute before:left-0 before:h-full before:w-[2px] before:bg-amber-200 before:content-[''] hover:transform hover:translate-x-2 transition-transform duration-300">
                <h4 class="text-lg font-semibold">Competition Of MAN INSAN CENDEKIA (COMIC)</h4>
                <p class="text-amber-200/80 text-sm font-medium mb-1">2022 — 2023</p>
                <p class="text-gray-400">KETUA KESEKRETARIATAN dan LOGISTIK.</p>
              </div>

              <div
                class="relative pl-6 before:absolute before:left-0 before:h-full before:w-[2px] before:bg-amber-200 before:content-[''] hover:transform hover:translate-x-2 transition-transform duration-300">
                <h4 class="text-lg font-semibold">Organisasi Siswa Intra MADRASAH</h4>
                <p class="text-amber-200/80 text-sm font-medium mb-1">2022 — 2023</p>
                <p class="text-gray-400">OSIM MAN INSAN CENDEKIA.</p>
              </div>

              <div
                class="relative pl-6 before:absolute before:left-0 before:h-full before:w-[2px] before:bg-amber-200 before:content-[''] hover:transform hover:translate-x-2 transition-transform duration-300">
                <h4 class="text-lg font-semibold">Organisasi Siswa Intra Sekolah</h4>
                <p class="text-amber-200/80 text-sm font-medium mb-1">2019 — 2020</p>
                <p class="text-gray-400">OSIS SMPN 4 PERCONTOHAN.</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </article>
  </div>

  <div
    class="bg-[#1e1e1f] px-5 py-5 md:px-12 md:py-10 text-left border border-[#383838] rounded-3xl text-amber-50 mx-3 mb-5">
    <article data-page="doing"></article>
    <div class="w-full mt-12 grid lg:grid-cols-4 grid-cols-1 gap-10">
      <div v-for="card in workExperience" :key="card.id" :class="card.className"
        class="flex-1 text-black dark:text-white border-neutral-200 dark:border-slate-800 item-tech">
        <div class="flex lg:flex-row flex-col lg:items-center p-3 py-6 md:p-5 lg:p-10 gap-2">
          <img :src="card.thumbnail" :alt="card.thumbnail" class="lg:w-32 md:w-20 w-16" />
          <div class="lg:ms-5">
            <h1 class="text-start text-xl md:text-2xl font-bold">{{ card.title }}</h1>
            <p class="text-start text-white-100 mt-3 font-semibold">{{ card.desc }}</p>
          </div>
        </div>
      </div>
    </div>
  </div>

  <div class="px-5 py-5 md:px-12 md:py-10 text-left text-amber-50 mx-3">
    <article>
      <header>
        <div
          class="text-2xl font-bold text-white mb-5 animate__animated animate__bounceInDown title-section flex items-center">
          Skill &nbsp;
          <div class="h-[1px] w-32 bg-amber-200 md:w-96 animate__animated animate__lightSpeedInLeft"
            data-aos-duration="600"></div>
        </div>
      </header>
      <section>
        <div>
          <ul class="flex flex-wrap text-sm font-medium text-center text-gray-500 dark:text-gray-400 mb-5">
            <li class="mr-2">
              <button class="inline-block px-4 py-3 rounded-lg hover:text-white animate__animated animate__flipInX"
                :class="{ 'text-amber-200 bg-amber-200 bg-opacity-10': activeTab === 1 }" @click="activeTab = 1">Tech
                Stack</button>
            </li>
            <li class="mr-2">
              <button class="inline-block px-4 py-3 rounded-lg hover:text-white animate__animated animate__flipInX"
                :class="{ 'text-amber-200 bg-amber-200 bg-opacity-10': activeTab === 2 }"
                @click="activeTab = 2">Tools</button>
            </li>
          </ul>
        </div>
        <div v-show="activeTab === 1">
          <div class="grid grid-cols-2 gap-4 pb-32 md:grid-cols-3 md:gap-8 xl:grid-cols-4 xl:gap-10 2xl:gap-12">
            <div v-for="item in tech" :key="item.id">
              <div
                class="item-tech flex cursor-pointer items-center gap-2 rounded-lg  border  px-2 py-2 hover:bg-amber-200 hover:bg-opacity-10 md:gap-3 lg:px-3 animate__animated animate__zoomInUp">
                <div class="flex h-12 w-12 items-center justify-center p-0 lg:h-16 lg:w-16 lg:p-2 zoom-in">
                  <img alt="HTML" loading="lazy" width="32" height="32" decoding="async" data-nimg="1"
                    class="img-tech drop-shadow-xl transition-all duration-300 h-[65%] w-[65%] lg:h-[85%] lg:w-[85%]  "
                    :src="item.imageUrl" style="color: transparent;">
                </div>
                <div class="flex items-center text-sm md:text-base lg:text-lg">
                  <div
                    class="tech font-medium text-secondary transition-all duration-300 translate-y-0 animate__animated animate__slideInRight">
                    {{ item.name }}
                  </div>
                  <div
                    class="status-tech opacity-0 absolute mt-5 text-[10px] text-amber-200 transition-all duration-300 md:text-xs lg:text-sm animate__animated animate__fadeIn">
                    {{ item.status }}</div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div v-show="activeTab === 2">
          <div class="grid grid-cols-2 gap-4 pb-32 md:grid-cols-3 md:gap-8 xl:grid-cols-4 xl:gap-10 2xl:gap-12">
            <div v-for="item in tools" :key="item.id">
              <div
                class="item-tech flex cursor-pointer items-center gap-2 rounded border  px-2 py-2 hover:bg-amber-200 hover:bg-opacity-10 md:gap-3 lg:px-3 animate__animated animate__zoomInUp">
                <div class="flex h-12 w-12 items-center justify-center p-0 lg:h-16 lg:w-16 lg:p-2 zoom-in">
                  <img alt="HTML" loading="lazy" width="32" height="32" decoding="async" data-nimg="1"
                    class="img-tech drop-shadow-xl transition-all duration-300 h-[65%] w-[65%] lg:h-[85%] lg:w-[85%]  "
                    :src="item.imageUrl" style="color: transparent;">
                </div>
                <div class="flex items-center text-sm md:text-base lg:text-lg">
                  <div
                    class="tech font-medium text-secondary transition-all duration-300 translate-y-0 animate__animated animate__slideInRight">
                    {{ item.name }}
                  </div>
                  <div
                    class="status-tech opacity-0 absolute mt-5 text-[10px] text-amber-200 transition-all duration-300 md:text-xs lg:text-sm animate__animated animate__fadeIn">
                    {{ item.status }}</div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>
    </article>
  </div>
</template>

<style>
@keyframes fadeInLeft {
  0% {
    opacity: 0;
    transform: translateX(100%);
  }

  100% {
    opacity: 1;
    transform: translateX(0);
  }
}

.fadeins-1 {
  animation-delay: 500ms;
}

.fadeins-2 {
  animation-delay: 800ms;
}

.img-tech,
.tech {
  transition: transform 0.3s ease;
}

.item-tech:hover .img-tech {
  transform: scale(1.3);
}

.item-tech:hover .tech {
  transform: translateY(-12px);
}

.item-tech:hover .status-tech {
  opacity: 1;
}

@keyframes move-border {
  0% {
    transform: translateX(-100%);
  }

  100% {
    transform: translateX(100%);
  }
}
</style>
