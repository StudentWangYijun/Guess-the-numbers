# Guess-the-numbers

<!DOCTYPE html>
<html>
<head lang="en">
    <meta charset="UTF-8">
    <title>Math.random()</title>
</head>
<body>
<script>
    function getRandom(m,n){
    	var digit=m+n-1;
    	var random=Math.floor(Math.random()*digit+m);
    	return  random;
    }
    var preset=getRandom(1,9);
    input=parseInt(prompt("请输入你猜的数字"));
    while(input!=preset){
    	
    	 if(input>preset){
	      alert("猜大啦");
	      input=parseInt(prompt("请输入你猜的数字"));
    }
         if(input<preset){
    	alert("猜小啦");
    	input=parseInt(prompt("请输入你猜的数字"));
    }   
    }
    	alert("恭喜你猜对啦！");
</script>
</body>
</html>
