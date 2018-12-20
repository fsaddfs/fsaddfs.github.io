#xss上传
---
##上传文件
- 前端检查
 ![123](https://github.com/fsaddfs/fsaddfs.github.io/blob/master/JPG/1.png)
- 发现burp没有抓到数据包，这说明是在前端检查文件后缀名
- 检查源码，发现如下
![123](https://github.com/fsaddfs/fsaddfs.github.io/blob/master/JPG/2.png)
- 这里有两种方式绕过
- 第一，禁用js，如下
![123](https://github.com/fsaddfs/fsaddfs.github.io/blob/master/JPG/3.png)
- 上传成功![123](https://github.com/fsaddfs/fsaddfs.github.io/blob/master/JPG/4.png)
- 第二，将文件名修改为jpg![123](https://github.com/fsaddfs/fsaddfs.github.io/blob/master/JPG/5.png)
- 再抓包把文件名修改回来![123](https://github.com/fsaddfs/fsaddfs.github.io/blob/master/JPG/6.png)
- 上传成功![123](https://github.com/fsaddfs/fsaddfs.github.io/blob/master/JPG/7.png)
- 黑名单判断
###上传图片