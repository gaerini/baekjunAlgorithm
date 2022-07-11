1. 이진탐색  
<hr/>  
데이터를 정렬하고 배열의 중간에 있는 임의의 값을 선택하여 찾고자 하는 값과 비교한다. 그 값이 중간 값보다 작으면 좌측 데이터만 확인하고 크면 우측 데이터만 확인하여 찾아낸다. 이 과정을 똑같은 방법으로 반복한다. 이런식으로 탐색을 하게 되면 기존의 하나하나 대조하며 찾는 과정에 비해 절반이나 그 작업 시간이 줄어든다.  


소스코드의 예시는 아래와 같다.  
``` python
# data는 오름차순으로 정렬된 리스트
def binary_search_recursion(target, start, end, data):
    if start > end:
        return None

    mid = (start + end) // 2

    if data[mid] == target:
        return mid
    elif data[mid] > target:
        end = mid - 1
    else:
        start = mid + 1        

    return binary_search_recursion(target, start, end, data)

# 테스트용 코드
if __name__ == '__main__':
    li = [i*3 for i in range(11)]
    target = 6
    idx = binary_search_recursion(target, 0, 10, li)

    print(li)
    print(idx)
```
