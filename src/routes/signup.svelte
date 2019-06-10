<svelte:head>
	<title>欢迎注册</title>
</svelte:head>


<form action="">
	<input type="text" placeholder="用户名" class="input">
	<input type="text" placeholder="手机号" class="input">
	<input type="password" placeholder="密码" class="input">
	<input type="password" placeholder="重复密码" class="input">

	<button class="button primary -small">注册</button>
</form>

<style>
form {
	padding: 20px;
}
.input{
	margin: 8px 0;
}

</style>