<script lang="ts">
  import Button from './ui/Button.svelte';
</script>

<header class="fixed top-0 left-0 right-0 z-50 bg-white/80 backdrop-blur-md border-b border-gray-100">
  <div class="max-w-[1400px] mx-auto px-6 h-16 flex items-center justify-between">
    <div class="flex items-center gap-8">
      <a href="/" class="text-xl font-bold tracking-tight">Cursor</a>
      <nav class="hidden md:flex items-center gap-6 text-sm text-gray-500 font-medium">
        <a href="#features" class="hover:text-black transition-colors">Features</a>
        <a href="#enterprise" class="hover:text-black transition-colors">Enterprise</a>
        <a href="#pricing" class="hover:text-black transition-colors">Pricing</a>
        <a href="#resources" class="hover:text-black transition-colors">Resources</a>
      </nav>
    </div>
    <div class="flex items-center gap-4">
      <a href="#signin" class="text-sm font-medium text-gray-500 hover:text-black transition-colors">Sign In</a>
      <Button href="#download" variant="primary" className="!py-1.5 !px-3 text-sm !rounded-md bg-black text-white">Download</Button>
    </div>
  </div>
</header>
