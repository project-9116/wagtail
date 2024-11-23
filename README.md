# wagtail
Wagtail'i inceleme kurcalama

# Kurma Kurulma Öncesi İlk Adımlar

## Python sürümünü yoklamak

```shell
python --version
# Veya:
python3 --version
# **Windows'da** (cmd.exe, Windows için Python Launcher ile):
py --version
```

## Bir sanal ortam yaratmak ve etkinleştirmek

```shell
py -m venv venv

# yarattıktan sonra

venv\Scripts\activate.bat

# venv\Scripts\activate.bat işlemez ise, şunu işletin:

mysite\env\Scripts\activate
```

## Wagtail'i kurmak

```shell
pip install wagtail
```

## Dışlanacakları belirtmek

- .gitignore belgesi varaltılıp içine "venv" yazarak sanal ortam belgeleri ve dizinleri dışlanır.

# Sitemizi Wagtail ile kendimiz üretmek istersek

Wagtail, django-admin başlangıç projesine benzer bir başlangıç komutları sağlar. Projenizde koşu wagtail başlangıç alanıma başlar, gerekli proje ayarları, boş bir HomePage modeli ve temel şablonlara ve örnek bir “arama” uygulaması da dahil olmak üzere birkaç Wagtail spesifik ekstraya ve örnek bir “arama” uygulaması dahil olmak üzere yeni bir site klasörü oluşturur.

```shell
wagtail start mysite mysite
```

**Dikkat**: "mysite" adlı dizin barındıran bir dizin içinde iken bu satırı işletiniz.

## Requirements.txt içinde belirtilmişleri kurmak

```shell
cd mysite
pip install -r requirements.txt
```