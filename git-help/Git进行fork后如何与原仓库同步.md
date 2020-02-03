在进行Git协同开发的时候，往往会去fork一个仓库到自己的Git中，过一段时间以后，原仓库可能会有各种提交以及修改，很可惜，Git本身并没有自动进行同步的机制，这个需要手动去执行。name如何进行自己的仓库和原仓库进行Gith同步的操作呢？

　　（1）使用终端命令行，首先在终端中配置原仓库的位置。进入项目目录，执行如下命令：查看你的远程仓库的路径。
　　![mark](http://img.blog.csdn.net/20151020143117598?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQv/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/Center)

　　（2）配置原仓库的路径：
     ![mark](http://img.blog.csdn.net/20151020143335915?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQv/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/Center)
　　（3）再次查看远程目录的位置：
　　![mark](http://img.blog.csdn.net/20151020143448200?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQv/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/Center)

　　（4）抓取原仓库的修改文件：
　　![mark](http://img.blog.csdn.net/20151020143559792?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQv/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/Center)

　　（5）切换到master分支。
　　![mark](http://img.blog.csdn.net/20151020143649113?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQv/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/Center)

　　（6）合并远程的master分支：
　　![mark](http://img.blog.csdn.net/20151020143727279?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQv/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/Center)

　　（7）此时，你的本地库已经和原仓库已经完全同步了。但是注意，此时只是你电脑上的本地库和远程的github原仓库同步了，你自己的github仓库还没有同步，此时需要使用“[Git](http://lib.csdn.net/base/git) push”命令把你本地的仓库提交到github中。
