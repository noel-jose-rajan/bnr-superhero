<script>
    import router from "page"
	import Home from "./pages/Home.svelte"
	import Login from "./pages/Login.svelte"

    let page;

	//Routing
 	router("/",      ()=>{page = Home})
	router("/login", ()=>{ page = Login})
	router.start()

</script>


<svelte:component this={page}  />
