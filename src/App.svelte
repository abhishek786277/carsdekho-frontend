<script>
  let count = 0;
  // @ts-ignore
  import { Router, Link, Route } from "svelte-routing";
  import Login from "./lib/Login.svelte";
  import Signup from "./lib/Signup.svelte";
  import Cars from "./lib/Cars.svelte";
  import "./app.css";
</script>

<main class="bg-gray-800">
  <Router>
    <nav
      class="h-12 bg-gray-800 shadow-lg sticky top-0 text-white flex items-center space-x-4 justify-between px-6"
    >
      <div>
        <h3 class="font-semibold text-2xl">CarsDekho</h3>
      </div>
      <div>
        <Link to="/" class="hover:bg-gray-700 p-2 rounded-md font-semibold"
          >Home</Link
        >
        <Link
          to="/login"
          class="hover:bg-gray-700  p-2 rounded-md font-semibold">Login</Link
        >
        <Link
          to="/signup"
          class="hover:bg-gray-700  p-2 rounded-md font-semibold">SignUp</Link
        >
      </div>
    </nav>
    <div>
      <Route path="/"><Cars /></Route>
      <Route path="/login"><Login /></Route>
      <Route path="/signup"><Signup /></Route>
    </div>
  </Router>
  <!-- <Cars/> -->
  <!-- <Login />
    <Signup /> -->
</main>

<style>
</style>
