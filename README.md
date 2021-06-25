# CNT310_python

def howManyMonths(start, rate, spending, target):
    # write your code here
    balance = start
    months = 0
    while (balance >=0 and balance < target and months < 1000):
        balance = balance * (1+rate)-spending
        months += 1
        
    if balance >= target:
        return months
    else:
        return -1
# any test cases you'd like to have
