<script>

  import SveltyPicker from 'svelty-picker'

  let myDate = '';
  let myTime = '';
  async function callPrediksi() {
       
       alert(myDate)
       alert(myTime)
   }
</script>

<main class="container mx-auto mt-10">
  
<div class="flex w-full gap-2">
  <div class="bg-white rounded-md shadow-lg w-2/5 p-2">
    <div class="flex flex-col w-full gap-2">
      <div class="flex justify-between items-center w-full border-b-2 border-slate-500 py-2">
        <h1 class="text-[20px] font-semibold uppercase">Prediksi</h1>
        <button on:click={() => {
          callPrediksi();
        }} class="bg-primary p-2 rounded-md text-white shadow-lg">CHECK</button>
      </div>
      <input 
        type="text" 
        placeholder="Type here" 
        class="input input-bordered focus:ring-0 focus:outline-0 rounded-sm w-full">
        <SveltyPicker 
          inputClasses="input input-bordered rounded-sm w-full text-center" format="yyyy-mm-dd" bind:value={myDate}></SveltyPicker>
        <SveltyPicker 
          inputClasses="input input-bordered rounded-sm w-full text-center" format="hh:ii" mode="time" bind:value={myTime}></SveltyPicker>
        
        <button  class="btn btn-primary">CLick Me</button>
    </div>
  </div>
  <div class="bg-amber-500 w-full p-2">
    <a href="#" class="block p-6 max-w-sm bg-white rounded-lg border border-gray-200 shadow-md hover:bg-gray-100 dark:bg-gray-800 dark:border-gray-700 dark:hover:bg-gray-700">
      <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Noteworthy technology acquisitions 2021</h5>
      <p class="font-normal text-gray-700 dark:text-gray-400">Here are the biggest enterprise technology acquisitions of 2021 so far, in reverse chronological order.</p>
    </a>
    
  </div>
</div>
  
</main>

<style global lang="postcss">
  @tailwind base;
  @tailwind components;
  @tailwind utilities;
</style>
