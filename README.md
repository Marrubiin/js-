# js-深浅复制

以数组为例：

var a1=[1,2];

var a2=a1;

a2并非新数组，而是指向a1的指针，改变a2中的值会改变a1的值，这种复制方式称为浅复制。

ES5可以通过concat方法复制数组
var a1=[1,2];

var a2=a1.concat();

ES6则可以通过扩展运算符直接复制数组

var a1=[1,2];

var a2=[...a1]; 或 var [...a2]=a1;

以上两种方式称为深复制
