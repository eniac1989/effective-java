---
layout: post
title: ارجحیت for each به for
chapter: آیتم ۵۸
author: داوود حسینی
---


استفاده از forEach به for و استفاده از iterator باید ترجیح داده بشه. چون forEach خواناتر و کم خطاتر هست. یکی از دلایلش عدم نیاز به ایجاد متغیر اضافی هستش مثلا توی for متغیر index و در روش iterator متغیر iterator تعریف میشن.
دلیل دیگه احتمال اشتباه در کد نویسی هست، مثالی که تو صفحه 265 زده.
البته در سه جا هم نمیشه از forEach استفاده کرد:
۱- اگر میخواید از  container (مثلا لیستتون) حین iterate چیزی رو حذف کنید. البته متد removeIf توی جاوا 8 اضافه شده
۲- وقتی که میخواید چیزی رو replace کنید. 
۳- وقتی میخواید همزمان روی چندتا contrainer لوپ بزنید.
تو این موارد از for یا iterator میشه استفاده کرد
تمام کلاسهایی که interface iterable رو implement کردن رو میشه روشون از با forEach لوپ زد.
اگر میخواید ی کلاس درست کنید که شامل یه سری آیتم هست بهتره این interface رو implement کنید تا کسایی که از کلاس استفاده میکنند بتونن باهاش از forEach استفاده کنن.