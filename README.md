Quyida sizning **`README.md`** faylingiz uchun mos yozilgan tarkib keltirilgan:

# E-Commerce API

Bu loyiha REST API orqali ishlaydigan e-commerce tizimi uchun backend xizmatidir. Ushbu loyiha Django va Django REST Framework (DRF) yordamida qurilgan. API faqat `title` va `description` ma'lumotlarini taqdim etadi.

## Loyihaning asosiy maqsadi

- E-commerce tizimi uchun RESTful API yaratish
- API orqali mahsulot ma'lumotlarini olish
- Django REST Framework'dan foydalanib, tezkor va ishonchli API yaratish

## Texnologiyalar

- **Python**: Backend dasturlash uchun
- **Django**: Tizimning asosiy ramkasi
- **Django REST Framework (DRF)**: RESTful API yaratish uchun
- **SQLite**: Ma'lumotlar bazasi sifatida (loyihani soddalashtirish uchun)

## API funksiyalari

API orqali quyidagi ma'lumotlarga kirish mumkin:

- **Title**: Mahsulotning nomi
- **Description**: Mahsulotning qisqacha ta'rifi

## O'rnatish bo'yicha ko'rsatmalar

1. Repozitoriyani klonlash:
   ```bash
   git clone https://github.com/AkramovFozil/e-commerce
   cd ecommerce
   ```

2. Virtual muhitni yaratish va faollashtirish:
   ```bash
   python -m venv env
   source env/bin/activate   # Windows uchun: env\Scripts\activate
   ```

3. Zaruriy kutubxonalarni o'rnatish:
   ```bash
   pip install -r requirements.txt
   ```

4. Ma'lumotlar bazasini sozlash:
   ```bash
   python manage.py migrate
   ```

5. Lokal serverni ishga tushirish:
   ```bash
   python manage.py runserver
   ```

## API foydalanish

1. API endpoint'lari ro'yxati:

   - Mahsulotlar ro'yxatini olish:  
     **GET** `/api/products/`

   - Mahsulotning batafsil ma'lumotini olish:  
     **GET** `/api/products/<id>/`

2. JSON formatida ma'lumotlar:

   ```json
   {
       "title": "Mahsulot nomi",
       "description": "Mahsulotning qisqacha ta'rifi"
   }
   ```


