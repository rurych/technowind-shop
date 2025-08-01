# 📘 Назва проєкту

> *Інформаційна система управління базами даних підприємства*

---

## 👤 Автор

- **ПІБ**: Рурич О.Б.
- **Група**: ФЕС – 41
- **Керівник**: асист. Гарбієль І.І.
- **Дата виконання**: 31.05.2025

---

## 📌 Загальна інформація

- **Тип проєкту**: Вебсайт / Інформаційна система
- **Мова програмування**: JavaScript (React)
- **Фреймворки / Бібліотеки**: React.js, Tailwind CSS
- **База даних**: Oracle SQL

---

## 🧠 Опис функціоналу

- 🔍 Пошук товарів за назвою
- 🛒 Додавання товарів до кошика
- 🧾 Оформлення замовлення
- 🔐 Реєстрація користувачів
- 📋 Сторінка товару з описом і фото
- 🧑‍💼 Особистий кабінет
- 🎨 Банери і фільтрація за категоріями

---

## 🧱 Опис основних компонентів

| Компонент / Файл     | Призначення |
|---------------------|-------------|
| `App.jsx`           | Головний компонент сайту
| `CartPage.jsx`      | Кошик користувача
| `CheckoutPage.jsx`  | Сторінка оформлення замовлення
| `Header.jsx`        | Шапка сайту з пошуком та навігацією
| `RegisterModal.jsx` | Модальне вікно реєстрації користувача
| `ProductPage.jsx`   | Детальна сторінка товару
| `products.js`       | Масив з товарами та фото

---

## ▶️ Як запустити проєкт "з нуля"

### 1. Встановлення інструментів

- Node.js v18+
- Oracle Database Express Edition (локально або хмарно)

### 2. Клонування репозиторію

```bash
git clone https://github.com/rurych/technowind-shop
cd technowind-shop
```

### 3. Встановлення залежностей

```bash
npm install
```

### 4. Запуск

```bash
npm run dev
```

---

## 🔌 Підключення до Oracle

> Для взаємодії з базою Oracle планується використання Node.js + oracledb

```js
const oracledb = require('oracledb');
const connection = await oracledb.getConnection({
  user: 'username',
  password: 'password',
  connectString: 'localhost/XEPDB1'
});
```

---

## 🖱️ Інструкція для користувача

1. **На головній сторінці:**
   - Обирай товари за категоріями
   - Натискай кнопку "Купити" для додавання до кошика
2. **У кошику:**
   - Видаляй товари або оформлюй замовлення
3. **Реєстрація:**
   - Натисни "Реєстрація", заповни форму (валідація email та паролю)

---

## 📷 Приклади / скриншоти

- 🖼 Головна сторінка
- 🖼 Сторінка товару
- 🖼 Кошик
- 🖼 Оформлення замовлення

(скріншоти збережено у папці `/screenshots/`)

---

## 🧪 Проблеми і рішення

| Проблема                 | Рішення                                     |
|-------------------------|---------------------------------------------|
| React помилка "undefined" | Імпортувати всі компоненти вручну          |
| Помилка з Oracle        | Перевірити облікові дані та підключення     |
| Стан кошика не зберігається | Перенесено у глобальний useState          |

---

## 🧾 Використані джерела / література

- React.js документація – https://reactjs.org/
- TailwindCSS – https://tailwindcss.com/
- Oracle SQL Developer – https://www.oracle.com/database/sqldeveloper/
- MDN Web Docs (HTML/CSS/JS) – https://developer.mozilla.org/
- StackOverflow
- Наукові джерела (Google Scholar): див. список у додатку до роботи
