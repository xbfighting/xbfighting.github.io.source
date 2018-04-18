---
title: 一个完整的GitFlow
date: 2016-12-22 16:32:02
tags: 
    - git
    - git-flow
    - demo
---
# 一个完整的GitFlow

简要说明：就像代码需要代码规范一样，代码管理同样需要一个清晰的流程和规范本。
本案例主要展示了一个项目通过使用GitFlow管理代码的从特性开发到测试、发布、热修复和代码回归的整个流程。
**PS:本案例中涉及到的分支的新建、合并和删除等操作都可以在GitLab上完成。**

---

## 1.项目初始化

- 在 GitLab上创建项目 "GitFlowDemo"

 ![在 GitLab上创建项目 "GitFlowDemo"][1]

- 目前只有一个分支 master

 ![目前只有一个分支 master][2]

- 本地获取项目

 ![目前只有一个分支 master][3]

- 首次提交，添加文件 "Demo.md"

 ![首次提交][4]

## 2.添加 Develop 分支

- 添加develop分支

``` bash
git branch develop
git push -u origin develop
```

![add develop][5]

- gitlab上已经存在develop分支

![dev has already in gitlab1][6]

- develop和master分支

![dev has already in gitlab2][7]

## 3.开始新Feature开发

- 基于develop添加Feature分支并推送到远端


``` bash
git branch feature/fea_AAA
git checkout feature/fea_AAA 
git push -u origin feature/fea_AAA 
```

![add featuee][8]

- gitlab 上出现feature/fea_AAA分支

![gitlab][9]

- 做一些改动并提交到feature/fea_AAA

``` bash
git status
git add Demo.md
git commit -m "[mod] add feature code"
```

![add some feature][10]

- gitlab

![gitlab][11]

## 4.完成Feature

- 拉取develop更新后合并develop至当前特性分支

``` bash
git pull origin develop
git merge develop
```

![merge develop][12]

- 切回develop分支，合并特性分支至develop分支后推送到远端分支（须确保特性分支经过测试）

``` bash
git checkout develop
git merge feature/fea_AAA 
git push origin develop
```

![merge fea][13]

- gitlab上develop和feature/fea_AAA已经在同一节点

![gitlab][14]

## 5.开始Relase

- 基于develop 添加Release分支并推送到远端

``` bash
git branch release/release_1.0.0
git checkout release/release_1.0.0
git push -u origin release/release_1.0.0
```

![add release][15]

- gitlab 上出现release/release_1.0.0分支

![gitlab][16]

## 6.完成Release（正式发布后进行）

- 合并Release到master

``` bash
git checkout master
git merge release/release_1.0.0 
git push
```

![merge release][17]

- 合并Release到Develop

``` bash
git checkout develop
git merge release/release_1.0.0 
git push
```

![merge release][18]

- 在master打标签 v1.0.0 记录本次发布

![gitlabtag1][19]

![gitlabtag2][20]

![gitlabtag3][21]

- 删除Release分支

![delete release][22]

## 7.开始Hotfix （和开始Release类似）

- 基于 master 添加HotFix分支并推送到远端。

``` bash
git checkout master
git branch hotfix/hotfix_1.0.0
git checkout hotfix/hotfix_1.0.0
git push -u origin hotfix/hotfix_1.0.0
```

## 8.完成Hotfix（和完成Release类似）

- 合并Hotfix到master

``` bash
git checkout master
git merge hotfix_1.0.0
git push
```

- 合并Hotfix到develop

``` bash
git checkout develop
git merge hotfix_1.0.0
git push
```

- 在master打标签 v1.0.1 记录本次发布

![tags][23]
## **至此一个完整的GitFlow完成。**

---

  [1]: http://o97p8x5mf.bkt.clouddn.com/01%20gitlab%E5%88%9B%E5%BB%BA%E9%A1%B9%E7%9B%AE.png
  [2]: http://o97p8x5mf.bkt.clouddn.com/01.01%20gitlab%E5%88%9B%E5%BB%BA%E9%A1%B9%E7%9B%AE%20%E5%8F%AA%E6%9C%89%E4%B8%80%E4%B8%AA%E5%88%86%E6%94%AF.png
  [3]: http://o97p8x5mf.bkt.clouddn.com/01.02%20gitbash%20master%20branch.png
  [4]: http://o97p8x5mf.bkt.clouddn.com/01.02.01%20master%20commit.png
  [5]: http://o97p8x5mf.bkt.clouddn.com/01.04%20develop%20branch%20remote.png
  [6]: http://o97p8x5mf.bkt.clouddn.com/01.05%20develop%20branch%20has%20already%20in%20gitlab%20.png
  [7]: http://o97p8x5mf.bkt.clouddn.com/01.06%20develop%20branch%20has%20already%20in%20gitlab%20.png
  [8]: http://o97p8x5mf.bkt.clouddn.com/02.01.add%20feature.png
  [9]: http://o97p8x5mf.bkt.clouddn.com/02.02.add%20feature.png
  [10]: http://o97p8x5mf.bkt.clouddn.com/02.03.add%20feature.png
  [11]: http://o97p8x5mf.bkt.clouddn.com/02.04.add%20feature.png
  [12]: http://o97p8x5mf.bkt.clouddn.com/03.01.do%20feature.png
  [13]: http://o97p8x5mf.bkt.clouddn.com/03.02.do%20feature.png
  [14]: http://o97p8x5mf.bkt.clouddn.com/03.03.do%20feature.png
  [15]: http://o97p8x5mf.bkt.clouddn.com/04.01.add%20release.png
  [16]: http://o97p8x5mf.bkt.clouddn.com/04.02.add%20release.png
  [17]: http://o97p8x5mf.bkt.clouddn.com/05.01.d0%20release.png
  [18]: http://o97p8x5mf.bkt.clouddn.com/05.02.do%20release.png
  [19]: http://o97p8x5mf.bkt.clouddn.com/05.03.01.do%20release.png
  [20]: http://o97p8x5mf.bkt.clouddn.com/05.04.01.do%20release.png
  [21]: http://o97p8x5mf.bkt.clouddn.com/05.05.do%20release.png
  [22]: http://o97p8x5mf.bkt.clouddn.com/05.06.do%20release.png
  [23]: http://o97p8x5mf.bkt.clouddn.com/06.01.01.do%20hotfix.png