<img src="./logos/yayoutube/xxxhdpi/app_icon.png" height="40px" />

# YaYouTube   
  
**Идея**: YouTube с голосовым переводчиком от Яндекса на основе браузера. 

В модах я новичек и поэтому веду логи по прогам — [тык](./Logs.md).
  
## Яндекс Браузер  
  
Используется версия  
  
**Информация:**  
  
```  
chrome://version/  
```  
  
**Расширения:**  
  
```  
chrome://extensions/  
```  
  
```  
chrome://apps/  
```  
  
**Настройки SponsorBlock:**  
  
```  
chrome-extension://mnjggcdmjocbbbhaepdhchncahnbgone/options/options.html  
```  
  
## Расширения  
  
**SponsorBlock**  
  
```  
mnjggcdmjocbbbhaepdhchncahnbgone  
```  
  
[Скачать](https://chromewebstore.google.com/detail/sponsorblock-for-youtube/mnjggcdmjocbbbhaepdhchncahnbgone)  
  
**Return YouTube Dislike**  
  
```  
gebbhagfogifgggkldgodflihgfeippi  
```  
  
[Скачать](https://chromewebstore.google.com/detail/return-youtube-dislike/gebbhagfogifgggkldgodflihgfeippi)  
  
**User JavaScript and CSS**  
  
```  
nbhcbdghjpllgmfilhnhkllmkecfmpld  
```  
  
[Скачать](https://chromewebstore.google.com/detail/user-javascript-and-css/nbhcbdghjpllgmfilhnhkllmkecfmpld)  
  
## Разработка 
  
### 1. Закреплённые ссылки  
  
Для практики решил попробовать сначала заменить закрепленные ссылки на домашней странице.  

При вставке кода XML нужно уменьшить до одной строки — [тык](https://formatter.org/xml-formatter).
  
1.1. res/values/**array.xml**

- bro_default_dashboard_urls_russia

```xml
<string-array name="bro_default_dashboard_urls_russia">
   <item>https://dzen.ru/?clid=clid7</item>
   <item>https://mail.yandex.ru</item>
   <item>https://yandex.ru/games/?utm_source=tableau</item>
   <item>https://m.vk.com</item>
   <item>https://www.gosuslugi.ru</item>
   <item>https://m.youtube.com</item>
   <item>https://travel.yandex.ru</item>
   <item>https://yandex.ru/pogoda</item>
   <item>https://m.market.yandex.ru/?clid=2288493</item>
</string-array>
```

```xml
<string-array name="bro_default_dashboard_urls_russia">
   <item>chrome://version/</item>
   <item>chrome://extensions/</item>
   <item>https://m.youtube.com</item>
</string-array>
```

- bro_default_dashboard_titles_russia

```xml
<string-array name="bro_default_dashboard_titles_russia">
   <item>Дзен</item>
   <item>Яндекс.Почта — бесплатная и надежная электронная почта</item>
   <item>Игры</item>
   <item>Мобильная версия ВКонтакте</item>
   <item>Портал государственных услуг Российской Федерации</item>
   <item>YouTube</item>
   <item>Путешествия</item>
   <item>Яндекс.Погода</item>
   <item>Яндекс.Маркет — покупки с быстрой доставкой</item>
</string-array>
```

```xml
<string-array name="bro_default_dashboard_titles_russia">
   <item>Браузер</item>
   <item>Расширения</item>
   <item>YouTube</item>
</string-array>
```

-----

1.2 res/values-sw600dp/**array.xml**

- bro_default_dashboard_urls_russia

```xml
<string-array name="bro_default_dashboard_urls_russia">
   <item>https://dzen.ru</item>
   <item>https://www.kinopoisk.ru</item>
   <item>https://mail.yandex.ru</item>
   <item>https://www.gosuslugi.ru</item>
   <item>https://m.youtube.com</item>
   <item>https://travel.yandex.ru</item>
   <item>https://m.vk.com</item>
   <item>https://market.yandex.ru/</item>
</string-array>
```

```xml
<string-array name="bro_default_dashboard_urls_russia">
   <item>chrome://version/</item>
   <item>chrome://extensions/</item>
   <item>https://m.youtube.com</item></string-array>
```

- bro_default_dashboard_titles_russia

```xml
<string-array name="bro_default_dashboard_titles_russia">
   <item>Дзен</item>
   <item>Кинопоиск</item>
   <item>Яндекс.Почта — бесплатная и надежная электронная почта</item>
   <item>Портал государственных услуг Российской Федерации</item>
   <item>YouTube</item>
   <item>Путешествия</item>
   <item>Мобильная версия ВКонтакте</item>
   <item>Яндекс.Маркет — покупки с быстрой доставкой</item>
</string-array>
```

```xml
<string-array name="bro_default_dashboard_titles_russia">
   <item>Браузер</item>
   <item>Расширения</item>
   <item>YouTube</item>
</string-array>
```