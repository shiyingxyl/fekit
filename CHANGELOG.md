# 0.2.32  #
* fix: fekit 支持 less @import 语法

# 0.2.31 #
* change: fekit publish 时过滤所有隐藏文件
* change: 可以通过 fekit.config 文件的 min 节点进行自定义编译参数设定
* add: fekit init 增加 README.md 的自动创建
* fix: fekit server 时支持使用软链

# 0.2.30 #
* change: fekit init 默认 config 文件修改为 modular 模式
* change: fekit install xxx -c，强制使用配置文件中的版本范围。 如果没有配置文件或配置文件中没有配置，则不安装

# 0.2.29 #
* change: fekit min 之前，删除 ver & prd 后再生成

# 0.2.28 #
* fix: require了不存在的文件时，编译出错应输出 [ERROR]

# 0.2.27  #
* fix: fekit server 全局 cache 问题

# 0.2.26 #
* change: fekit publish 时，过滤.git , .svn
* fix: fekit server 刷新 cache 时消除 deps 的内容
* change: fekit min 支持只生成 ver 或 mapping 

# 0.2.25 #
* change: fekit server -r aaa:bbb，进行路由功能时，不自动添加前后斜线 https://github.com/rinh/fekit/issues/25
* change: 修改加速方案，改为缓存编译内容

# 0.2.24  #
* change: 编译js时，判断require后如果没有任何字符，则在后面追加分号

# 0.2.23 #
* change: fekit server -b ./project，server功能默认不开启全目录加速，需要时请指定特定目录进行加速
* change: fekit server -r aa:bb -r cc:dd，server的路由功能可以使用多个
* fix: fekit install，在 windows 下会将目录权限丢失

# 0.2.22 #
* fix: fekit min 当指定压缩某非fekit项目文件时失败
* fix: module 被编译后不追加 ;

# 0.2.21  #
* change: fekit convert --qzz，将转换后的require路径设置为以 ./ 开始
* add: fekit min 后，会在 ver 文件中生成 versions.mapping 文件，该文件包括本次编辑产生的所有版本号文件及版本号的键值对

# 0.2.20 #
* fix: compiler 修改 modular 模式为 basename

# 0.2.19 #
* fix: fekit server , contnet-type bug

# 0.2.18 #
* add: 增加单元测试方案(mocha) fekit test
* fix: 解决 server 中不可识别后缀名的 content-type。 https://github.com/rinh/fekit/pull/20
* change: fekit min 的路径可指定，使用 -o
* change: fekit min 编译出现错误时的提示信息更友好
* add: fkeit min -n 可以指定不进行压缩处理
* add: fekit sync 时可以指定 shell 执行
* fix: fekit server 当遇到引错路径的情况会导致 server crash

# 0.2.17 #
* fix: 处理 require 的匹配方式 , 识别 // 及 Ext.require 这样的代码

# 0.2.16  #
* add: 兼容 0.1.x 的源码格式

# 0.2.15  #
* fix: server transfer 没有正确处理非 -t 的情况 
* add: 导出 minCode 功能

# 0.2.14 #
* add: server 添加了 transfer 功能
* add: min 添加了编译使用的毫秒数
* add: min 添加了使用版本

# 0.2.13  #
* change: 组件(定义为compiler:component)的编译模式强制使用 modular

# 0.2.12 #
* fix: convert 时，export 中的路径永远使用 /
* fix: 删除文件夹会导致 watch 中断

# 0.2.11 #
* fix: convert 中使用的 findit 在 windows 下不能正常工作  https://github.com/substack/node-findit/issues/5
* add: 增加 server 的 boost 功能 , 使用 watch file 方式动态缓存 file checksum

# 0.2.10 #
* fix: 使用 node 0.10.x 中的 setImmediate ，并兼容老版本 node 的 process.nextTick
* 优化 module io 读入次数
* fix: min -f 单独压缩文件的问题
* fix: 当引用路径为 require('../xxx') 或 require('xxx') 时，加载错误的问题

# 0.2.9 #
* fix: 修正 cake bump 的方式， 将exec改为spawn

# 0.2.8  #

* add: 增加 cake bump
* add: 增加 unpublish 前的警告

# 0.2.7  #

* add: 使用changelog记录变更

# 0.2.6 #

* fix: 由async引起的 RangeError: Maximum call stack size exceeded

# 0.2.0 #

* 完成组件化工作

# 0.1.29 #

# 0.0.1 #

* initial 
