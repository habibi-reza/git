## git - Jadi
<style>
.rtl {
direction: rtl;
float: right;
text-align: right;
font-family: IRANSans;
}
</style>
```shell
$ git init
```
<span class="rtl">گیت را در دایرکتوری جاری اجرا می‌کند.</span><br />

```shell
$ git add .
$ git commit -m 'SOME Messages ...'
```
<span class="rtl">بعد از ساخت گیت برای ایجاد برنچ master.</span><br />

```shell
$ git status
```
<span class="rtl">اتفاقات و تغییرات را در این دایرکتوری نشان می‌دهد.</span><br />

```shell
$ git add FILE_NAME
```
<span class="rtl">اگر بخواهیم فایل مشخصی را به stage اضافه کنیم.</span><br />

```shell
$ git add -A
```
<span class="rtl">اگر بخواهیم تمام فایل‌های دایرکتوری را به stage اضافه نماییم.</span><br />

```shell
$ git commit -m 'SOME Messages ...'
```
<span class="rtl">فایل‌هایی که بخواهیم به stage اضافه نماییم را باید commit کنیم با یک message.</span><br />

```shell
$ git log
```
<span class="rtl">تمام پیام‌هایی که در هنگام commit کردن وارد کردیم در اینجا نمایش داده می‌شود.</span><br />

```shell
$ git diff HEAD
```
<span class="rtl">آخرین تغییراتی که در فایل‌ها انجام شده است را نسبت به حالت قبلی (قبل از commit کردن) نشان می‌دهد.</span><br /><span class="rtl">(HEAD همان commit آخر ما هست.)</span><br />

```shell
$ git diff --staged
```
<span class="rtl">آخرین تغییرات فایل‌های روی stage را نشان می‌دهد.</span><br />

```shell
$ git reset FILE_NAME
```
<span class="rtl">اگر بخواهیم فایل خاصی را از stage پاک کنیم که commit نشود.</span><br />

```shell
$ git checkout -- FILE_NAME
```
<span class="rtl">اگر بخواهیم آخرین تغییرات فایلی خاص را به ذخیره قبلی (آخرین commit) بازگردانیم.</span><br />

```shell
$ git branch
```
<span class="rtl">نشان می‌دهد چند شاخه در گیت جاری داریم.</span><br />

```shell
$ git branch NAME_OF_BRANCH
```
<span class="rtl">ایجاد شاخه جدید در گیت جاری.</span><br />

```shell
$ git checkout NAME_OF_BRANCH
```
<span class="rtl">جابجایی بین شاخه‌ها.</span><br />

```shell
$ git merge NAME_OF_BRANCH
```
<span class="rtl">در صورتی که بخواهیم تغییرات انجام شده در برنچ مشخصی را با گیت مستر ادغام نماییم.</span><br />

```shell
$ git rm FILE_NAME
```
<span class="rtl">برای پاک کردن فایل مشخصی هم از گیت و هم از فایل سیستم. </span><br />

```shell
$ git branch -d NAME_OF_BRANCH
```
<span class="rtl">حذف شاخه مشخصی در گیت جاری.</span><br />

```shell
$ git clone URL_ADDRESS
```
<span class="rtl">برای اضافه کردن یک دایرکتوری گیت مثلا از روی گیت هاب بر روی کامپیوتر شما.</span><br />

```shell
$ git push origin master
```
<span class="rtl">توجه: origin همان جایی که پروژه گیت را در اینترنت داریم.</span><br />
<span class="rtl">تغییرات master را بر روی origin می‌نویسد. (push می‌کند)</span><br />
<span class="rtl">نیازی به اتصال با نام کاربری و رمز عبور دارد.</span><br />

```shell
$ git pull origin master
```
<span class="rtl">تغییرات origin را بر روی master می‌نویسد. (pull می‌کند) </span><br />
<span class="rtl">نیازی به اتصال با نام کاربری و رمز عبور ندارد.</span><br />

```shell
$ git (pull or push) -u origin master
```
<span class="rtl">تغییرات origin را بر روی master می‌نویسد (pull می‌کند) یا تغییرات master را بر روی origin می‌نویسد. (push می‌کند)</span><br /><span class="rtl">دفعه بعد دیگر نیازی نیست origin و master را بنویسیم. فقط کافیست تایپ کنیم:</span><br /><br />

```shell
$ git (pull or push)
```
<br />
```shell
$ git remote add origin URL_ADDRESS
```
<span class="rtl">یک آدرس اینترنتی را به عنوان برنچ ریموت اضافه می‌کند و نام آن را origin می‌گذارد.</span><br />

```shell
$ git show COMMIT_NUMBER
```
<span class="rtl">نمایش تغییرات بر اساس شماره ‌commit که می‌گوید که در شماره commit مورد نظر چه اتفاقی افتاده است.</span><br />

```shell
$ git tag
```
<span class="rtl">تگ‌های زده شده تا کنون را نشان می‌دهد.</span><br />

```shell
$ git tag -a SOME_TEXT COMMIT_NUMBER -m 'SOME_MESSAGES...'
```
<span class="rtl">a- مخفف annotate (یه نوشته‌ای بذارم کنارش!) و با یک پیام متناسب (با توجه به شماره commit درج شده).</span><br />

```shell
$ git tag -a SOME_TEXT -m 'SOME_MESSAGES...'
```
<span class="rtl">a- مخفف annotate (یه نوشته‌ای بذارم کنارش!) و با یک پیام متناسب (آخرین commit زده شده).</span><br />

```shell
$ git tag -l "SOME_TEXT"
```
<span class="rtl">l- لیست تمام تگ‌هایی که در داخل دابل کوتیشن درخواست می‌کنیم را به ما می‌دهد. مثال:</span><br />

```shell
$ git tag -l "V*"
```
<span class="rtl">لیست تمام تگ‌هایی که با V شروع می‌شود را به ما می‌دهد.</span><br />

```shell
$ git show SOME_TAG
```
<span class="rtl">نام ایجاد کننده، تاریخ ایجاد، تغییرات نسبت به commitهای قبلی و … بر اساس نام تگ را نمایش می‌دهد.</span><br />

```shell
$ git push origin SOME_TAG
```
<span class="rtl">تگ مشخصی را بر روی origin می‌نویسد. (push می‌کند)</span><br />

```shell
$ git push origin --tags
```
<span class="rtl">تمام تگ‌ها را بر روی origin می‌نویسد. (push می‌کند)</span><br />

```shell
$ git checkout SOME_TAG
```
<span class="rtl">جابجایی بین تگ‌های مشخص.</span><br />

```shell
$ git checkout -b <new-branch-name>
```
<span class="rtl">برای اینکه بتوان تغییراتی که روی تگ‌های مشخص (مثلا ورژن) قابل اعمال باشد باید شاخه (branch) جدیدی برای این کار ساخته شود.</span><br /><br />

```shell
$ gpg --list-keys 
```
<span class="rtl">لیست کلیدهای موجود در سیستم را نشان می‌دهد.</span><br />

```shell
$ gpg --gen-key 
```
<span class="rtl">برای تولید کلید عمومی و خصوصی جدید.</span><br />

```shell
$ git config --global user.name
```
<span class="rtl">نمایش نام کاربری عمومی.</span><br />

```shell
$ git config --global user.email
```
<span class="rtl">نمایش ایمیل کاربر عمومی.</span><br />

```shell
$ git config --global user.signingkey
```
<span class="rtl">نمایش کلید امضا عمومی.</span><br />

```shell
$ gpg --list-secret-keys --keyid-format LONG
```
<span class="rtl">نمایش کلید ایجاد شده.</span><br />

```shell
$ git config --global user.signingkey 26EB79AE89CD20D0
```
<span class="rtl">اعمال کلید ایجاد شده توسط gpg.</span><br />

```shell
$ git tag -s SOME_TEXT -m 'SOME_MESSAGES...'
```
<span class="rtl">s- مخفف sign (امضاش کن!) و با یک پیام متناسب (آخرین commit زده شده).</span><br />

```shell
$ git show SOME_TAG_SIGNED
```
<span class="rtl">نام ایجاد کننده، تاریخ ایجاد، امضای ایجاد کننده، تغییرات نسبت به commitهای قبلی و … بر اساس نام تگ را نمایش می‌دهد.</span><br /><br />

```shell
$ git tag -v SOME_TAG_SIGNED
```
<span class="rtl">برای اطمینان از امضای تگی مشخص از این دستور استفاده می‌شود.</span><br />

```shell
$ git commit -S -m 'SOME Messages ...'
```
<span class="rtl">با اضافه کردن S- این commit امضا می‌شود.</span><br />

```shell
$ git help COMMAND 
```
<span class="rtl">برای دیدن راهنمای هر دستور به صورت بالا عمل نمایید.</span><br />

```shell
$ git blame NAME_OF_FILE -L{NUMBER_OF_LINE} 
```
<span class="rtl">برای مشاهده تغییرات و مسئول ایجاد (نفری که تغییرات را انجام داده است) آن در یک فایل (و به طور در دقیق‌تر با سوئیچ L- در یک خط مشخص یا در چندین خط) از دستور بالا استفاده می‌شود. به طور مثال:</span><br /><br />

```shell
$ git blame NAME_OF_FILE -L8
```
<span class="rtl">مشاهده تغییرات و مسئول ایجاد آن در فایلی مشخص و در خط 8</span><br />

```shell
$ git blame NAME_OF_FILE -L8,10 
```
<span class="rtl">مشاهده تغییرات و مسئول ایجاد آن در فایلی مشخص و در خط 8 تا 10</span><br />

```shell
$ git bisect start
binary search commit 
```
<span class="rtl">به منظور خطایابی در کد زده شده از این دستور استفاده می‌‌شود. در ابتدای امر باید در بالاترین سطح (دایرکتوری) باشید. با اعمال دستور فوق می‌توانید عملیات را شروع نمایید.</span><br /><br />

```shell
$ git bisect bad COMMIT_NUMBER
```
<span class="rtl">با دستور فوق اعلام می‌کنید که وضعیت در اینجایی که هستید بد است (البته اگر در ادامه دستور فوق commit number ای هم زده شود نشان می‌دهد که وضعیت در آن commit بد است)</span><br /><br />

```shell
$ git bisect good COMMIT_NUMBER
```
<span class="rtl">در ادامه‌ی دستور فوق،‌ گیت برای شما در commit های قبلی جستجو کرده و با مقایسه تغییرات به شما پیشنهاد می‌دهد که مثلاً در commit های قبلی فلان commit خوب است؟ که اگر با آن موافق بودید (یعنی باگ ایجاد شده برطرف می‌شد!) می‌توانید از دستور بالا استفاده فرمایید.</span><br />