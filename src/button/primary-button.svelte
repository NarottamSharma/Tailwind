<script>
  const { label = 'Button', ...props } = $props();
</script>

<button class="rounded-md bg-blue-600 px-3 py-1.5 text-white shadow-sm hover:bg-blue-500" {...props}>
  {label}
</button>
