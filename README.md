def fiboouter(n):
    prevNum = 0
    currentNum = 1
    for i in range(1,n):
        prevPrevNum = prevNum
        prevNum = currentNum
        currentNum = prevNum + prevPrevNum
    return currentNum
def fiberecur(n):
    if n == 0:
        return 0
    elif(n==1):    
        return 1
    else :
        return fiberecur(n-1)+fiberecur(n-2)
if __name__ == "__main__":
    num = int(input("Enter a number"))
    print(f"Using recursions value of fib({num}) is {fiberecur(num)}")
    print(f"Using recursions value of fib({num}) is {fiboouter(num)}")
