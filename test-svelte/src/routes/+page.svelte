<script>
  export let data;

  let { blog_post } = data

</script>

{#each blog_post as blog_post}
  <h1>{blog_post.title}</h1>
  <h2>By:{blog_post.author}</h2>
  <h2>Posted:{blog_post.date_created}</h2>
  <h3>Tags:{blog_post.tags}</h3>
  <p>{blog_post.text_box}</p>
  <h3>Summary</h3>
  <p>{blog_post.summary}</p>
{/each}