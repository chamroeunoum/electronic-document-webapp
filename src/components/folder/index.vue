<template>
  <div class="w-full " >
    <!-- <router-view ></router-view> -->
    <router-view v-slot="{ Component }">
      <transition :name="$route.meta.transition">
        <component :is="Component" />
      </transition>
    </router-view>
  </div>
</template>
