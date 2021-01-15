# AutoLotteryNum
import random 

f = open('복권 번호.txt', 'w')

i = 0
while i <5:
    # 일반 복권 번호 생성기5 
    lotto = str(sorted(random.sample(range(1,46),6)))
    f.write(lotto)
    f.write("\n")
    i = i +1
    

f.write("\n")

    
#연금복권 번호
a = 0
while a < 5:
    lotto2 = str(sorted(random.sample(range(1,6), 1)))
    f.write(lotto2)
    f.write("\n")
    li = list(range(0, 10))
    lotto3 = str([random.choice(li) for i in range(6)])
    f.write(lotto3)
    f.write("\n")
    a = a +1


f.close()


    


