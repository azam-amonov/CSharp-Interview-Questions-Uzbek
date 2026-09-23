## Savol ¹ 15 - GQ Umumiy savollar

---

### Delegat nima?

Delegat - bu methodga reference saqlaydigan o'zgaruvchi.Delegatlar funktsiya pointeri hisoblanadi va funksiya parametriga
funksiya berish uchun foydalaniladi.
Barcha delegatlar System.Delegate dan keladi. Delegat ham, u nazarda tutilgan method ham bir xil  bo'lishi mumkin.
Delegatlar event handling, LINQ queries, asinxron dasturlash va boshqalar uchun zarurdir.
Va, albatta, kodingizni sodda va ixcham qilish uchun delegatlardan foydalaniladi.


Misol:
```
using System;

public delegate void MyDelegate(string message);

class Program
{
    static void PrintMessage(string message)
    {
        Console.WriteLine("Message: " + message);
    }

    static void Main(string[] args)
    {
        MyDelegate delegateInstance = new MyDelegate(PrintMessage);

        delegateInstance("Hello, world!");
    }
}
```