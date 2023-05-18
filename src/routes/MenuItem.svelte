<script lang="ts">
    export let label;
    export let isActive;
  </script>
  
  <style>
    .menu-item {
        box-shadow: 0.1cm;
        border-color: black;
        border-style: dotted;
      /* Estilos para o item do menu */
    }
  
    .active {
        background-color: rgb(205, 170, 229);
        text-decoration: solid;

        border-color: rgba(78, 34, 149, 0.412);
        border-style: dotted;
      /* Estilos para o item ativo do menu */
    }

  </style>
  
  <div class="menu-item {isActive ? 'active' : ''}">
    <span>{label}</span>
  </div>
  