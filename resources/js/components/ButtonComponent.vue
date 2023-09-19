<template>
  <button type="button" :class="'btn btn-'+color+' mt-1'" @click="toggleShow">{{buttonName}}</button>
</template>
<script>
export default {
  props: {
    color: String,
    buttonName: String,
  },
  methods: {
    toggleShow() {
      // Emit event ke komponen induk untuk mengubah nilai show
      this.$emit('toggle-show');
    },
  },
};
</script>
