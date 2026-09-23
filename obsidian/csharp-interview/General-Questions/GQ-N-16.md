## Savol ¹ 16 - GQ Umumiy savollar

---

### Delegate turlari

Delegate turlari:

1.Single Delegate - Faqatgina bitta method chaqira oladigan delegate
2.Multicast Delegate - Ko'plab kiritish parametrlari va qaytarish turlari bilan
ushbu metodlarni aks ettirish imkonini beradi.
3.Generic Delegate - bu delegate holatni aniqlashni talab qilmaydi.
Va u 3 hil ko'rinishda bo'ladi:Action,Func,Predicate

Action - Yuqoridagi delegatlar va event misolida biz Action kalit so'zidan foydalanib delegat va event
ta'rifini almashtirishimiz mumkin. Action delegate argumentlar bo'yicha chaqirilishi mumkin bo'lgan,
ammo natijani qaytarmaydigan usulni belgilaydi

```
using System;

class Program
{
    static void Main()
    {
        // Declare an Action delegate that takes no parameters and returns void
        Action sayHello = () => Console.WriteLine("Hello!");

        // Declare an Action delegate that takes an integer parameter and returns void
        Action<int> printNumber = (number) => Console.WriteLine($"The number is: {number}");

        // Declare an Action delegate that takes two string parameters and returns void
        Action<string, string> concatenateStrings = (str1, str2) =>
        {
            string result = str1 + str2;
            Console.WriteLine($"Concatenated string: {result}");
        };

        // Invoke the delegates
        sayHello(); // Output: Hello!
        printNumber(10); // Output: The number is: 10
        concatenateStrings("Hello", "World"); // Output: Concatenated string: HelloWorld
    }
}
```
Func - Func delegati argumentlar bo'yicha chaqirilishi mumkin bo'lgan usulni belgilaydi va natijani qaytaradi.
```
using System;

class Program
{
    static void Main()
    {
        // Declare a Func delegate that takes no parameters and returns an integer
        Func<int> getRandomNumber = () => new Random().Next();

        // Declare a Func delegate that takes two integers and returns their sum
        Func<int, int, int> addNumbers = (x, y) => x + y;

        // Declare a Func delegate that takes a string and returns its length
        Func<string, int> getStringLength = (str) => str.Length;

        // Invoke the delegates
        int randomNumber = getRandomNumber(); // Get a random number
        int sum = addNumbers(5, 10); // Get the sum of two numbers
        int length = getStringLength("Hello, world!"); // Get the length of the string

        Console.WriteLine($"Random Number: {randomNumber}");
        Console.WriteLine($"Sum of Numbers: {sum}");
        Console.WriteLine($"Length of String: {length}");
    }
}
```
Predicate - argumentlar bo'yicha chaqirilishi mumkin bo'lgan methodni belgilaydi va har doim boolean type qaytaradi.

```
using System;
using System.Collections.Generic;

class Program
{
    static void Main()
    {
        // Define a Predicate delegate to check if a string starts with the letter 'A'
        Predicate<string> startsWithA = (str) => str.StartsWith("A", StringComparison.OrdinalIgnoreCase);

        // Create a list of strings
        List<string> names = new List<string> { "Alice", "Bob", "Anna", "David", "Alex" };

        // Filter the list to get only names starting with 'A'
        List<string> namesStartingWithA = names.FindAll(startsWithA);

        // Print the names starting with 'A'
        Console.WriteLine("Names starting with 'A':");
        foreach (var name in namesStartingWithA)
        {
            Console.WriteLine(name);
        }
    }
}
```