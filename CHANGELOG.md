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