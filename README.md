# Git_Document
Document about Git learning
 
<p align="center">
 <img alt="Git-Logo" src="image/git.png">
</p>

<p dir=rtl>
  گیت، یک سیستم کنترل نسخه منبع آزاد و رایگان است که در ابتدا Linus Torvalds  در سال 2005 ایجاد کرد.
</p>
<p dir=rtl>
گیت توزیع می شود: به این معنی که هر توسعه دهنده، تاریخچه ی کامل مخزن کد خود را به صورت محلی دارد. این باعث می شود که Clone اولیه مخزن کندتر شود، اما عملیات بعدی مانند Commit, blame, diff, Merge و Log سریع تر انجام می شود.
 </p>
 <p dir=rtl>
وی‌سی‌اس (سیستم کنترل نسخه) Version Control System یا به اختصار VCS به ابزاری اطلاق می‌گردد که این امکان را در اختیارمان می‌گذارد تا دست به مدیریت نسخه‌‌بندی یک پروژه بزنیم.
  </p>


<h3 dir=rtl>
  اصطلاحات رایج در Git:
</h3>

<table>
  <tr>
    <th><b><i>اصطلاح</i></b></th>
    <th><b><i>توضیحات</i></b></th>
  </tr>
  <tr>
    <td><b>Repo</b></td>
    <td dir=rtl>این اصطلاح برگرفته از واژه Repository به معنی «مخزن» یا «منبع» است</td>
  </tr>
  <tr>
    <td><b>Clone</b></td>
    <td dir=rtl> چنانچه بخواهیم یک ریپازیتوری آنلاین را دریافت نموده و روی سیستم لوکال خود شروع به کار روی آن نماییم، نیاز است تا ابتدا کل پروژه را دانلود نماییم که به این کار کلون کردن گفته می‌شود. </td>
  </tr>
  <tr>
    <td><b>Stage</b></td>
    <td dir=rtl>در سیستم گیت اِستِیج کردن پروژه بدان معنا است که قصد داریم تا تغییراتی که در سورس‌کد پروژه خود اِعمال نموده‌ایم را آماده سازیم تا در تاریخچه تغییرات گیت ذخیره گردند. </br>به عبارت دیگر، با اِستِیج کردن پروژه به سیستم می‌فهمانیم که قصد داریم کدام فایل‌ها و فولدرها به عنوان یک نسخهٔ جدید از پروژه ذخیره گردند</td>
  </tr>
  <tr>
    <td><b>Commit</b></td>
    <td dir=rtl> اساساً برای آن که بتوانیم دست به نسخه‌بندی ریپازیتوری خود بزنیم، نیاز است تا در صورت اِعمال هر گونه تغییری آن را به اصطلاح کامیت نماییم. معنی لغوی این اصطلاح «مرتکب شدن» است اما در فضای سیستم‌های کنترل نسخه می‌توان معادلی همچون «ذخیره کردن تغییرات» برایش در نظر گرفت </td>
  </tr>
  <tr>
    <td><b>Push</b></td>
    <td dir=rtl>چنانچه بخواهیم علاوه بر داشتن یک ریپازیتوری به صورت آفلاین آن را در سرویس‌های مطرحی همچون گیت‌هاب یا گیت‌لَب نیز ذخیره‌ سازیم،‌ نیاز به ارسال کلیهٔ‌ فایل‌ها و فولدرهای پروژه روی یک ریپازیتوری آنلاین داریم که به این فرآیند «پوش» گفته می‌شود.</td>
  </tr>
  <tr>
    <td><b>Pull</b></td>
    <td dir=rtl>  در صورتی که بخواهیم تغییراتی که سایر دولوپرها روی یک ریپازیتوری آنلاین همچون گیت‌هاب انجام داده‌اند را دریافت کنیم، نیاز به دریافت تغییرات داریم که به این فرآیند «پول» گفته می‌شود. </td>
  </tr>
    <tr>
    <td><b>Branch</b></td>
    <td dir=rtl> هر ریپازیتوری یک شاخهٔ اصلی دارد که تحت عنوان Master شناخته می‌شود اما این در حالی است که تک‌تک اعضای تیم می‌توانند شاخه‌هایی با نام‌هایی کاملاً دلخواه از شاخهٔ اصلی جدا کرده و شروع به کار روی آن‌ها کنند و در نهایت دولوپر اصلی پروژه می‌تواند شاخه‌های فرعی را، در صورت تأیید شدن، با شاخهٔ اصلی ادغام نماید. </td>
  </tr>
    </tr>
    <tr>
    <td><b>Merge</b></td>
    <td dir=rtl>  همان‌طور که پیش از این توضیح داده شد، چنانچه در یک ریپازیتوی علاوه بر شاخهٔ اصلی شروع به ساخت یک سری شاخهٔ‌ فرعی نماییم،‌ در نهایت نیاز است تا کلیهٔ شاخه‌‌های فرعی با شاخهٔ به اصطلاح مَستر ادغام شوند که به این پروسه «مِرج» گفته می‌شود. </td>
  </tr>
  <tr>
    <td><b>Origin</b></td>
    <td dir=rtl> یک اسمی است که وقتی از یک سایت مثلا github یک چیزی یا پروژه ای را clone می کنیم معمولا اسمش را می گذارند origin </td>
  </tr>
    <tr>
    <td><b>Untracked file</b></td>
    <td dir=rtl> فایل هایی که هنوز stage نشده اند و گیت هیچ history از آن نداره </td>
  </tr>
</table>

</br>
<h3 dir=rtl>
  دستورات رایج در Git:
</h3>

<table>
  <tr>
    <th><b><i>دستورات</i></b></th>
    <th><b><i>توضیحات</i></b></th>
  </tr>
  <tr>
    <td><b>git init</b></td>
    <td dir=rtl> کامند init برگرفته از کلمه Initialize به معنی «شروع کردن» است. پس از اجرای موفقیت‌آمیز این کامند،‌ پوشه‌ای تحت عنوان git. ساخته می‌شود </td>
  </tr>
  <tr>
    <td><b>git status</b></td>
    <td dir=rtl> برای اطلاع از وضعیت ریپو  </td>
  </tr>
  <tr>
    <td><b>git add {اسم فایل} </br> git add -A </br> git add '*.html'</b></td>
    <td dir=rtl> کلیه کامندهای گیت با دستور git آغاز می‌شوند و برای مرحله اِستیج از دستور add استفاده کرده و فایلی که قصد داریم در هیستوری ذخیره گردد را مینویسیم </td>
  </tr>
   <tr>
    <td><b>git commit -m 'یک توضیح مناسب'</b></td>
    <td dir=rtl> با استفاده از دستور add تغییرات آمادهٔ ذخیره‌سازی شده‌اند اما این کار هنوز صورت نگرفته است که برای این منظور، با استفاده از دستور commit این کار انجام میدهیم </br> می توان از آپشن a- هم استفاده کرد تا فرایند اضافه شدن به استیج همزمان در اینجا انجام شود</td>
  </tr>
  <tr>
    <td><b>git log </br> git log --oneline</b></td>
    <td dir=rtl>برای این که به لیستی کامیت‌هایی که تاکنون انجام داده‌ایم دست یابیم </br> چنانچه تعداد کامیت‌ها زیاد بوده و بخواهیم گزارشی خلاصه دریافت کنیم، می‌توانیم از دستور oneline استفاده نماییم. </br> هر کامیت نیز از یک کد هَش به منظور شناسایی برخوردار است </td>
  </tr>
  <tr>
    <td><b>git diff HEAD </br> git diff --staged</b></td>
    <td dir=rtl> برای مشاهده اینکه در حال حاضر چه تغییراتی صورت گرفته است </td>
  </tr>
      <tr>
    <td><b>git reset {اسم فایل} </br> git reset {بخشی از کد هش کامیت} </br></b></td>
    <td dir=rtl> برای خارج کردن یک فایل از حالت استیج </br> برای رفتن به یک کامیت خاص </br> در این حالت می توان از آپشن --hard نیز استفاده کرد </td>
  </tr>
  </tr>
      <tr>
    <td><b>git checkout -- {اسم فایل} </b></td>
    <td dir=rtl> برای در نظر نگرفتن تغییرات انجام شده بر روی فایل </td>
  </tr>
  <tr>
    <td><b></br>git branch </br> git branch {اسم برای شاخه} </br> git branch -d {اسم شاخه} </br> git checkout {اسم شاخه} </br> git checkout -b {اسم برای شاخه </b></td>
    <td dir=rtl> مشاهده شاخه های موجود </br> ساختن شاخه جدید </br> حذف شاخه مشخص </br> تعویض و رفتن به شاخه خاص </br> ساخت شاخه جدید و همزمان رفتن به آن </td>
  </tr>
  <tr>
    <td><b>git merge {اسم شاخه ای که می خواهیم ادغام کنیم}</b></td>
    <td dir=rtl> برای ادغام شاخه ها </td>
  </tr>
    <tr>
    <td><b>git rm {اسم فایل}</b></td>
    <td dir=rtl> برای حذف یک فایل از شاخه مربوطه </td>
  </tr>
  <tr>
    <td><b>git clone {آدرس گیت هاب}</b></td>
    <td dir=rtl> برای کپی یا به اصطلاح clone گرفتن از ریپوی خاص در گیت هاب </td>
  </tr>
      <tr>
    <td><b>git push</b></td>
    <td dir=rtl> برای اعمال تغییرات ایجاد شده در لوکال بر روی گیت هاب یا origin </br> git push origin master(main) </td>
  </tr>
  <tr>
    <td><b>git pull</b></td>
    <td dir=rtl> برای گرفتن آخرین تغییرات در گیت هاب بر روی clone خود </br> git pull origin master(main) </td>
  </tr>
  <tr>
    <td><b>git remote</b></br><b>git remote -v</b></td>
    <td dir=rtl> git remote add {Repo name} { Address for Repo EX: https://github.com/test-repo} </br> git push -u origin master</td>
  </tr>
  <tr>
    <td><b>git show</b></td>
    <td dir=rtl> {شناسه commit مربوطه} git show </br> جزییات تغییرات در آن کامیت را نشان می دهند</td>
  </tr>
  <tr>
    <td><b>git --version</b></td>
    <td dir=rtl> مشخص شدن ورژن گیت </td>
  </tr>
  <tr>
    <td><b>git config --global user.name {نام کاربری} </br> git config user.name </b></td>
    <td dir=rtl> برای تنظیم کردن نام کاربری </br> برای مشخص شدن نام کاربر گیت در حال حاضر </br> آپشن global بدان معنا است که تنظیمات در سراسر سیستم اِعمال خواهد شد</td>
  </tr>
  <tr>
    <td><b>git config --global user.email {آدرس ایمیل} </br> git config user.email </b></td>
    <td dir=rtl> برای تنظیم کردن آدرس ایمیل </br> برای مشخص شدن آدرس ایمیل گیت در حال حاضر </br> آپشن global بدان معنا است که تنظیمات در سراسر سیستم اِعمال خواهد شد</td>
  </tr>
  <tr>
    <td><b></b></td>
    <td dir=rtl>  </td>
  </tr>
  </table>

</br>
<h3 dir=rtl>
  سایر دستورات در Git:
</h3>

<table>
  <tr>
    <th><b><i>دستورات</i></b></th>
    <th><b><i>توضیحات</i></b></th>
  </tr>
  <tr>
    <td></br><b>git tag</br>git tag -a V2.0 -m 'کامنت'</br>git tag -l "v*"</br>git show V2.0</br>git push origin V2.0</br>git push origin --tags</br>git checkout V2.0</b></br></td>
    <td dir=rtl>مشاهده تگ ها</br>اضافه کردن تگ با کامنت مناسب</br>دیدن همه تگ ها که با حرف v شروع میشن</br>دیدن جزییات برای لاگی که تگ V2.0 دارد</br>اعمال تغییرات بر روی گیت هاب با تگ بجای شماره کامیت</br>اعمال تگ های ایجاد شده به گیت هاب</br>رفتن به تگ V2.0</td>
  </tr>
  <tr>
    <td><b>git help blame</br>git blame {اسم فایل} -L{شماره خط یا رنجی از خط ها}</b></td>
    <td dir=rtl>برای دیدن توضیحات دستورات گیت</br>برای پیدا کردن آخرین شخصی که خط از فایل رو تغییر داده</td>
  </tr>
  <tr>
    <td><b>git bisect [start | bad | good]</b></td>
    <td dir=rtl>برای پیدا کردن جایی که نسخه از کد درست کار کرده.</td>
  </tr>
  <tr>
    <td><b>git stash</br>git stash list</br>git stash save {یک پیغام}</br>git stash drop {stash اسم}</br>git stash show -p {stash اسم}</br>git stash apply {stash اسم}</br>git stash pop {stash اسم}</b></td>
    <td dir=rtl>برای ذخیره تغییرات در یک جای دیگر و تغییر شاخه از این دستور استفاده می شود</br>لیست تغییرات ذخیره شده با اسم آنها</br>برای ذخیره تغییرات با یک پیغام خاص</br>برای حذف یک stash</br>برای مشاهده جزییات یک stash</br> برای اعمال یک stash</br>برای اعمال یک stash با حذف آن ازقسمت ذخیره ها</td>
  </tr>
  <tr>
    <td><b>.gitignore</b></td>
    <td dir=rtl>یک فایل در پروژه برای کانفیک فایلهایی که گیت آن ها را در نظر نگیرد. اسم آن فایل ها در ایجا آورده می شود</td>
  </tr>
  <tr>
    <td><b>git rebase</b></td>
    <td dir=rtl> برای اطلاع از وضعیت ریپو  </td>
  </tr>
  </table>
