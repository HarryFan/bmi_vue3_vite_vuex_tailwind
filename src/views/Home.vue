<script>
import { defineComponent } from 'vue'
import ButtonRepo from '@/components/ButtonRepo.vue'

export default defineComponent({
  components: { ButtonRepo },
})
</script>

<template>
  <main class="dark:bg-gray-900">
    <div class="bg-gray-50 dark:bg-gray-800"> <!-- 深色模式下背景色更改 -->
      <div
        class="max-w-screen-xl px-4 py-12 mx-auto sm:px-6 lg:py-16 lg:px-8 lg:flex lg:items-center lg:justify-between"
      >
        <h2
          class="text-3xl font-extrabold leading-9 tracking-tight text-gray-900 dark:text-white sm:text-4xl sm:leading-10" <!-- 深色模式下标题文本颜色更改 -->
        >
          Ready to dive in?
          <br />
          <span class="text-indigo-600 dark:text-indigo-400"> <!-- 深色模式下标注文本颜色更改 -->
            Vite 2.x + Vue 3.x + Tailwind 2.x
          </span>
        </h2>
        <div class="flex mt-8 lg:flex-shrink-0 lg:mt-0">
          <div class="inline-flex rounded-md shadow">
            <router-link
              to="/about"
              class="inline-flex items-center justify-center px-5 py-3 text-base font-medium leading-6 text-white transition duration-150 ease-in-out bg-indigo-600 border border-transparent rounded-md hover:bg-indigo-500 dark:hover:bg-indigo-400 focus:outline-none dark:bg-indigo-700 dark:border-indigo-700" <!-- 深色模式下路由链接样式更改 -->
            >
              Next Page
            </router-link>
          </div>
          <ButtonRepo /> <!-- 确保ButtonRepo组件也有适当的深色模式样式 -->
        </div>
      </div>
    </div>
  </main>
</template>
