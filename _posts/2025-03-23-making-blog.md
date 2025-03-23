---
title: 개발은 1도 모르는 깃허브 블로그 제작 일지
tags: TeXt, 기획, 개발, 깃헙, 깃허브, 블로그
---
   
개발자가 아님에도 깃허브 블로그를 사용하는 이유    

## 1. 회사에서 개발자분들은 협업을 위해 깃허브(Github)를 사용하는데, 솔루션에 익숙해지면 업무 협업에 도움이 될 것 같다.   
## 2. 개발을 위해 파이썬(Python)을 배우려고 생각 중인데, 깃허브(Github)는 코딩에 최적화된 솔루션이다.   
## 3. 파이썬을 배우기 위해 설치해놓은 vscode로 글을 쓸 수 있다.   
## 4. 디자인 협업을 위해 마크업(Mark-up) 지식이 필요한데, 글 작성 시 필요한 마크다운(Mark-down)과의 관계는 정확히 모르겠지만 그래도 도움이 될 것 같다.   
   
   
## 20250319   
초보자를 위한 깃허브 (github) blog 만들기에 도전해보기로 한다.   
우선 깃허브 계정에 가입했지만 뭐가 뭔지 아직 모르겠다.   

## 20250321   
깃허브 가입 후 리포지터리(Repository)를 만들었다.   
리포지터리는 '개별 저장소'의 느낌이다.
   
코딩을 위해 Mac OS에서 '터미널(Terminal)'이라는 응용프로그램을 사용한다.   
"MacTerminal은 Mac에서 사용할 수 있는 최초의 통신 및 터미널 에뮬레이션 응용 프로그램 소프트웨어 프로그램입니다."   
   
깃허브 로그인에 문제가 생겨 해결을 위해 깃허브에서 토큰을 발행하여 로그인했다.
(https://coderefactoring.tistory.com/entry/터미널-깃허브-PUSH-로그인-안됨-문제-해결-fatal-Authentication-failed-for-httpsgithubcom) 감사합니다.   
   
여러가지 
Home brew 설치 https://brew.sh 코드를 터미널에 붙여넣기 한 후 password는 pc 로그인 비밀번호 입력했다.
Home brew 오류 zsh: command not found: brew https://miracleground.tistory.com/entry/Mac에서-Homebrew-설치-후-zsh-command-not-found-brew-오류해결
Ruby & Jekyll 설치 https://skylarcoding.tistory.com/139
Jekyll 수정 시 I를 눌러 편집할 수 있음 esc + :wq 엔터
E325: ATTENTION 에러 -> e해서 edit 하면됨
ERROR:  While executing gem ... (Gem::FilePermissionError)
    You don't have write permissions for the /Library/Ruby/Gems/2.6.0 directory.  >>> 잘못 입력한 것
에러 
설치하려는 폴더 비우고 설치

Npm 설치 https://joyfulhome.tistory.com/180
설치안하면 ERROR '/assets/js/dist/theme.min.js' not found.

https://jjikin.com/posts/Jekyll-Chirpy-테마를-활용한-Github-블로그-만들기(2023-6월-기준)/

도움을 주신 https://wlqmffl0102.github.io/posts/Making-Git-blogs-for-beginners-1/ 블로그 주인장 dodev님 감사합니다. 


3/22 
모두 지우고 처음부터 다시!
1. Ruby 설치 rbenv install 3.1.6
2. Jekyll 설치 gem install jekyll
3. Bundler install
4. 깃허브 리포지터리 생성 및 로컬 위치에 clone
5. 루트 폴더로 이동 cd namsuin.github.io
6. Jekyll 설치 jekyll new ./ 
7. 번들 설치
* $ bundle install
* $ bundle update
* $ bundle install
8. 테마 다운로드 및 압축 로컬에 풀기
9. bundle exec jekyll serve
10. bundle install
11. _config.yml 파일 custom하기
12. 레포지터리에 반영하기
* $ git add -A                          // 모든 수정 파일을 추가합니다.
* $ git status                          // 파일 변경사항을 확인합니다.
* $ git commit -m "원하는 커밋 제목"     // 커밋을 메시지를 작성합니다.
* $ git push                            // 레포지토리로 수정 사항을 업로드합니다.
13. Create auto

리포지터리가 너무 지저분해져서 아예 리셋!
rbenv rehash
rbenv global 3.1.6
gem install bundler jekyll
bundle install
bundle exec jekyll serve
이것 저것 찾아보다 드디어 블로그 생성 완료!

<!--more-->

---

궁금한 점이 있다면 저에게 [email](mailto:plansuin@gmail.com) 을 보내주세요!
제가 할 수 있는 한 최선의 답변을 드리도록 하겠습니다. :star2:

[![Star This Project](https://img.shields.io/github/stars/kitian616/jekyll-TeXt-theme.svg?label=Stars&style=social)](https://github.com/kitian616/jekyll-TeXt-theme/)
