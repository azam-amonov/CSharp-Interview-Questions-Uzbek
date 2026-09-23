__OOP__  Obyetkga yo'naltirilgan dasturlash, bu dasturni bir-birini o'zaro aloqada bo'lgan obyektlar to'plami sifatida qaraydi. Bundas biz dasturda shunchaki buyruqlar to'plami emas balki aniq _(yoki abstract)_  modellarga qaraymiz.

**OOP dasturlash to'rtta asosiy ustundan iborat:**
- **[[Encapsulation]]**  -- _Inkapsulatsia_ obyetkta bog'liq bo'lgan ma'lumot va methodlarni tashqi dunyodan yashirish.
- **[[Inheritance]]** --  _Vorislik_ ota (base) klassda mavjud bo'lgan xususiyatlarni bola (voris) klassda ham mavjud bo'lishi.
- **[[Polymorphism]]**  --  _Polimarfizm_ turli obyetlarnin bir xil turdachi vazfani turlicha bajarishi 
- **[[Abstraction]]**  -- _Abstraksiya_ yoki _mavhumlik_ obyetning faqatgina asosiy vazifalarni ko'rsatib qolgan ichkarida bajarilayotgan vazifalarini yashirish.

**Klass va obekt tushunchasi:** 
Bu ikki tushunchani tushunish uchun uy va chizma  misolida ko'rish mumkin.
- __Klass__ ([[Class]]) bu chizma. Chizmada uyning tuzilishi, balandigi unnda nimalar bo'lishi va qanday xususiyatlar b'lishi kerakligini bilib olamiz. 
- __Ob'ekt__ ([[Object]]) bu tayyor uy. Bu aniq bir eszimlpayar, unda klassda ko'rsatilgan barcha talablar mavjud bo'ladi. 

__.NET-da qaday ishlaydi (under the hood)__
C# da kod yozilganda quyidagilar sodir bo'ladi:
1. __Class__ yig'ilgan _([[build]])_  bo'lgan holatda  _[[Metadata]]_ ko'rinishida saqlanadi  ([[DLL]] yoki [[EXE]]). Qachonki dastur ishga tushda [[CLR (Common language runtime)]] ma'lumotlarni aynan metadatadan olaib ishlatadi.
2. __Ob'ekt__ esa  [[new]] keyword ishlatilganda yaratiladi. Shu vaqtda CLR ([[Managed heap]]) dan ob'ekt uchun joy ajratadi.

#oop
#junToMid-8 
