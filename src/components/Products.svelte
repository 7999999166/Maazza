<script>
  import { db } from "../db.js";


  async function addFriend() {

    var xyz = new Promise (function(returns){returns(db.friends.add({name: 'Madhubala',age: 19}));}) ;
    var abc = await xyz ;
    console.log(abc);
     
  } 

</script>
<div>
  <button class="btn btn-primary" on:click={addFriend}>Click me</button>
</div>