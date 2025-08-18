<script>
  const { label = 'Button', ...props } = $props();
</script>

<button class="bg-blue-500" {...props}>{label}</button>
