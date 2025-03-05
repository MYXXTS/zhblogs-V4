<template>
  <footer class="mt-auto w-full py-12">
    <div class="mx-auto max-w-7xl">
      <div
        class="flex flex-col justify-center text-lg leading-8 text-neutral-500 dark:text-neutral-500"
      >
        <div class="w-full text-center">
          <span>尝试链接几乎所有的中文博客</span>
        </div>
        <div class="w-full text-center">
          <NuxtLink to="https://beian.miit.gov.cn">
            闽ICP备 2023011626号-3
          </NuxtLink>
        </div>
        <div class="w-full text-center">
          <span
            >Copyright © 2022 - {{ year }} |
            <NuxtLink to="https://github.com/zh-blogs">
              <i class="ri-github-fill" /> 集博栈（原中文博客列表导航）
            </NuxtLink>
          </span>
        </div>
      </div>
    </div>
  </footer>
</template>

<script lang="ts" setup>
const year = computed(() => {
  return new Date().toLocaleDateString().split('/')[0]
})
</script>
