<template>
  <div class="lg:py-5">
    <div
      class="border w-64 mx-auto rounded-lg h-80 hover:opacity-75 hover:cursor-pointer"
    >
      <label :for="recipeId">
        <img
          class="rounded-t-lg h-40 w-full"
          :src="require(`~/assets/image/${image}.jpg`)"
        />
        <h2 class="py-5 px-2 text-lg font-semibold">{{ title }}</h2>
        <p class="px-2 text-xs">
          {{ text }}
        </p>
      </label>
    </div>

    <!-- Put this part before </body> tag -->
    <input :id="recipeId" type="checkbox" class="modal-toggle" />
    <label :for="recipeId" class="modal cursor-pointer">
      <label class="modal-box relative" for="">
        <img
          class="w-4/5 m-auto"
          :src="require(`~/assets/image/${image}.jpg`)"
        />
        <h2 class="px-2 pt-7 text-lg font-semibold">使われている材料</h2>
        <div class="flex items-center space-x-2 py-8">
          <p
            v-for="item in items"
            :key="item"
            class="bg-red-200/50 w-1/3 rounded-full text-xl text-center"
          >
            {{ item }}
          </p>
        </div>
        <NuxtLink
          :to="'/' + recipeId"
          class="btn btn-outline text-red-400 flex justify-center"
          >もっと見る</NuxtLink
        >
      </label>
    </label>
  </div>
</template>

<script>
export default {
  props: {
    title: { type: String, default: '' },
    text: { type: String, default: '' },
    items: {
      type: Array,
      default: () => [],
    },
    image: { type: String, default: '' },
    recipeId: { type: Number, default: 0 },
  },
}
</script>
