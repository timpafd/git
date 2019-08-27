# github中文解释
Repository(仓库)、Star(收藏类似书签)、Fork(复制项目)、pull requests(发起请求，上传修改文件给原主人，其同意修改后合并到项目)、Watch(关注)、Issues(卡片式讨论)

##git使用
1.  git安装好后需设置git名字与邮箱地址
` git config --global user.name "名字"`
`git config --global user.email "邮箱"`
*git名字、邮箱与github名字、邮箱关系：
> 1、如果git-email和github-email不一致，则即使github-username和git-username用户名相同，用户在本地git和在github上操作也会被认为是不同的用户在操作，意味着：github-email用户创建了仓库，git-email用户从本地上传的代码。
> 2、如果git-email和github-email一致，则认为是同一用户，意味着：用户在本地git上操作再push到github上，和直接在github上操作没有区别

2.  创建git仓库:

         `git init`

3.  添加文件到Git仓库，分两步:

        `1、git add <file>(可以是多个文件中间用空格隔开)`
        `2、git commit -m <message>(说明性文字message,字符串类型)`

4.  查看文件是否被修改:

        `git status`

5.  查看修改内容:

        `git diff <file>`

6. 查看提交历史及HEAD:

        `git log`

        查看简略信息：

        `git log --pretty=oneline`

7. 版本回退:

        ` git reset --hard HEAD^`

    可以把'HEAD^'写成'commit id'即sha1值的前几位

    > 首先，Git必须知道当前版本是哪个版本，在Git中，用HEAD表示当前版本，也就是最新的提交1094adb...（注意我的提交ID和你的肯定不一样），上一个版本就是HEAD^，上上一个版本就是HEAD^^，当然往上100个版本写100个^比较容易数不过来，所以写成HEAD~100。

8. 查看历史:

        `git reflog`

    > Git提供了一个命令git reflog用来记录你的每一次命令

    >显示整个本地仓储的commit, 包括所有branch的commit, 甚至包括已经撤销的commit, 只要HEAD发生了变化, 就会在reflog里面看得到. git log只包括当前分支的commit.

        `git reflog --relative-date`

    >显示相对时间的commit纪录.

### 文件操作

1. 丢弃工作区的修改

        `git checkout -- file`

    > 把文件在工作区的修改全部撤销有两种情况：(1) 文件自修改后还没有被放到暂存区，现在，撤销修改就回到和版本库一模一样的状态。(2) 文件已经添加到暂存区后，又作了修改，现在，撤销修改就回到添加到暂存区后的状态。

    > 命令中的`--`很重要，没有`--`，就变成了“切换到另一个分支”的命令
    
2. 删除文件

        `git rm <file>`

    文件只是删除了最新的版本历史版本还在
    可使用上一条命令恢复误删文件

#### git目录
1.  工作区（Working Directory）：即所有能看到的非隐藏目录
2.  版本库（Repository）：工作区内的隐藏目录`.git`即使git版本库。

    > Git的版本库里存了很多东西，其中最重要的就是称为stage（或者叫index）的暂存区，还有Git为我们自动创建的第一个分支master，以及指向master的一个指针叫HEAD。

    > 创建Git版本库时，Git自动为我们创建了唯一一个master分支，所以，git commit就是往master分支上提交更改。

    > git add命令实际上就是把要提交的所有修改放到暂存区（Stage），然后，执行git commit就可以一次性把暂存区的所有修改提交到分支。
