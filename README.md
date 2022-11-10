import random
r = [['{1}','{2}','{3}'], ['{1}','{2}','{3}'], ['{1}','{2}','{3}']]
'''
   {1}, {2}, {3}
   {1}, {2}, {3}
   {1}, {2}, {3}
'''
qa = random.randint(1, 3)
us = random.randint(1, 3)
print(qa, us)
def royxat():
    for i in r:
        print(i)
sanoq = 8
while sanoq!=0:
    royxat()
    q = int(input('Qatorni kiriting: '))
    u = int(input('Ustunni kiriting: '))
    if q==qa and u==us:
        r[q-1][u-1]='{*}'
        royxat()
        print('Bombaga tushdiz!!')
        break
    else:
        r[q - 1][u - 1] = '{🥳}'
        sanoq -= 1
    if sanoq == 0:
        print('Tabriklaymiz, Siz yutdingiz')
        r[q - 1][u - 1] = '{🥳}'
        royxat()
