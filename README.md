# 代码片段工具库


## 安装及快速开始
可以发布到npm或公司私有库

### 方式1: 临时指向源(如果发布到的是公司私有库)
``` bash
npm install -g lhb-snippets --registry=http://
```
### 方式2: 切换源(如果发布到的是公司私有库)

``` bash
npm config set registry http://
```

安装:

``` bash
npm install -g lhb-snippets
```

### 帮助
在命令后添加 -h 可查看详细帮助,例:

``` bash
lhb-snippets create -h
```

### 创建指定文件名或文件夹下的文件代码片段

```js
lhb-snippets create <file-name>

or

lhb-snippets create <path/file-name>

```

### 更新代码片段并发布npm包
1. 在package.json中增加version版本号
2. 在Changelog.md中添加版本修改记录
3. 如果有新增的代码片段文件或目录，要在docs.md中添加创建指令及描述
4. 将代码push到gitlab
5. 执行npm publish发布npm包
