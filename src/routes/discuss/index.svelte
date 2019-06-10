<svelte:head>
	<title>优惠福利攻略</title>
</svelte:head>

<script context="module">
	// export function preload({ params, query }) {
	// 	return this.fetch(`blog.json`).then(r => r.json()).then(posts => {
	// 		return { posts };
	// 	});
	// }
	let posts = [
		{
			slug:1,
			title: 'aa',
		},
		{
			slug: 2,
			title: 'bb',
		},
		{
			slug: 3,
			title: 'cc',
		},
		{
			slug: 4,
			title: 'dd',
		}
	]
</script>

<script>
	// export let posts;
</script>


<div class="fiter">
	<span class="active">全部</span>
	<span>发帖时间</span>
	<span>回复时间</span>
	<span>热帖</span>
</div>
<ul>
	{#each posts as post}
		<!-- we're using the non-standard `rel=prefetch` attribute to
				tell Sapper to load the data for the page as soon as
				the user hovers over the link or taps it, instead of
				waiting for the 'click' event -->
		<li>
			<a rel='prefetch' href='discuss/{post.slug}'>{post.title}</a>
			<div class="user">
				<div class="advta">
					<img alt='Borat' src='great-success.png' >
				</div>
				<div>
					<p class="name">小明同学</p>
					<p class="time">3天前</p>
				</div>
			</div>
			<div class="desc">
				<p>这股力量阿斯顿六块腹肌撒科技这股力量阿斯顿六块腹肌撒科技这股力量阿斯顿六块腹肌撒科技这股力量阿斯顿六块腹肌撒科技</p>
				<p>有效期</p>
				<p>分类</p>
				<img alt='Borat' src='great-success.png'>
				<p></p>
			</div>
			<div class="tag">
				<span>pos机</span>
				<span>信用卡</span>
			</div>
			<div class="see">
				<span>左边</span>
				<span>右边</span>
			</div>
		</li>
	{/each}
	<li>
		<!-- <a rel='prefetch' href='discuss/{post.slug}'>{post.title}</a> -->
		<div class="user">
			<div class="advta">
				<img alt='Borat' src='great-success.png' >
			</div>
			<div>
				<p class="name">小明同学</p>
				<p class="time">3天前</p>
			</div>
		</div>
		<div class="desc">
			<p>这股力量阿斯顿六块腹肌撒科技这股力量阿斯顿六块腹肌撒科技这股力量阿斯顿六块腹肌撒科技这股力量阿斯顿六块腹肌撒科技</p>
			<p>有效期</p>
			<p>分类</p>
			<img alt='Borat' src='great-success.png'>
			<p></p>
		</div>
		<div class="tag">
			<span>pos机</span>
			<span>信用卡</span>
		</div>
		<div class="see">
			<span>左边</span>
			<span>右边</span>
		</div>
	</li>
	<li>
		<div class="user">
			<div class="advta">
				<img alt='Borat' src='great-success.png' >
			</div>
			<div>
				<p class="name">小明同学</p>
				<p class="time">3天前</p>
			</div>
		</div>
		<div class="desc">
			<p>这股力量阿斯顿六块腹肌撒科技这股力量阿斯顿六块腹肌撒科技这股力量阿斯顿六块腹肌撒科技这股力量阿斯顿六块腹肌撒科技</p>
			<p>有效期</p>
			<p>分类</p>
			<img alt='Borat' src='great-success.png'>
			<p></p>
		</div>
		<div class="tag">
			<span>pos机</span>
			<span>信用卡</span>
		</div>
		<div class="see">
			<span>左边</span>
			<span>右边</span>
		</div>
	</li>
	<li>
		<div class="user">
			<div class="advta">
				<img alt='Borat' src='great-success.png' >
			</div>
			<div>
				<p class="name">小明同学</p>
				<p class="time">3天前</p>
			</div>
		</div>
		<div class="desc">
			<p>这股力量阿斯顿六块腹肌撒科技这股力量阿斯顿六块腹肌撒科技这股力量阿斯顿六块腹肌撒科技这股力量阿斯顿六块腹肌撒科技</p>
			<p>有效期</p>
			<p>分类</p>
			<img alt='Borat' src='great-success.png'>
			<p></p>
		</div>
		<div class="tag">
			<span>pos机</span>
			<span>信用卡</span>
		</div>
		<div class="see">
			<span>左边</span>
			<span>右边</span>
		</div>
	</li>
	<li>
		<div class="user">
			<div class="advta">
				<img alt='Borat' src='great-success.png' >
			</div>
			<div>
				<p class="name">小明同学</p>
				<p class="time">3天前</p>
			</div>
		</div>
		<div class="desc">
			<p>这股力量阿斯顿六块腹肌撒科技这股力量阿斯顿六块腹肌撒科技这股力量阿斯顿六块腹肌撒科技这股力量阿斯顿六块腹肌撒科技</p>
			<p>有效期</p>
			<p>分类</p>
			<img alt='Borat' src='great-success.png'>
			<p></p>
		</div>
		<div class="tag">
			<span>pos机</span>
			<span>信用卡</span>
		</div>
		<div class="see">
			<span>左边</span>
			<span>右边</span>
		</div>
	</li>


</ul>


<style>
.fiter{
	line-height: 42px;
}
.fiter span{
	margin: 0 12px;
}
.fiter span.active{
    border-bottom: 2px solid #ff5e3a;
    padding-bottom: 10px;
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

li{
    padding: 10px 15px;
	border-top: 5px #e6ecf5 solid;
}
.user{
	display: flex;
    align-items: center;
    margin-bottom: 6px;
}
.name{
	font-size: 16px;
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
.desc{
	margin-bottom: 6px;
}
.desc img{
	height: 140px;
    object-fit: contain;
}
.tag span{
    background: #000;
    color: #fff;
    margin-right: 6px;
    border-radius: 4px;
    padding: 2px 6px;
    font-size: 12px;
}
.see{
	display: flex;
	border-top: 1px #f2f5f9 solid;
	color: #888da8;
    padding-top: 10px;
    margin-top: 10px;
}
.see span{
	flex: 1;
	text-align: center;
}
.see span:first-child{
	border-right: 1px #f2f5f9 solid;
}
</style>
