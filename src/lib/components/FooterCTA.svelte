<script lang="ts">
  import Button from './ui/Button.svelte';
</script>

<section class="py-32 px-6 max-w-[1400px] mx-auto text-center">
  <h2 class="text-5xl md:text-6xl font-medium tracking-tight text-gray-900 mb-12">
    Try Cursor now.
  </h2>
  <Button href="#download" variant="primary" className="!rounded-full !px-6 !py-3 text-base flex items-center gap-2 mx-auto">
    Download for Linux
    <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-download"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/><polyline points="7 10 12 15 17 10"/><line x1="12" x2="12" y1="15" y2="3"/></svg>
  </Button>
</section>
