## Savol ¹ 13 - GQ Umumiy savollar
---

## Jagged Array nima ?

C# dasturlash tilida Jagged Array - bu bir nechta massivlarni (array) yaratish uchun foydalaniladigan bir massiv turidir.
Bu massivning har bir elementi ikkinchi bir massivni (array) o'z ichiga oladi.Boshqa massivlardan (array) farqi ichki elementlar uzunligi(Length) 
harxil bo'lishi mumkin.


```
int[][] jaggedArray = new int[3][];
jaggedArray[0] = new int[] {1,2,3,4};
jaggedArray[1] = new int[] {1,2,3};
jaggedArray[2] = new int[] {1,2};
```