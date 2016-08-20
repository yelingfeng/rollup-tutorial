# rollup-tutorial

rollup 入门到放弃
- [x] rollup 是什么东西
- [x] rollup 特性
- [ ] rollup 插件介绍
- [ ] 综合使用指南之站在巨人的肩膀上之开发自己的小类库


## rollup 是什么东西?

“A next-generation ES6 module bundler” 下一代es6模块化<code>bundler</code>, <code>bundler</code>用过<code>webpack</code>的都知道 一般编译后都文件都是叫bundler.js,所以不难理解 这东西就是转换工具 把你的es6代码编译成各种版本的js（amd,cmj,umd）那么引出了下个问题
用它干嘛？ 它有啥牛逼的 ？那么我告诉你 它没啥牛逼的哈， 那为啥还要用它呢 其实我也不知道 我只是简单的想装个逼。

## rollup 特性

### Tree-shaking
   
  tree-shaking 是什么? 这东西就是一个按需打包 只打包你需要的  [看例子](http://rollupjs.org)
  
``javascript``

math.js

export function square ( x ) {
	return x * x;
}
export function cube ( x ) {
	return x * x * x;
}

// 
import { cube } from './maths.js';
console.log( cube( 5 ) ); 

``

用rollup打包commonjs后

``javascript``

'use strict';

function cube ( x ) {
	return x * x * x;
}
console.log( cube( 5 ) ); 

``
可以看到 它只打包了你引用的cube函数 

## rollup 
//TODO



  
