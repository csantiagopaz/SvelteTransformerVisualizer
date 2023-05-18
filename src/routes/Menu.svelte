<script lang="ts">
  import MenuItem from './MenuItem.svelte';

  export let items = [];   
  export let activeItem;
  </script>
  
  <style>
.menu {
  border-color: rgba(3, 45, 255, 0.412);
  border-style: dotted;
  width: 80vw;
  display: flex;
  justify-content: space-between;
}
  </style>
  
  <div class="menu">
    {#each items as item (item)}     
     <MenuItem
        label={item}
        isActive={item === activeItem}
      />
    {/each}
  </div>
  