# 1. Introduction

本书籍是作者记录的DIY的一些小projects，在这个过程中，学到了很多地道的English。Hope you can enjoy！
你可以按目录查找你需要的DIY知识。
很多DIY 只是不知道key word，造成了搜索的困难。如果知道 key words，网上一搜，就能找到你想要的。

But：

即使是 youtube，很多人都讲的不清不楚，对于beginner来说，看完视频不光效率低下，可能还是没能解决你的问题！
不多说，直接看本书吧！

Enjoy the reading.

**You can search the content via the left-top search box.**

~lomorage2 at gmail dot com.


**Reference：**
1. [gitbook config](https://www.mapull.com/gitbook/comscore/others/book.html)
2. cmd:
   > gitbook install

   > ./run.sh

3. My Windows Dev Env:
   
```Shell
    $ node --version
    v18.13.0

    $ npm --version
    8.19.3
```

4. If you meet gitbook polyfill issue on **graceful-fs**, please comments out as below:

```JavaScript
    c:\Users\%User%\AppData\Roaming\npm\node_modules\gitbook-cli\node_modules\npm\node_modules\graceful-fs\polyfills.js

    fs.chmodSync = chmodFixSync(fs.chmodSync)
    fs.fchmodSync = chmodFixSync(fs.fchmodSync)
    fs.lchmodSync = chmodFixSync(fs.lchmodSync)

    //fs.stat = statFix(fs.stat)
    //fs.fstat = statFix(fs.fstat)
    //fs.lstat = statFix(fs.lstat)

    fs.statSync = statFixSync(fs.statSync)
    fs.fstatSync = statFixSync(fs.fstatSync)
    fs.lstatSync = statFixSync(fs.lstatSync)
```