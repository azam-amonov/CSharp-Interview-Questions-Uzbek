## Savol N_5 - GQ Umumiy savollar

---

### Interface va abstract class o'rtasida nima farq bor?

---

Abstract class ni ishlatishdan maqsad bu - Bir nechta olingan(Multiple derived) class larni ulashadigan
base class ning umumiy kengaytmasi(definition) taminlash hisoblanadi. Shuning uchunn interface va abstract
class deyarlik bir xil bo'lgan C# 8 dan oldin, hozirda bular o'rtasidagi asosiy farq bu interface class method yoki 
property uchun default implementatsiya belgilay olishida edi. C# 8 dan boshlab interface lar property va
method uchun default implementatsiyani amalga oshira oladi.

Yana boshqa farq esa, bitta abstract class bir dona inheritance ni amalga oshira oladi holos, usha bitta class
esa koplab interface lardan implementatsiya ola oladi.
