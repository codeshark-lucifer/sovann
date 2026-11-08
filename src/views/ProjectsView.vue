<script setup>
import { ref } from 'vue'

const data = ref([
  {
    id: '001',
    thumbnail: 'https://images.unsplash.com/photo-1522202176988-66273c2fd55f?auto=format&fit=crop&w=900&q=80',
    url: 'https://example.com/project-1',
    title: 'E-commerce Dashboard',
    description: 'A modern dashboard for managing online sales, inventory, and customer insights.',
    category: 'UI/UX Design'
  },
  {
    id: '002',
    thumbnail: 'https://images.unsplash.com/photo-1460925895917-afdab827c52f?auto=format&fit=crop&w=900&q=80',
    url: 'https://example.com/project-2',
    title: 'Learning Platform',
    description: 'An educational platform with lesson tracking, progress analytics, and course enrollment.',
    category: 'Web App'
  },
  {
    id: '003',
    thumbnail: 'https://images.unsplash.com/photo-1516321318423-f06f85e504b3?auto=format&fit=crop&w=900&q=80',
    url: 'https://example.com/project-3',
    title: 'Travel Booking System',
    description: 'A responsive booking website for flights, hotels, and travel packages.',
    category: 'Frontend Development'
  },
  {
    id: '004',
    thumbnail: 'https://images.unsplash.com/photo-1552664730-d307ca884978?auto=format&fit=crop&w=900&q=80',
    url: 'https://example.com/project-4',
    title: 'Business Portfolio',
    description: 'A sleek portfolio website for a creative agency with strong branding and storytelling.',
    category: 'Branding'
  }
])
</script>

<template>
  <section class="px-6 py-12 md:px-12 lg:px-20">
    <div class="mb-8 text-center">
      <p class="text-sm font-semibold uppercase tracking-[0.25em] text-emerald-600">Projects</p>
      <h1 class="mt-3 text-4xl font-bold text-slate-900">My Recent Work</h1>
    </div>

    <ul class="grid gap-8 md:grid-cols-2 xl:grid-cols-3">
      <li v-for="item in data" :key="item.id" class="overflow-hidden rounded-2xl border border-slate-200 bg-white shadow-sm transition hover:-translate-y-1 hover:shadow-lg">
        <img :src="item.thumbnail" :alt="item.title" class="h-56 w-full object-cover" />

        <div class="space-y-4 p-5">
          <span class="inline-block rounded-full bg-emerald-100 px-3 py-1 text-xs font-semibold uppercase tracking-wide text-emerald-700">
            {{ item.category }}
          </span>

          <div>
            <h3 class="text-2xl font-bold text-slate-800">{{ item.title }}</h3>
            <p class="mt-2 text-sm leading-6 text-slate-600">{{ item.description }}</p>
          </div>

          <a
            :href="item.url"
            target="_blank"
            class="inline-block rounded-md bg-slate-900 px-4 py-2 text-sm font-medium text-white transition hover:bg-slate-700"
          >
            View Project
          </a>
        </div>
      </li>
    </ul>
  </section>
</template>
