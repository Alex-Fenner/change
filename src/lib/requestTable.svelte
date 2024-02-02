<script>
	import Pagination from "./pagination.svelte";

</script>
<div class="flex items-center justify-center my-5">
    <div class="flex-auto">
      <h1 class="text-base font-semibold leading-6 text-xl ">Change Requests</h1>
       </div>
    <div class="mt-4 ml-16 mt-0 flex-none">
        <button class="btn btn-primary btn-sm" onclick="my_modal_3.showModal()">New Request</button>  
    </div>
  </div>






  <ul role="list" class="divide-y divide-base-300">
    <li class="relative flex justify-between gap-x-6 py-5 hover:bg-base-200 rounded-md">
      <div class="flex min-w-0 gap-x-4 pl-2">
        <div class="min-w-0 flex-auto">
          <p class="text-sm font-semibold leading-6 pl-1 ">
            <a href="/hello-world">
              <span class="absolute inset-x-0 -top-px  bottom-0"></span>
              SQL Downtime 
            </a>
          </p>
          <div class="flex">
            <span class="badge badge-success badge-outline mr-1">Moderate</span>
          <span class="badge badge-ghost badge-outline">17/02/24</span></div>
        </div>
      </div>
      <div class="flex shrink-0 items-center gap-x-4 ">
        <div class="sm:flex sm:flex-col  ">
            <div class="badge badge-success badge-outline">Approved</div>
          <p class="text-xs leading-6 ">Last Updated 13:01</p>
         
        </div>
        <svg class="h-5 w-5 flex-none" viewBox="0 0 20 20" fill="currentColor" aria-hidden="true">
          <path fill-rule="evenodd" d="M7.21 14.77a.75.75 0 01.02-1.06L11.168 10 7.23 6.29a.75.75 0 111.04-1.08l4.5 4.25a.75.75 0 010 1.08l-4.5 4.25a.75.75 0 01-1.06-.02z" clip-rule="evenodd" />
        </svg>
      </div>
    </li>
    
  </ul>
  <Pagination/>
  