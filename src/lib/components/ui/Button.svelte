<script lang="ts">
  export let variant: 'primary' | 'secondary' | 'ghost' = 'primary';
  export let href: string = '';
  export let className: string = '';
</script>

{#if href}
  <a
    {href}
    class="inline-flex items-center justify-center px-4 py-2 rounded-lg font-medium transition-colors duration-200 {className}
    {variant === 'primary' ? 'bg-black text-white hover:bg-gray-800' : ''}
    {variant === 'secondary' ? 'bg-gray-100 text-gray-900 hover:bg-gray-200' : ''}
    {variant === 'ghost' ? 'text-gray-600 hover:text-gray-900' : ''}"
  >
    <slot />
  </a>
{:else}
  <button
    class="inline-flex items-center justify-center px-4 py-2 rounded-lg font-medium transition-colors duration-200 {className}
    {variant === 'primary' ? 'bg-black text-white hover:bg-gray-800' : ''}
    {variant === 'secondary' ? 'bg-gray-100 text-gray-900 hover:bg-gray-200' : ''}
    {variant === 'ghost' ? 'text-gray-600 hover:text-gray-900' : ''}"
  >
    <slot />
  </button>
{/if}
