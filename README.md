# سوالاتی که در مصاحبه فنی فرانت‌اند جواب کاملا درستی برای آن‌ها نداشتم
در طی یک سال گذشته در چند مصاحبه برای موقعیت شغلی فرانت‌اند دولوپر و سینیور فرانت‌اند دولوپر شرکت کردم و هرجا سوالی ازم پرسیدن که جواب درستی برای اون نداشتم از مصاحبه کننده خواستم تا زمانی به من بده تا بتونم اون سوال رو یک جا یادداشت کنم که بعدا بتونم بیشتر در موردش بخونم. 
در اینجا میخوام لیستی کامل از اون سوالات رو قرار بدم تا هم خودم بتونم بعدا بهش مراجعه کنم هم شاید برای بقیه مفید باشه.
طبیعتا بنظرم مهم نیست که اسم شرکتی که باهاشون مصاحبه کردم رو بنویسم و فقط سوال‌ها مهمه. البته بعضی هاشون هم بنظرم اصلا سوالات مهم و کاربردی ای نیستن ولی راستش اگه وقتی که داشتن این سوال ها رو ازم میپرسیدن من قبلش در موردش بیشتر میخوندن و راحتتر جواب میدم جدا از نتیجه مصاحبه بنظرم خودم هم حس بهتری داشتم از اینکه جواب سوال رو راحت و دقیق میدونم و صرفا یک چیزی که حدس میزنم رو با شک نمیگم.
در قدم اول این متن رو میخوام توی گیت‌هاب منتشر کنم تا اگه کسی هم تجربه مشابه‌ای داشت به این ریپازیتوری یک pull request بده و گزینه خودش رو اضافه کنه تا شاید بتونه منبع خوبی بشه برای یادگیری و مسلط شدن توی مصاحبه.

## سوالات مربوط به CSS
### تفاوت display: inline و display: inline-block
>  تفاوت عمده این است که inline-block اجازه می دهد تا عرض و ارتفاع را روی عنصر تنظیم کنید. همچنین با استفده از display: inline اندازه padding و margin رعایت نمی‌شود ولی با display: inline-block رعایت می‌شود.
>
 ### توضیح  flex-shirink
 > باعث میشه که بتونیم مشخص کنیم یک آیتم چقدر میتونه کوچیکتر بشه نسبت به بقیه آیتمها در فلکس. معمولا با flex-grow و flex-basis استفاده میشه
## سوالات مربوط به javascript
### توضیح primitive type
>  این تایپها که شامل string, boolean, number, null, undefind و symbol هستن به in-built data types هم معروف هستن. این تایپ ها مستقیم در مموری ذخیره میشن و مقدار آن ها بعد از تخصیص قابل تغییر نیستن. تایپهای non-primitive شامل object ها و functionها میشن که به اون ها reference data types هم گفته میشه. به صورت کلی pirmitive تایپ ها immutable هستن و non-primitiveها mutable هستن.
### عملکرد this در arrow function
> در arrow function ها this همیشه ثابت میماند و به نزدیکترین function پدر خود مربوط میشود. وقتی که یک فانکشن را صدا میزنم که  arrow function است در واقع this در اون کار نمیکند و bind صورت نمیگیرد.
### توضیح IIFE
> مخفف عبارت Immediately Invoked Function Expression است و به فانکشنهایی گفته میشه که دقیقا بعد از تعریف کردنشون اجرا میشن
### توضیح  Event Capturing
> در جاوااسکریپت اگر چندتا المنت داشته باشیم که زیر همدیگه قرار بگیرن و وقتی که بخواییم eventlistener بنویسم در حالت پیشفرض آرگومان eventlistener به حالت false قرار داره و با این حالت اون ایونت به حالت event bubbling کار میکند و مثلا اگر console.log برای کلیک روی همهی المنتها گذاتشته باشیم وقتی که روی المنت پایینی (فرزند) کلیک میکنیم به ترتیب اول متن مربوط به المنت فرزند چاپ میشود و سپس متن مربوط به المنت والد. اما اگر آرگومان سوم eventlistener رو true قرار دهیم حالت event capturing رو روشن میکنیم و متن خروجی console.log ترتیب برعکسی رو پیدا میکنه. به این دلیل اتفاق میوفتد چون در حالت capturing تمام ایونت ها از window به پایین از طریق dom به هدفی که در eventlistener گذاشته شده میرسن.
### توضیح function()()
> : وقتی که در یک فانکشن نیاز باشه که یک فانکشن دیگه return بشه میتونیم از این قائده استفاده کنیم که در فاکنشن دوم بتونیم پارامتری بفرستیم.
###  hoisting در global scope
> در بحث hoisting در جاوااسکریپت در واقع برخورد متفاوتی بین var و بین const, let هست. به عنوان مثال اگر اول a = 20 قرار داده باشید و بعد var a = 10 رو بنویسیم مشکلی ایجاد نمیشود و ۲۰ خروجی داده میشه ولی اگه اینکارو با const انجام بدیم به ارور TypeError: Assignment to constant variable. برمیخوریم و وقتی با let انجام بدیم به ارور ReferenceError: Cannot access 'a' before initialization برمیخوریم
> 
## سوالات مربوط به React
### تفاوت </> و <React.fragment> 
> در شرایطی که نیاز باشه مثلا key برای یک فرگمنت بذاریم باید از React.Fragment استفاده کنیم.
