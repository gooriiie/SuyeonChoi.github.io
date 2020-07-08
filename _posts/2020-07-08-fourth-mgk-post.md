---
title: "2020년 7월 07일 모각코 3일차"
date: 2020-07-08
categories: MGK
--- 

### 2020년 7월 07일 모각코 3일차 진행  
+ 금일의 모각코 진행 목표  
 1. Github 팀블로그 쓰는법 알려주기: PR방법    
 2. 알고리즘: 재귀, 백트래킹 공부하고 해당문제 최소 1개 풀기
 (재귀 대신 Greedy알고리즘을 공부하려고 했지만 재귀를 공부하는 것이 백트래킹과 더 잘 어울릴 것 같아서 수정)   
 3. React & Redux: Mooc 3강 강의 듣기  
 
   
+ 금일의 모각코 진행 결과  
 1. 팀블로그를 돌아가면서 쓰기 위하여 팀원들에게 레포를 포크하여 Pull Request하는법을 15분정도 알려주었다.  
 2. 재귀와 백트래킹에 대해 공부한 뒤, [백트래킹 문제](https://www.acmicpc.net/problem/15649)를 풀고
 이를 [레포](https://github.com/SuyeonChoi/Algorithms/tree/master/BaekJoon/Python/%EB%B0%B1%ED%8A%B8%EB%9E%98%ED%82%B9)에 push하였다.  
 ```python
 N, M = map(int, input().split())
 arr = [0 for _ in range(N+1)]
 isused = ['F' for _ in range(N+1)]
 def solution(n):
     if n == M:
         for i in range(M):
             print(arr[i], end=' ')
         print()
         return
     for i in range(1, N+1):
         if isused[i] == 'F':
             arr[n] = i
             isused[i] = 'T'
             solution(n+1)
             isused[i] = 'F'  
 solution(0)
 ```
 아직 익숙하지 않아 처음에 구현할 때는 다소 어려웠다. 백트래킹 문제를 좀 더 풀어보며 감을 익혀야겠다...  
 3. React & Redux: Udemy에서 강의 하나를 듣고 튜토리얼을 따라가며 유튜브 검색 웹 페이지를 만들었다.  
  웹 페이지 사진을 첨부하고 싶으나 당일 사용가능한 쿼리문을 초과해버렸다..ㅠ  
  다음부터는 아껴서 테스트해야겠다..  
