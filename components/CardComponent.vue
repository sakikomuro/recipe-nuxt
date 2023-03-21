<template>
  <div
    class="border border-red-200 w-64 mx-auto rounded-lg h-80 hover:opacity-75 hover:cursor-pointer"
  >
    <NuxtLink :to="'/' + recipeId">
      <img class="rounded-t-lg" :src="url" />
      <h2 class="py-5 px-2 text-lg font-semibold">{{ title }}</h2>
      <p class="px-2 text-xs">
        {{ text }}
      </p>
    </NuxtLink>
  </div>
</template>

<script>
export default {
  props: {
    title: { type: String, default: '' },
    text: { type: String, default: '' },
    url: { type: String, default: '' },
    recipeId: { type: Number, default: 0 },
  },
}
</script>
