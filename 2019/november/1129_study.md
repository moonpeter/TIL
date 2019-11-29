# Q56. 리스트의 함수 응용

#### 다음의 딕셔너리가 주어졌을 때 한국의 면적과 가장 비슷한 국가와 그 차이를 출력하세요.

~~~python
nationWidth = {
	'korea': 220877, 
	'Rusia': 17098242, 
	'China': 9596961, 
	'France': 543965, 
	'Japan': 377915,
	'England' : 242900,
}

w = nationWidth['korea']
nationWidth.pop('korea')
l = list(nationWidth.items())
print("l :", l)
gap = max(nationWidth.values())
print("gap :", gap)
item = 0
print("item :", item)

for i in l:
    if gap > abs(i[1] - w):
        print("i[1]:",i[1])
        gap = abs(i[1] - w)
        print("2nd i[1]:",i[1])
        print("gap:",gap)
        print("item:", item)

        item = i
        print("2nd i:",i)
        print("2nd gap:",gap)
        print("2nd item:", item)
print(item[0],item[1]-220877)  ### item[0]밖에 없는데 item[1] ?????

--------------------------------------------------------------------------

l : [('Rusia', 17098242), ('China', 9596961), ('France', 543965), ('Japan', 377915), ('England', 242900)]
gap : 17098242
item : 0
#####(1번째)#####
i[1]: 17098242
2nd i[1]: 17098242
gap: 16877365
item: 0
2nd i: ('Rusia', 17098242)
2nd gap: 16877365
2nd item: ('Rusia', 17098242)
#####(2번째)#####
i[1]: 9596961
2nd i[1]: 9596961
gap: 9376084
item: ('Rusia', 17098242)
2nd i: ('China', 9596961)
2nd gap: 9376084
2nd item: ('China', 9596961)
#####(3번째)#####
i[1]: 543965
2nd i[1]: 543965
gap: 323088
item: ('China', 9596961)
2nd i: ('France', 543965)
2nd gap: 323088
2nd item: ('France', 543965)
#####(4번째)#####
i[1]: 377915
2nd i[1]: 377915
gap: 157038
item: ('France', 543965)
2nd i: ('Japan', 377915)
2nd gap: 157038
2nd item: ('Japan', 377915)
#####(5번째)#####
i[1]: 242900
2nd i[1]: 242900
gap: 22023
item: ('Japan', 377915)
2nd i: ('England', 242900)
2nd gap: 22023
2nd item: ('England', 242900)
-----------------
England 22023
~~~


