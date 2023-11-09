# EX 09 Interface

## Aim:

To write a C# program using interface concept.

## Algorithm:
Step 1: Create an interface.

Step 2: Create a child class.

Step 3: Declare 2 functions deposit() and withdrawal() as abstract methods in the interface.

Step 4: Create those 2 functions in the child class and perform respective operation.

Step 5: Use while loop and and switch case to Get the choice from the user whether to perform withdrawal or deposit operation.

Step 6: After performing the functions display the remaining balance of the use.


## Program:
```
NAME : KAVIYA SHREE S
Reg.No: 212222110018

using System;
public interface Bank
{
    void deposit();
    void withdrawal();
}
class Program : Bank
{

    int amount, ch, balance = 5000;
    public Program()
    {
        Console.WriteLine("1.Deposit\n2.Withdrawal");
        ch = Convert.ToInt32(Console.ReadLine());
        if (ch == 1)
        {
            deposit();
        }
        else
        {
            withdrawal();
        }

    }
    public void withdrawal()
    {
        int amount = Convert.ToInt32(Console.ReadLine());
        balance -= amount;
        Console.WriteLine(balance);
    }
    public void deposit()
    {
        int amount = Convert.ToInt32(Console.ReadLine());
        balance += amount;
        Console.WriteLine(balance);
    }

}
class example
{
    public static void Main()
    {
        Program c = new Program();
        c.deposit();
        c.withdrawal();
    }
}
```

## Output:
<img width="866" alt="image" src="https://github.com/kaviya2839/Interface/assets/120553351/e8957b3d-d1fb-48c4-a2d1-76bd09f922ad">


## Result:
Thus the C# program using interface concept has been implemented successfully.
