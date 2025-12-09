<script lang="ts">
  import Button from './ui/Button.svelte';
</script>

<section class="pt-32 pb-16 px-6 max-w-[1400px] mx-auto">
  <div class="max-w-4xl mb-12">
    <h1 class="text-6xl md:text-7xl font-medium tracking-tight text-gray-900 mb-8 leading-[1.1]">
      Built to make you extraordinarily productive, Cursor is the best way to code with AI.
    </h1>
    <div class="flex items-center gap-4">
      <Button href="#download" variant="primary" className="!rounded-full !px-6 !py-3 text-base flex items-center gap-2">
        Download for Linux
        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-download"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/><polyline points="7 10 12 15 17 10"/><line x1="12" x2="12" y1="15" y2="3"/></svg>
      </Button>
    </div>
  </div>

  <div class="relative w-full aspect-[16/10] bg-gray-100 rounded-lg overflow-hidden shadow-2xl border border-gray-200">
    <!-- Placeholder for the IDE screenshot -->
    <div class="absolute inset-0 bg-gray-50 flex items-center justify-center text-gray-400">
        <img src="https://www.cursor.com/_next/image?url=%2F_next%2Fstatic%2Fmedia%2Fhero-screenshot.6d7c80a2.png&w=3840&q=75" alt="Cursor IDE" class="w-full h-full object-cover" />
    </div>
  </div>
  
  <div class="mt-16 text-center">
    <p class="text-sm text-gray-500 font-medium mb-8">Trusted every day by millions of professional developers.</p>
    <div class="flex flex-wrap justify-center items-center gap-x-12 gap-y-8 opacity-60 grayscale text-gray-900">
       <!-- Stylized text approximations of logos -->
       <span class="font-bold text-2xl tracking-tighter">stripe</span>
       <span class="font-medium text-xl tracking-wide">OpenAI</span>
       <div class="flex items-center gap-1">
         <div class="w-4 h-4 rounded-full border-2 border-current"></div>
         <span class="font-medium text-xl tracking-tight">Linear</span>
       </div>
       <div class="flex items-center gap-1">
          <span class="font-bold text-xl uppercase tracking-wider">DATADOG</span>
       </div>
       <div class="flex items-center gap-1">
          <span class="font-bold text-xl uppercase">NVIDIA</span>
       </div>
       <span class="font-bold text-xl tracking-tight">Figma</span>
       <span class="font-semibold text-xl lowercase">ramp</span>
       <div class="flex items-center gap-1">
          <span class="font-bold text-xl tracking-tight">Adobe</span>
       </div>
    </div>
  </div>
</section>
