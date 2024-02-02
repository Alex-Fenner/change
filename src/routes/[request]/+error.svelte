<script>
	import { page } from '$app/stores';
    import { onMount } from 'svelte'
    import { themeChange } from 'theme-change'
    onMount(() => {
  themeChange(false)
  // 👆 false parameter is required for svelte
})
</script>

<div class="flex flex-col items-center justify-center  h-screen">
<h1 class="text-primary text-5xl lg:text-9xl">{$page.status}</h1>
<h1>{$page.error.message}</h1>
<a href="/">
<button class="btn btn-outline btn-primary mt-5" >Back to Safety</button></a>
</div>