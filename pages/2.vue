import HeaderComponent from '../components/HeaderComponent.vue';

<template>
  <div class="pb-10">
    <HeaderComponent></HeaderComponent>
    <div class="w-4/5 lg:w-3/5 mx-auto">
      <h1 class="pt-10 font-bold text-2xl">ローストビーフ</h1>

      <div class="flex flex-col space-y-9 lg:flex-row lg:items-center py-10">
        <div class="flex flex-col flex-1">
          <img class="w-80 h-64" src="~/assets/image/img2.jpg" alt="" />
        </div>
        <div class="mx-auto flex-1 align-top w-full">
          <h2 class="font-bold pb-3">&lt; 材料 &gt;</h2>
          <ul
            class="lg:px-5 flex flex-col space-y-1 [&>li]:border-dotted [&>li]:border-slate-300 [&>li]:border-b-2 [&>li]:flex [&>li]:justify-between"
          >
            <li>
              <p>牛もも肉</p>
              <p>300g</p>
            </li>
            <li>
              <p>オリーブオイル</p>
              <p>大さじ1</p>
            </li>
            <h3>A</h3>
            <li>
              <p>塩</p>
              <p>適量</p>
            </li>
            <li>
              <p>こしょう</p>
              <p>適量</p>
            </li>
            <p class="text-sm"></p>
            <h3>B</h3>
            <li>
              <p>たまねぎ</p>
              <p>半分</p>
            </li>
            <li>
              <p>料理酒</p>
              <p>大さじ1</p>
            </li>
            <li>
              <p>しょうゆ</p>
              <p>大さじ1</p>
            </li>
            <li>
              <p>砂糖</p>
              <p>小さじ2</p>
            </li>
            <li>
              <p>にんにく</p>
              <p>1片</p>
            </li>
          </ul>
        </div>
      </div>

      <div>
        <h2 class="font-bold py-5">&lt; 作り方 &gt;</h2>
        <ul class="list-decimal px-5 flex flex-col space-y-1">
          <p>
            <span class="font-bold">準備1：</span>オーブンを120度に予熱しておく
          </p>
          <p>
            <span class="font-bold">準備2：</span>牛もも肉は常温に戻しておく
          </p>

          <li>牛もも肉全体に<span class="font-bold">A</span>をすり込む。</li>
          <li>
            フライパンにオリーブオイルを入れ、<span class="font-bold">1</span
            >の前面に焼き色が付くまで強火で焼く。
          </li>
          <li>
            天板にクッキングシートを敷き、<span class="font-bold">2</span
            >を乗せて120度のオーブンで25分程焼き、さらに20分置く。
          </li>
          <li>
            <span class="font-bold">2</span
            >で使用したフライパンにBを入れ中火で熱する。
          </li>
          <li>
            <span class="font-bold">3</span
            >を好みの厚さにスライスし皿に盛り付け、<span class="font-bold"
              >4</span
            >をかける。
          </li>
          <li>完成</li>
        </ul>
      </div>
    </div>
  </div>
</template>
