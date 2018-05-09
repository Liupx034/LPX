# MyCode

<!DOCTYPE html>
<html>
	<head>
		<meta charset="UTF-8">
		<title></title>
	</head>
	<body>
		<form>
	          <input type="checkbox" value="足球"/>足球
	           <input type="checkbox" value="篮球"/>篮球
	           <input type="checkbox" value="游泳"/>游泳
	           <input type="checkbox" value="唱歌"/>唱歌
	        </form>
	        <p>
		<button id="b1">全选</button>
		<button id="b2">全不选</button>
		<button id="b3">反选</button>
	</p>
	</body>
	 <script src="jquery-1.8.3.min.js" type="text/javascript" charset="utf-8"></script>	<script>
	$("#b1").click(function(){
		$(":checkbox").attr("checked",true);
	})
	$("#b2").click(function(){
		$(":checkbox").attr("checked",false);
	})
	$("#b3").click(function(){
		$(":checkbox").each(function(){
			this.checked=!this.checked;
		})
		
	})
	
</script>
</html>
