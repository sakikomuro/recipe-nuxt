import HeaderComponent from '../components/HeaderComponent.vue';

<template>
  <div class="pb-10">
    <HeaderComponent></HeaderComponent>
    <div class="w-4/5 lg:w-3/5 mx-auto">
      <h1 class="pt-10 font-bold text-2xl">アヒージョ</h1>

      <div class="flex flex-col space-y-9 lg:flex-row lg:items-center py-10">
        <div class="flex flex-col flex-1">
          <img class="w-80 h-64" src="~/assets/image/ajillo.jpg" alt="" />
        </div>
        <div class="mx-auto flex-1 align-top w-full">
          <h2 class="font-bold pb-3">&lt; 材料 &gt;</h2>
          <ul
            class="flex flex-col space-y-1 [&>li]:border-dotted [&>li]:border-slate-300 [&>li]:border-b-2 [&>li]:flex [&>li]:justify-between lg:px-5"
          >
            <li>
              <p>小エビ</p>
              <p>８尾</p>
            </li>
            <li>
              <p>マッシュルーム</p>
              <p>5個</p>
            </li>
            <li>
              <p>厚切りベーコン</p>
              <p>50g</p>
            </li>
            <p class="text-sm">（好きな具材で結構です）</p>

            <li>
              <p>にんにく</p>
              <p>1~2片</p>
            </li>
            <li>
              <p>オリーブオイル</p>
              <p>100ml</p>
            </li>
            <li>
              <p>塩</p>
              <p>適量</p>
            </li>
            <li>
              <p>こしょう</p>
              <p>適量</p>
            </li>
          </ul>
        </div>
      </div>

      <div>
        <h2 class="font-bold py-5">&lt; 作り方 &gt;</h2>
        <ul class="list-decimal px-5 flex flex-col space-y-1">
          <li>にんにくをみじん切りにする。</li>
          <li>
            スキレットに<span class="font-bold">1</span
            >を入れ、にんにくがきつね色になるまで熱する。
          </li>
          <li>
            <span class="font-bold">2</span
            >に小エビ、マッシュルーム、ベーコンを入れる。
          </li>
          <li>全体に火が通ったら塩とこしょうをお好みで入れる。</li>
          <li>完成</li>
        </ul>
      </div>
    </div>
  </div>
</template>
