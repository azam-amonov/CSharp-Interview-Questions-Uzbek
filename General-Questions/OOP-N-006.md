OOP: Vertual method nima?

Virtual metod doimiy implementatsiyaga ega bo'lishi kerak.Lekin,voris classdan qayta yozilishi mumkin, ammo majburiy emas.
U "override" kalit so'zi yordamida qayta yozilishi mumkin.

Namuna:
using System;

class BaseClass
{
    // Virtual metodni e'lon qilamiz
    public virtual void Display()
    {
        Console.WriteLine("Base class method is called");
    }
}

class DerivedClass : BaseClass
{
    // BaseClass dan qayta yozilgan Display metod
    public override void Display()
    {
        Console.WriteLine("Derived class method is called");
    }
}

//Program
class Program
{
    static void Main(string[] args)
    {
        // BaseClass obyektini yaratamiz
        BaseClass baseObj = new BaseClass();
        // Display metodini chaqiramiz
        baseObj.Display(); // "Base class method is called"

        // DerivedClass obyektini yaratamiz
        DerivedClass derivedObj = new DerivedClass();
        // Display metodini chaqiramiz
        derivedObj.Display(); // "Derived class method is called"
    }
}
