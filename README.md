```markdown
# v2rayNG

یک کلاینت V2Ray برای اندروید که از [هسته Xray](https://github.com/XTLS/Xray-core) و [هسته v2fly](https://github.com/v2fly/v2ray-core) پشتیبانی می‌کند

[![API](https://img.shields.io/badge/API-21%2B-yellow.svg?style=flat)](https://developer.android.com/about/versions/lollipop)
[![Kotlin Version](https://img.shields.io/badge/Kotlin-2.3.0-blue.svg)](https://kotlinlang.org)
[![GitHub commit activity](https://img.shields.io/github/commit-activity/m/2dust/v2rayNG)](https://github.com/2dust/v2rayNG/commits/master)
[![CodeFactor](https://www.codefactor.io/repository/github/2dust/v2rayng/badge)](https://www.codefactor.io/repository/github/2dust/v2rayng)
[![GitHub Releases](https://img.shields.io/github/downloads/2dust/v2rayNG/latest/total?logo=github)](https://github.com/2dust/v2rayNG/releases)
[![Chat on Telegram](https://img.shields.io/badge/Chat%20on-Telegram-brightgreen.svg)](https://t.me/v2rayn)

### کانال تلگرام
[github_2dust](https://t.me/github_2dust)

### نحوه استفاده

#### Geoip و Geosite
- فایل‌های geoip.dat و geosite.dat در مسیر `Android/data/com.v2ray.ang/files/assets` قرار دارند (این مسیر ممکن است در برخی دستگاه‌های اندروید متفاوت باشد)
- قابلیت دانلود نسخه بهبود یافته را از این [مخزن](https://github.com/Loyalsoldier/v2ray-rules-dat) دریافت می‌کند (توجه: نیاز به یک پروکسی فعال دارد)
- آخرین [لیست دامنه](https://github.com/Loyalsoldier/v2ray-rules-dat) و [لیست IP](https://github.com/Loyalsoldier/geoip) رسمی می‌توانند به صورت دستی وارد شوند
- امکان استفاده از فایل dat شخص ثالث در همان پوشه وجود دارد، مانند [h2y](https://guide.v2fly.org/routing/sitedata.html#%E5%A4%96%E7%BD%AE%E7%9A%84%E5%9F%9F%E5%90%8D%E6%96%87%E4%BB%B6)

### اطلاعات بیشتر در [ویکی](https://github.com/2dust/v2rayNG/wiki) ما

### راهنمای توسعه

پروژه اندروید در پوشه V2rayNG می‌تواند مستقیماً در Android Studio یا با استفاده از Gradle wrapper کامپایل شود. اما هسته v2ray داخل aar (احتمالاً) قدیمی است.  
aar می‌تواند از پروژه Golang به نام [AndroidLibV2rayLite](https://github.com/2dust/AndroidLibV2rayLite) یا [AndroidLibXrayLite](https://github.com/2dust/AndroidLibXrayLite) کامپایل شود.
برای شروع سریع، راهنمای [Go Mobile](https://github.com/golang/go/wiki/Mobile) و [Makefiles برای توسعه‌دهندگان Go](https://tutorialedge.net/golang/makefiles-for-go-developers/) را بخوانید

v2rayNG می‌تواند روی شبیه‌سازهای اندروید اجرا شود. برای WSA، مجوز VPN باید از طریق دستور زیر اعطا شود:
`appops set [package name] ACTIVATE_VPN allow`
```