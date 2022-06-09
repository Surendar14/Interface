# Interface

## Aim:
   To write a C# program using interface concept

## Algorithm:


## Program:
~~~
using System;
public interface Bank
{
    void deposit();
    void withdrawal();
}

public class Example : Bank
{
    int amount, ch, balance = 5000;
    public Example()
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

public class Hello
{
    public static void Main()
    {
        Example c = new Example();
        c.deposit();
        c.withdrawal();
    }
}
~~~

## Output:

![Screenshot (92)](https://user-images.githubusercontent.com/75235759/172882157-32f05399-87e9-4790-9ab7-3c27e5f9c081.png)



## Result:
Thus, C# program using interface concept was developed.
