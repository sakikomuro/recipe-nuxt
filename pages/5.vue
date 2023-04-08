import HeaderComponent from '../components/HeaderComponent.vue';

<template>
  <div class="pb-10">
    <HeaderComponent></HeaderComponent>
    <div class="w-4/5 lg:w-3/5 mx-auto">
      <h1 class="pt-10 font-bold text-2xl">鶏むね肉の甘辛唐揚げ</h1>

      <div class="flex flex-col space-y-9 lg:flex-row lg:items-center py-10">
        <div class="flex flex-col flex-1">
          <img class="w-80 h-64" src="~/assets/image/img5.jpg" alt="" />
        </div>
        <div class="mx-auto flex-1 align-top w-full">
          <h2 class="font-bold pb-3">&lt; 材料 &gt;</h2>
          <ul
            class="flex flex-col space-y-1 [&>li]:border-dotted [&>li]:border-slate-300 [&>li]:border-b-2 [&>li]:flex [&>li]:justify-between lg:px-5"
          >
            <li>
              <p>鶏むね肉</p>
              <p>250g</p>
            </li>
            <li>
              <p>薄力粉</p>
              <p>大さじ3</p>
            </li>
            <li>
              <p>片栗粉</p>
              <p>大さじ1</p>
            </li>

            <li>
              <p>白いりごま</p>
              <p>適量</p>
            </li>
            <li>
              <p>油</p>
              <p>適量</p>
            </li>

            <h3>A</h3>
            <li>
              <p>しょうゆ</p>
              <p>大さじ2</p>
            </li>
            <li>
              <p>みりん</p>
              <p>大さじ2</p>
            </li>
            <li>
              <p>砂糖</p>
              <p>大さじ3</p>
            </li>
            <li>
              <p>料理酒</p>
              <p>大さじ2</p>
            </li>
          </ul>
        </div>
      </div>

      <div>
        <h2 class="font-bold py-5">&lt; 作り方 &gt;</h2>
        <ul class="list-decimal px-5 flex flex-col space-y-1">
          <li>鶏肉を一口大に切り、薄力粉をまぶす。</li>
          <li>
            鍋に油を注ぎ、<span class="font-bold">1</span
            >を揚げる。鶏肉に火が通り、きつね色になったら油を切る。
          </li>
          <li>
            別のフライパンに<span class="font-bold">A</span
            >を入れ、中火で煮立たせる。
          </li>
          <li>
            水溶き片栗粉を<span class="font-bold">3</span
            >に少しずつ混ぜ合わせ、とろみをつける。
          </li>
          <li>
            <span class="font-bold">4</span>に<span class="font-bold">2</span
            >を入れ、鶏肉全体にソースを絡ませたら完成。
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>
