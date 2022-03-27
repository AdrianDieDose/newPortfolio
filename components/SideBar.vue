<template>
  <div
    class="fixed top-0 left-0 h-screen w-52 m-0 flex flex-col bg-gray-900 text-white shadow-lg"
  >
    <side-bar-icon :icon="icon" :class="size" :tooltip="tooltip" />
    <side-bar-icon :icon="icon2" :class="size" :tooltip="tooltip" />
    <side-bar-icon :icon="icon3" :class="size" :tooltip="tooltip" />
    <side-bar-icon :icon="icon4" :class="size" :tooltip="tooltip" />
  </div>
</template>

<script>
import SideBarIcon from '@/components/SideBarIcon.vue'
export default {
  name: 'SideBar',
  components: { SideBarIcon },
  data() {
    return {
      icon: 'fa-solid fa-user-secret',
      icon2: 'fa-solid fa-align-left',
      icon3: 'fa-solid fa-apple-whole',
      icon4: 'fa-solid fa-arrow-pointer',
      size: 'fa-4x',
      tooltip1: 'This is a tooltip',
    }
  },
  computed: {
    tooltip() {
      return this.tooltip1
    },
  },
}
</script>
