<script>
    import { user } from '../store.js';
  
    let newName = $user.name;
    let newPass = $user.pass;
  
    function updateUserInfo() {
      user.set({ name: newName, pass: newPass });
      newName = '';
      newPass = '';
    }
  </script>
  
  <form on:submit|preventDefault={updateUserInfo}>
    <label>
      New Name:
      <input type="email" bind:value={newName} />
    </label>
  
    <label>
      New Password:
      <input type="password" bind:value={newPass} />
    </label>
  
    <button type="submit">Update</button>
  </form>
  