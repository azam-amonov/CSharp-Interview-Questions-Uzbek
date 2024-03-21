## Savol ¹ 13 - GQ Umumiy savollar

---

### Generic class nima?

C# dasturlash tilida  generic classlar asosan biror bir toifadagi qabul qilish uchun yaratilgan umumiy klaslardir.
Ular turli tipdagi ma'lumotlarni o'z ichiga olgan holda qo'llanilishi mumkin.

Generic class yaratish uchun burcahkli qavslar (<>) ishlatiladi

```
class Student<T>
{
	// block of code
}
```

Misol: Ikta tip (type) qabul qiluvchi class yaratamiz
```
public class Pair<TFirst, TSecond>
{
    public TFirst First { get; set; }
    public TSecond Second { get; set; }

    public Pair(TFirst first, TSecond second)
    {
        First = first;
        Second = second;
    }

    public void DisplayPair()
    {
        Console.WriteLine($"First: {First}, Second: {Second}");
    }
}
```

Endi ularga xarhil tipdagi qiymatlarni berib ishlatib ko'ramiz:
```
class Program
{
    static void Main(string[] args)
    {
        // String tipidagi Pair obyekti yaratish
        Pair<string, int> pair1 = new Pair<string, int>("Hello", 2024);
        pair1.DisplayPair();

        // output ("Hello",2024)

        // Integer tipidagi Pair obyekti yaratish
        Pair<int, double> pair2 = new Pair<int, double>(10, 5.5);
        pair2.DisplayPair();
        // output (10,5.5)
    }
}
```