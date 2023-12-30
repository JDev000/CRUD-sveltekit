<script>
    import { user } from '..//store.js';
  </script>
  
  <form action="#">
      <input type="email" placeholder="Enter your Name" bind:value={$user.name}>
      <input type="password" placeholder="Enter your Password" bind:value={$user.pass}>
      <button>submit</button>
  </form>
  