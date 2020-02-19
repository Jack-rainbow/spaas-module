### nuxt配置ts

1.安装所需插件

- npm i -D @nuxt/typescript ts-node @types/node @nuxt/typescript-build @nuxt/types
- npm install -S  vue-property-decorator 

2.nuxt.config.js

修改nuxt.config.js文件后缀为 nuxt.config.ts

### 引入nuxt问题？

1.为什么引入？

2.解决什么问题？

3.带来什么收获？

4.为项目带来什么好处？

5.运行、打包

6.tslint是否需要加？

7.vue-property-decorator 与@vue/composition-api 对比？


>区别：

- 1.出品地方
 
    [vue-property-decorator](https://github.com/kaorun343/vue-property-decorator)社区出品

    vue-class-component官方出品

- 2.内部区别
   
   1.vue-class-component提供了Vue、Component等

   2.vue-property-decorator深度依赖了vue-class-component，拓展出了更多操作符：@Prop、@Emit、@Inject、@Model、@Provide、@Watch
   
   3.vue-property-decorator在vue-class-component的基础上增加了更多与Vue相关的装饰器，使Vue组件更好的跟TS结合使用。这两者都是离不开装饰器的，（decorator）装饰器已在ES提案中。Decorator是装饰器模式的实践。装饰器模式呢，它是继承关系的一个替代方案。动态地给对象添加额外的职责。

- 3.使用vuex
  
  1.如果引入了vue-property-decorator，但使用vuex，必须引用vuex-class

- 4.如果以后3.0呢？或者更长远的呢？



vue-property-decorator 优点
- 装饰器
  
    1.@Component (from vue-class-component)
    
    2.@Prop
    
    3.@Model
    
    4.@Watch
    
    5.@Emit
    
    6.@Inject
    
    7.@Provide


综合以上描述,故使用vue-property-decorator