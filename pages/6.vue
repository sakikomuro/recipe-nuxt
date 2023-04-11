import HeaderComponent from '../components/HeaderComponent.vue';

<template>
  <div class="pb-10">
    <HeaderComponent></HeaderComponent>
    <div class="w-4/5 lg:w-3/5 mx-auto">
      <h1 class="pt-10 font-bold text-2xl">よだれ鶏</h1>

      <div class="flex flex-col space-y-9 lg:flex-row lg:items-center py-10">
        <div class="flex flex-col flex-1">
          <img class="w-80 h-64" src="~/assets/image/img6.jpg" alt="" />
        </div>
        <div class="mx-auto flex-1 align-top w-full">
          <h2 class="font-bold pb-3">&lt; 材料 &gt;</h2>
          <ul
            class="flex flex-col space-y-1 [&>li]:border-dotted [&>li]:border-slate-300 [&>li]:border-b-2 [&>li]:flex [&>li]:justify-between lg:px-5"
          >
            <li>
              <p>鶏むね肉</p>
              <p>200g</p>
            </li>
            <li>
              <p>長ねぎ</p>
              <p>半分</p>
            </li>
            <li>
              <p>料理酒</p>
              <p>大さじ1</p>
            </li>

            <li>
              <p>砂糖</p>
              <p>小さじ1</p>
            </li>

            <h3>A</h3>
            <li>
              <p>しょうゆ</p>
              <p>大さじ1</p>
            </li>
            <li>
              <p>砂糖</p>
              <p>大さじ1</p>
            </li>
            <li>
              <p>お酢</p>
              <p>大さじ1</p>
            </li>
            <li>
              <p>ラー油</p>
              <p>大さじ1</p>
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
          <li>
            鶏むね肉にフォークで数カ所に穴をあけ、料理酒と砂糖を加え馴染ませる。
          </li>
          <li>
            <span class="font-bold">1</span
            >を耐熱皿に入れてラップをかけ500Wで5分加熱する。一度取り出して鶏肉を裏返し、さらに5分加熱する。火が通っていないようなら様子を見ながら加熱する。
          </li>
          <li>
            <span class="font-bold">2</span
            >を取り出して粗熱を取り、お好みの厚さにスライスする。
          </li>
          <li>
            長ねぎをみじん切りにし<span class="font-bold">A</span
            >と混ぜ合わせる。
          </li>
          <li>
            お皿に<span class="font-bold">3</span>を盛り付け、<span
              class="font-bold"
              >4</span
            >を上からかけたら完成。
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>
