<script lang="ts" setup>
import { LogIn } from 'lucide-vue-next'
</script>

<template>
  <header class="sticky top-0 z-50 w-full border-b bg-background/95 backdrop-blur supports-[backdrop-filter]:bg-background/60">
    <div class="container flex h-14 items-center">
      <div class="mr-4 flex">
        <NuxtLink to="/" class="mr-6 flex items-center space-x-2">
          <span class="font-bold text-lg">AI Review Hub</span>
        </NuxtLink>
      </div>
      <div class="flex flex-1 items-center justify-between space-x-2 md:justify-end">
        <nav class="flex items-center space-x-4">
          <Button variant="ghost">
            Home
          </Button>
          <Button variant="ghost">
            Categories
          </Button>
          <Button variant="ghost">
            About
          </Button>
        </nav>
        <div class="flex items-center space-x-2">
          <LangToggle />
          <ModeToggle />
          <Button variant="default" class="gap-2">
            <LogIn class="h-5 w-5" />
            Sign in
          </Button>
        </div>
      </div>
    </div>
  </header>
</template>
