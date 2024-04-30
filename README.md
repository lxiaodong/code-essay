# 个人网站介绍 

个人网站完全通过 `markdown` 进行记录，使用了 [hugo](https://gohugo.io/getting-started/) 进行生成私人笔记项目。
themes使用的是 [mainroad](https://themes.gohugo.io/themes/mainroad/)

# 使用方法

## windows下使用
#### 安装hugo(windows)
> 参考地址：https://gohugo.io/getting-started/installing
```text
    mkdir $HOME/src
    cd $HOME/src
    git clone https://github.com/gohugoio/hugo.git
    cd hugo
    go install --tags extended
```

#### 引用
```text
    cd hugo
    git clone https://github.com/lxiaodong/blog
```

#### 启动
```text
    cd blog
    hugo server -D
```

## docker下使用
> 参考地址：https://github.com/klakegg/docker-hugo
```text
   docker pull klakegg/hugo
   mkdir /home/xxx/hugo/ #hugo 自定义
   cd /home/xxx/hugo
   git clone https://github.com/lxiaodong/blog
   docker run --rm -it -v $(pwd)/blog:/src -p 1313:1313 klakegg/hugo:0.107.0  server
```

# 引申

## 搭建Site
> 参考地址：https://gohugo.io/getting-started/quick-start/
```text
    cd hugo
    hugo new site xxx-site
```
## 安装theme (可自行定义)
> 参考地址：https://github.com/adityatelange/hugo-PaperMod/wiki/Installation

```text
    git submodule add --depth=1 https://github.com/adityatelange/hugo-PaperMod.git themes/PaperMod
    git submodule update --init --recursive # needed when you reclone your repo (submodules may not get cloned automatically)
```