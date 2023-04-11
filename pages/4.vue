import HeaderComponent from '../components/HeaderComponent.vue';

<template>
  <div class="pb-10">
    <HeaderComponent></HeaderComponent>
    <div class="w-4/5 lg:w-3/5 mx-auto">
      <h1 class="pt-10 font-bold text-2xl">アラビアータ</h1>

      <div class="flex flex-col space-y-9 lg:flex-row lg:items-center py-10">
        <div class="flex flex-col flex-1">
          <img class="w-80 h-64" src="~/assets/image/img4.jpg" alt="" />
        </div>
        <div class="mx-auto flex-1 align-top w-full">
          <h2 class="font-bold pb-3">&lt; 材料（2人分） &gt;</h2>
          <ul
            class="flex flex-col space-y-1 [&>li]:border-dotted [&>li]:border-slate-300 [&>li]:border-b-2 [&>li]:flex [&>li]:justify-between lg:px-5"
          >
            <p class="text-sm"></p>

            <li>
              <p>お好きなパスタ</p>
              <p>160g</p>
            </li>
            <li>
              <p>トマト缶</p>
              <p>1缶</p>
            </li>
            <li>
              <p>にんにくみじん切り</p>
              <p>1片</p>
            </li>
            <li>
              <p>赤唐辛子</p>
              <p>1〜2本</p>
            </li>
            <li>
              <p>オリーブオイル</p>
              <p>大さじ1</p>
            </li>
            <li>
              <p>塩</p>
              <p>適量</p>
            </li>
            <li>
              <p>水</p>
              <p>400g</p>
            </li>
          </ul>
        </div>
      </div>

      <div>
        <h2 class="font-bold py-5">&lt; 作り方 &gt;</h2>
        <ul class="list-decimal px-5 flex flex-col space-y-1">
          <li>
            フライパンにオリーブオイル、にんにく、赤唐辛子を入れ弱火で熱する。
          </li>
          <li>香りが出てきたらトマト缶、水、塩を加え軽く沸騰させる。</li>
          <li>
            パスタを加え表記時間通りに茹でる。時々パスタがくっつかないように混ぜる。
          </li>
          <li>蓋をあけ、ひと混ぜしたら完成。</li>
        </ul>
      </div>
    </div>
  </div>
</template>
