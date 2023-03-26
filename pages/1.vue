import HeaderComponent from '../components/HeaderComponent.vue';

<template>
  <div>
    <HeaderComponent></HeaderComponent>
    <div class="w-3/5 mx-auto">
      <h1 class="pt-10 font-bold text-2xl">きのこのマリネ</h1>

      <div class="flex items-center py-10">
        <div class="flex flex-col flex-1">
          <img
            class="w-80 h-64"
            src="https://www.higashimaru.co.jp/img/recipe/0324_pic.jpg"
            alt=""
          />
        </div>
        <div class="mx-auto flex-1 h-64 align-top">
          <h2 class="font-bold py-5">&lt; 材料 &gt;</h2>
          <ul class="list-disc px-5 flex flex-col space-y-1">
            <li>好きなきのこ3種</li>
            <li>白だし</li>
            <li>レモン汁</li>
            <li>オリーブオイル</li>
          </ul>
        </div>
      </div>

      <div>
        <h2 class="font-bold py-5">&lt; 作り方 &gt;</h2>
        <ul class="list-decimal px-5 flex flex-col space-y-1">
          <li>きのこをフライパンに入れ、汗をかくまで強火で放置しておく</li>
          <li>たれを混ぜ合わせておく</li>
          <li>きのこが汗をかいてきたら上下返し、軽く炒める</li>
          <li>
            きのこを皿に取り出し、同じフライパンにタレを入れ軽く煮立たせる。この時フライパンをこそぐようにする
          </li>
          <li>
            お皿に取り出しておいたきのこを再度フライパンに乗せ混ぜ合わせる
          </li>
          <li>完成</li>
        </ul>
      </div>
    </div>
  </div>
</template>
