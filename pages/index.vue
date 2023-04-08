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
        placeholder="食材、料理名で検索"
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
          searches: [
            'キノコ',
            'まりね',
            'エリンギ',
            'えりんぎ',
            'ブナピー',
            'しめじ',
            'まいたけ',
          ],
          image: 'img1',
        },
        {
          id: 2,
          title: 'ローストビーフ',
          text: 'オーブンでじっくり焼くローストビーフ。たまねぎソースが良いアクセント',
          items: ['牛肉', 'たまねぎ'],
          searches: [
            '牛肉',
            '牛もも肉',
            '玉ねぎ',
            'たまねぎ',
            'タマネギ',
            'オーブン',
          ],
          image: 'img2',
        },
        {
          id: 3,
          title: 'アヒージョ',
          text: 'にんにくの風味で食欲をそそるアヒージョ。簡単、美味しいアヒージョ。',
          items: ['きのこ', 'ベーコン', 'シーフード'],
          searches: [
            'きのこ',
            'キノコ',
            'マッシュルーム',
            'ベーコン',
            'えび',
            'エビ',
            'エリンギ',
            'ブロッコリー',
            'トマト',
            'シーフード',
          ],
          image: 'img3',
        },
        {
          id: 4,
          title: 'アラビアータ',
          text: 'フライパンひとつで簡単。お好きなパスタで作ってください',
          items: ['トマト', 'パスタ', 'にんにく'],
          searches: [
            'あらびあーた',
            'ニンニク',
            'にんにく',
            'トマト',
            'トマト缶',
            '唐辛子',
            'とうがらし',
            'コンキリエ',
            'パスタ',
            'ぱすた',
          ],
          image: 'img4',
        },
        {
          id: 5,
          title: '鶏むね肉の甘辛唐揚げ',
          text: 'むね肉を使用しているのでヘルシーでコスパ抜群！',
          items: ['鶏むね肉'],
          searches: ['胸肉', '鶏肉', 'あんかけ', 'とり肉', 'むね肉'],
          image: 'img5',
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
          const result = recipe.searches.find((search) => {
            return search.includes(this.searchItem)
          })
          return result !== undefined || recipe.title.includes(this.searchItem)
        })
      }
    },
  },
}
</script>
