1. 리스트 원소 정렬 sort()  
<hr/>  

``` python
A = [2, 1, 3]
A.sort() # 오름차순 정렬
A.sort(reverse = True) # 내림차순 정렬
```
* 결과  
[1, 2, 3]
[3, 2, 1]  
2. map 함수로 띄어쓰기로 입력받은 숫자를 리스트로 만들기  
``` python
n = int(input())

nums = list(map(int,input().split()))

print(nums)
```
2. 리스트에서 특정 항목을 검색하는 법  
<hr/>  

* in 키워드 사용
``` python
a = [1, 2, 3, 4, 5]
print(5 in a) #있다면 True 없다면 False

```



