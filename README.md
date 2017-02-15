# dou361.github.io
个人博客

blog结构说明


	_data			网站关键字语言国际化
	_drafts			草稿临时文件
	_includes		加载包含部分方便重用
	_layouts		布局
	_plugins		插件
	_posts			帖子markdown文章存放
	_site			jekyll方式生成的网站内容
	about			关于
	archives		归档
	assets			网站基本的网页内容
	categories		分类
	search			搜索
	tags			标签
	_config.xml		网站配置文件
	404.html		外链的腾讯公益404页面
	atom.xml		订阅网志的格式和rss类似
	CNAME			别名域名跳转使用
	Gemfile			gem文件
	Gemfile.lock	gem文件上锁，如果需要重新安装需要删除该文件
	index.html		首页
	rss.xml			订阅
	sitemap.txt		站点地图


## index.html		首页 layout index.html

## _layouts模板

	layout.html		公共部分，所有的模板都共用这部分模板
	page.html			首页 layout page.html
	archives.html		归档 layout archives.html
	categories.html		分类 layout categories.html
	tags.html			标签 layout tags.html
	photo.html			图片 layout post.html
	post.html			帖子 layout post.html
	search.html			搜索 layout

## _includes包括

	layout.html			公共部分，所有的模板都共用这部分模板
	index.html			首页
	page.html			首页 _partial/archive.html
	archives.html		归档 _partial/archive.html
	categories.html		分类 _partial/archive.html
	tags.html			标签 _partial/archive.html
	post.html			帖子 _partial/archive.html
	search.html			搜索 _partial/search.html

### _partial部分

	after_footer.html	首页底部之后（主要是js函数 分析 回到顶部 mathjax tinysou_search）
	analytics.html		分析
	archive.html		归档（根据首页、归档、分类、标签显示对应的）
	article.html		文章（item显示或者详情显示）
	article_row.html	文章行显示
	footer.html			首页底部（版权声明）
	before_header.html	首页头部之前（js link）
	header.html			首页头部（网站名称 菜单 搜索）
	mathjax.html
	search.html
	sidebar.html		侧边栏（右边的控件内容）
	tinysou_search.html
	totop.html			回到顶部

#### post

	article.html		文章（[轮播图]  头部 内容 脚部 评论 分页）
	gallery.html		画廊
	header.html			文章头部
	footer.html			文章的底部（文章详情中显示分享，非详情中显示评论数）
	catetags.html		文章底部的分类和标签显示
	jiathis.html		文章底部的分享显示
	comment.html		评论（duoshuo 或者 disqus）
	pagination.html		文章的分页（上一篇下一篇）

### _widget控件
首页中侧边栏展示的内容

	category.html	分类
	tag.html		标签
	links.html		友情链接
	rss.html		订阅
	douban.html		豆瓣
	weibo.html		微博

