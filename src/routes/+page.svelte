<script lang="ts">
  import { onMount } from 'svelte';
  import NavBar from './NavBar.svelte';
  

  let scrollY = 0;
  let navBarVisible = true;

  onMount(() => {
    window.addEventListener('scroll', () => {
      navBarVisible = window.scrollY < scrollY;
      scrollY = window.scrollY;
    });
  });

    let text = "";

    onMount(async () => {
        const res = await fetch('../test.txt');
        const data = await res.text();
        text = data.split('*').map(paragraph => paragraph.trim());
    });

</script>

<style>
  .container {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 100vh;
    width: 80vw;
    margin: 0 auto;
    border: 1px solid #ff0000;
    padding: 10px;
    box-sizing: border-box;
    font-family: Arial, sans-serif;
    font-size: 18px;
    text-align: center;
    margin-top: 5vh;
  }
  p {
    margin-bottom: 20px;
  }
</style>

{#if navBarVisible}
  <NavBar />
{/if}

<div class="container">
    {#each text as paragraph (paragraph)}
        <p>{paragraph}</p>
    {/each}
</div>
