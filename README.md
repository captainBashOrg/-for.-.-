print('Цикл for. Элементы списка. Полезные функции в цикле')



numbers =   [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15]
primes = []
not_primes = []
uno = []

for i in range ( len(numbers) ):
    #print (numbers[i])
    if numbers[i] == 1:
        uno.append (numbers[i])
        continue # единица не определилась
    else:
        sipm = 0
        for j in range ( 2, numbers[i]):
            #print ( i, j, numbers[i])
            if numbers[i] % j == 0:
                sipm = 1
                #break

        if sipm == 0:
            primes.append (numbers[i])
        else:
            not_primes.append (numbers[i])

if  (len (uno)) >0:
    print("единички", uno)
    
if  (len(primes)) > 0:
    print("простые", primes)

if  (len(not_primes)) > 0:
    print("Непростые", not_primes)







