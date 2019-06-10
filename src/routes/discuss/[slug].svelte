<script context="module">
	// export async function preload({ params, query }) {
	// 	// the `slug` parameter is available because
	// 	// this file is called [slug].html
	// 	const res = await this.fetch(`blog/${params.slug}.json`);
	// 	const data = await res.json();

	// 	if (res.status === 200) {
	// 		return { post: data };
	// 	} else {
	// 		this.error(res.status, data.message);
	// 	}
	// }
	let comment = [
		{title: 'aasaa',content: 'aaaa'},
		{title: 'bbb',content: 'bbb'},
		{title: 'cccc',content: 'ccc'},
		{title: 'dddd',content: 'ddd'},
	]
</script>



<!-- <svelte:head>
	<title>{post.title}</title>
</svelte:head>

<h1>{post.title}</h1>

<div class='content'>
	{@html post.html}
</div> -->


<div class="detail">
	<h2>这是标题啊 啊啊啊 啊阿克苏绝代风华啊！</h2>

	<div class="user">
		<div class="advta">
			<img alt='Borat' src='great-success.png' >
		</div>
		<div>
			<p class="name">小明同学</p>
			<p class="time">3天前</p>
		</div>
	</div>
	<div>
		这是正文
		这是正文
		这是正文
		这是正文
		这是正文
		这是正文
		这是正文
		这是正文
		这是正文
		这是正文
	</div>

	<div class="likes">
		<div>see</div>
		<div>like</div>
		<div>notlike</div>
	</div>

	<div class="comment">
		<div class="top">
			跟帖回复
			<span class="fr">0个回复</span>
		</div>

		{#if comment.length==0}
			<div class="nolist">(┬＿┬) 暂无回复</div>
		{:else} 
			<ul>
				<li>
					<div class="user">
						<div class="advta">
							<img alt='Borat' src='great-success.png' >
						</div>
						<div>
							<span class="fl">小明同学</span>
							<span class="fr">18👍</span>
							<!-- <p class="time">3天前</p> -->
						</div>
					</div>
					<div class="text">
						<p>这是回复内容这是回复内容这是回复内容这是回复内容这是回复内容</p>
						<div>4小时前 · <span>回复</span> · <span>删除</span></div>
					</div>
				</li>
				<li>
					<div class="user">
						<div class="advta">
							<img alt='Borat' src='great-success.png' >
						</div>
						<div>
							<span class="left">小明同学</span>
							<span class="right">18👍</span>
							<!-- <p class="time">3天前</p> -->
						</div>
					</div>
					<div class="text">
						<p>这是回复内容</p>
						<div>4小时前 · <span>回复</span></div>
					</div>
				</li>
				<li>
					<div class="user">
						<div class="advta">
							<img alt='Borat' src='great-success.png' >
						</div>
						<div>
							<span class="left">小明同学</span>
							<span class="right">18👍</span>
							<!-- <p class="time">3天前</p> -->
						</div>
					</div>
					<div class="text">
						<p>这是回复内容</p>
						<div>4小时前 · <span>回复</span></div>
					</div>
				</li>
				<li>
					<div class="user">
						<div class="advta">
							<img alt='Borat' src='great-success.png' >
						</div>
						<div>
							<span class="left">小明同学</span>
							<span class="right">18👍</span>
							<!-- <p class="time">3天前</p> -->
						</div>
					</div>
					<div class="text">
						<p>这是回复内容</p>
						<div>4小时前 · <span>回复</span></div>
					</div>
				</li>
			</ul>
		{/if}
	</div>
</div>


<style>
.detail {
	padding: 1.2em;
}
.user{
	display: flex;
    align-items: center;
    margin-bottom: 6px;
}
.name{
	font-size: 14px;
	font-weight: 400;
	margin-bottom: 12px;
}
.user .time{
	font-size: 14px;
	color: #aeb1b5;
}
.user .time:before{
	content: '';
    width: 10px;
    height: 10px;
    position: relative;
    background: #000;
    border-radius: 50%;
    display: inline-block;
    margin-right: 5px;
}
.advta{
	width: 36px;
	height: 36px;
	border-radius: 50%;
	overflow: hidden;
	margin-right: 10px;
	box-shadow: 0 1px 4px 0 rgba(0,0,0,.3);
}
.advta img{
	object-fit: cover;
    height: 100%;
}

.comment .top{
	line-height: 36px;
	font-size: 16px;
}
.comment .top span{
	font-size: 14px;
	color: #9a9fbf;
}
.comment li{
	margin-top: 20px;
}
.comment li .text{
	margin-left: 46px;
}

.nolist{
	color: #9a9fbf;
	border-top: 1px solid #e6ecf5;
	font-size: 16px;
	line-height: 100px;
	text-align: center;
}

.likes{
	display: flex;
	justify-content: space-around;
	margin: 30px 0;
}
.likes>div{
	border-radius: 36px;
	width: 76px;
	line-height: 38px;
	border: 1px solid #e6ecf5;
	text-align: center;
}

</style>