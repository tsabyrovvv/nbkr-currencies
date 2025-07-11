# 🇰🇬 НБКР Exchange - Курсы валют Кыргызстана

Современный веб-интерфейс для просмотра официальных курсов валют Национального банка Кыргызской Республики с конвертером валют в реальном времени.

![Preview](https://img.shields.io/badge/Status-Live-brightgreen) ![Tech](https://img.shields.io/badge/Tech-Vanilla_JS-yellow) ![API](https://img.shields.io/badge/API-NBKR-blue)

## ✨ Особенности

- 📊 **Ежедневные курсы** - актуальные данные от НБКР
- 📅 **Еженедельные курсы** - сводные данные за неделю  
- 💱 **Конвертер валют** - мгновенная конвертация по официальным курсам
- 📋 **Справочник валют** - полный список доступных валют
- 🎨 **Современный дизайн** - темная тема с градиентами и анимациями
- 📱 **Адаптивность** - отлично работает на всех устройствах
- ⚡ **Быстрая загрузка** - оптимизированный код без зависимостей

## 🚀 Демо

Попробуйте живую версию: [НБКР Exchange](https://currencies.sabyrov.dev)

## 🛠 Технологии

- **Frontend**: Vanilla JavaScript, HTML5, CSS3
- **API**: Национальный банк КР (nbkr.kg)
- **CORS Proxy**: Собственный FastAPI сервер
- **Стилизация**: CSS Grid, Flexbox, CSS Animations

## 📦 Установка

### Клонирование репозитория
```bash
git clone https://github.com/tsabyrovvv/currencies.git
cd nbkr-exchange
```

### Локальный запуск
```bash
# Просто откройте index.html в браузере
open index.html

# Или запустите локальный сервер
python -m http.server 8080
```

## 🔧 Настройка CORS Proxy

Для работы с API НБКР требуется CORS прокси. Включен готовый код:

### Установка прокси
```bash
pip install fastapi uvicorn httpx
python cors-proxy.py
```

### Настройка в коде
```javascript
// Замените на ваш домен
const CORS_PROXY = 'https://your-proxy-domain.com/?url=';
```

## 💱 Конвертер валют

Встроенный конвертер поддерживает:

- ✅ Все валюты из ежедневных курсов НБКР
- ✅ Кыргызский сом (KGS) как базовая валюта
- ✅ Учет номинала валют
- ✅ Мгновенные расчеты
- ✅ Обмен валют местами одним кликом

### Поддерживаемые валюты
```
USD, EUR, RUB, CNY, KZT, GBP, JPY, CHF, CAD, AUD, 
SEK, NOK, DKK, INR, TRY и другие официальные валюты НБКР
```

## 📖 API Endpoints

Используются следующие endpoints НБКР:

| Endpoint | Описание |
|----------|----------|
| `/XML/daily.xml` | Ежедневные курсы валют |
| `/XML/weekly.xml` | Еженедельные курсы |
| `/XML/CurrenciesReferenceList.xml` | Справочник валют |

## 🎨 Дизайн

- **Цветовая схема**: Темная тема с градиентами
- **Анимации**: Плавные переходы и hover эффекты
- **Типографика**: Inter font family
- **Адаптивность**: Mobile-first подход
- **Glassmorphism**: Полупрозрачные элементы с blur эффектом

## 📱 Браузеры

Поддерживается всеми современными браузерами:

- ✅ Chrome 90+
- ✅ Firefox 88+  
- ✅ Safari 14+
- ✅ Edge 90+

### Идеи для улучшений
- [ ] График изменения курсов
- [ ] Уведомления о изменениях
- [ ] Экспорт данных в CSV
- [ ] PWA поддержка
- [ ] Темная/светлая тема
- [ ] Мультиязычность

## 📄 Лицензия

Этот проект лицензирован под MIT License - см. файл [LICENSE](LICENSE) для деталей.

## 👨‍💻 Разработчик

**Сабыров Тимур**
- Website: [sabyrov.dev](https://sabyrov.dev)
- Email: timur@sabyrov.dev

## 🙏 Благодарности

- [Национальный банк КР](https://nbkr.kg) за предоставление открытого API
- [Inter Font](https://rsms.me/inter/) за красивый шрифт
- Сообществу open source за вдохновение

## 📊 Статистика проекта

![GitHub stars](https://img.shields.io/github/stars/tsabyrovvv/currencies?style=social)
![GitHub forks](https://img.shields.io/github/forks/tsabyrovvv/currencies?style=social)
![GitHub issues](https://img.shields.io/github/issues/tsabyrovvv/currencies)
![GitHub last commit](https://img.shields.io/github/last-commit/tsabyrovvv/currencies)

---

⭐ **Если проект понравился, поставьте звездочку!** ⭐