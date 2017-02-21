 ## 包装对象
1.var（字面量） 一个（string|number|boolean），会触发包装对象，包装对象在吊用身上的自定义属性是undefined；因为会被销毁，不会为原型添加属性和方法；  要用构造函数的方法（new）；
 ## toString
1. toString() 返回的是某个对象分类的一个字符串值;
2. 在内置的原型上都有toString方法，（不要重写它）；
3. 调用 Object.prototype.toString.call()方法来显示出对象类型 显示方式为[object Class] object小写， 类型首字母大写；
```
<script>
    var arr = [1,2,3,4];
	console.log( arr.toString());//1,2,3,4 
	console.log( {}.toString.call(arr));//[object Array]
</script>
```
4. 对象的类型有
```
Object Array Function Date RegExp Math Null Undefined
```




