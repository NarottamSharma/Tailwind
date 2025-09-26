<script>
  const { title = 'Card Title', description = '' } = $props();
  
</script>

<div class="border-2 p-4 rounded-md bg-slate-50 border-slate-500" >
  <h2 class="font-semibold text-lg   " >{title}</h2>
  <p class="mt-1   "  >{description}</p>
</div>
