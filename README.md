<!DOCTYPE html>
<html>
<head>
<meta charset="utf-8">
<title>jQuery网站公告上下滚动展示 - 站长素材</title>

<script type="text/javascript" src="js/jquery.min.js"></script>
<script type="text/javascript">
	function timer(opj){
		$(opj).find('ul').animate({
			marginTop : "-3.5rem"  
			},500,function(){  
			$(this).css({marginTop : "0.7rem"}).find("li:first").appendTo(this);  
		})  
	}
	$(function(){ 
		var num = $('.notice_active').find('li').length;
		if(num > 1){
		   var time=setInterval('timer(".notice_active")',3500);
		}
	});
</script>

<style type="text/css">
/*border-bottom: 1px solid #F0F0F0;*/
	.huadong {width: 60rem;height:4rem;padding: 0.5rem 0 0.3rem 0; border-bottom: 1px solid #F0F0F0; position:relative;font: 12px/1.5 "Hiragino Sans GB","Microsoft YaHei",simsun;margin:0 auto;}
	.huadong .huabox {  margin:0 auto; width: 80%; line-height: 4rem;}
	.huadong .hdimg {float:left;line-height:3.5rem;}
	.huadong .hdimg img { width: 100%; vertical-align:middle;}
	.huadong h5 {font-size:1rem;float:left; line-height: 2.2rem; margin: 0.8rem 0 0 0; }
	.huadong .gg_more { float: left;}
	.huadong .gg_more a { font-size: 0.8rem; text-decoration:none;}
	
	.huadong .notice_active {
			float: left;
			width: 55%;
			height: 4rem;
			padding: 0;
			overflow: hidden;
			position: relative;
	}
	.huadong .notice_active li{list-style-type:none;line-height: 2.4rem;overflow: hidden;}
	/*.huadong .notice_active li.notice_active_ch {}*/
	.huadong .notice_active li.notice_active_ch span {color:#656972;font-size:1rem;display: block;overflow: hidden; width:80%;float: left;
	overflow: hidden;margin:0 0 2rem 0;}
	.huadong .gg_more .news_ck {
			float: left;
			margin: 0 1rem 0 1rem;
			color: #888;
			width: 5rem;
			height: 2rem;
			line-height: 2rem;
			display: block;
			border: 1px solid #656972;
			text-align: center;
			border-radius: 0.7rem;
			font-size: 0.8rem;
			margin-top: 1rem;
		}
	.huadong .gg_more .news_more {
		
	}
	.huadong .notice_active li.notice_active_ch em {text-align:right;float:right;color:#888;font-size:0.8rem;font-style:normal;  }
</style>

</head>
<body>

<div class="huadong">
	<div class="huabox">
	<div class="hdimg"><img src="image/lingdang.png"></div>
	<h5>【公告】</h5>
		<div class="notice_active">
			<ul>
				<li class="notice_active_ch">
					<span>滑动轮播1a去哦我我iwoi我i滑动轮播3滑</span>                
					
					<em>2017-01-20</em>
				</li>
				<li class="notice_active_ch">
					<span>滑动轮播2滑动轮播3</span>                
					
					<em>2017-01-20</em>
				</li>
				<li class="notice_active_ch">
					<span>站长素材文字滚动播放</span>                
					
					<em>2017-01-20</em>
				</li>
				
			</ul>   
	
		</div>
	</div>
</div>

<div style="text-align:center;margin:50px 0; font:normal 14px/24px 'MicroSoft YaHei';">
<p>适用浏览器：360、FireFox、Chrome、Safari、Opera、傲游、搜狗、世界之窗. 不支持IE8及以下浏览器。</p>
<p>来源：<a href="http://sc.chinaz.com/" target="_blank">站长素材</a></p>
</div>
</body>
</html>
