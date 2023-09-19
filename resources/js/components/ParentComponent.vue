<template>
  <div class="container">
    <div class="mt-5">
      <p v-if="show == false">Hello... Im Bagus Untoro</p>
      <p v-if="show == true">Im Intern in Jesara</p>
    </div>
    <button-component color="primary" buttonName="Click me" @toggle-show="toggleShow" />
  </div>
</template>
<script>
export default {
  data() {
    return {
      show: false,
    };
  },
  methods: {
    toggleShow() {
      // Ubah nilai show ketika tombol di komponen anak diklik
      this.show = !this.show;
    },
  },
};
</script>
