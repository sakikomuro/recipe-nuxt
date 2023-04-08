<template>
  <NuxtLink to="/">
    <h1
      class="font-serif font-bold text-red-400 text-5xl text-center tracking-wider border-b py-4"
    >
      <button @click="headerClick">Recipe</button>
    </h1>
  </NuxtLink>
</template>

<script>
export default {
  methods: {
    headerClick() {
      this.$emit('onClick')
    },
  },
}
</script>
