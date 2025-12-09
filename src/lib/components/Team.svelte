<script lang="ts">
  import Button from './ui/Button.svelte';
</script>

<section class="py-24 px-6 max-w-[1400px] mx-auto">
  <div class="max-w-2xl mb-12">
    <h2 class="text-4xl md:text-5xl font-medium tracking-tight text-gray-900 mb-8 leading-[1.1]">
      Cursor is an applied team focused on building the future of coding.
    </h2>
    <Button href="#careers" variant="primary" className="!rounded-full !px-6 !py-2 text-sm flex items-center gap-2">
      Join us
      <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14"/><path d="m12 5 7 7-7 7"/></svg>
    </Button>
  </div>

  <div class="w-full aspect-[21/9] bg-gray-200 rounded-xl overflow-hidden relative">
    <!-- Placeholder for team image -->
     <div class="absolute inset-0 flex items-center justify-center bg-gray-300 text-gray-500">
        Team Image Placeholder
     </div>
  </div>
</section>
