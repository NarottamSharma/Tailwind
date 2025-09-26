<script>
  const { id = 'input', label, description, error, ...props } = $props();
  const descriptionId = description ? `${id}-description` : undefined;
  const errorId = error ? `${id}-error` : undefined;
</script>

<div class="space-y-1">
  <label class="block font-medium text-slate-900  " for={id}>{label}</label>
  <input
  class="block bg-white w-full outline outline-slate-600 rounded px-2 py-1 focus:outline-2 focus:outline-blue-400 focus:bg-blue-100 focus:text-neutral-900 placeholder-slate-700 placeholder:italic border outline-offset-4 user-invalid:outline-red-600"
    {id}
    aria-describedby={descriptionId}
    aria-invalid={!!error}
    aria-errormessage={errorId}
    {...props}
  />
  {#if description}
    <p id={descriptionId}>{description}</p>
  {/if}
  {#if error}
    <p id={errorId}>{error}</p>
  {/if}
</div>
