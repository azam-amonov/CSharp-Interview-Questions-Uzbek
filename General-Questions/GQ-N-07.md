## Savol N_7 - GQ Umumiy savollar

---

### Generic lar nima ?

---

Generic class, method, struct yoki interface biror code da aniq bir belgilangan type bolmasligini 
aniqlash uchun ishlatiladi.


```C#
public class GenericClass<T>
{
public void SomeMethod(T input) { }
}
```

Bu bizga bitta funksionallikni yozish imkonini beradi va shuningdek koplab tiplar uchun ham foydalanishimiz mumkin.
Aniq bir data type foydalanish o'rniga biz generic type parametrni ishlatishimiz mumkin, bu parametr odatda T bilan belgilanadi. 