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
        placeholder="Search"
        type="text"
        class="border border-gray-700 rounded-lg w-full h-10 px-11 tracking-wider"
      />
    </div>
    <div
      class="grid grid-cols-1 space-y-9 lg:grid-cols-3 lg:space-y-0 w-4/5 mx-auto"
    >
      <CardComponent
        v-for="card in list"
        :key="card.id"
        :recipe-id="card.id"
        :title="card.title"
        :text="card.text"
        :url="card.url"
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
      list: [
        {
          id: 1,
          title: 'さつまいも',
          text: 'ほくほく',
          url: 'https://smtgvs.weathernews.jp/s/topics/img/201911/201911050195_top_img_A.jpg?1573098462',
        },
        {
          id: 2,
          title: 'じゃがいも',
          text: 'わくわく',
          url: 'https://www.hyponex.co.jp/yasai_daijiten/websys/wp-content/uploads/2020/09/%E3%82%B8%E3%83%A3%E3%82%AC%E3%82%A4%E3%83%A2C-770x475.jpg',
        },
        {
          id: 3,
          title: 'なす',
          text: 'ぷりっ',
          url: 'https://cdn.macaro-ni.jp/assets/img/shutterstock/shutterstock_208420516.jpg?p=1x1',
        },
        {
          id: 4,
          title: 'なす',
          text: 'ぷりっ',
          url: 'https://cdn.macaro-ni.jp/assets/img/shutterstock/shutterstock_208420516.jpg?p=1x1',
        },
      ],
    }
  },
}
</script>
