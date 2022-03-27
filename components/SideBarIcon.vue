<template>
  <div class="sidebar-icon group">
    <font-awesome-icon :icon="icon"></font-awesome-icon>
    <span class="sidebar-tooltip group-hover:scale-100">{{ tooltip }} 🧐</span>
  </div>
</template>

<script>
export default {
  name: 'SideBarIcon',
  components: {},
  props: ['icon', 'size', 'tooltip'],
}
</script>
