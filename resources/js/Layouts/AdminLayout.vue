<template>
  <Head :title="title" />
  <div>
    <!-- Main Sidebar Container -->
    <SideBar />
    <div class="relative md:ml-64 bg-blueGray-100">
      <header class="bg-white" v-if="$slots.header">
        <div class="max-w-full mx-auto py-8 px-14 sm:px-14 lg:px-14">
          <slot name="header"></slot>
        </div>

      </header>

      <!-- page content -->
      <div class="py-7">
        <div class="max-w-full mx-auto px-14 sm:px-14 lg:px-14">
          <main>
            <slot></slot>
          </main>
        </div>
      </div>

      <!-- <header-stats /> -->
      <!-- <div class="px-4 md:px-10 mx-auto w-full -m-24">
        <footer-admin />
      </div> -->
    </div>
  </div>
</template>
<script>
import SideBar from "@/Components/SideBar/AdminSidebar.vue";
export default {
  props: {
    title: String,
  },
  components: {
    SideBar,
  },
};
</script>
