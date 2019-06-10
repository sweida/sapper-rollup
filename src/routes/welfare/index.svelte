<svelte:head>
	<title>优惠福利攻略</title>
</svelte:head>

<script>
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


<div class="fiter">
	<span class="active">全部</span>
	<span>信用卡</span>
	<span>电影票</span>
	<span>星巴克</span>
	<span>美食</span>
	<span>购物</span>
	<span>推荐</span>
</div>

<ul>

	{#each posts as post}
	<li>
		<!-- <a href="welfare/{post.slug}">{post.title}</a> -->
		<div class="imgBox">
			<img alt='Borat' src='great-success.png' >
		</div>
		<div>
			<p>华夏行用卡每月领2杯星巴克</p>
			<p>有效期：2019-04-01 至 2019-06-30</p>
			<p>地区：不限</p>
			<p>分类</p>
			<p></p>
		</div>
	</li>
	{/each}
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
ul{
	padding: 15px;
}
li{
	margin:  0 0 16px;
	height: 110px;
    border-radius: 4px;
    padding: 15px;
	display: flex;
	box-shadow: 0 1px 4px 0 rgba(0,0,0,.3);
}
.imgBox{
    width: 120px;
    padding-right: 15px;
}
.imgBox img{
	height: 100%;
	object-fit: contain;
}
</style>