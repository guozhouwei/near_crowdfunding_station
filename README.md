# NEAR去中心化募捐活动平台
## React项目文件结构
```shell
NEAR_CROWDFUNDING_STATION
                |___  node_modules
                |___  public
                |___  src
                |___  App.css
                |___  package.json

```

### ➜ package.json
```shell
这个文件是管理下载的依赖包,在项目中经常用到的是"react"库，“react-dom”（将jsx语法渲染到dom中）
在项目中最重要的命令是“start”启动项目，"bulid"的作用就是将项目打包。
``` 

### ➜ public文件夹
• favicon.ico
```shell
是浏览器tab上图标，也是这个项目的一个标志，也可以说是代表一个公司的标志。可以替换。
```
• index.html
```html
项目的入口文件，引用了第三方类库啊，还可以引入cdn
<div id="root"></div>是项目的总容器，所有的内容存储在这个容器中。这个容器有且只能有一个。
```

### ➜ src文件夹
• index.js
```html
存放的是这个项目的核心内容，也就是我们的主要工作区域。其中，index.js文件是和index.html进行关联的文件的唯一接口。
其中：
ReactDOM.render(）的作用是将<App/>的内容渲染到根“root”中去。
document.getElementById('root')中的"root"便是index.html中的"root"了，<App />便是引用页面内容了。在这里，<App />也可以写一些内容(结构,样式,逻辑)是整个项目的根组件。比如:

        ReactDOM.render(<p>Hello World</p>, document.getElementById('root'));

import App from './App'是为了将App.js的内容引入到index.js文件中。
```

• App.js
```html
该类是继承react提供的component，export default App;是为了将App公开，index.js才能够引用。App.js继承了component的话，必须使用render进行渲染。return的内容是类似于html结构的内容，就是jsx，jsx语法是react的主要语法。内部的div的className是为了区分html语法的一个类名，这个是div的样式引用。在这个文件中，只能用一个div容器，如果在div的同级目录添加别的内容，便会报错: 
        ⓧ [js] JSX 表达式必须具有一个父元素。
className="App"，是引用到App.css的样式。注意，页面内容样式是就近原则，首先用App.css的样式，App.css是组件的样式，index.css是全局的样式。
```





# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can't go back!**

If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you couldn't customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)
