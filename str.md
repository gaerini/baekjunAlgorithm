1. join() 함수를 이용해서 문자열 문자 바꾸기
<hr/>  

``` python
a = "Kimjiho"

l = list(a) # 문자열을 리스트로 바꾸기
l[4] = "u"

a = "".join(l) # 리스트 원소들을 띄어쓰기 없이 붙여 하나의 문자열로 만든다.

'''
결과
Kimjuho
'''
```

