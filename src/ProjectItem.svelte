<script>
  export let items = [];
  export let activeTabValue = 1;

  const handleClick = (tabValue) => () => (activeTabValue = tabValue);
</script>

<main>
  <!-- <h1> Recent Projects :::</h1> -->
  <div class="modal">
    <ul>
      {#each items as item}
        <li class={activeTabValue === item.value ? "active" : ""}>
          <span on:click={handleClick(item.value)}></span>
        </li>
      {/each}
    </ul>
    {#each items as item}
      {#if activeTabValue == item.value}
        <div class="box">
          <svelte:component this={item.component} />
        </div>
      {/if}
    {/each}
  </div>
</main>

<style>
  .modal {
    border-radius: 10px;
    max-width: 85%;
    margin-top: 5rem;
    text-align: center;
  }
  .box {
    margin-bottom: 10px;
    padding: 40px;
    border-radius: 0 0 0.5rem 0.5rem;
    border-top: 0;
  }
  ul {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    margin-left: 10rem;
    padding-left: 0;
    margin-bottom: 0;
    list-style: none;
  }
  li {
    margin-bottom: -1px;
  }

  span {
    border: 1px solid transparent;
    border-radius: 50%;
    display: block;
    margin-left: 2rem;
    padding: 0.75rem 0.75rem;
    cursor: pointer;
    background-color: #000000;
  }

  span:hover {
    border-color: #e9ecef #e9ecef #dee2e6;
  }

  li.active > span {
    color: #495057;
    background-color: rgb(229, 224, 224);
    border-color: #dee2e6 #dee2e6 #fff;
  }
</style>
