# Git Practice

**Quick Start**

0. git repo 생성 및 폴더 생성
1. echo "# github-practice" >> README.md
2. git init
3. git add README.md
4. git commit -m "first commit"
5. git branch -M main
6. git remote add origin git@github.com:moonhyun94/github-practice.git
7. git push -u origin main

---

**SSH**

**.ssh 폴더 안에 있는 id_rsa.pub을 등록하면 매번 번거롭게 로그인 하지 않아도 됨**

---

**Pull Request**

1. pull request를 보내고자 하는 repo를 fork

2. fork 한 repo를 local에 clone (ex: upstream)

3. <img width="500" alt="12" src="https://user-images.githubusercontent.com/55631006/111112901-4beebd00-85a4-11eb-8467-208b5e62d637.PNG">  *http는 fork한 repo의 주소*

4. git remote -v 를 통해 잘되었는지 체크한 뒤 git fetch upstream

5. git checkout upstream/main(=branch-name) => upstream의 main branch로 변경

6. git branch -a 를 통해 현재 어떤 branch를 사용하고 있는지 체크 가능

7.  <img width="500" alt="13" src="https://user-images.githubusercontent.com/55631006/111114218-44c8ae80-85a6-11eb-9f22-653e15daa7fa.PNG"></img>    
나의 main branch로 돌아와 git merge upstream/main => 나의 fork repository와 original repository간 merge

9.  나의 repo에서 code 등을 수정하고 pull request를 보냄

10. 나의 request가 confirm 되면 적용됨

