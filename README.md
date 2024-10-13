# SWE_2021_41_2024_2_week_6
>## week4 Assignment
>>[SWE_2021_41_2024_2_week_4](https://github.com/yonggile/SWE_2021_41_2024_2_week_4)
'''python
def isHappy(n):
  answer=False
  if n <1 or n>2**31-1:
    return False
  def asd(a):
    sum=0
    while(a>0):
      sum=sum+(a%10)**2
      a=a//10
    return sum
  check=list()
  while n !=1 and n not in check:
    check.append(n)
    n=asd(n)
    print(n)
  return n==1
'''
## 주어진 숫자가 범위를 초과하지 않는지 확인 후 각 자리의 숫자를 제곱하여 더하여 반복하여 순환하지 않고 0으로 되는 happy number를 찾는 코드이다.
