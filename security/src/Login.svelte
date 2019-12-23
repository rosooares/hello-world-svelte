<script>
	export let username = "";
	export let password = "";
	function submit(e) {
		e.preventDefault();
		const obj = {
			'username': username,
			'password': password,
		};
		console.log('obj', obj);
	}
</script>

<form>
	<input type="text" name={username} bind:value={username} placeholder="Username"/>
	<input type="password" name={password} bind:value={password} placeholder="Password"/>
	<button type="text" value="Login" on:click={submit}> Login </button>
</form>

<style>
	form {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

</style>