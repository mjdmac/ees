<template>
  <admin-layout>
    <template #header>
      <!-- Task Header -->
      <div class="grid grid-cols-2">
        <div>
          <h2 class="font-semibold text-xl text-gray-800 leading-tight">
            <span>Tasks</span>
          </h2>
        </div>
        <!-- Task Header -->

        <!-- Task Page Buttons -->
        <div class="space-x-5" align="right">
            <div class="inline-block">
              <button
                @click="openModal(true)"
              >
              Create
              </button>
            </div>
        </div>
        <!-- Task Page Buttons -->

      </div>
    </template>
  </admin-layout>
</template>

<script>
import { defineComponent } from "vue";
import AdminLayout from "@/Layouts/Adminlayout";

export default defineComponent({
  components: {
    AdminLayout,
  },
});
</script>
