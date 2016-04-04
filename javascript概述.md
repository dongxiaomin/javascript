# javascript概述
 
## 程序语言

* 基础逻辑处理部分

  *变量 数据类型  (数据存储)
  *分支和循环运算符    (逻辑操作)
  *函数（对语言的扩展）

### 变量类型
  ```javascript
   var vr=1.2;            //Number
   var vr='11';           //String
   var vr=false;          //Boolean
   var vr=[1,2,3]         //Array
   var vr={a:1,b:2}       //Object
   var vr=function(){}    //Function
   var vr=undefined
   var vr=null
```   

### 运算符
```javascript
   + - * / %
   ===  !==  >   <   >=   <=
   &&   ||  !
```

###  分支语句
```javascript
   if()
   if()else
   if()else if()else if()
    
   switch(x){
   case 1:
   break;
   case 2:
   break;
   default:
   break;
}
```


###  循环语句
```javascript
for(var i=0,k=12;i<100;i++){
 } 

 while(){}

 do{} while()
```

### 函数语句
```javascript
 function xx(){

}

var fn=function(){
	//arguments
}
fn(a,b) 


functoin A(c){
	this.x=c;
}
A.prototype.console=function(){
	console.log(this.x);
}
var obj=new A(1)
obj.console();

```   


dom对象   dom集合

### 数组的常用方法
### 字符串中的常用方法
### 函数对象中的方法    bind apply call
### 对象的增删改查 原型链
### 数字对象上的方法     toFixed()
### Math对象身上的方法



##  针对特定用途的部分

> 当js用浏览器运行的那一刻
> 浏览器会创建一个window对象
> window对象中很多属性和方法
> 这些属性和方法不用加window.就可以用


### 选取元素
```javascript
* var el=document.getElementById();           //对象
* var el=document.querySelector();           //ie8   

* var el=document.getElementsByClassName();      //集合
* var el=document.getElementsByName();
* var el=document.getElementsByTagName();
* var el=document.querySelectorAll();        //ie8
```

### 筛选元素

>从一个dom对象开始，根据逻辑关系再去寻找dom对象
>父元素
* el.parentNode
* el.parentElement


>子元素
* el.children
* el.firstChild;
* el.firstElementChild;

* el.lastChild;  
* el.lastElementChild;

>兄弟元素
* el.nextSibling;
* el.nextElementSibling;

* el.previous
* el.previousSibling;

### 操作样式
* el.style(设置行内样式的值)
   * el.style.color='red';      
   * el.style.size=1;

### 获取位置信息
* el.style.screenX
* el.style.screenY
*  offsetTop         // y轴
*  offsetLeft        //x轴
*  


###获取元素信息        (HTMLELEMENT)
* el.offsetWidth
* el.offsetHeight
* el.offsetLeft
* el.offsetsetTop
* el.offsetParent              //具有定位属性的父元素
* el.getBoundingClietRect()    //方法  

计算元素距离浏览器窗口位置
* el.innerHTML                 //可读可写
* getComputedStyle(el,null).width   //100px

### 操作属性           (ELEMENT)
<div class="a" id="1"></div>
* el.setAttribute();
* el.getAttribute();
* el.removeAttribute();
* el.hasAttribute();
* el.className;
* el.id;
* el.classList;

### 操作节点  (Node)
* el.appendChild;      //dom对象
* el.removeChild;
* el.insertBefore;      //dom
* el.cloneNode;
* el.replaceChild;





### 其他


按照我们正常的编程思路
第一步找出元素
我们从document对象开始，利用这身上的方法
找出我们需要的元素（dom元素 或 dom集合）





dom对象
js会用一个很大的对象来代表页面中我们看到的那个元素

dom集合
在一个类数组对象中存储很多dom对象构成一个集合

var domobj={
  0:domobj;
  0:domobj;
  0:domobj;
  length:3,
  _proto_:Object;{
      
}

}


//set必须传一个值x。
var obj={
  a:1,
  b:2,
  set c (x){console.log(111);},
  get d (){return 5;}
}