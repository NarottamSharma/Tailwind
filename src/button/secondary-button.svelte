<script>
  const { label = 'Button', ...props } = $props();
</script>

<button
  class="-inset offset -8 rounded-md bg-white px-3 py-1.5 shadow-sm ring-2 outline-4 outline-slate-600 ring-inset hover:bg-slate-100 hover:outline-3"
  {...props}>{label}</button>
