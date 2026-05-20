<script setup>
import Header from '@/components/Header.vue';
import { ArrowLeftIcon, SearchIcon, XIcon } from '@lucide/vue';
import { ref } from 'vue';

const query = ref('');
</script>

<template>
  <main class="max-w-7xl w-full mx-auto min-h-screen h-full px-4 pb-5">
    <Header />
    <a href="/"
      class="w-max mt-5 flex items-center gap-1 text-sm hover:underline text-[#A0A0C0] hover:text-white transition-colors">
      <ArrowLeftIcon class="w-4 h-4" />
      Voltar
    </a>

    <section class="mt-6">
      <div class="relative flex items-center">
        <SearchIcon class="absolute left-3 w-4 h-4 text-[#505070] pointer-events-none" />
        <input v-model="query" type="text" placeholder="Pesquisar um Destino ou Comunidade"
          class="w-full bg-[#0F0F1E] border-2 border-[#16162A] rounded-lg pl-9 pr-9 py-2.5 text-sm text-white placeholder-[#505070] outline-none focus:border-[#b06aff5c] transition-colors" />
        <button v-if="query" @click="query = ''"
          class="absolute right-3 text-[#505070] hover:text-white transition-colors">
          <XIcon class="w-4 h-4" />
        </button>
      </div>
    </section>
  </main>
</template>