#JavaScript
## 数据类型
- **基本数据类型**  
数字，字符串，boolean，undefined，null
- **复杂数据类型**
object，array,function
### 字符转换函数
1.a.toString(),括号内输入的数字代表进制，null,undefined没有这个方法
2。String（a）,可以将null,undefined转换成字符null,undefined
3.parseInt(),parseFloat(),将字符串转换为数字，转换规则是：从第一个非空白字符（空格、换行、tab）开始转换，直到遇到一个非数字字符为止。
### Boolean
对于布尔转换函数Boolean(),除过 null，undefined,0,NaN,空字符串外，其余都为true
### 比较运算符
  console.log(undefined == null); // true
  console.log(NaN == NaN); //false

  // 比较字符编码时，是一位一位进行比较。如果两位一样，则比较下一位，所以借用它可以来对英文进行排序。
        console.log('56' > '123'); //  true
        console.log('abc' > '123'); // 97>1 true



隐式转换规则：
转换成string类型：+  
转换成Number类型：++/--(自增或自减) + - * / (算术运算符)  > <   >= <=  == != === !===  
转换成boolean : !(逻辑非运算符)  

对于复杂数据类型来说：西先是调用valueOf方法求原值，如果原值不是number类型，则使用toString()方法转换成string  
相关面试题如下：
````
var a = ???
if(a ==1&& a ==2&&a ==3){
  console.log(1);
}
如何完善a使其正确输出1
````

[隐式转换最全总结](https://blog.csdn.net/itcast_cn/article/details/82887895#commentBox)