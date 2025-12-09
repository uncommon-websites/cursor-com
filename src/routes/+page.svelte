<script lang="ts">
  import Header from "$lib/components/Header.svelte";
  import Hero from "$lib/components/Hero.svelte";
  import FeatureSection from "$lib/components/FeatureSection.svelte";
  import Testimonials from "$lib/components/Testimonials.svelte";
  import Frontier from "$lib/components/Frontier.svelte";
  import Changelog from "$lib/components/Changelog.svelte";
  import Team from "$lib/components/Team.svelte";
  import Highlights from "$lib/components/Highlights.svelte";
  import FooterCTA from "$lib/components/FooterCTA.svelte";
  import Footer from "$lib/components/Footer.svelte";
</script>

<div class="bg-white min-h-screen font-sans selection:bg-[#FF4F00] selection:text-white">
  <Header />
  
  <main>
    <Hero />
    
    <div class="space-y-0">
      <FeatureSection 
        title="Agent turns ideas into code" 
        description="A human-AI programmer, orders of magnitude more effective than any developer alone."
        linkText="Learn about Agent"
        imagePosition="right"
      >
        <div slot="image" class="w-full h-full bg-gray-50 flex items-center justify-center relative overflow-hidden">
             <!-- Placeholder for Agent UI -->
             <div class="absolute top-4 left-4 right-4 bottom-0 bg-white shadow-lg rounded-t-lg border border-gray-200 p-4">
                <div class="flex gap-2 mb-4">
                    <div class="w-3 h-3 rounded-full bg-red-400"></div>
                    <div class="w-3 h-3 rounded-full bg-yellow-400"></div>
                    <div class="w-3 h-3 rounded-full bg-green-400"></div>
                </div>
                <div class="space-y-2">
                    <div class="h-2 bg-gray-100 rounded w-3/4"></div>
                    <div class="h-2 bg-gray-100 rounded w-1/2"></div>
                    <div class="h-2 bg-gray-100 rounded w-full"></div>
                </div>
             </div>
        </div>
      </FeatureSection>

      <FeatureSection 
        title="Magically accurate autocomplete" 
        description="Our custom Tab model predicts your next action with striking speed and precision."
        linkText="Learn about Tab"
        imagePosition="left"
      >
        <div slot="image" class="w-full h-full bg-gray-900 flex items-center justify-center relative overflow-hidden p-8 font-mono text-sm">
             <div class="text-gray-400 w-full">
                <span class="text-purple-400">def</span> <span class="text-blue-400">calculate_metrics</span>(data):<br/>
                &nbsp;&nbsp;return &#123;<br/>
                &nbsp;&nbsp;&nbsp;&nbsp;<span class="text-green-400">"accuracy"</span>: <span class="text-gray-500">calculate_accuracy(data),</span><br/>
                &nbsp;&nbsp;&nbsp;&nbsp;<span class="text-gray-600">// Ghost text showing prediction</span><br/>
                &nbsp;&nbsp;&#125;
             </div>
        </div>
      </FeatureSection>

      <FeatureSection 
        title="Everywhere software gets built" 
        description="Cursor is in GitHub reviewing your PRs, a teammate in Slack, and anywhere else you work."
        linkText="Learn about Cursor's ecosystem"
        imagePosition="right"
      >
        <div slot="image" class="w-full h-full bg-white flex items-center justify-center relative overflow-hidden border border-gray-200">
             <!-- Placeholder for Ecosystem -->
             <div class="flex items-center gap-4">
                <div class="w-16 h-16 bg-gray-100 rounded-lg flex items-center justify-center">GitHub</div>
                <div class="text-gray-300">→</div>
                <div class="w-16 h-16 bg-black text-white rounded-lg flex items-center justify-center">Cursor</div>
                <div class="text-gray-300">→</div>
                <div class="w-16 h-16 bg-purple-100 text-purple-800 rounded-lg flex items-center justify-center">Slack</div>
             </div>
        </div>
      </FeatureSection>
    </div>

    <Testimonials />
    
    <Frontier />
    
    <Changelog />
    
    <Team />
    
    <Highlights />
    
    <FooterCTA />
  </main>

  <Footer />
</div>

