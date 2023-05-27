<script>
  import PopupOrder from "../components/popupOrder.svelte";
  import { writable } from "svelte/store";
  // let showPopup = false
  let condition = writable(true); 
  function toggleState() {
    // Update the value of the store to the opposite of its current value
    condition.update((state) => !state);
  }
  console.log($condition);
</script>

<div class="bg-black/30 h-screen flex justify-center items-center relative">
  <button
  
    on:click={toggleState}
    class="absolute top-5 px-4 py-3 bg-slate-500 text-white rounded-md mb-3"
    >عرض الطلب</button
  >
  {#if $condition}
    <PopupOrder on:closePopup={() => (condition = false)} />
  {/if}
</div>
