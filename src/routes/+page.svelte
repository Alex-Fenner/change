<script>
	import NewRequestModal from "../lib/newRequestModal.svelte";
import Navbar from "../lib/navbar.svelte";
	import RequestTable from "../lib/requestTable.svelte";


    

 
</script>

<Navbar/>
<!-- You can open the modal using ID.showModal() method -->
<div class="p-2">
    <RequestTable/>
</div>

<NewRequestModal/>




