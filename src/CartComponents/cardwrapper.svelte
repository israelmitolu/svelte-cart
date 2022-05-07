<script>
    import Card from "./Card.svelte";
    import items from "../stores/items.js";
  </script>
  
  <div class="container">
    <div class="row">
    
  
      {#each items as item}
      <div class="col-md-4">
  
      <Card {item} /> 
    </div> 
    {/each} 
   </div> </div> 

   <!-- In the above code, we are importing the Card.svelte & item.js files we created earlier and displaying the cards using Bootstrap classes. -->