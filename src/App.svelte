<script lang="ts">
  import 'bulma/css/bulma.css'
  import Article from './Article.svelte'
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
      description: "にじさんじの相羽ういはさん 公式のメンバー一覧の模写 https://nijisanji.ichikara.co.jp/member/", image: "images/20200815相羽ういは.jpg",
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
    },
    {
      title: "2020/08/23",
      description: "にじさんじの月ノ美兎委員長 公式のメンバー一覧の模写 https://nijisanji.ichikara.co.jp/member/", image: "images/20200823月ノ美兎.jpg",
      alt: "月ノ美兎",
      keep_list: [
        "髪の影を描いた",
        "顔の影をつけた",
        "色塗りは乗算レイヤーでやるようにした"
      ],
      problem_list: [
        "肩幅が少し広い",
        "腰回りも少し太い",
        "他の髪に重なる部分になるときれいな線画が描けない"
      ],
      try_list: [
        "好みの絵の髪をトレスする",
        "hitokakuをやる"
      ]
    },
    {
      title: "2020/09/03",
      description: "月に寄りそう乙女の作法の桜小路ルナ様(公式のざっくり立ち絵模写)", image: "images/20200903桜小路ルナ様.jpg",
      alt: "桜小路ルナ様",
      keep_list: [
        "服の影を描いた",
        "手を描いた(模写とはいえ、以前より改善が見られる)",
        "肩幅がいい感じになった"
      ],
      problem_list: [
        "服のデザインがちょっと違う",
        "服の影の位置が違う",
        "右腕の周辺の線画が足りていないため、影がモヤッとしている",
        "目の塗りに自信がない"
      ],
      try_list: [
        "引き続きhitokakuをやる",
        "一枚コピーしたい絵を決めて、しばらくその絵だけを練習する",
        "目の塗り方をYouTube等で観る"
      ]
    },
  ]
</script>

<section class="section">
  <div class="container">
    <h1 class="title">{title}</h1>
    <Article article_infos={article_infos} />
  </div>
</section>

<style>
</style>
