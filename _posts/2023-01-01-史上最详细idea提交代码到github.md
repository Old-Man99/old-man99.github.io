## github上创建空项目

### 1. 登录自己的github

<img src="../../../images/blogContent/image1.png" referrerpolicy='no-referrer' style =" margin = auto">

### 2. 在github上创建repository

<img src="../../../images/blogContent/image2.png" referrerpolicy='no-referrer' style =" margin = auto">

### 3. 填写仓库基本信息创建

<img src="../../../images/blogContent/image3.png" referrerpolicy='no-referrer' style =" margin = auto">

### 4. 创建后把仓库的git地址copy出来备用`https://github.com/ShengLiuDave/java_test.git`

<img src="../../../images/blogContent/image4.png" referrerpolicy='no-referrer' style =" margin = auto">



## idea上代码关联本地git

### 1. 在idea中进入设置页面 `settings ---> Version Control ---> Git`, 找到git，idea一般会默认自动跟本地git进行关联，如果没有关联，则手动选择git安装路径下的文件进行关联

<img src="../../../images/blogContent/image5.png" referrerpolicy='no-referrer' style =" margin = auto">

### 2. idea中创建git仓库, 点击`VCS ---> import into version control ---> create git repository`

<img src="../../../images/blogContent/image6.png" referrerpolicy='no-referrer' style =" margin = auto">

### 3. 选择相应的项目, 点击Open

<img src="../../../images/blogContent/image7.png" referrerpolicy='no-referrer' style =" margin = auto">

### 4. 看到项目中文件名出现颜色，此时IDEA已为我们创建了一个git仓库

<img src="../../../images/blogContent/image8.png" referrerpolicy='no-referrer' style =" margin = auto">



## idea上代码本地提交

### 1. 点击要提交的项目, 找到git并点击`Commit`

<img src="../../../images/blogContent/image9.png" referrerpolicy='no-referrer' style =" margin = auto">

### 2. 选择你要提交的文件, `Commit`

<img src="../../../images/blogContent/image10.png" referrerpolicy='no-referrer' style =" margin = auto">

### 3. 创建Remotes, 点击`VCS ---> Git ---> Remotes`

<img src="../../../images/blogContent/image11.png" referrerpolicy='no-referrer' style =" margin = auto">

### 4. 点击加号，添加一个远程仓库的地址, 填入相应的远程仓库地址之后点击OK

**url为上面github创建仓库时copy下来备用的**

<img src="../../../images/blogContent/image12.png" referrerpolicy='no-referrer' style =" margin = auto">

### 5. 选择`CVS ---> Git ---> Push`

<img src="../../../images/blogContent/image13.png" referrerpolicy='no-referrer' style =" margin = auto">

### 6. 点击Push

<img src="../../../images/blogContent/image14.png" referrerpolicy='no-referrer' style =" margin = auto">

### 7. 输入github账号密码登录

<img src="../../../images/blogContent/image15.png" referrerpolicy='no-referrer' style =" margin = auto">



## 解决Push rejected: Push to origin/master was rejected

### 1. 第一次提交代码时可能会出现下面这种情况, 如果跟我一样就继续往下看, 如果没有请忽略

Push rejected: Push to origin/master was rejected

<img src="../../../images/blogContent/image16.png" referrerpolicy='no-referrer' style =" margin = auto">

### 2. 打开Terminal终端, 切换到项目路径下

<img src="../../../images/blogContent/image17.png" referrerpolicy='no-referrer' style =" margin = auto">

### 3. 执行`git pull`

<img src="../../../images/blogContent/image18.png" referrerpolicy='no-referrer' style =" margin = auto">

### 4. 执行`git pull origin master --allow-unrelated-histories`和`git push -u origin master -f`

<img src="../../../images/blogContent/image19.png" referrerpolicy='no-referrer' style =" margin = auto">



## 查看效果

<img src="../../../images/blogContent/image20.png" referrerpolicy='no-referrer' style =" margin = auto">

