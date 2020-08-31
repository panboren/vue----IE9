
vue-cli4兼容ie9配置

第一步，我们安装兼容依赖

cnpm install babel-polyfill --save
 cnpm install es6-promise --save
 

第二步，我们在main.js 添加一段代码 【这里是兼容es6的】

import promise from 'es6-promise' 
promise.polyfill() // 兼容 Promise
第三步，在项目目录下的 【vue.config.js】里面配置另一个兼容处理，初始化的时候就不会报错

module.exports = {
    configureWebpack: config => {
        config.entry.app = ["babel-polyfill", "./src/main.js"];
    }
}
这样子就完成兼容了。
---------------------------------------------------------------
链接：https://www.cnblog.co/web/2020-04-16/387.html


VUE组件汇总
网址：https://juejin.im/post/5af16a2cf265da0b8636353b

UI组件
element ★13489 - 饿了么出品的Vue2的web UI工具套件
Vux ★8133 - 基于Vue和WeUI的组件库
iview ★6634 - 基于 Vuejs 的开源 UI 组件库
mint-ui ★6253 - Vue 2的移动UI元素
muse-ui ★3705 - 三端样式一致的响应式 UI 库
vue-material ★3328 - 通过Vue Material和Vue 2建立精美的app应用
vuetify ★2925 - 为移动而生的Vue JS 2组件框架
Keen-UI ★2749 - 轻量级的基本UI组件合集
vonic ★1913 - 快速构建移动端单页应用
vue-multiselect ★1539 - Vue.js选择框解决方案
eme ★1529 - 优雅的Markdown编辑器
vueAdmin ★1455 - 基于vuejs2和element的简单的管理员模板
bootstrap-vue ★1267 - 应用于Vuejs2的Twitter的Bootstrap 4组件
Vue.Draggable ★1191 - 实现拖放和视图模型数组同步
eagle.js ★1128 - hacker的幻灯片演示框架
vue-awesome-swiper ★1012 - vue.js触摸滑动组件
vue-table ★1009 - 简化数据表格
vue-chat ★859 - vuejs和vuex及webpack的聊天示例
vue-blu ★850 - 帮助你轻松创建web应用
vue-recyclerview ★849 - 管理大列表的vue-recyclerview
VueCircleMenu ★838 - 漂亮的vue圆环菜单
vue-infinite-scroll ★779 - VueJS的无限滚动指令
buefy ★755 - 响应式UI组件轻量级库
vue-beauty ★749 - 由vue和ant design创建的优美UI组件
vue-waterfall ★737 - Vue.js的瀑布布局组件
radon-ui ★715 - 快速开发产品的Vue组件库
vue-loop ★701 - 无限的内容循环
vue-chartjs ★694 - vue中的Chartjs的封装
vue-carbon ★684 - 基于 vue 开发MD风格的移动端
vue-syntax-highlight ★655 - Sublime Text语法高亮
vue-echarts ★649 - VueJS的ECharts组件
vue-quill-editor ★615 - 基于Quill适用于Vue2的富文本编辑器
vue-amap ★571 - 基于Vue 2和高德地图的地图组件
vue-calendar ★536 - 日期选择插件
vue-infinite-loading ★501 - VueJS的无限滚动插件
vue-swipe ★481 - VueJS触摸滑块
vue-music-player ★451 - Vuejs写一个音乐播放器
vue-scroller ★444 - Vonic UI的功能性组件
vue-datepicker ★436 - 日历和日期选择组件
vue-core-image-upload ★393 - 轻量级的vue上传插件
vue-progressbar ★379 - vue轻量级进度条
Gokotta ★375 - 简单的音乐播放器
vue-sortable ★373 - 轻松添加拖拽排序
vue-picture-input ★352 - 移动友好的图片文件输入组件
vue-echarts-v3 ★351 - VueJS组件封装
markcook ★343 - 好看的markdown编辑器
vue-video-player ★336 - VueJS视频及直播播放器
vue-google-maps ★334 - 带有双向数据绑定Google地图组件
vue-trend ★332 - 简单优雅的星光线条
vuejs-datepicker ★314 - vue日期选择器组件
vue-fullcalendar ★313 - 基于vue.js的全日历组件
vue-html5-editor ★303 - html5所见即所得编辑器
vue-upload-component ★298 - Vuejs文件上传组件
DataVisualization ★298 - 数据可视化
vue-tables-2 ★291 - 显示数据的bootstrap样式网格
VueStar ★270 - 带星星动画的vue点赞按钮
vue-data-tables ★266 - VueJS2数据表格
vue-paginate ★261 - 分页数据的简约VueJS插件
vue-ydui ★247 - 基于Vue2的移动端和微信UI
vue-mugen-scroll ★239 - 无限滚动组件
vue-virtual-scroller ★238 - 带任意数目数据的顺畅的滚动
vue2-calendar ★236 - 支持lunar和日期事件的日期选择器
vue-dropzone ★233 - 用于文件上传的Vue组件
vue2-douban-market ★233 - 仿豆瓣市集webapp项目
vue-js-modal ★228 - 移动友好的Vuejs2的modal
vue-slider ★224 - vue 滑动组件
vue-datetime-picker ★224 - 日期时间选择控件
rubik ★217 - 基于Vuejs2的开源 UI 组件库
vue-datasource ★210 - 创建VueJS动态表格
vue-image-crop-upload ★205 - vue图片剪裁上传组件
Vueditor ★204 - 所见即所得的编辑器
mint-loadmore ★203 - VueJS的双向下拉刷新组件
vue-slider-component ★202 - 在vue1和vue2中使用滑块
vue-chat ★200 - Vue全家桶+Socket.io+Express/Koa2打造一个智能聊天室
mavonEditor ★179 - 基于Vue的markdown编辑器
vue-carousel-3d ★173 - VueJS的3D轮播组件
vue-baidu-map ★170 - 基于 Vue 2的百度地图组件库
sweet-modal-vue ★170 - 精美的点击提示对话框
vue-particles ★168 - 粒子背景的vue组件
vue-swiper ★167 - 易于使用的滑块组件
vue-simplemde ★166 - VueJS的Markdown编辑器组件
vue-slide ★161 - vue轻量级滑动组件
vue-dragula ★157 - 使拖放变得简单
vue-drag-and-drop-list ★156 - 创建排序列表的Vue指令
vue2-editor ★155 - HTML编辑器
vue-charts ★152 - 轻松渲染一个图表
vue-data-grid ★151 - VueJS复杂桌面交互示例
vuwe ★150 - 基于微信WeUI所开发的专用于Vue2的组件库
vue-progressive-image ★148 - Vue的渐进图像加载插件
vue-msgbox ★148 - vuejs的消息框
vue-lazyload-img ★147 - 移动优化的vue图片懒加载插件
vue-dragging ★146 - 使元素可以拖拽
vue-instant ★143 - 轻松创建自动提示的自定义搜索控件
vue-social-sharing ★142 - 社交分享组件
vue-images ★139 - 显示一组图片的lightbox组件
vue-impression ★134 - 移动Vuejs2 UI元素
vue-mdEditor ★131 - 基于VUE的markdown文本编辑器
vue-typer ★130 - 模拟用户输入选择和删除文本的Vue组件
vue-highcharts ★130 - HighCharts组件
vue-tooltip ★129 - 带绑定信息提示的提示工具
vue-svgicon ★127 - 创建svg图标组件的工具
wdui ★124 - 基于Vue2的UI组件库
vue2-loading-bar ★118 - 最简单的仿Youtube加载条视图
vue-tabs-component ★116 - 渲染tabs的Vue组件
MagicMusic ★113 - 不一样的音乐
vue-region-picker ★111 - 选择中国的省份市和地区
vue-datatable ★102 - 使用Vuejs创建的DataTableView
vue-loading ★102 - 元素中加载block的Vue指令
vodal ★99 - 动画的vue模态
vue-img-inputer ★97 - 基于Vue2的图片输入框
vue-video ★96 - Vue.js的HTML5视频播放器
vue-touch-ripple ★95 - vuejs的触摸ripple组件
vue-event-calendar ★91 - 简单小巧的事件日历组件
v-bar ★91 - 虚拟响应跨浏览器滚动条
vue2-timepicker ★84 - 下拉时间选择器
vuejs-paginate ★80 - 分页VueJS组件
vue-toast-mobile ★79 - VueJS的toast插件
vue-datepicker ★78 - 漂亮的Vue日期选择器组件
vue-easy-slider ★77 - Vue 2.x的滑块组件
vue-float-label ★76 - VueJS浮动标签模式
vue-scrollbar ★76 - 最简单的滚动区域组件
vant ★74 - 有赞出品的Vue2.0移动UI
vue-json-tree-view ★74 - Vue的JSON树视图
vue-slick ★73 - 实现流畅轮播框的vue组件
vue-keynote ★73 - 实现声明性代码幻灯片
vue-google-signin-button ★73 - 导入谷歌登录按钮
vue-rate ★68 - Vue评分组件
awesome-mask ★67 - 拥有独一无二mask的表单
vue-radial-progress ★65 - Vue.js放射性进度条组件
vue-quill ★65 - vue组件构建quill编辑器
vue-date-picker ★63 - VueJS日期选择器组件
coffeebreak ★62 - 实时编辑CSS组件工具
vue-good-wizard ★61 - VueJS 2.x wizard plugin
vue-loading ★60 - 使用SVG加载
datepicker ★59 - 基于flatpickr的时间选择组件
vue-placeholders ★58 - 处理占位符图片和乱码
we-vue ★55 - Vue2及weui1开发的组件
vue-fullcalendar ★55 - vue FullCalendar封装
vue-chartkick ★53 - VueJS一行代码实现优美图表
cxlt-vue2-toastr ★52 - 弹出提示的Vue2组件
vue-formly ★51 - VueJS的JS表单
vue2-autocomplete ★51 - vue2的自动完成组件
vue-morris ★50 - Vuejs组件封装Morrisjs库
veui ★50 - VueJS百度企业UI
vue-components ★49 - 移动端UI组件库
vue-star-rating ★49 - 简单高度自定义的星星评级组件
vue-tagsinput ★48 - 基于VueJS的标签组件
vue-tabs ★47 - 多tab页轻型框架
vue-popup-mixin ★47 - 用于管理弹出框的遮盖层
vue-ripple-directive ★45 - 使用Vue指令的Material波纹效果
vue-cropper ★42 - 一个简单的vue 的图片裁剪插件
vue-ztree ★41 - 用 vue 写的树层级组件
vue-touch-keyboard ★41 - VueJS虚拟键盘组件
cubeex ★40 - 包含一套完整的移动UI
vue-chart ★40 - 强大的高速的vue图表解析
vue-music-master ★40 - vue手机端网页音乐播放器
vue-bootstrap-table ★39 - 可排序可检索的表格
vue-emoji ★39 - 好用的emoji插件
handsontable ★39 - 网页表格组件
vue-form-2 ★37 - 全面的HTML表单管理的解决方案
vue-area ★37 - 省市区三级联动插件
vue-side-nav ★37 - 响应式的侧边导航
vue-image-scroll ★36 - 仿网易云音乐的vue图片滚动插件
vue-pull-to-refresh ★35 - Vue2的上拉下拉
mint-indicator ★35 - VueJS移动加载指示器插件
vue-image-clip ★34 - 基于vue的图像剪辑组件
vue-material-design ★34 - Vue MD风格组件
vue-simple-upload ★31 - 简单的VueJS上传组件
chartjs ★29 - Vue Bulma的chartjs组件
vue-lazy-background-images ★29 - 懒加载背景组件的Vue组件
vue-ripple ★29 - 制作谷歌MD风格涟漪效果的Vue组件
vue-scroll ★27 - vue滚动
laravel-vue-pagination ★26 - VueJS分页组件
vue-datepicker-simple ★26 - 基于vue的日期选择器
vue-m-carousel ★26 - vue 移动端轮播组件
vue-parallax ★23 - 整洁的视觉效果
vue-img-loader ★22 - 图片加载UI组件
vue-tree ★22 - vue树视图组件
vue-verify-pop ★22 - 带气泡提示的vue校验插件
vue-waves ★22 - waves的VueJS版本
vue-smoothscroll ★20 - smoothscroll的VueJS版本
vue-city ★19 - 城市选择器
vue-laypage ★17 - 简单的VueJS分页组件
vue-typewriter ★15 - vue组件类型
vue-ios-alertview ★14 - iOS7+ 风格的alertview服务
vue-cmap ★14 - Vue China map可视化组件
paco-ui-vue ★12 - PACOUI的vue组件
vue-cascading-address ★9 - vue地区选择器
dd-vue-component ★7 - 订单来了的公共组件库
vue-button ★5 - Vue按钮组件
开发框架
vue.js ★56380 - 流行的轻量高效的前端组件化方案
vue-admin ★4612 - Vue管理面板框架
quasar ★2353 - 响应式网站和混合移动应用程序
electron-vue ★2085 - Electron及VueJS快速启动样板
vue-element-admin ★1986 - vue2管理系统模板
vuepack ★1618 - 现代VueJS启动器
N3-components ★656 - 快速构建页面和应用
VueThink ★373 - 前后端分离框架
vue-2.0-boilerplate ★358 - Vue2单页应用样板​
vue-spa-template ★344 - 前后端分离后的单页应用开发
Framework7-Vue ★283 - VueJS与Framework7结合
vue-bulma ★215 - 轻量级高性能MVVM Admin UI框架
vuetiful ★189 - 创建业务及管理应用程序
vue-stack-2.0 ★155 - Vue2项目样板
vue2-admin-lte ★154 - vue2版本的adminLTE
jspangAdmin ★140 - 基于Vue2的后台管理系统
vue-fullstack ★140 - 实时的用户友好的后台系统
vue-paper-dashboard ★120 - Vue的Tim Paper 仪表盘
vue-webgulp ★113 - 仿VueJS Vue loader示例
vue-element-starter ★83 - vue启动页
vuemin ★17 - 基于Vue的企业级前端开发框架
vue-team-template ★12 - 一种构建vue项目的选择方案
实用库
vuex ★8043 - 专为 Vue.js 应用程序开发的状态管理模式
vue-loader ★1847 - Vue.js 针对Webpack的组件装载插件
vue-validator ★1807 - vue的验证器插件
vue-lazyload ★1224 - 用于懒加载的Vue模块
vuelidate ★1075 - 简单轻量级的基于模块的Vue.js验证
vue-i18n ★1053 - VueJS的多语言切换插件
qingcheng ★736 - qingcheng主题
Vue-Socketio ★533 - VueJS的socketio实现
vue-awesome ★532 - VueJS字体Awesome组件
vue-desktop ★496 - 创建管理面板网站的UI库
vue-axios ★491 - 将axios整合到VueJS的封装
vue-meta ★467 - 管理app的meta信息
vue-head ★396 - head标签的meta信息操作
meteor-vue-component ★382 - vue和meteor整合
avoriaz ★338 - VueJS测试实用工具库
portal-vue ★239 - 在组件外部渲染DOM
vue-flatpickr ★228 - 封装Flatpickr的Vue组件
vue-timeago ★195 - VueJS的时间前组件
blessed-vue ★181 - 编写命令行UI的VueJS运行时
vue-unit ★179 - 创建单元测试组件
vue-authenticate ★177 - 简单的VueJS身份认证库
vue-scrollTo ★174 - 滚动到元素的VueJS指令
vue-svg-icon ★157 - vue2的可变彩色svg图标方案
vue-focus ★148 - 可重用VueJS组件的焦点指令
meteor-vue ★134 - VueJS和Meteor的桥接
element-admin ★130 - 支持 vuecli 的 Element UI 的后台模板
vuep ★118 - 用实时编辑和预览来渲染Vue组件
vuet ★116 - 一个跨页面、跨组件的状态管理插件
vue-bootstrap-modal ★112 - vue的Bootstrap样式组件
vue-animate ★106 - 跨浏览器CSS3动画库
vue-property-decorator ★104 - VueJS和属性Decorator
vue-aplayer ★100 - 便于配置的音乐播放器vue2组件
vue-password-strength-meter ★97 - 交互式密码强度计
vue-websocket ★91 - VueJS的Websocket插件
vue-local-storage ★88 - 具有类型支持的Vuejs本地储存插件
vue-recyclist ★88 - vuejs无限滚动列表
vue-lazy-render ★87 - 用于Vue组件的延迟渲染
vue-qart ★86 - 用于qartjs的Vue2指令
vue-framework7 ★85 - 结合VueJS使用的Framework7组件
vue-cordova ★85 - Cordova的VueJS插件
http-vue-loader ★84 - 从html及js环境加载vue文件
vue-parallax ★84 - 快速60fps视差滚动效果组件
vue-clipboard ★84 - VueJS的剪贴板
vue-kindergarten ★83 - 将kindergarten集成到VueJS应用
vue-events ★83 - 简化事件的VueJS插件
vue-notifications ★80 - 非阻塞通知库
vue-online ★77 - reactive的在线和离线组件
vue-shortkey ★74 - 应用于Vue.js的Vue-ShortKey 插件
vue-bus ★71 - VueJS的事件总线
vuex-i18n ★71 - 定位插件
uiv ★70 - Vue实现的Bootstrap组件
vue-router-transition ★69 - 页面过渡插件
vue-gesture ★69 - VueJS的手势事件插件
vue-clip ★67 - 简约的破解文件上传器
vue-electron ★66 - 将选择的API封装到Vue对象中的插件
cleave ★64 - 基于cleave.js的Cleave组件
vuemit ★63 - 处理VueJS事件
vue-worker ★56 - 使用webworkers的Vue插件
vue-acl ★54 - VueJS访问控制列表插件
vue-ts-loader ★54 - 在Vue装载机检查脚本
Vue.resize ★51 - 检测HTML调整大小事件的vue指令
vuedeux ★50 - 轻量级开源实用用层
vue-ls ★49 - 适配Vuecontext中LocalStorage的Vue插件
lazy-vue ★48 - 懒加载图片
vue-pagination-2 ★46 - 简单通用的分页组件
v-media-query ★44 - vue中添加用于配合媒体查询的方法
vue-observe-visibility ★42 - 当元素在页面上可见或隐藏时检测
vue-lazy-component ★38 - 懒加载组件或者元素的Vue指令
vue-reactive-storage ★37 - vue插件的Reactive层
vue-helmet ★37 - HTML标题管理器
voir ★35 - 保持mutation与视图组件的分离
vuex-shared-mutations ★34 - 分享某种Vuex mutations
vue-drag-zone ★28 - 适用于Vue2的dom拖动组件
vue-eslint-parser ★27 - ESLint自定义解析
modal ★26 - Vue Bulma的modal组件
vue-plan ★25 - Vuex-状态管理
vue-file-base64 ★22 - 将文件转换为Base64的vue组件
vue-methods-promise ★21 - 使vue方法支持promise
Vue.ImagesLoaded ★20 - 检测图片加载的VueJS指令
Famous-Vue ★16 - Famous库的vue组件
leo-vue-validator ★15 - 异步的表单验证组件
vue-titlecase ★13 - 用于字符串titlecased的VueJS过滤器
Vue-Easy-Validator ★12 - 简单的表单验证
vue-zoombox ★12 - 一个高级zoombox
vue-truncate-filter ★10 - 截断字符串的VueJS过滤器
vue-router-storage ★9 - vue历史路由持久化的解决方案
vue-input-autosize ★9 - 基于内容自动调整文本输入的大小
vue-data-validator ★4 - Vuejs2的数据验证插件
vue-lazyloadImg ★4 - 图片懒加载插件
服务端
nuxt.js ★4564 - 用于服务器渲染Vue app的最小化框架
unvue ★310 - 使用简单的通用VueJS应用
express-vue ★302 - 简单的使用服务器端渲染vue.js
vue-ssr ★92 - 非常简单的VueJS服务器端渲染模板
doubanMovie-SSR ★85 - Vue豆瓣电影服务端渲染
vue-ssr ★80 - 结合Express使用Vue2服务端渲染
vue-easy-renderer ★44 - Nodejs服务端渲染
辅助工具
vue-play ★641 - 展示Vue组件的最小化框架
DejaVue ★635 - Vuejs可视化及压力测试
vscode-VueHelper ★228 - 目前vscode最好的vue代码提示插件
vue-generate-component ★56 - 轻松生成Vue js组件的CLI工具
vue-multipage-cli ★40 - 简单的多页CLI
VuejsStarterKit ★29 - vuejs starter套件
应用实例
koel ★7773 - 基于网络的个人音频流媒体服务
pagekit ★4225 - 轻量级的CMS建站系统
vue-manage-system ★2057 - 后台管理系统解决方案
vuedo ★1265 - 博客平台
jackblog-vue ★1120 - 个人博客系统
PJ Blog ★1018 - 开源博客
vue-cnode ★787 - 重写vue版cnode社区
vms ★629 - vuejs2管理系统
CMS-of-Blog ★541 - 博客内容管理器
goldfish ★518 - 用于HashiCorp Vault的Admin UI
rss-reader ★368 - 简单的rss阅读器
vue-ghpages-blog ★254 - 依赖GitHub Pages无需本地生成的静态博客
vue-blog ★143 - 使用Vue2.0 和Vuex的vue-blog
swoole-vue-webim ★137 - Web版的聊天应用
tomato5 ★134 - 实时的协作工具
Loopa-News ★133 - 开源社会新闻应用
vue2-management-platform ★74 - vue2.0+ elementUI 后台管理平台
vue-dashing-js ★70 - nuvo-dashing-js的fork
fewords ★63 - 功能极其简单的笔记本
adminify ★46 - 一个基于Vuetify material的Admin面板
Demo示例
vue2-elm ★8036 - 重写饿了么webapp
Vue-cnodejs ★2491 - 基于vue重写Cnodejs.org的webapp
NeteaseCloudWebApp ★1549 - 高仿网易云音乐的webapp
vue2-happyfri ★1535 - vue2及vuex的入门练习项目
vue-zhihu-daily ★1010 - 知乎日报 with Vuejs
vue2-demo ★994 - 从零构建vue2 + vue-router + vuex 开发环境
vue-wechat ★939 - vue.js开发微信app界面
eleme ★882 - 高仿饿了么app商家详情
vue-demo ★755 - vue简易留言板
bilibili-vue ★694 - 全栈式开发bilibili首页
spa-starter-kit ★646 - 单页应用启动套件
VueDemo_Sell_Eleme ★636 - Vue2高仿饿了么外卖平台
vue-music ★621 - Vue 音乐搜索播放
douban ★606 - 基于vue全家桶的精致豆瓣DEMO
vue-Meizi ★604 - vue最新实战项目
maizuo ★603 - vue/vuex/redux仿卖座网
vue-WeChat ★558 - 基于Vue2高仿微信App的单页应用
vue-demo-kugou ★500 - vuejs仿写酷狗音乐webapp
vue2-manage ★457 - 基于 vue + element-ui 的后台管理系统
zhihudaily-vue ★455 - 知乎日报web版
vue-163-music ★448 - vue仿网易云音乐客户端版
vue-axios-github ★448 - 登录拦截登出功能
douban ★440 - 模仿豆瓣前端
vue-shopping ★404 - 蘑菇街移动端
vue2.0-taopiaopiao ★402 - vue2.0与express构建淘票票页面
xyy-vue ★396 - 大学生交流平台
easy-vue ★370 - 使用Vue实现简易web
vue2.x-douban ★360 - Vue2实现简易豆瓣电影webApp
vue2-MiniQQ ★351 - 基于Vue2实现的仿手机QQ单页面应用
mi-by-vue ★291 - VueJS仿小米官网
daily-zhihu ★275 - 基于Vue2的知乎日报单页应用
vue-leancloud-blog ★268 - 一个前后端完全分离的单页应用
VueMusic-PC ★260 - Vue.js高还原网易云音乐系列
node-vue-server-webpack ★253 - Node.js+Vue.js+webpack快速开发框架
beauty ★245 - 豆瓣美女clone
vue-adminLte-vue-router ★243 - vue和adminLte整合应用
vue-fis3 ★217 - 流行开源工具集成demo
notepad ★216 - 本地存储的记事本
vue-demo-maizuo ★210 - 使用Vue2全家桶仿制卖座电影
Pixel-Web ★198 - 一个 Vue 微博客户端
netease_yanxuan ★198 - vue版网易严选
tmdb-app ★194 - TMDbVueJS应用
vue-express-mongodb ★189 - 简单的前后端分离案例
vue-zhihudaily ★187 - 知乎日报 Web 版本
Vdo ★179 - VueJS与MD重构豆瓣
vue-blog ★171 - 单用户博客
Wuji ★168 - 吾记网页版
hello-vue-django ★160 - 使用带有Django的vuejs的样板项目
Zhihu-Daily-Vue.js ★157 - Vuejs单页网页应用
tencent-sports ★154 - Vue全家桶仿腾讯体育
gouyan-movie-vue ★151 - 基于vue的在线电影影讯网站
x-blog ★145 - 开源的个人blog项目
vue-musicApp ★132 - 使用vue全家桶制作的音乐播放器
vue-cnode ★131 - vue单页应用demo
webpack-vue-vueRouter ★130 - webpack及vue开发的简单项目实例
vue-koa-demo ★128 - 使用Vue2和Koa1的全栈demo
vueBlog ★127 - 前后端分离博客
websocket_chat ★127 - 基于vue和websocket的多人在线聊天室
houtai ★125 - 基于vue和Element的后台管理系统
vue-toutiao ★121 - vuejs高仿今日头条移动端
vue-cnode ★121 - 开源的CNode社区
vue-mini-shop ★121 - VueJS在线商店
photoShare ★120 - 基于图片分享的社交平台
iview2-management-system ★119 - 后台管理系统解决方案简单示例
doubanMovie ★119 - 豆瓣电影展示
eleme-vue2 ★112 - 仿饿了么H5纯前端Vue版
vue-zhihu-daily ★111 - 基于Vue全家桶开发的知乎日报
Vue-News ★107 - 基于vue全家桶的仿知乎日报单页应用
douban-movie ★107 - 仿豆瓣电影wap端
generator-loopback-vue ★104 - 典型前后端分离项目模板
vue-quasar-admin-example ★99 - 将Quasar和VueJS应用于SPA项目
vue-zhihudaily-2.0 ★97 - 使用Vue2.0+vue-router+vuex创建的zhihudaily
vue-todos ★95 - vue最新实战项目教程
vue-music ★91 - 网易云音乐Demo
vue-qqmusic ★90 - Vue全家桶+Mint-Ui打造高仿QQMusic
vue2.x-Cnode ★88 - 基于vue全家桶的Cnode社区
vue-ruby-china ★86 - VueJS框架搭建的rubychina平台
doubanMovie-SSR ★85 - Vue豆瓣电影服务端渲染
vue-jd ★76 - 京东移动web商城
vue-nReader ★73 - 使用vue2.0 + vue-router + vuex 的一个多页面小说阅读webapp
VueBlog ★73 - 前后端分离的个人博客
Zhihu_Daily ★73 - 基于Vue和Nodejs的Web单页应用
vue-koa2-login ★67 - 使用 VueJS & NodeJS 实现的登录注册
webApp ★64 - Vue2的移动端webApp音乐播放器
vue-trip ★64 - vue2做的出行webapp
seeMusic ★63 - 跨平台云音乐播放器
github-explorer ★63 - 寻找最有趣的GitHub库
vue-cli-multipage-bootstrap ★60 - 将vue官方在线示例整合到组件中
vue-XiaoMi-Shop ★59 - 高仿小米商城的项目
Vue-NetEaseCloudMusic ★59 - 模仿IOS版网易云音乐的手机网站
life-app-vue ★59 - 使用vue2完成多功能集合到小webapp
doubanApp ★55 - 用vue2实现仿豆瓣app
ios7-vue ★52 - 使用vue2.0 vue-router vuex模拟ios7
canvas-vue ★50 - 一个Vue+Cnavas酷炫后台管理
vue-bushishiren ★49 - 不是诗人应用
vue-ssr-boilerplate ★48 - 精简版的ofvue-hackernews-2
vuecommunity ★47 - vue.js中文社区
vue-music163 ★47 - 音乐VueJS项目
Vue2-MV ★45 - 仿网易云音乐MV的webapp
musiccloudWebapp ★44 - 用vuejs仿网易云音乐
cnode-vue ★40 - 基于vue和vue-router构建的cnodejs web网站SPA
Framework7-VueJS ★38 - 使用移动框架的示例
m-eleme ★37 - 基于Vue全家桶仿饿了么移动端webapp
sls-vuex2-demo ★37 - vuex2商城购物车demo
eagles ★36 - 各种组件封装
Todos_Vuejs ★35 - vuejs2搭建的极简的todolist
vue-cnode ★35 - 用 Vue 做的 CNode 官网
HyaReader ★35 - 移动友好的阅读器
Vue-Admin ★33 - 基于Vue2的Admin系统
vue2-hybridapp-haoshiqi ★32 - 实现单页面webapp以及hybridapp
zhihu-daily ★32 - 轻松查看知乎日报内容
gank ★32 - gankio资源的阅读应用
vue-h5plus ★31 - 前卫的vue及html5plus跨平台demo
vue-cnode-mobile ★29 - 搭建cnode社区
vue-weather ★26 - 基于vue.js 2.0的百度天气应用
vue-user-center ★26 - vuejs直播类应用web端个人中心
zhihu-daily-vue ★22 - 知乎日报
vue-cnode ★22 - 使用cNode社区提供的接口
vue-starter ★22 - VueJs项目的简单启动页
node-vue-fabaocn ★21 - 基于 node 和 vue 实现的移动官网
vue-memo ★20 - 用 vue写的记事本应用
v-notes ★20 - 简单美观的记事本
vue-flexible-app ★19 - vue开发的一个简易app
simply-calculator-vuejs ★19 - 用VueJS实现简易计算器
vue-dropload ★19 - 用以测试下拉加载与简单路由
Vuejs-SalePlatform ★19 - vuejs搭建的售卖平台demo
vue-shopping-mall ★16 - 基于Vue.js 2.x系列 + vue2-router + axios + iview 商城
qqmusic ★13 - QQ音乐vue
vue-weather ★12 - VueJS天气demo
