What is a Destructor in C#?

Destructor xotirani tozalashda va manbalarni bo'shatishda foydalaniladi.Lekin, 
C# da bu vazifani o'zining garbage collectori bajaradi.
System. GC.Collect() - bu orqali biz tozalash uchun garbage collectorni ichki tomondan chaqiramiz.
Biroq,ba'zan destructorlarni o'zimiz(ruchnoy) implentatsiya qilishimiz muhimdir.

Namuna:
~Car()
{
  Console.writeline(“....”);
}