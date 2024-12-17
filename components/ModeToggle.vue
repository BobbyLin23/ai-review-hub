<script setup lang="ts">
import { Moon, Sun } from 'lucide-vue-next'

const colorMode = useColorMode()

function toggleTheme() {
  colorMode.preference = colorMode.value === 'dark' ? 'light' : 'dark'
}
</script>

<template>
  <Button variant="ghost" size="icon" @click="toggleTheme">
    <Sun v-if="colorMode.value === 'dark'" class="h-5 w-5" />
    <Moon v-else class="h-5 w-5" />
    <span class="sr-only">Mode Toggle</span>
  </Button>
</template>
