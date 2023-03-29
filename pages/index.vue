<template>
  <div>
    <HeaderComponent></HeaderComponent>
    <div class="w-4/5 flex my-20 items-center relative sm:w-1/3 mx-auto">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        fill="none"
        viewBox="0 0 24 24"
        stroke-width="1.5"
        stroke="currentColor"
        class="w-6 h-6 absolute left-3"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          d="M21 21l-5.197-5.197m0 0A7.5 7.5 0 105.196 5.196a7.5 7.5 0 0010.607 10.607z"
        />
      </svg>

      <input
        v-model="searchItem"
        placeholder="Search"
        type="text"
        class="border border-gray-700 rounded-lg w-full h-10 px-11 tracking-wider font-serif"
      />
    </div>
    <div
      class="grid grid-cols-1 space-y-9 lg:grid-cols-3 lg:space-y-0 w-4/5 mx-auto"
    >
      <CardComponent
        v-for="card in result"
        :key="card.id"
        :recipe-id="card.id"
        :title="card.title"
        :text="card.text"
        :image="card.image"
        :items="card.items"
      >
      </CardComponent>
    </div>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
  data() {
    return {
      recipes: [
        {
          id: 1,
          title: 'きのこのマリネ',
          text: 'シャキシャキきのこのマリネをおうちで手軽に！白だしとレモン汁でさっぱり美味しい',
          items: ['きのこ', '白だし', 'レモン汁'],
          image: 'mushroom',
        },
        {
          id: 2,
          title: 'ローストビーフ',
          text: 'オーブンでじっくり焼くローストビーフ。たまねぎソースが良いアクセント',
          items: ['牛肉', 'たまねぎ'],
          image: 'beef',
        },
        {
          id: 3,
          title: 'なす',
          text: 'ぷりっ',
          items: ['きのこ', '白だし'],
          image: 'beef',
        },
        {
          id: 4,
          title: 'なす',
          text: 'ぷりっ',
          items: ['きのこ', '白だし'],
          image: 'beef',
        },
      ],
      searchItem: '',
    }
  },
  computed: {
    result() {
      if (this.searchItem === '') {
        return this.recipes
      } else {
        return this.recipes.filter((recipe) => {
          const result = recipe.items.find((item) => {
            return item.includes(this.searchItem)
          })
          return result !== undefined || recipe.title.includes(this.searchItem)
        })
      }
    },
  },
}
</script>
