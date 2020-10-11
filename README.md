> 记录一下git 常用命令，以及相关应用场景解决方案

### 基础命令

```shell
// 配置本地账户信息
$> git config --global user.name '[name]'
$> git config --gloabl user.email '[email]'

// 初始化项目
$> git init              // 本地初始化一个git 项目
$> git clone [url]          // 克隆一个远程仓库，比如GitHub
$> git remote add origin [url]      // 关联到一个远程仓库 

// 分支管理
$> git branch [name]         // 创建一个分支
$> git checkout [branch-name]      // 切换到另一个分支
$> git merge [branch-name]             // 合并指定分支到当前分支上
$> git branch -d [branch-name]            // 删除一个指定分支
```


### 应用场景
#### 分支合并
#### 关联远程分支

关联远程仓库，有两种情况：

手动创建一个GitHub远程仓库。

1. 本地初始化后远程关联

    ```shell
    $> git init

    // 远程仓库创建完成后，进行关联
    $> git remote add origin git@github.com:ngd-b/Git-Project.git
    // 关联后，切换到远程的分支
    $> git checkout main
    ```
    现在GitHub上新建的主分支改为main，不是master

2. 克隆一个远程的仓库
    ```sh
    $> git clone git@github.com:ngd-b/Git-Project.git
    ```

### 其他



### 参考
[Git 教程- 廖雪峰](https://www.liaoxuefeng.com/wiki/896043488029600)