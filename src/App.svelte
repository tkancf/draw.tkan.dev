<script lang="ts">
  import Article from './Article.svelte';
  let title: string = "draw.tkan.dev";
  let article_infos = [
    {
      title: "2020/08/14",
      description: "お絵描きはじめました。にじさんじの愛園愛美さん", image: "images/20200814_aizono.jpg",
      alt: "愛園愛美",
      keep_list: ["下手ながらも全身を色付きで描いた"],
      problem_list: [
        "顔が可愛く描けてない",
        "手の形がおかしい",
        "髪が折り紙みたい"
        ],
      try_list: [
        "参考にする対象の絵の比率を測って、それを参考にして描く",
        "四角で形を作った後に、丸く指を描くようにすると多少マシになった気がするので、それをもう少し練習してみる",
        "房ごとに線画を描く"
        ]
    },
    {
      title: "2020/08/15",
      description: "今日描いたのはにじさんじの相羽ういはさん 公式のメンバー一覧の模写です。https://nijisanji.ichikara.co.jp/member/", image: "images/20200815相羽ういは.jpg",
      alt: "相羽ういは",
      keep_list: [
        "下手ながらも全身を色付きで描いた",
        "前回より目が上手く描けるようになった"
      ],
      problem_list: [
        "髪の塗り方をどうすればよいか分からない",
        "足が太い(女性らしい足の太さとか、腰のかたちで描きたい)",
        "影の描き方、光が当たっている部分の描き方が分からない"
      ],
      try_list: [
        "YouTubeに髪の描き方みたいな動画がいくつかあったので、それを観て参考にする",
        "人体のバランスがそもそもよく分かっていないので、解説サイトを読んで練習する"
      ]
    }
  ]
</script>

<main>
  <h1>{title}</h1>
  <Article article_infos={article_infos} />
</main>

<style>
</style>
