<script lang="ts">
  export let article_infos: Array<{title: string, image:string, alt: string, keep_list, problem_list, try_list: Array<string>}>;
</script>

<article>
  {#each article_infos as a}
  <h2>{a.title}</h2>
  <img src={a.image} alt={a.alt} width=500>
  <div>{a.description}</div>
  <h3>Keep</h3>
    <ul>
    {#each a.keep_list as ak}
      <li>{ak}</li>
    {/each}
    </ul>
  <h3>Problem</h3>
    <ul>
    {#each a.problem_list as ap}
      <li>{ap}</li>
    {/each}
    </ul>
  <h3>Try</h3>
    <ul>
    {#each a.try_list as at}
      <li>{at}</li>
    {/each}
    </ul>
  {/each}
</article>
