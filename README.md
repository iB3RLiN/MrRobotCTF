# MrRobotCTF
##  Mr Robot CTF حل روم
<span dir="rtl"> مستوى الصعوبة: متوسط </span>
## https://tryhackme.com/room/mrrobot

### nmap اول شي نسوي فحص للمنافذ المفتوحة باداة 
![nmap](https://user-images.githubusercontent.com/73380139/189776233-b228f6b0-28a0-4c90-a762-7cb14669ec59.png)

### dirsearch وراح نحاول نخمن المسارات باستخدام
![dir](https://user-images.githubusercontent.com/73380139/189776590-9a6b0aa4-4595-4a13-8904-9d254761a23d.png)

### robots حصلنا بعض المسارات ولما نفحص 
<H3 dir="ltr">  "flag1" راح نحصل هذي الرسالة اللي لو تبعنا المسار اللي فيها راح نحصل العلم الاول</H3>

![robotsFile](https://user-images.githubusercontent.com/73380139/189777491-3d578088-9941-45cf-bba7-f1d29fd123b2.png)

<h3 dir="ltr">حصلناه</h3>

![firstFlag](https://user-images.githubusercontent.com/73380139/189780146-bdff1d57-7401-483c-a8f1-5e9a047156dd.png)

<h3 dir="ltr">ولما نرجع لنتائج تخمين المسارات راح نشوف صفحة فيها رسالة لكن المهم اننا لما نفحص العناصر راح نلقى</h3>

<h3 dir="ltr">encoding رسالة مخفية ومعمول لها </h3>

![inspctLic](https://user-images.githubusercontent.com/73380139/189781592-04adb6b3-bf9b-427f-aec5-78ee28318ca5.png)

<h3 dir="ltr">decoding نعمل</h3>

![base64](https://user-images.githubusercontent.com/73380139/189782432-12dc78fc-3921-4d28-bc43-6e8117567340.png)

<h3 dir="ltr"> حصلنا يوزر وباسورد</h3>

<h3 dir="ltr"> رح نجرب هذي البيانات على صفحة دخول الادمن </h3>

![loginByWP](https://user-images.githubusercontent.com/73380139/189783855-3efd4b18-4f9f-4323-830d-5eb8afdb25f2.png)

<h3 dir="ltr"> دخلنا وبعد جولة في الداش بورد راح نلقى لوحة تسمح لنا نعدل اكواد الموقع</h3>
<h3 dir="ltr"> php لاحظ وجود قالب 404 مكتوب بلغة </h3>
<h3 dir="ltr"> php-reverse-shell راح نستغلة ونرفع  </h3>

![editThemes](https://user-images.githubusercontent.com/73380139/189784025-556585fa-d5b4-4a9f-a12d-2b68483e4a83.png)


<h3 dir="ltr">netcat نفتح اتصال</h3>
<h3 dir="ltr"> ونفعل الشيل </h3>

![netcat](https://user-images.githubusercontent.com/73380139/189784460-c6fa138a-eaec-442a-bdf9-2f618c4b4a72.png)

<h3 dir="ltr"> حصلنا العلم لكن ما معنا صلاحية نقراء الملف لكن فيه ملف لليوزر مع هاش الباسورد</h3>
<h3 dir="ltr"> ناخذ الهاش ونروح للشيخ جوجل</h3>
<h3 dir="ltr"> حصلنا الباسورد</h3>

![MD5Crack](https://user-images.githubusercontent.com/73380139/189785045-eb8cfec8-4f6d-4d7f-8fac-a1b4fe247a74.png)

<h3 dir="ltr"> لكن ما راح نحتاجة لان لازم صلاحية روت للعلم الثالث فراح نختصر</h3>
<h3 dir="ltr"></h3>

![find](https://user-images.githubusercontent.com/73380139/189786166-9c589a94-3150-4e2b-b59c-e046b46c3e83.png)

<h3 dir="ltr"> nmap من خلال </h3>
<h3 dir="ltr"> راح ناخذ شيل بصلاحيات روت </h3>
<h3 dir="ltr"> وهذا العلم الثاني </h3>

![privRootAndFlag2](https://user-images.githubusercontent.com/73380139/189785815-7a1237ce-13e6-4508-a94d-bf1355e340cd.png)

<h3 dir="ltr">وهذا العلم الثالث في مسار الروت </h3>

![flag3](https://user-images.githubusercontent.com/73380139/189785633-ea24e3d1-2f97-40b2-80e5-eada841e4fa5.png)

<h3 dir="ltr"> المراجع </h3>

https://gtfobins.github.io/gtfobins/nmap/

<https://github.com/pentestmonkey/php-reverse-shell>

<https://gtfobins.github.io/>

https://www.youtube.com/watch?v=BQ4xeeNAbaw&ab_channel=DarkSec


