---
title:  "알고리즘-수학"
date:   2022-08-21
categories: [Algorithm]
tags: [Algorithm, Math]
---

## 최대공약수(GCD)
**유클리드 호제법**을 사용해서 구할 수 있음  
**유클리드 호제법**이란?  
두 수 a,b의 최대공약수는 b, a%b의 공약수와 같다.  
위를 이용해 아래와 같은 코드를 짤 수 있음  
**재귀사용**
```java
public int gcd(int a, int b){
  if(b==0){
    return a;
  }else{
    return gcd(b,a%b);
  }
}
```
**재귀 사용X**
```java
public int gcd(int a, int b){
  while( b != 0){
    int r = a%b;
    a = b;
    b = r;
  }
  return a;
}
```

<br>

## 최소공배수(LCM)
두 수 a,b의 최대공약수를 g라고 했을 때  
**최소 공배수 l = g * (a/g) * (b/g)**

<br>

## 소수
### 어떤 수 N이 소수인지 아닌지 판별하는 방법
```java
public boolean prime(int n){
  if(n<2) return false;
  for(int i=2;i*i<n;i++){
    if(n%i == 0){
      return false;
    } 
  }
  return true;
}
```
### N보다 작거나 같은 모든 자연수 중에서 소수를 찾아내는 방법
**에라토스테네스의 체**를 사용  
**에라토스테네스의 체**란?  
N까지의 모든 수에 대해 2부터 제곲 값이 N보다 작은 i까지의 배수들을 지워나가고 남는 수가 소수임  
```java
int N;
int prime[N];
int pn = 0;
boolean check[N+1];
 public int primeNum(int N){
   int answer = 0;
   for(int i=2;i<N;i++){
     if(check[i]==false){
       prime[answer++] = i;
       for(int j = i*i;j<=n;j+=i){
         check[j] = true;
       }
     }
   }
   return answer;
 }
```
