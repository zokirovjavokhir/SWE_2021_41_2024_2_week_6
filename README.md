# SWE_2021_41_2024_2_week_6

## Week 4 Assignment
https://github.com/zokirovjavokhir/SWE_2021_41_2024_2_week_4  
```bash
def isHappy(n):
    square = set()
    while n != 1 and n not in square:
        square.add(n)
        n = sum(int(digit) ** 2 for digit in str(n))
    return n == 1

n = int(input("Enter a number: "))
print(isHappy(0))
```  
The function **isHappy(n)** that checks whether a given number n is a happy number. A happy number is defined as a number that eventually reaches 1 when replaced by the sum of the squares of its digits. If it loops endlessly without reaching 1, it is not a happy number.

---
## Week 5 Assignment
```bash
docker exec ossp-container cat /etc/os-release
```
This code retrieves and displays the contents of the **/etc/os-release** file from the **ossp-container.**



```bash
docker exec ossp-container git —version
```
This command is used to check the version of **Git** installed inside the running Docker container named **ossp-container.**

```bash
docker exec ossp-container python -—version
```
This command is used to check the version of **Python** installed inside the running Docker container named **ossp-container.**

```bash
docker inspect --format="{{ HostConfig Binds }}" ossp-container
```
This code will output a list of volume bindings for the **ossp-container.** These bindings represent the directories or files on the host machine that are mounted into the container.
