<script lang="ts">
  import SectionWrapper from './SectionWrapper.svelte';
  import SolutionBlock from './SolutionBlock.svelte';
</script>

<SectionWrapper withBorderBottom={true} className="">
  <div class="px-4 md:px-12">
    <div class="py-16 text-center" id="solutions">
      <h2 class="font-serif text-4xl text-gray-900">How Avelero works</h2>
    </div>

    <!-- Block 1 -->
    <SolutionBlock
      label="Automated Data Transformation"
      title="From spreadsheets to passports in minutes"
      description="Upload Excel files, PDFs, or connect your PLM system. Our AI-powered engine detects missing information, enriches your data with validated sources, and calculates carbon and water impact using cradle-to-gate LCA methodology."
    >
      <!-- Visual for Block 1: Files -->
      <div class="relative w-full h-full flex items-center justify-center">
        <!-- Central Hub -->
        <div class="w-16 h-16 bg-white shadow-lg rounded-lg flex items-center justify-center z-10 border border-gray-100">
           <div class="w-8 h-8 bg-gray-900 rounded-sm"></div>
        </div>
        
        <!-- Connected Files -->
        <div class="absolute top-1/4 left-1/4 bg-white p-3 shadow rounded border border-gray-100 animate-pulse">
            <div class="w-8 h-10 bg-primary-100 rounded flex items-center justify-center text-[10px] font-bold text-primary-700">.XLSX</div>
            <div class="mt-1 text-[10px] text-center">Materials</div>
        </div>
        <div class="absolute top-1/4 right-1/4 bg-white p-3 shadow rounded border border-gray-100">
            <div class="w-8 h-10 bg-primary-600 rounded flex items-center justify-center text-[10px] font-bold text-white">.CSV</div>
            <div class="mt-1 text-[10px] text-center">Production</div>
        </div>
        <div class="absolute bottom-1/4 left-1/3 bg-white p-3 shadow rounded border border-gray-100">
            <div class="w-8 h-10 bg-primary-400 rounded flex items-center justify-center text-[10px] font-bold text-white">.PDF</div>
            <div class="mt-1 text-[10px] text-center">Suppliers</div>
        </div>
         <div class="absolute bottom-1/4 right-1/3 bg-white p-3 shadow rounded border border-gray-100">
            <div class="w-8 h-10 bg-gray-200 rounded flex items-center justify-center text-[10px] font-bold text-gray-600">API</div>
            <div class="mt-1 text-[10px] text-center">PLM</div>
        </div>
        
        <!-- Connecting Lines (Simplified) -->
        <svg class="absolute inset-0 w-full h-full pointer-events-none opacity-20" viewBox="0 0 400 300">
            <path d="M100 100 L200 150 M300 100 L200 150 M150 220 L200 150 M250 220 L200 150" stroke="currentColor" stroke-width="1" stroke-dasharray="4 4" />
        </svg>
      </div>
    </SolutionBlock>

    <!-- Block 2 -->
    <SolutionBlock
      label="Modular Passport Design"
      title="Your brand, your way"
      description="Drag-and-drop interface lets you arrange sections, customize typography and colors, and maintain brand consistency across your entire catalog. Every passport reflects your identity with embedded care guides, repair services, and resale options."
      reversed={true}
    >
      <!-- Visual for Block 2: Passport Preview -->
      <div class="bg-white rounded-lg shadow-xl p-6 w-3/4 max-w-sm border border-gray-100">
        <div class="flex items-center justify-between mb-4">
            <div class="text-xs font-bold text-gray-900">PRODUCT PASSPORT</div>
            <div class="text-xs text-gray-400">QR #A4821</div>
        </div>
        <div class="aspect-square bg-gray-100 rounded mb-4 flex items-center justify-center text-xs text-gray-400">
            Product Image
        </div>
        <h4 class="font-serif text-lg mb-2">Organic Cotton Tee</h4>
        <div class="space-y-2 mb-4">
            <div class="flex items-center gap-2 text-xs">
                <div class="w-3 h-3 bg-primary-500 rounded-full"></div>
                <span class="text-gray-600">Carbon: 2.4kg CO₂e</span>
            </div>
            <div class="flex items-center gap-2 text-xs">
                <div class="w-3 h-3 bg-primary-400 rounded-full"></div>
                <span class="text-gray-600">Water: 180L</span>
            </div>
        </div>
        <button class="w-full bg-gray-900 text-white py-2 rounded text-sm font-medium flex items-center justify-center space-x-2">
            <span>View Full Passport</span>
            <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M14 5l7 7m0 0l-7 7m7-7H3"></path></svg>
        </button>
      </div>
    </SolutionBlock>

    <!-- Block 3 -->
    <SolutionBlock
      label="EU Compliance Built-In"
      title="Stay ahead of regulations"
      description="Built to meet French Anti-Waste Law and EU ESPR requirements. We actively track regulatory developments so you don't have to. Deploy with confidence knowing your passports enable access to European markets."
    >
       <!-- Visual for Block 3: Compliance Badge -->
       <div class="bg-white rounded shadow-lg p-8 w-2/3 max-w-xs border border-gray-100 relative" id="compliance">
          <div class="flex justify-between items-center mb-6 border-b pb-2">
              <div class="font-bold text-xs">COMPLIANCE STATUS</div>
              <div class="w-4 h-4 bg-green-500 rounded-full"></div>
          </div>
          <div class="mb-6">
              <h5 class="font-bold text-sm mb-2">EU Regulations</h5>
              <div class="space-y-2">
                  <div class="flex items-center gap-2 text-[10px]">
                      <svg class="w-3 h-3 text-green-600" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
                      <span class="text-gray-700">French Anti-Waste Law (AWL)</span>
                  </div>
                  <div class="flex items-center gap-2 text-[10px]">
                      <svg class="w-3 h-3 text-green-600" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
                      <span class="text-gray-700">EU ESPR Aligned</span>
                  </div>
                  <div class="flex items-center gap-2 text-[10px]">
                      <svg class="w-3 h-3 text-green-600" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path></svg>
                      <span class="text-gray-700">Market Access Ready</span>
                  </div>
              </div>
          </div>
          <div class="text-[8px] text-gray-400 leading-relaxed">
              Last updated: Tracking active regulatory developments
          </div>
       </div>
    </SolutionBlock>
  </div>
</SectionWrapper>
