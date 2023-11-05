# <p align="center">EXP 09 - Interface</p>

## Aim:
To Develop a small bank application by declaring deposit() and withdrawal() as abstract methods in the interface. Get the choice from the user whether to perform withdrawal or deposit operation. After the operation completes, display the balance amount.

## Algorithm:

Step 1: Create an interface.

Step 2: Create a child class.

Step 3: Declare 2 functions deposit() and withdrawal() as abstract methods in the interface.

Step 4: Create those 2 functions in the child class and perform respective operation.

Step 4: Use if-else conditional statement to get the choice from the user whether to perform withdrawal or deposit operation.

Step 5: After performing the functions display the remaining balance of the user.

## Program:
```
Developed by : Saravana Kumar S
Register no : 212221230088
````
```c#
using System;
public interface Bank
{
    void deposit(int amount);
    void withdrawal(int amount);
}
class program: Bank
{
    int balance = 10000;
    public void deposit(int amount)
    {
        balance += amount;
        Console.WriteLine("The balance is:"+balance);
    }
    public void withdrawal(int amount)
    {
        balance -= amount;
        Console.WriteLine("The balance is:" + balance);
    }
}
class program1
{
    public static void Main()
    {
        program obj1= new program();
        program obj2= new program();
        int a, amount;
        Console.WriteLine("choose whether deposit(1) or withdrawal(2):");
        a = Convert.ToInt32(Console.ReadLine());
        if (a == 1)
        {

            Console.WriteLine("Enter the amount:");
            amount = Convert.ToInt32(Console.ReadLine());
            obj1.deposit(amount);
        }
        else if (a == 2)
        {
            Console.WriteLine("Enter the amount:");
            amount = Convert.ToInt32(Console.ReadLine());
            obj2.withdrawal(amount);
        }
        else
        {
            Console.WriteLine("Enter a valid integer");
        }
    }
}
```


## Output:
### Deposit:
<img src="out1.png" width=350>

### Withdrawal:
<img src="out2.png" width=350>



## Result:
Thus, a C# program was developed for a bank application using interface.