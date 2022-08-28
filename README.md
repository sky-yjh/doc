git init -> 初始化仓库

git status -> 查看 git 管理状态

git add . -> 添加当前项目中的所有文件

git commit -m "描述" -> 提交版本



git restore --staged 文件名：将以 add 的文件取消回到以变动状态

git restore 文件名：将未 add 的文件重置到版本原始状态





git log -> 只能查看提交记录（向下重置版本）

git reflog -> 查看 git 所有版本变更记录

git reset --hard \<hash值\>  -> 高版本向低版本回滚





git branch -> 查看分支

git branch 分支名字 -> 新建分支（基于当前分支的版本）

git branch -d 分支名字 -> 删除分支

git merge 分支名字 -> 先切换到主分支，再选择要合并的分支

git checkout 分支名称 -> 切换分支





git remote add origin 链接 -> 添加远程仓库

git push -u origin 分支名称 -> 推送代码





git clone 链接 -> 第一次拉项目

git pull origin 分支 -> 增量更新





git tag -a 分支名字 -m "分支描述" -> 创建标签

git push origin --tags -> 推送标签

git pull origin --tags -> 拉去标签





-- 配置



$ git config --global user.name <用户名>

$ git config --global user.email <邮箱地址>

$ git config --global http.proxy socks5://127.0.0.1:7890

$ git config --global https.proxy socks5://127.0.0.1:7890





-- 仓库

$ git remote get-url origin

$ git remote set-url origin git@github.com:askfiy/nvim.git



增加小乌龟的使用



### git  问题结局

#### git push错误failed to push some refs to的解决

​        这个问题是因为远程库与本地库不一致造成的，那么我们把远程库同步到本地库就可以了。使用指令

​		`git pull --rebase origin main`

 		产生原因：修改了线上的仓库同时对本地仓库进行了不同更新，所以需要先将本地改动存在rebase里，将远程仓库先pull下来，再上传本地仓库。



