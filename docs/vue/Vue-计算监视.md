# Vue-计算监视
## KeyPoint
1. 所有被Vue管理的函数，最好写成普通函数，这样this的指向才是vm或组件实例对象。
2. 所有不被Vue管理的函数（定时回调函数、ajax的回调函数、Promise的回调函数），最好写成箭头函数，这样this的指向才是vm或组件实例对象。

## 问
1. computed和watch有什么区别？
2. 

## 答
1. computed能完成的功能，watch也能完成。但watch能完成的功能，computed不一定能完成。例如watch能进行异步操作。
