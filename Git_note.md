# Git global setup

git config --global user.name "Zhang Ming"
git config --global user.email "zhangming_0706@163.com"

# Create a new repository

git clone https://git.lug.ustc.edu.cn/jackzhang/rl-trip-ppo.git

cd rl-trip-ppo

touch README.md

git add README.md

git commit -m "add README"

git push -u origin master


# Push an existing folder

cd existing_folder

git init

git remote add origin https://git.lug.ustc.edu.cn/jackzhang/rl-trip-ppo.git

git add .

git commit -m "Initial commit"

git push -u origin master

# Push an existing Git repository

cd existing_repo

git remote rename origin old-origin

git remote add origin https://git.lug.ustc.edu.cn/jackzhang/rl-trip-ppo.git

git push -u origin --all

git push -u origin --tags

# git 删除历史commit

  1.滚回上一次提交
  
    git reset --hard HEAD^
    
  2. 强制提交本地代码
  
  git push origin master -f

