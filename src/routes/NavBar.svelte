<script lang="ts">

import Menu from './Menu.svelte';


const items = [ 
     'Item 1',
     'Item 2',
     'Item 3' 
  ];

  let activeItem = 'Item 1' ;

  // Any script for the NavBar goes here
</script>

<style>
  .nav-bar {
    margin: 0 auto;
    height: 10vh;
    width: 80vw;
    background-color: #333;
    color: #fff;
    display: flex;
    justify-content: center;
    align-items: center;
    position: sticky;
    top: 0;
    z-index: 100;

    border-color: rgba(255, 94, 0, 0.412);
    border-style: dotted;
  }
</style>

<div class="nav-bar">
  <Menu {items} {activeItem}/>
</div>
