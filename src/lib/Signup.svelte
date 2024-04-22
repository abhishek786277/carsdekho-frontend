<script>
  const formvalue = {
    name:"",
    email: "",
    password: "",
  };
  // Example POST method implementation:
  async function postData(url = "http://localhost:3000/user/createuser") {
    const response = await fetch(url, {
      method: "POST",
      headers: {
        "Content-Type": "application/json",
      },
      body: JSON.stringify(formvalue),
    });
    return response.json();
  }

  async function handleSignup() {
    const data = await postData();
    console.log(data);
    // navigate('/')
  }
</script>

<div class="flex justify-center items-center w-full min-h-screen bg-gray-800">
  <form
    action=""
    class="flex flex-col gap-6 h-fit w-fit border p-10 shadow-md shadow-black bg-white rounded-lg"
  >
    <div class="flex flex-col">
      <label for="name" class="text-base font-semibold">Name:</label>
      <input
        type="text"
        id="name"
        bind:value={formvalue.name}
        placeholder="Enter your name"
        class="px-4 py-2 border rounded-lg"
      />
    </div>
    <div class="flex flex-col">
      <label for="email" class="text-base font-semibold">Email:</label>
      <input
        type="email"
        id="email"
        bind:value={formvalue.email}
        placeholder="Enter your email"
        class="px-4 py-2 border rounded-lg"
      />
    </div>
    <div class="flex flex-col">
      <label for="password" class="text-base font-semibold">Password:</label>
      <input
        type="password"
        id="password"
        bind:value={formvalue.password}
        placeholder="Enter your password"
        class="px-4 py-2 border rounded-lg"
      />
    </div>
    <div class="flex flex-col items-center">
      <button
        class="text-base font-semibold w-fit p-3 rounded-md hover:bg-gray-800 hover:text-white"
        on:click|preventDefault={handleSignup}>Submit</button
      >
    </div>
  </form>
</div>
