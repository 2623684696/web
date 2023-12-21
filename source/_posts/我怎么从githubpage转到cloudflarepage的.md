---
title: 我怎么从githubpage转到cloudflarepage的
date: 2023-12-21 12:11:44
tags:
---
我刚开始想直接用我原来的githubpage改一下的，然后发现了一个问题。
那是用hexo d穿的，导致整个储存库里面都是已经编译完的静态界面，完全不是源文件。
而cloudflare那边的运作是让你把本地编译也给传上去，让cloudflare帮你编译，你只需要写完然后pull。
这个问题让我直接开了个新库，然后上传的时候有很想不通的事情
cloudflare会报错
fatal: No url found for submodule path '.deploy_git' in .gitmodules
真的是及其神奇，最后靠Restent OU的远程魔法搞好的
然后就是给cloudflare一个npm run build构建参数 输出为/public
然后就完成了