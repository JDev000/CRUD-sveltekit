<script>
    import { user } from '../store';
  
    function deleteUser() {
      user.set({ name: '', pass: '' }); // Set user to an empty state, simulating deletion
    }
  </script>
  
  <h1>Delete?</h1>
  
  <button on:click={deleteUser}>Delete User</button>
  