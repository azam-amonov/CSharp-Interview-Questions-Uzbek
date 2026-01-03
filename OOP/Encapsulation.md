Inkapsulatsiya bu servis yoki metoddagi user uchun ochiq bo'lishi kerak bo'lmagan va faqat [[Service Class]]  ichidagi mavjud bo'lgan [[public]]  metodlar orqali murojjat qilish imkonini berish. Bunda qiymat user to'gridan to'g'ri qiymatga o'zgatirsh imkonini cheklaydi va ma'lumot himoyalanadi. Misol tariqasida bankomatning ishlashini keltirish mumkin!

**Simple Explanation:**
*Inkapsulatsiya* - bu bankomat korpusi u ichgi ma'lumotlarni tashqi dunyodan himoyalab turadi, bankomat ichidagi mexanizimlar, naqt pullar va h.k. User (foydalanuvchi) uchun eda, ichgi [[private]] [[field]]-larga murojaat qila olish uchun tashqa public [[method]]-lar taqdim qilinadi, bular tugmalar, ekran va plastik karta kiritish uchun joy. Bunda ichgi jarayonlar esa [[Abstract]] hisoblanadi. 

[[Metadata]] va [[CLR (Common language runtime)]] ishlash mexanizmi:
CLR [[private]] bo'lgan bo'lgan o'zgaruvchilarga tashqaridan hechkim o'zgartirib qo'ymasligni ta'minlaydi. Bu bizning bankomatdagi, pullar va mezanizimlar.

Metadata esa [[public]] #keyWord bilan belginlangan qolgan servislar undan foydalanish mumkin ekanini xabar beradi.

Code example:

```C#
public class BankAccount
{
	// Inkapsulatsia qilingan filed - tashqi dunyodan yashirilgan! 
	private decimal _balance;
	
	public void Deposit(decimal amount)
	{
		if(amount > 0)
		{
			_balance += amount;
		}
	}
}
```



#oop #junToMid-8 