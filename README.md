# 🛒 Click & Cart — Full-Stack E-Commerce Web App

![React](https://img.shields.io/badge/React.js-18-61DAFB?style=for-the-badge&logo=react&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-3.x-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-8.0-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Redux](https://img.shields.io/badge/Redux-Toolkit-764ABC?style=for-the-badge&logo=redux&logoColor=white)
![Vercel](https://img.shields.io/badge/Deployed-Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)

> A fully functional full-stack e-commerce application with product listing, cart, wishlist, authentication, and checkout — built with React.js (frontend) and Java Spring Boot (backend).

🌐 **Live Demo:** [click-cart-ecommerce.vercel.app](https://ecommers-pied.vercel.app/) <!-- update with your actual URL -->

---
**Home Page**

![home](https://github.com/user-attachments/assets/0a6cd817-b4c8-4369-b54c-f87986cf929e)

**Products Page**

![products](https://github.com/user-attachments/assets/347a6bb2-3a4b-433e-b0cb-4dd3c3c7b5a9)

---

## ✨ Features

- 🔐 **User Authentication** — Register, Login, protected routes
- 🛍️ **Product Listing** — Browse all products with details
- 🛒 **Cart Management** — Add, remove, update quantity
- ❤️ **Wishlist** — Save favourite products
- 💳 **Checkout Flow** — Order placement with form validation
- 📱 **Responsive Design** — Works on mobile, tablet, and desktop
- 🔗 **REST API** — Clean Spring Boot backend with JPA/Hibernate
- 🗄️ **MySQL Database** — Persistent data storage

---

## 🧰 Tech Stack

### Frontend
| Technology | Purpose |
|---|---|
| React.js 18 | UI framework |
| Redux Toolkit | Global state management (cart, auth) |
| React Router | Client-side routing |
| CSS / Global Styles | Styling |
| Axios | API calls to backend |

### Backend
| Technology | Purpose |
|---|---|
| Java + Spring Boot | REST API server |
| Spring Data JPA / Hibernate | ORM & database interaction |
| Spring Security | Authentication & authorization |
| MySQL | Relational database |
| Maven | Build tool |

---

## 📁 Project Structure

```
Click-Cart-Ecommerce/
│
├── backend/                        # Spring Boot Application
│   ├── src/main/java/com/ecommerce/back/
│   │   ├── controller/
│   │   │   └── ContactController.java
│   │   ├── model/
│   │   │   └── Contact.java
│   │   ├── repository/
│   │   │   └── ContactRepository.java
│   │   └── BackendApplication.java
│   ├── src/main/resources/
│   │   └── application.properties
│   └── pom.xml
│
└── frontend/                       # React Application
    └── src/
        ├── components/
        │   ├── Footer.jsx
        │   ├── Navbar.jsx
        │   └── Products.jsx
        ├── pages/
        │   ├── Home.jsx
        │   ├── Product.jsx
        │   ├── Products.jsx
        │   ├── Cart.jsx
        │   ├── Wishlist.jsx
        │   ├── Checkout.jsx
        │   ├── Login.jsx
        │   ├── Register.jsx
        │   ├── AboutPage.jsx
        │   ├── ContactPage.jsx
        │   └── PageNotFound.jsx
        ├── redux/                  # Redux store & slices
        ├── global.css
        └── index.js
```

---

## 🚀 Getting Started

### Prerequisites
- Java 17+
- MySQL 8.0+
- Maven 3.x

---

### 🔧 Backend Setup

```bash
# 1. Clone the repository
git clone https://github.com/Princejwl/Click-Cart-Ecommerce-.git
cd Click-Cart-Ecommerce-/backend

# 2. Create MySQL database
mysql -u root -p
CREATE DATABASE ecommerce_db;

# 3. Update application.properties
```

Edit `src/main/resources/application.properties`:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/ecommerce_db
spring.datasource.username=your_username
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

```bash
# 4. Run the backend
mvn spring-boot:run
# Backend runs at: http://localhost:8080
```

---

### 💻 Frontend Setup

```bash
# 1. Navigate to frontend
cd ../frontend

# 2. Install dependencies
npm install

# 3. Start development server
npm start
# Frontend runs at: http://localhost:3000
```

---

## 🌐 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| `POST` | `/api/auth/register` | Register new user |
| `POST` | `/api/auth/login` | User login |
| `GET` | `/api/products` | Get all products |
| `GET` | `/api/products/{id}` | Get product by ID |
| `POST` | `/api/cart` | Add item to cart |
| `GET` | `/api/cart/{userId}` | Get user cart |
| `DELETE` | `/api/cart/{id}` | Remove cart item |
| `POST` | `/api/contact` | Submit contact form |

---

## 🔑 Environment Variables

Create a `.env` file in the frontend folder:

```env
REACT_APP_API_URL=http://localhost:8080/api
```

---

## 📦 Deployment

- **Frontend** → Deployed on **Vercel** (auto-deploy from GitHub `main` branch)
- **Backend** → Can be deployed on Railway / Render / AWS EC2

---

## 🙋‍♂️ Author

**Prince Jaiswal**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Prince_Jaiswal-0A66C2?style=flat&logo=linkedin)](https://linkedin.com/in/Prince_Jaiswal)
[![GitHub](https://img.shields.io/badge/GitHub-PrinceJwl-181717?style=flat&logo=github)](https://github.com/Princejwl)
[![Email](https://img.shields.io/badge/Email-princejaiswal0920@gmail.com-D14836?style=flat&logo=gmail)](mailto:princejaiswal0920@gmail.com)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

⭐ **If you found this project helpful, please give it a star!**
