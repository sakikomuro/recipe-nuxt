import HeaderComponent from '../components/HeaderComponent.vue';

<template>
  <div class="pb-10">
    <HeaderComponent></HeaderComponent>
    <div class="w-4/5 lg:w-3/5 mx-auto">
      <h1 class="pt-10 font-bold text-2xl">きのこのマリネ</h1>

      <div class="flex flex-col space-y-9 lg:flex-row lg:items-center py-10">
        <div class="flex flex-col flex-1">
          <img class="w-80 h-64" src="~/assets/image/img1.jpg" alt="" />
        </div>
        <div class="mx-auto flex-1 align-top w-full">
          <h2 class="font-bold pb-3">&lt; 材料 &gt;</h2>
          <ul
            class="flex flex-col space-y-1 [&>li]:border-dotted [&>li]:border-slate-300 [&>li]:border-b-2 [&>li]:flex [&>li]:justify-between lg:px-5"
          >
            <li>
              <p>エリンギ</p>
              <p>1パック</p>
            </li>
            <li>
              <p>まいたけ</p>
              <p>1パック</p>
            </li>
            <li>
              <p>ブナピー</p>
              <p>1パック</p>
            </li>

            <p class="text-sm">（好きなきのこで結構です）</p>

            <h3>A</h3>
            <li>
              <p>白だし</p>
              <p>大さじ3</p>
            </li>
            <li>
              <p>レモン汁</p>
              <p>大さじ2</p>
            </li>
            <li>
              <p>お酢</p>
              <p>大さじ2</p>
            </li>
            <li>
              <p>オリーブオイル</p>
              <p>大さじ1</p>
            </li>
            <li>
              <p>こしょう</p>
              <p>少々</p>
            </li>
          </ul>
        </div>
      </div>

      <div>
        <h2 class="font-bold py-5">&lt; 作り方 &gt;</h2>
        <ul class="list-decimal px-5 flex flex-col space-y-1">
          <li>きのこを好みの大きさに割く。大きめに割くのがおすすめ。</li>
          <li>
            きのこをフライパンに入れ、強火で熱する。この時きのこをあまり動かさない。
          </li>
          <li>きのこが汗をかいてきたら上下返し、軽く炒める。</li>
          <li>
            一旦きのこを皿に取り出し、同じフライパンに<span class="font-bold"
              >A</span
            >を入れ軽く煮立たせる。
          </li>
          <li>
            取り出しておいたきのこを<span class="font-bold">3</span
            >に入れ、混ぜ合わせる
          </li>
          <li>粗熱をとって冷蔵庫で30分〜1時間冷やして完成</li>
        </ul>
      </div>
    </div>
  </div>
</template>
