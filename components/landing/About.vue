<script setup>
definePageMeta({
  layout: 'landing',
})


const TeamImg4 = 'https://source.unsplash.com/IF9TK5Uy-KI'

import TeamImg1 from '~/assets/img/Anna.jpg'
import TeamImg2 from '~/assets/img/c_erbay.jpg'
import TeamImg3 from '~/assets/img/paco1.jpg'
import TeamImg5 from '~/assets/img/rüdiger.jpg'

const team = [
  {
    name: 'Anna Balthasar',
    title: 'Co-Founder & CEO',
    avatar: {
      src: TeamImg1,
      width: 480,
      height: 560,
    },
  },
  {
    name: 'Civan Erbay',
    title: 'Co-Founder & Development',
    avatar: {
      src: TeamImg2,
      width: 580,
      height: 580,
    },
  },
  {
    name: "Francisco 'Paco' Muro",
    title: 'Co-Founder & Creative Technologist',
    avatar: {
      src: TeamImg3,
      width: 580,
      height: 580,
    },
  },
  {
    name: 'Martin Sprundflasche',
    title: 'Data Scientist',
    avatar: {
      src: TeamImg4,
      width: 580,
      height: 580,
    },
  },
 /*  {
    name: 'Christian Straßer',
    title: 'Data Scientist',
    avatar: {
      src: TeamImg5,
      width: 580,
      height: 580,
    },
  }, */
  {
    name: 'Rüdiger Hass',
    title: 'QA Engineer',
    avatar: {
      src: TeamImg5,
      width: 580,
      height: 580,
    },
  },
]
</script>

<template>
  <LandingContainer>
    <LandingSectionhead>
      <template v-slot:title>About</template>
      <!-- <template v-slot:desc>We are a small passionate team.</template> -->
    </LandingSectionhead>

    <div class="flex flex-col gap-3 mx-auto max-w-4xl mt-16">
      <h2 class="font-bold text-3xl text-gray-800">
        Empowering the world with AI.
      </h2>
      <p class="text-lg leading-relaxed text-slate-500">
        We're a multi-cultural team with diverse backgrounds, bringing
        different personalities, experiences and skills to the job.
      </p>
    </div>
    <div class="grid md:grid-cols-3 gap-10 mx-auto max-w-4xl mt-12">
      <div v-for="item of team" class="group">
        <div class="w-full aspect-square">
          <img
            :src="item.avatar.src"
            :width="item.avatar.width"
            :height="item.avatar.height"
            format="avif"
            alt="Team"
            class="w-full h-full object-cover rounded transition group-hover:-translate-y-1 group-hover:shadow-xl"
          />
        </div>

        <div class="mt-4 text-center">
          <h2 class="text-lg text-gray-800">{{ item.name }}</h2>
          <h3 class="text-sm text-slate-500">{{ item.title }}</h3>
        </div>
      </div>
      <!-- {
        team.map((item) => (
          <div class="group">
            <div class="w-full aspect-square">
              <Image
                {...item.avatar}
                format="avif"
                alt="Team"
                class="w-full h-full object-cover rounded transition  group-hover:-translate-y-1 group-hover:shadow-xl"
              />
            </div>

            <div class="mt-4 text-center">
              <h2 class="text-lg text-gray-800"> {item.name}</h2>
              <h3 class="text-sm text-slate-500"> {item.title}</h3>
            </div>
          </div>
        ))
      } -->
    </div>
  </LandingContainer>
</template>
