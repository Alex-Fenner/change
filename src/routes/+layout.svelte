<script>
    import "../app.css";

    import { onMount } from "svelte";
    import Keycloak from "keycloak-js";
    

    onMount(  () => {
        let instance = {
            url: "http://localhost:8084",
            realm: "Change_App",
            clientId: "change"
        };
        let keycloak = new Keycloak(instance);
        
        let initOptions = { onLoad: "login-required" };
        keycloak.init(initOptions).then(function (authenticated) {
                console.info(authenticated);
                console.log(keycloak.idTokenParsed.name)
                
            }).catch(function () {
                alert("unauthorized");
            });
        }
    );

    import { onNavigate } from '$app/navigation';

onNavigate((navigation) => {
	if (!document.startViewTransition) return;

	return new Promise((resolve) => {
		document.startViewTransition(async () => {
			resolve();
			await navigation.complete;
		});
	});
});

  </script>
  


  

<div class="max-w-screen-xl mx-auto ">
    
    <slot />
    
</div>

