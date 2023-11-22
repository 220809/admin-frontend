# Ant Design Pro

This project is initialized with [Ant Design Pro](https://pro.ant.design). Follow is the quick guide for how to use.

## Environment Prepare

Install `node_modules`:

```bash
npm install
```

or

```bash
yarn
```

## Provided Scripts

Ant Design Pro provides some useful script to help you quick start and build with web project, code style check and test.

Scripts provided in `package.json`. It's safe to modify or add additional script:

### Start project

```bash
npm start
```

### Build project

```bash
npm run build
```

### Check code style

```bash
npm run lint
```

You can also use script to auto fix some lint error:

```bash
npm run lint:fix
```

### Test code

```bash
npm test
```

## 项目结构

> ├── config 　# umi 配置，包含路由，构建等配置  
> ├── mock 　　# 本地模拟数据  
> ├── public  
> │ 　　 └── favicon.png 　　# 图标  
> ├── src  
> │ 　　 ├── assets 　　　# 本地静态资源  
> │ 　　 ├── components 　　　# 业务通用组件  
> │ 　　 ├── e2e 　　　# 集成测试用例  
> │ 　　 ├── layouts 　　　# 通用布局  
> │ 　　 ├── models 　　　# 全局 dva model  
> │ 　　 ├── pages 　　　# 业务页面入口和常用模板 ├── tests 　　　# 测试工具  
> ├── README.md # 项目说明  
> └── package.json # 项目依赖配置
>
> 页面目录说明  
> src  
> ├── components  
> └── pages  
> 　　　 ├── Welcome // 路由组件下不应该再包含其他路由组件，基于这个约定就能清楚的区分路由组件和非路由组件了  
> 　　　|　　　 ├── components // 对于复杂的页面可以再自己做更深层次的组织，但建议不要超过三层  
> 　　　|　　　 ├── Form.tsx  
> 　　　|　　　 ├── index.tsx // 页面组件的代码  
> 　　　|　　　 └── index.less // 页面样式  
> 　　　 ├── Order // 路由组件下不应该再包含其他路由组件，基于这个约定就能清楚的区分路由组件和非路由组件了  
> 　　　|　　　 ├── index.tsx  
> 　　　|　　　 └── index.less  
> 　　　 ├── User  
> 　　　|　　　 ├── components // group 下公用的组件集合  
> 　　　|　　　 ├── Login // group 下的页面 Login  
> 　　　|　　　 ├── Register // group 下的页面 Register  
> 　　　|　　　 └── util.ts // 这里可以有一些共用方法之类，不做推荐和约束，看业务场景自行做组织  
> 　　　 └── \*
