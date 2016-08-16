# 前端面试题
### javascript


*	第一题
	
	[typeof null, null instanceof Object]  结果是？
	
*	第二题

```
var val = 'smtg';

console.log('Value is ' + (val === 'smtg') ? 'Something' : 'Nothing');

//输出结果是？
```
*	第三题

```
    var name = 'World!';
    (function () {
      if (typeof name === 'undefined') {
        var name = 'Jack';
        console.log('Goodbye ' + name);
      } else {
        console.log('Hello ' + name);
      }
    })();

    //输出结果是？
```
*	第四题

```
var ary = [0,1,2];
ary[10] = 10;
ary.filter(function(x) { return x === undefined;});

//输出结果是？
```
*	第五题

```
    function showCase(value) {
      switch(value) {
        case 'A':
          console.log('Case A');
          break;
        case 'B':
          console.log('Case B');
          break;
        case undefined:
          console.log('undefined');
          break;
        default:
          console.log('Do not know!');
      }
    }
    showCase(new String('A'));	

    //输出结果是？
```

*	第六题

```
function showCase2(value) {
      switch(value) {
      case 'A':
        console.log('Case A');
        break;
      case 'B':
        console.log('Case B');
        break;
      case undefined:
        console.log('undefined');
        break;
      default:
        console.log('Do not know!');
      }
    }
    showCase(String('A'));
    
    //输出结果是？
```

*	第七题

	[]==[] 结果是？



*	第八题

```
var Foo = {};
Foo.method = function() {
    function test() {
    	console.log(this);
    }
    test();
}

Foo.metnod();

//输出结果是？
```

*	第九题 

```
function Foo() {
    this.value = 42;
    this.method = function() {
        console.log(this.value);
    };
    setTimeout(this.method, 500);
}
new Foo();

//输出结果是？
```

*	第10题

```
function foo() { }
    var oldName = foo.name;
    foo.name = "bar";
    [oldName, foo.name]
```

* 	第11题

	Javascript实现格式化输出，比如输入999999999，输出为999,999,999


### HTML&CSS
*	HTML5 为什么只需要写 <!DOCTYPE HTML>？	




*	使用link和@import有什么区别？




*	常见的浏览器内核有哪些？	



*	盒模型



*	用纯CSS创建一个三角形的原理是什么？





参考资料

*	[JavaScript专业八级测试，你能做对几道？](http://ourjs.com/detail/52fb82e13bd19c4814000001)
*	[js秘密花园](http://www.jb51.net/onlineread/JavaScript-Garden-CN/#function.constructors)
*	[面试题](https://github.com/markyun/My-blog/tree/master/Front-end-Developer-Questions/Questions-and-Answers)
