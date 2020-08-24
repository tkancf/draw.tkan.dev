<script lang="ts">
  import Article from './Article.svelte';
  let title: string = "draw.tkan.dev";
  let articles = [
    {
      title: "2020/08/14",
      description: "お絵描きはじめました。にじさんじの愛園愛美さん",
      image: "images/20200814_aizono.jpg",
      alt: "愛園愛美",
      keep_list: ["moge"],
      problem_list: ["hoge"],
      try_list: ["hoge"]
    },
  ]
</script>

<main>
  <h1>{title}</h1>
  <Article article_infos={articles} />
</main>

<style>
</style>
