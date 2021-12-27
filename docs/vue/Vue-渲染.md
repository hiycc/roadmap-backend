# Vue-渲染
## KeyPoint
1. 使用v-if时元素可能无法获取，而使用v-show一定可以获取。
2. v-if和v-else-if使用时结构不能打断
3. 

## 问
1. v-if和v-show的应用场景？
2. template和v-if如何搭配使用？

## 答
1. v-if适合切换频率低的场景，v-show适合切换频率高的场景。
2. 当你需要有条件渲染某些DOM元素但又不想用div包裹元素时，可以用template搭配v-if（不能用v-show）
```html
<template v-if="n === 1">
  <h2>你好</h2>
  <h2>尚硅谷</h2>
  <h2>北京</h2>
</template>
<!-- 渲染出来后template会层结构会自动消失 -->

<div v-if="n === 1">
  <h2>你好</h2>
  <h2>尚硅谷</h2>
  <h2>北京</h2>
</div>
```
3. 