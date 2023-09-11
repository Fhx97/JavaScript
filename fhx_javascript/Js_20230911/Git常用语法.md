# 推码流程
  ## 1.初始化项目
    git init

  ## 2.建立本地仓库和远程仓库的连接
    git remote add origin 远程仓库URL  （移除git仓库连接可使用 git remote remove origin）

  ## 3.将码云上的仓库pull到本地
    git pull origin 分支名称

  ## 4.创建并切换分支
    git checkout -b 分支名称  （本地和远程仓库的分支要一致（选择指定推送的分支，使用git branch可以查看分支））

  ## 5.将文件加载到暂存区
    git add .    （add错了可以使用git rm --cached 文件名 删除对应的文件）

  ## 6.将文件提交到本地仓库（-m 描述信息）
    git commit -m "上传说明，资源描述"

  ## 7.将本地仓库推送到远程仓库
    git push origin 分支名称


# 常用命令
  ## 1.从远程仓库克隆项目到本地
      git clone  项目地址       
  
  ## 2.初始化本地仓库.
      git init   (创建本地仓库)
 
  ## 3.本地仓库与远程仓库关联.
      git remote add 仓库名 仓库地址 (仓库名自定义 例如:origin)
  
  ## 4.查看仓库名
      git remote     (查看远程仓库的仓库名,加-v 查看仓库名和地址)
  
  ## 5.更改远程仓库地址
      git remote ser-url 仓库名 仓库地址  
 
  ## 6.将文件添加添加到暂存区
      git add .    ( . 代表所有,可以指定为具体文件) 

  ## 7.将暂存区中的文件提交到本地仓库
      git commit -m "注说明"
 
  ## 8.查看所有分支
      git branch   （查看本地分支,加-a查看本地分支和远程分支,结果列表中前面标*标识当前使用分支.）
  
  ## 9.创建分支
      git branch 分支名称 
  
  ## 10.切换分支
      git checkout 分支名称

  ## 11.将本地仓库的文件推到远程仓库
      git push 仓库名 分支名称   (推送时建议先(pull)更新一下)

  ## 12.将远程仓库更新到本地
      git pull 仓库名  分支名称  

  ## 13.修改远程仓库名称
      git remote rename 旧名称  新名称

  # 14.查看提交记录
      git log   

  # 15.回滚提交
      git reset --hard commithash     (Reset会把后面提交的记录直接删掉)
      - 例如：git reset --hard 7b8bcaa0b02959126b923fe554824fa9df1dfd87

  # 16.分支合并到主分支上
      git merge 分支名称