<script>
export default {
  data() {
    return {
      activeTab: 1,
      items: [
        {
          id: 1,
          name: 'Personal Website',
          imageUrl: 'jehar',
          status: 'My personal website, I created this website to display my profile, skills and projects.',
          tech: 'HTML, CSS, Javascript',
          github: 'https://github.com/Jemjeqt/Website_Jehar',
          demo: 'null'
        },
        {
          id: 2,
          name: 'JemJeeqt Movies',
          imageUrl: 'jemjeeqtmovie',
          status: 'Web untuk mencari berbagai Film-film terbaru yang sedang Trend.',
          tech: 'ReactJS, Tailwind, DB Movie api',
          github: 'https://github.com/Jemjeqt/movies',
          demo: 'null'
        },
        {
          id: 3,
          name: 'SIMPLE CALCULATOR',
          imageUrl: 'calculator',
          status: 'Kalkulator simple yang dibuat sebagai bahan pembelajaran dasar dari Javascript.',
          tech: 'HTML, CSS, Javascript',
          github: 'https://github.com/Jemjeqt/Calculator_Jehar',
          demo: 'null'
        },
        {
          id: 4,
          name: 'Login Page',
          imageUrl: 'loginpage',
          status: 'Sebuah design Page Halaman untuk keperluan user Login.',
          tech: 'HTML, CSS, Javascript',
          github: 'https://github.com/Jemjeqt/LoginPage_Jehar',
          demo: 'null'
        },
        {
          id: 5,
          name: 'Weather App',
          imageUrl: 'weather',
          status: 'Aplikasi sederhana yang dapat berfungsi untuk menampilkan informasi cuaca di suatu tempat tertentu.',
          tech: 'HTML, CSS, Javascript, API Weather',
          github: 'https://github.com/Jemjeqt/WeatherApp_Jehar',
          demo: 'null'
        },
        {
          id: 6,
          name: 'C O M I C',
          imageUrl: 'comic',
          status: 'Situs web resmi acara besar tahunan sekolah COMIC dibuat langsung menggunakan WIX.',
          tech: 'WIX',
          github: 'null',
          demo: 'https://comic2k22.wixsite.com/comic2k22'
        },
        {
          id: 7,
          name: 'Anime List',
          imageUrl: 'animelist',
          status: 'Website simulasi untuk mencari referensi Anime-Anime terpopuler dalam dunia.',
          tech: 'ReactJS, Tailwind, DB Movie api',
          github: 'https://github.com/Jemjeqt/AnimeList_Jehar',
          demo: 'https://cuyanimelist.vercel.app/'
        }
      ]
    };
  }
}
</script>

<template>
  <div class="portfolio-section px-5 py-5 md:px-12 md:py-10 text-left text-amber-50 mx-3">
    <article data-page="about">
      <!-- Header Section -->
      <header>
        <div
          class="text-2xl font-bold text-white mb-10 fadein-bot title-section flex items-center justify-center flex-col">
          <h4>Project Experience</h4>
          <h4 class="text-base font-normal text-transparent bg-clip-text bg-gradient-to-r from-slate-100 to-amber-300">
            Explore the projects I've worked on so far</h4>
        </div>
      </header>

      <!-- Projects Grid Section -->
      <section>
        <div class="projects-container">
          <div class="grid grid-cols-1 gap-6 md:grid-cols-2 lg:grid-cols-3 pb-32 fade-zoom-in">
            <div v-for="item in items" :key="item.id" class="project-card-wrapper">
              <div class="item-card">
                <!-- Image Section -->
                <div class="zoom-in">
                  <img :src="`/img/portfolio-${item.imageUrl}.png`" :alt="item.name" loading="lazy" decoding="async">
                </div>

                <!-- Content Section -->
                <div class="content-wrapper">
                  <!-- Project Title -->
                  <div class="title-text font-medium text-secondary">
                    {{ item.name }}
                  </div>

                  <!-- Project Description -->
                  <div class="description">
                    {{ item.status }}
                  </div>

                  <!-- Technology Stack -->
                  <div class="tech-stack">
                    {{ item.tech }}
                  </div>

                  <!-- Links Section -->
                  <div class="links-wrapper">
                    <a v-if="item.github !== 'null'" :href="item.github" target="_blank" rel="noreferrer"
                      title="View github repository" class="icon-link">
                      <svg stroke="currentColor" fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round"
                        stroke-linejoin="round" height="16" width="16" xmlns="http://www.w3.org/2000/svg">
                        <path
                          d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22">
                        </path>
                      </svg>
                    </a>
                    <a v-if="item.demo !== 'null'" :href="item.demo" target="_blank" rel="noreferrer"
                      title="View finished project" class="icon-link">
                      <svg stroke="currentColor" fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round"
                        stroke-linejoin="round" height="18" width="18" xmlns="http://www.w3.org/2000/svg">
                        <path d="M18 13v6a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h6"></path>
                        <polyline points="15 3 21 3 21 9"></polyline>
                        <line x1="10" y1="14" x2="21" y2="3"></line>
                      </svg>
                    </a>
                  </div>
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
/* Base Styles */
.portfolio-section {
  background-color: #121212;
}

/* Card Styles */
.item-card {
  @apply relative overflow-hidden;
  height: 450px;
  background: rgba(30, 30, 31, 0.8);
  backdrop-filter: blur(8px);
  transition: all 0.5s cubic-bezier(0.4, 0, 0.2, 1);
  border: 1px solid rgba(56, 56, 56, 0.5);
  border-radius: 0.75rem;
}

/* Image Container */
.zoom-in {
  width: 100%;
  height: 200px;
  overflow: hidden;
  border-radius: 8px;
  position: relative;
}

.zoom-in img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: transform 0.8s cubic-bezier(0.4, 0, 0.2, 1);
}

/* Content Wrapper */
.content-wrapper {
  padding: 1.25rem;
  height: calc(100% - 200px);
  display: flex;
  flex-direction: column;
}

/* Title Styles */
.title-text {
  font-size: 1.25rem;
  margin-bottom: 0.75rem;
  color: #ffffff;
}

/* Description Styles */
.description {
  font-size: 0.875rem;
  color: #c1c1c1;
  margin-bottom: 1rem;
  flex-grow: 1;
  overflow-y: auto;
}

/* Tech Stack Styles */
.tech-stack {
  color: #ffd700;
  font-size: 0.875rem;
  margin-bottom: 1rem;
}

/* Links Section */
.links-wrapper {
  display: flex;
  justify-content: flex-end;
  gap: 0.75rem;
}

.icon-link {
  color: #ffd700;
  transition: all 0.3s ease;
}

/* Hover Effects */
.item-card:hover {
  transform: translateY(-8px);
  background: rgba(40, 40, 40, 0.95);
  box-shadow: 0 15px 30px rgba(0, 0, 0, 0.3);
  border-color: rgba(255, 215, 0, 0.2);
}

.item-card:hover .zoom-in img {
  transform: scale(1.1) rotate(-2deg);
}

.icon-link:hover {
  transform: scale(1.2);
  color: #ffffff;
}

/* Animations */
.fade-zoom-in {
  animation: cardEntrance 0.8s cubic-bezier(0.4, 0, 0.2, 1) forwards;
}

@keyframes cardEntrance {
  from {
    opacity: 0;
    transform: scale(0.95);
  }

  to {
    opacity: 1;
    transform: scale(1);
  }
}

/* Scrollbar Styling */
.description::-webkit-scrollbar {
  width: 4px;
}

.description::-webkit-scrollbar-track {
  background: rgba(30, 30, 31, 0.8);
}

.description::-webkit-scrollbar-thumb {
  background: #ffd700;
  border-radius: 2px;
}

/* Responsive Adjustments */
@media (max-width: 768px) {
  .item-card {
    height: auto;
    min-height: 400px;
  }

  .zoom-in {
    height: 180px;
  }

  .content-wrapper {
    height: auto;
  }
}
</style>