<script lang="ts">
  import SectionWrapper from './SectionWrapper.svelte';
</script>

<SectionWrapper withBorderBottom={true} className="py-12">
  <div class="px-4 md:px-12 flex flex-col md:flex-row items-center justify-between gap-8">
    <!-- Logos -->
    <div class="flex flex-wrap items-center gap-8 md:gap-12 grayscale opacity-70">
        <!-- Fashion Brand 1 -->
        <div class="h-6 font-bold text-lg tracking-wider uppercase">MAISON VERT</div>
        <!-- Fashion Brand 2 -->
        <div class="h-8 flex flex-col leading-none text-xs font-serif uppercase tracking-widest">
            <span>Atelier</span>
            <span>Durable</span>
        </div>
        <!-- Fashion Brand 3 -->
        <div class="h-6 font-bold text-lg lowercase italic font-serif">éthique</div>
        <!-- Fashion Brand 4 -->
        <div class="h-6 font-medium text-lg flex items-center gap-1">
            <span class="font-bold">◆</span>NORDIC THREADS
        </div>
    </div>

    <!-- Trust Text -->
    <div class="text-gray-400 text-sm font-light text-right md:text-left">
      Trusted by leading EU fashion brands
    </div>
  </div>
</SectionWrapper>
