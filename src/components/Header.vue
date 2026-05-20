<script setup>
import { CopyIcon } from '@lucide/vue';

</script>

<template>
  <header class="flex justify-between items-center pt-5 p-2.5">
    <div>
      <a href="/" class="text-2xl font-thin italic">CHRONOVERSE</a>
      <p class="text-[#A0A0C0] text-xs mt-1">Plataforma de Identidade e Progresso Interoperável</p>
    </div>
    <div class="flex justify-between items-center gap-6 text-[#A0A0C0] text-xs">
      <span>CONECTADO COMO <span class="text-gray-300">USUARIO 123</span></span>
      <span class="w-px h-8 bg-gray-800 block rounded"></span>
      <div class="cursor-pointer flex items-center gap-1">
        <span>X0d12Des...</span>
        <CopyIcon class="w-3.5 h-3.5" />
      </div>
    </div>
  </header>
</template>
