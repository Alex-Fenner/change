<script>
    import { onMount } from 'svelte'
    import { themeChange } from 'theme-change'
    onMount(() => {
  themeChange(false)
  // 👆 false parameter is required for svelte
})
</script>
<div class="navbar bg-base-100 ">
    <div class="flex-1">
      <svg class="w-8 fill-blue-500 stroke-none" version="1.1" viewBox="0.0 0.0 564.7716535433071 668.1811023622047" fill="none" stroke-miterlimit="10" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns="http://www.w3.org/2000/svg"><clipPath id="p.0"><path d="m0 0l564.77167 0l0 668.1811l-564.77167 0l0 -668.1811z" clip-rule="nonzero"/></clipPath><g clip-path="url(#p.0)"><path fill="#000000" fill-opacity="0.0" d="m0 0l564.77167 0l0 668.1811l-564.77167 0z" fill-rule="evenodd"/><path fill="#ff0000" d="m41.85302 355.65485l68.031494 0l0 304.0315l-68.031494 0z" fill-rule="evenodd"/><path stroke-width="1.0" stroke-linejoin="round" stroke-linecap="butt" d="m41.85302 355.65485l68.031494 0l0 304.0315l-68.031494 0z" fill-rule="evenodd"/><path fill="#ff0000" d="m41.85302 355.65485l0 -114.20471l68.031494 114.20471z" fill-rule="evenodd"/><path  stroke-width="1.0" stroke-linejoin="round" stroke-linecap="butt" d="m41.85302 355.65485l0 -114.20471l68.031494 114.20471z" fill-rule="evenodd"/><path fill="#ff0000" d="m109.884514 8.494751l212.53543 0l0 68.18897l-212.53543 0z" fill-rule="evenodd"/><path  stroke-width="1.0" stroke-linejoin="round" stroke-linecap="butt" d="m109.884514 8.494751l212.53543 0l0 68.18897l-212.53543 0z" fill-rule="evenodd"/><path fill="#ff0000" d="m109.884514 8.518373l0 67.02362l-42.04724 -67.02362z" fill-rule="evenodd"/><path stroke="#ff0000" stroke-width="1.0" stroke-linejoin="round" stroke-linecap="butt" d="m109.884514 8.518373l0 67.02362l-42.04724 -67.02362z" fill-rule="evenodd"/><path fill="#ff0000" d="m316.63083 8.59726l0 0c110.22113 -3.594726 202.4509 85.99264 206.1738 200.2668c3.7229004 114.274185 -82.466095 210.11043 -192.66995 214.23582l-2.3692932 -68.04303c72.684326 -2.8215942 129.49173 -67.22885 126.99127 -143.98044c-2.5004578 -76.7516 -63.365204 -136.88493 -136.06134 -134.42627z" fill-rule="evenodd"/><path stroke="#ff0000" stroke-width="1.0" stroke-linejoin="round" stroke-linecap="butt" d="m316.63083 8.59726l0 0c110.22113 -3.594726 202.4509 85.99264 206.1738 200.2668c3.7229004 114.274185 -82.466095 210.11043 -192.66995 214.23582l-2.3692932 -68.04303c72.684326 -2.8215942 129.49173 -67.22885 126.99127 -143.98044c-2.5004578 -76.7516 -63.365204 -136.88493 -136.06134 -134.42627z" fill-rule="evenodd"/><path fill="#ff0000" d="m331.1916 355.65485l0 68.75592l-51.93698 -68.75592z" fill-rule="evenodd"/><path stroke="#ff0000" stroke-width="1.0" stroke-linejoin="round" stroke-linecap="butt" d="m331.1916 355.65485l0 68.75592l-51.93698 -68.75592z" fill-rule="evenodd"/></g></svg>
    </div>

    <label class="swap swap-rotate mr-2">
  
        <!-- this hidden checkbox controls the state -->
        <input type="checkbox" class="theme-controller " data-toggle-theme="dark,light" />
        
        <!-- sun icon -->
        <svg class="swap-on fill-current w-7 h-7" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M5.64,17l-.71.71a1,1,0,0,0,0,1.41,1,1,0,0,0,1.41,0l.71-.71A1,1,0,0,0,5.64,17ZM5,12a1,1,0,0,0-1-1H3a1,1,0,0,0,0,2H4A1,1,0,0,0,5,12Zm7-7a1,1,0,0,0,1-1V3a1,1,0,0,0-2,0V4A1,1,0,0,0,12,5ZM5.64,7.05a1,1,0,0,0,.7.29,1,1,0,0,0,.71-.29,1,1,0,0,0,0-1.41l-.71-.71A1,1,0,0,0,4.93,6.34Zm12,.29a1,1,0,0,0,.7-.29l.71-.71a1,1,0,1,0-1.41-1.41L17,5.64a1,1,0,0,0,0,1.41A1,1,0,0,0,17.66,7.34ZM21,11H20a1,1,0,0,0,0,2h1a1,1,0,0,0,0-2Zm-9,8a1,1,0,0,0-1,1v1a1,1,0,0,0,2,0V20A1,1,0,0,0,12,19ZM18.36,17A1,1,0,0,0,17,18.36l.71.71a1,1,0,0,0,1.41,0,1,1,0,0,0,0-1.41ZM12,6.5A5.5,5.5,0,1,0,17.5,12,5.51,5.51,0,0,0,12,6.5Zm0,9A3.5,3.5,0,1,1,15.5,12,3.5,3.5,0,0,1,12,15.5Z"/></svg>
        
        <!-- moon icon -->
        <svg class="swap-off fill-current w-7 h-7" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M21.64,13a1,1,0,0,0-1.05-.14,8.05,8.05,0,0,1-3.37.73A8.15,8.15,0,0,1,9.08,5.49a8.59,8.59,0,0,1,.25-2A1,1,0,0,0,8,2.36,10.14,10.14,0,1,0,22,14.05,1,1,0,0,0,21.64,13Zm-9.5,6.69A8.14,8.14,0,0,1,7.08,5.22v.27A10.15,10.15,0,0,0,17.22,15.63a9.79,9.79,0,0,0,2.1-.22A8.11,8.11,0,0,1,12.14,19.73Z"/></svg>
        
      </label>
    <div class="flex-none gap-2">
      <div class="dropdown dropdown-end">
        <div tabindex="0" role="button" class="btn btn-ghost btn-circle avatar">
          <div class="w-10 rounded-full">
            <img alt="Tailwind CSS Navbar component" src="https://daisyui.com/images/stock/photo-1534528741775-53994a69daeb.jpg" />
          </div>
          
        </div>
        
        <ul tabindex="0" class="mt-3 z-[1] p-2 shadow menu menu-sm dropdown-content bg-base-200 rounded-box w-52">

          <li><a>Logout</a></li>
        </ul>
      </div>
    </div>
  </div>