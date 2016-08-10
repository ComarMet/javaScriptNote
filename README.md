# javaScriptNote

JavaScript : 

ECMAScripe  几乎没有兼容性问题
DOM 有一些兼容性问题
BOM 没有兼容性问题几乎不兼容

typeof  类型  相当于iOS 里面isequalclass
undefined   没有定义或者定义的时候没有负值
function 	方法  object  get

currentstyle 集合

insertBefore  元素插入
append child 元素追加
元素追加 让第一个发的内容排在第一个
	<body>
	<input type="text"  id="text"/>	
	<input type="button" value="添加" id="btn" />
	
	<ul id="uill">
	
	</ul>
		
	</body>
	window.onload = function () {
			var oBtn = document.getElementById('btn');
			var oText = document.getElementById('text')
			var oUl = document.getElementById('uill')
			
			oBtn.onclick = function (){
				
				var oli = document.createElement('li');
				var ali  = document.getElementsByTagName('li');

				oli.innerHTML = oText.value;
			if(ali.length==0){
				oUl.appendChild(oli);
			}else {
				oUl.insertBefore(oli,ali[0]);
		}
				
	}

}
			
