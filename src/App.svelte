<script>
  import LogtoClient from '@logto/browser';
  import { onMount } from 'svelte';
  let logtoClient;
  onMount(async () => {
      logtoClient = new LogtoClient({
          endpoint: 'https://j79tk5.logto.app/',
          appId: 'DRWBOmiaeIkJtHJQ4catO',
      });
      // will rerun when client is logged-in, populated with client info
      try {
              await logtoClient.handleSignInCallback(window.location.href);
              console.log(logtoClient); // true
          } catch {
  
              console.log("Not logged-in")
          }
  });
  
  </script>


<p>Create a user in <a href="https://cloud.logto.io">logto</a></p>
<p>Create a vanilla app and adapt code in the source of this page (src/page.svelte)</p>
<button on:click={logtoClient.signIn('http://localhost:5173')}>
  Sign In
</button>
<p>Now open your console to see signed-in client</p>
<p>So easy!</p>
<button on:click={logtoClient.signOut('http://localhost:5173')}>
  Sign Out
</button>
