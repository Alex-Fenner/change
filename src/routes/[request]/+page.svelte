<script>
	/** @type {import('./$types').PageData} */
	export let data;
	import ActivityFeed from '../../lib/activityFeed.svelte';
	import ChangeDetails from '../../lib/changeDetails.svelte';
   import Navbar from '../../lib/navbar.svelte';
   console.log(data.title)


</script>

<Navbar/>




  
  <main>
    <header class="relative isolate pt-1">
      <div class="absolute inset-0 -z-10 overflow-hidden" aria-hidden="true">
        
        <div class="absolute inset-x-0 bottom-0 h-px bg-gray-900/5"></div>
      </div>
  
      <div class="mx-auto max-w-7xl px-4 py-2 sm:px-6 lg:px-8">
        <div class="mx-auto flex max-w-2xl items-center justify-between gap-x-8 lg:mx-0 lg:max-w-none">
          <div class="flex items-center gap-x-6">
            <a href="/">
           <button class="btn btn-outline btn-sm">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                <path stroke-linecap="round" stroke-linejoin="round" d="M9 15 3 9m0 0 6-6M3 9h12a6 6 0 0 1 0 12h-3" />
              </svg>
              Back</button></a>
          </div>
          <div class="flex items-center gap-2">
            <button class="btn btn-outline btn-sm">Edit</button>
            <button class="btn btn-success btn-sm">Approve</button>
            <button class="btn btn-error btn-sm">Reject</button>
            <div class="relative sm:hidden">
              <button type="button" class="-m-3 block p-3" id="more-menu-button" aria-expanded="false" aria-haspopup="true">
                <span class="sr-only">More</span>
                <svg class="h-5 w-5 text-gray-500" viewBox="0 0 20 20" fill="currentColor" aria-hidden="true">
                  <path d="M10 3a1.5 1.5 0 110 3 1.5 1.5 0 010-3zM10 8.5a1.5 1.5 0 110 3 1.5 1.5 0 010-3zM11.5 15.5a1.5 1.5 0 10-3 0 1.5 1.5 0 003 0z" />
                </svg>
              </button>
  
             
              <div class="absolute right-0 z-10 mt-0.5 w-32 origin-top-right rounded-md bg-white py-2 shadow-lg ring-1 ring-gray-900/5 focus:outline-none" role="menu" aria-orientation="vertical" aria-labelledby="more-menu-button" tabindex="-1">
                <!-- Active: "bg-gray-50", Not Active: "" -->
                <button type="button" class="block w-full px-3 py-1 text-left text-sm leading-6 text-gray-900" role="menuitem" tabindex="-1" id="more-menu-item-0">Copy URL</button>
                <a href="#" class="block px-3 py-1 text-sm leading-6 text-gray-900" role="menuitem" tabindex="-1" id="more-menu-item-1">Edit</a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </header>
  
    <div class="mx-auto max-w-7xl px-4 py-8 sm:px-6 lg:px-8">
      <div class="mx-auto grid max-w-2xl grid-cols-1 grid-rows-1 items-start gap-x-8 lg:mx-0 lg:max-w-none lg:grid-cols-3">

        <ChangeDetails/>
        <ActivityFeed/>
        
      </div>
    </div>
  </main>
  
  


