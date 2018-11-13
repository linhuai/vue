# VUE


##Vue挂载的三种方法

第一种,最常见.vue-cli模板就是这样

```
import Vue from 'vue'
import App from './App'
 

new Vue({
	el: '#app',    // #app 元素的 outerHTML 是 Vue 模板，该模板可以被编译成 render function。
	template: '<App/>',
	components: { App }
})
```

第二种

```
new Vue({
	router,
	store,
	render: h => h(App)
}).$mount('#app')
```
 

第三种

```
new Vue({
  el: '#app', 
  router,
  render: h => h(App)
})
```

###Plugins


```
HtmlWebpackPlugin
HtmlWebpackPlugin简化了HTML文件的创建，以便为你的webpack包提供服务。这对于在文件名中包含每次会随着编译而发生变化哈希的 webpack bundle 尤其有用。 你可以让插件为你生成一个HTML文件，使用lodash模板提供你自己的模板，或使用你自己的loader。

ExtractTextWebpackPlugin
Extract text from a bundle, or bundles, into a separate file.

webpack-merge

```
