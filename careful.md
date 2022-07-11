1. integer끼리 연산을 한 결과는 float이기 때문에 연산값을 리스트 인덱스로 쓰기 위해선 자료형을 int로 바꿔주어야한다.  
<hr/>  

``` python
print(type ( 15/3 ))
# 결과
<class 'float'>
```  
2. sort()는 메소드이기 때문에 반환값이 존재하지 않는다. 따라서 다음과 같은 코드는 nonetype error를 일으킬 수 있다.  

``` python
a = [3, 4, 5, 1, 2]
a = a.sort()
print(a)
# NoneType Err 발생
```

