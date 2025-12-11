<script lang="ts">
  import SectionWrapper from './SectionWrapper.svelte';
</script>

<SectionWrapper withBorderBottom={true} className="py-20 md:py-24">
  <div class="px-4 md:px-12 max-w-4xl mx-auto text-center">
    <h1 class="font-serif text-5xl md:text-7xl text-gray-900 mb-6 leading-tight">
      EU-compliant product <br/> passports in days
    </h1>
    <p class="text-gray-500 text-lg md:text-xl max-w-2xl mx-auto mb-10 leading-relaxed font-light">
      Transform compliance from burden to opportunity. Automated data enrichment and modular design deliver beautiful, brand-aligned digital product passports that delight customers and meet EU regulations.
    </p>
    <div class="flex flex-col sm:flex-row gap-4 justify-center items-center">
      <a href="#contact" class="inline-flex items-center px-6 py-3 bg-gray-900 text-white font-medium rounded hover:bg-gray-800 transition-colors">
        Talk to Founders <span class="ml-2">→</span>
      </a>
      <a href="https://passport.avelero.com" target="_blank" class="inline-flex items-center px-6 py-3 bg-white border border-gray-300 text-gray-900 font-medium rounded hover:bg-gray-50 transition-colors">
        View Live Demo
      </a>
    </div>
  </div>

  <div class="mt-16 md:mt-20 px-4 md:px-12">
    <div class="relative w-full aspect-[16/9] md:aspect-[21/9] rounded-lg overflow-hidden bg-gray-200">
      <!-- Placeholder for image -->
      <img 
        src="/generated/image-fashion-designer-working-at-a-clean-mode-1765494452185-0.webp" 
        alt="Sustainable fashion design workspace" 
        class="w-full h-full object-cover"
      />
    </div>
  </div>
</SectionWrapper>
