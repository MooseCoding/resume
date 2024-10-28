<script>
  export let title = "";
  export let description = "";
  export let image = "";
  export let url = "";
  export let cardClass = ""; 
</script>

{#if url}
<div class="card {cardClass}">
  <a href={url} target="_blank" rel="noopener noreferrer" class="block rounded-lg shadow-lg overflow-hidden transform transition-transform hover:scale-105">
      {#if image}
          <img src={image} alt={title} class="w-full h-48 object-cover" />
      {/if}
      <div class="p-4">
          <h2 class="text-xl font-bold mb-2">{title}</h2>
          <p>{description}</p>
      </div>
  </a>
</div>
{:else}
<div class="card rounded-lg shadow-lg overflow-hidden transform transition-transform hover:scale-105 {cardClass}">
  {#if image}
      <img src={image} alt={title} class="w-full h-48 object-cover" />
  {/if}
  <div class="p-4">
      <h2 class="text-xl font-bold mb-2">{title}</h2>
      <p>{description}</p>
  </div>
</div>
{/if}

<style>
  .card {
      max-width: 300px;
      margin: auto;
      transition: transform 0.2s ease-in-out;
  }
  .card img {
      border-top-left-radius: 0.5rem; 
      border-top-right-radius: 0.5rem; 
  }
  .card-content {
      padding: 16px;
  }
</style>