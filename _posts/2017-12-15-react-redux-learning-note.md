---
layout: post
title: React & Redux 學習筆記
subtitle: 一起來釐清一些觀念吧！
category: 程式學習
tags: [coding, react, redux, 學習]
published: false
img-src: /img/2017/12-15
url:  /2017-12-15-react-redux-learning-note
image: /img/2017/12-15/logo.jpg
---


來介紹一下一些 React 的基本概念吧。
###React 是什麼？

a javascript library

首先先熟悉
1. JSX  
	優點
	- 簡潔(sugar syntax)
	- [prevent injection attacks](https://goo.gl/Po4AJi)
	- Represents Objects
2. ES16
	- class
	- arrow function 
	- let & const
3. Components
	
	- Function based  
		* 簡潔快速
		* Stateless
	- Class based  
		* Stateful
		* Life Cycle
		* re-rendered when state got changes  
			only when you call `this.setState({});` will re-rendered,
			never call `this.state.example='exampleString';`.  
		* 
	重要的性質: 
		- Composing, 可連續排在一起
		- Props are Read-Only	 
			All React components must act like pure functions with respect to
			their props.
		example: [a clock](https://goo.gl/wksPGG)
		- Controlled Components
			form elements such as <input>, <textarea>, and <select> typically
			maintain their own state and update it based on user input. 

			An input form element whose value is controlled by React in this way
			is called a “controlled component”.



	
	####注意！
	State Updates May Be Asynchronous
	```
	this.setState(function(prevState, props) {
		return {
			counter: prevState.counter + props.increment
		};
	});
	```
	

	
		
			

		


<div><a class="hashtag"></a></div>




