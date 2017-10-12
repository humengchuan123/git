# git
       这是一个小的技巧，对于新手使用git。

       使用git 新建分支以及管理分支
       Created Saturday 24 November 2012
       在你的github分支上， 你需要保持你的主分支干净， 我说的干净就是没有任何改变，
       那么你可以在任何时候从你的主分支修建一个分支。每次， 你想提交一个补
       丁或者一个新特性时，你需要为它新建一个分支，而这个分支无论如何都会从你的主分支复制过来。
       
       当你要在一个分支做拉请求时， 你也能够继续在其他分支上工作，而且也能够在其它分支上做拉请求。
       在你新建一个新分支从主分支上拉下来所有改变之前，你的主分支需要确保是最新的。
       
       在本地电脑新建一个分支： Git branch <新分支名字>
       将新分支发布在github上： git push origin <新分支名字> [*如果边看边做，会出错，请往下看]
       切换到你的新分支: git checkout <新分支名字> [* 事实上切换到其它分支都是这个命令]
       当你想要在你的分支上提交内容，请确保是在你的那个分支上。
       [* 我的一篇博文上写到了在终端上显示当前分支以及显示当前分支是否做过修改即该分支是否干净]
       查看所有已存在的分支，你可以使用： git branch
       
       它就会有如下显示：
       approval_messages
       master
       master_clean
       [* '·'代表了你现在所在分支]
       为你的分支加入一个新的远程端： git remote add <远程端名字> <地址>
       [* 前文提到出错的地方就是缺少了这一步，如果你在github申请了帐号，
       可以新建一个仓库，这时就会有一个地址[git@github.com:用户名/项目名.git]，
       远程段名字可以随便取，如上文的origin]
       
       
       通过提交将所有修改提交到你的分支上： git push origin <远程端分支> 
       [* 原文有点问题，远程端分支一般是与本地分支是对应的，当然你也可以在本地一个分支
       提交到远程端分支的另一个分支如： git push origin master 提交到远程端的主分支上]
       在本地删除一个分支： git branch -d <本地分支>
       
       
       在github远程端删除一个分支： git push origin :<远程端分支>
       唯一不同的就是冒号代表了删除
       如果你想要改变默认分支， 在github上是很容易的，在你的分支上到Admin页面，
       在下拉菜单里选择你想要设置为默认分支的那个分支。
       
       git中常用的命令：
       $git branch <新分支名字>
       
       $git push origin <新分支名字> <将新分支发布在github上>
       
       git checkout <新分支名字>  切换到你的新分支
       
       $git add {}    《添加你所要上传的文件或者代码》
       
       $git commit -m "提交的描述"  《列出提交，或者修改原因，方便出现错误时，可以回滚》
       
       $git status 《列出文件信息，查看那些文件为跟踪或者已修改》
       
       $git rm
       
       $git mv
       
       $gitignore

       mkdir 创建文件

       git merge  （分子名）  分支合并

       git pull origin master  主分支改变情况

       Linux 命名 进入编辑命令：vim (文件名)    可输入模式 ： 点 i    存储： 点esc  ：w  enter  退出编辑模式：q   存储退出 ：wq

       利用git 启一个http sever ：npm install http-server -g  
        http-server -p (端口)

        浏览器版本检测跟新：<!--[if lte IE 8]>
    <p class="browserupgrade">您的浏览器版本老的可笑，请到 <a href="http://browsehappy.com 

           ">这里</a> 更新，以获取最佳的体验</p>
              <![endif] -->