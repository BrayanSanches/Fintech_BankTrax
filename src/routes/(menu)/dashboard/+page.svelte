<script>
    import * as Icon from 'svelte-google-materialdesign-icons';
    import Chart from '../../../lib/components/chart.svelte'
 
</script>

<div class="flex bg-gray-100 min-h-screen">
    <aside class="hidden sm:flex sm:flex-col">
      <a href="/dashboard" class="inline-flex items-center justify-center h-20 w-20 bg-green-600 hover:bg-green-500 focus:bg-green-500">
        <div class="flex justify-center text-gray-100"> <Icon.Insights size="50" class="mt-1"  /></div>
      </a>
      <div class="flex-grow flex flex-col justify-between text-gray-500 bg-gray-800">
        <nav class="flex flex-col mx-4 my-6 space-y-4">
          <a href="/dashboard" class="inline-flex items-center justify-center py-3 hover:text-gray-400 hover:bg-gray-700 focus:text-gray-400 focus:bg-gray-700 rounded-lg">
            <span class="sr-only">Folders</span>
            <svg aria-hidden="true" fill="none" viewBox="0 0 24 24" stroke="currentColor" class="h-6 w-6">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 7v10a2 2 0 002 2h14a2 2 0 002-2V9a2 2 0 00-2-2h-6l-2-2H5a2 2 0 00-2 2z" />
            </svg>
          </a>
          <a href="/dashboard" class="inline-flex items-center justify-center py-3 text-green-600 bg-white rounded-lg">
            <span class="sr-only">Dashboard</span>
            <svg aria-hidden="true" fill="none" viewBox="0 0 24 24" stroke="currentColor" class="h-6 w-6">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 19v-6a2 2 0 00-2-2H5a2 2 0 00-2 2v6a2 2 0 002 2h2a2 2 0 002-2zm0 0V9a2 2 0 012-2h2a2 2 0 012 2v10m-6 0a2 2 0 002 2h2a2 2 0 002-2m0 0V5a2 2 0 012-2h2a2 2 0 012 2v14a2 2 0 01-2 2h-2a2 2 0 01-2-2z" />
            </svg>
          </a>
          <a href="/dashboard" class="inline-flex items-center justify-center py-3 hover:text-gray-400 hover:bg-gray-700 focus:text-gray-400 focus:bg-gray-700 rounded-lg">
            <span class="sr-only">Mensajes</span>
            <svg aria-hidden="true" fill="none" viewBox="0 0 24 24" stroke="currentColor" class="h-6 w-6">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" />
            </svg>
          </a>
          <a href="/dashboard" class="inline-flex items-center justify-center py-3 hover:text-gray-400 hover:bg-gray-700 focus:text-gray-400 focus:bg-gray-700 rounded-lg">
            <span class="sr-only">Documentos</span>
            <svg aria-hidden="true" fill="none" viewBox="0 0 24 24" stroke="currentColor" class="h-6 w-6">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M7 21h10a2 2 0 002-2V9.414a1 1 0 00-.293-.707l-5.414-5.414A1 1 0 0012.586 3H7a2 2 0 00-2 2v14a2 2 0 002 2z" />
            </svg>
          </a>
        </nav>
        
        <div class="inline-flex items-center justify-center h-20 w-20 border-t border-gray-700">
          
          <button class="p-3 hover:text-gray-400 hover:bg-gray-700 focus:text-gray-400 focus:bg-gray-700 rounded-lg">
            <span class="sr-only">Ajustes</span>
            <svg aria-hidden="true" fill="none" viewBox="0 0 24 24" stroke="currentColor" class="h-6 w-6">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M10.325 4.317c.426-1.756 2.924-1.756 3.35 0a1.724 1.724 0 002.573 1.066c1.543-.94 3.31.826 2.37 2.37a1.724 1.724 0 001.065 2.572c1.756.426 1.756 2.924 0 3.35a1.724 1.724 0 00-1.066 2.573c.94 1.543-.826 3.31-2.37 2.37a1.724 1.724 0 00-2.572 1.065c-.426 1.756-2.924 1.756-3.35 0a1.724 1.724 0 00-2.573-1.066c-1.543.94-3.31-.826-2.37-2.37a1.724 1.724 0 00-1.065-2.572c-1.756-.426-1.756-2.924 0-3.35a1.724 1.724 0 001.066-2.573c-.94-1.543.826-3.31 2.37-2.37.996.608 2.296.07 2.572-1.065z" />
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 12a3 3 0 11-6 0 3 3 0 016 0z" />
            </svg>
          </button>
        </div>
      </div>
    </aside>
    <div class="flex-grow text-gray-800">

      <main class="p-6 sm:py-3 sm:px-6 space-y-6">
        <div class="flex flex-col space-y-6 md:space-y-0 md:flex-row justify-between">
          <div class="mr-6">
            <h1 class="text-4xl font-semibold mb-2">Dashboard Ingenius</h1>
            <h2 class="text-gray-600 ml-0.5">Tu plataforma financiera de confianza</h2>
          </div>
          <div class="flex flex-wrap items-start justify-end -mb-3">

            <button class="inline-flex px-5 py-3 text-white bg-green-600 hover:bg-green-700 focus:bg-green-700 rounded-md ml-6 mb-3">
              <svg aria-hidden="true" fill="none" viewBox="0 0 24 24" stroke="currentColor" class="flex-shrink-0 h-6 w-6 text-white -ml-1 mr-2">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 6v6m0 0v6m0-6h6m-6 0H6" />
              </svg>
              Crear nuevo dashboard
            </button>
          </div>
        </div>
        <section class="grid md:grid-cols-2 xl:grid-cols-4 gap-6">
          <div class="flex items-center p-8 bg-white shadow rounded-lg">
            <div class="inline-flex flex-shrink-0 items-center justify-center h-16 w-16 text-yellow-600 bg-yellow-100 rounded-full mr-6">
                <span><Icon.Warning /></span>
            </div>
            <div>
              <span class="block text-2xl font-bold">S/.200</span>
              <span class="block text-gray-500">Proximo a vencer</span>
            </div>
          </div>
          <div class="flex items-center p-8 bg-white shadow rounded-lg">
            <div class="inline-flex flex-shrink-0 items-center justify-center h-16 w-16 text-green-600 bg-green-100 rounded-full mr-6">
              <svg aria-hidden="true" fill="none" viewBox="0 0 24 24" stroke="currentColor" class="h-6 w-6">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 7h8m0 0v8m0-8l-8 8-4-4-6 6" />
              </svg>
            </div>
            <div>
              <span class="block text-2xl font-bold">S/.10000</span>
              <span class="block text-gray-500">Cash</span>
            </div>
          </div>
          <div class="flex items-center p-8 bg-white shadow rounded-lg">
            <div class="inline-flex flex-shrink-0 items-center justify-center h-16 w-16 text-red-600 bg-red-100 rounded-full mr-6">
              <svg aria-hidden="true" fill="none" viewBox="0 0 24 24" stroke="currentColor" class="h-6 w-6">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 17h8m0 0V9m0 8l-8-8-4 4-6-6" />
              </svg>
            </div>
            <div>
              <span class="inline-block text-2xl font-bold">S/.500</span>
             
              <span class="block text-gray-500">Deudas pasadas</span>
            </div>
          </div>

        </section>
        <section class="grid md:grid-cols-2 xl:grid-cols-4 xl:grid-rows-3 xl:grid-flow-col gap-6">
          <div class="flex flex-col md:col-span-2 md:row-span-2 bg-white shadow rounded-lg">
            <Chart/>
          </div>
          <div class="flex items-center p-8 bg-white shadow rounded-lg">
            <div class="inline-flex flex-shrink-0 items-center justify-center h-16 w-16 text-yellow-600 bg-yellow-100 rounded-full mr-6">
              <span><Icon.Warning /></span>
            </div>
            <div>
              <span class="block text-2xl font-bold">Texto</span>
              <span class="block text-gray-500">Texto</span>
            </div>
          </div>
          <div class="flex items-center p-8 bg-white shadow rounded-lg">
            <div class="inline-flex flex-shrink-0 items-center justify-center h-16 w-16 text-teal-600 bg-teal-100 rounded-full mr-6">
              <svg aria-hidden="true" fill="none" viewBox="0 0 24 24" stroke="currentColor" class="h-6 w-6">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z" />
              </svg>
            </div>
            <div>
              <span class="block text-2xl font-bold">Texto</span>
              <span class="block text-gray-500">Texto</span>
            </div>
          </div>
          <div class="row-span-3 bg-white shadow rounded-lg">
            <div class="flex items-center justify-between px-6 py-5 font-semibold border-b border-gray-100">
              <span>Historial de pagos</span>
              <button type="button" class="inline-flex justify-center rounded-md px-1 -mr-1 bg-white text-sm leading-5 font-medium text-gray-500 hover:text-gray-600" id="options-menu" aria-haspopup="true" aria-expanded="true">
                Descendiente
                <svg class="-mr-1 ml-1 h-5 w-5" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor">
                  <path fill-rule="evenodd" d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z" clip-rule="evenodd" />
                </svg>
              </button>
              <!-- Refer here for full dropdown menu code: https://tailwindui.com/components/application-ui/elements/dropdowns -->
            </div>
            <div class="overflow-y-auto" style="max-height: 20rem;">
              <ul class="p-6 space-y-6">
                <li class="flex items-center">
                  <div class="h-10 w-10 mr-3 bg-green-100 text-green-600 rounded-full overflow-hidden flex items-center">
                    <span><Icon.Check class="ml-2"/></span>
                  </div>
                  <span class="text-gray-600">Pagada</span>
                  
                  <span class="ml-auto font-semibold">S/.300</span>
                </li>
                <li class="flex items-center">
                  <div class="h-10 w-10 mr-3 bg-green-100 text-green-600 rounded-full overflow-hidden flex items-center">
                    <span><Icon.Check class="ml-2"/></span>
                  </div>
                  <span class="text-gray-600">Pagada</span>
                  <span class="ml-auto font-semibold">S/.300</span>
                </li>
                <li class="flex items-center">
                  <div class="h-10 w-10 mr-3 bg-green-100 text-green-600 rounded-full overflow-hidden flex items-center">
                    <span><Icon.Check class="ml-2"/></span>
                  </div>
                  <span class="text-gray-600">Pagada</span>
                  <span class="ml-auto font-semibold">S/.300</span>
                </li>
                <li class="flex items-center">
                  <div class="h-10 w-10 mr-3 bg-green-100 text-green-600 rounded-full overflow-hidden flex items-center">
                    <span><Icon.Check class="ml-2"/></span>
                  </div>
                  <span class="text-gray-600">Pagada</span>
                  <span class="ml-auto font-semibold">S/.300</span>
                </li>
                <li class="flex items-center">
                  <div class="h-10 w-10 mr-3 bg-green-100 text-green-600 rounded-full overflow-hidden flex items-center">
                    <span><Icon.Check class="ml-2"/></span>
                  </div>
                  <span class="text-gray-600">Pagada</span>
                  <span class="ml-auto font-semibold">S/.300</span>
                </li>
                <li class="flex items-center">
                  <div class="h-10 w-10 mr-3 bg-green-100 text-green-600 rounded-full overflow-hidden flex items-center">
                    <span><Icon.Check class="ml-2"/></span>
                  </div>
                  <span class="text-gray-600">Pagada</span>
                  <span class="ml-auto font-semibold">S/.300</span>
                </li>
                <li class="flex items-center">
                  <div class="h-10 w-10 mr-3 bg-green-100 text-green-600 rounded-full overflow-hidden flex items-center">
                    <span><Icon.Check class="ml-2"/></span>
                  </div>
                  <span class="text-gray-600">Pagada</span>
                  <span class="ml-auto font-semibold">S/.300</span>
                </li>
                <li class="flex items-center">
                  <div class="h-10 w-10 mr-3 bg-green-100 text-green-600 rounded-full overflow-hidden flex items-center">
                    <span><Icon.Check class="ml-2"/></span>
                  </div>
                  <span class="text-gray-600">Pagada</span>
                  <span class="ml-auto font-semibold">S/.300</span>
                </li>
              </ul>
            </div>
          </div>
          <div class="flex flex-col row-span-3 bg-white shadow rounded-lg">
            <div class="px-6 py-5 font-semibold border-b border-gray-100">Submenu</div>
            <div class="p-4 flex-grow">
              <div class="flex items-center justify-center h-full px-4 py-24 text-gray-400 text-3xl font-semibold bg-gray-100 border-2 border-gray-200 border-dashed rounded-md">Chart</div>
            </div>
          </div>
        </section>

      </main>
    </div>
</div>