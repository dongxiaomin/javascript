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
* var el=document.getElementById()
* var el=document.getElementsClassName()
* var el=document.getElementsByTagName()
* var el=document.getElementsByName()

```

### 筛选元素

* el.nextSibling;
* el.previousSibling;
### 操作样式
* el.style.color='red';
* el.style.size=1;
### 获取位置信息
* el.style.screenX
* el.style.screenY
*  offsetTop         // y轴
*  offsetLeft        //x轴
*  

### 操作属性
* el.currentStyle.width            //ie
* getComputerStyle(el,null).width  //FF

### 操作节点
* document.createElement（元素标签名）
* el.parentNode;
* el.childNodes;
* el.firstChild;
* el.lastChild;


* var el=document.documentElement



### 其他





