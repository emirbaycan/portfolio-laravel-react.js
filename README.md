# Portfolio React Laravel

**Full-Stack Developer Portfolio** built with **Laravel 10 (API)** and **React 18 (SPA)**. This project serves as a modern, responsive, and customizable portfolio platform, ideal for showcasing personal projects, skills, and professional experiences.

---

## 🚀 Features

* **React 18** frontend with component-based architecture
* **Laravel 10** backend serving as a RESTful API
* **Tailwind CSS** for rapid and responsive UI design
* **Vite** for fast development and optimized builds
* **TypeScript** support for type safety and scalability
* **ESLint & Prettier** configured for consistent code formatting
* **Authentication** system ready for integration
* **Modular structure** for easy customization and scalability

---

## 📁 Project Structure

```
portfolio-react-laravel/
├── app/                # Laravel backend application
├── bootstrap/          # Laravel bootstrap files
├── config/             # Configuration files
├── database/           # Migrations and seeders
├── public/             # Public assets and entry points
├── resources/
│   ├── js/             # React frontend source code
│   └── views/          # Blade templates (if any)
├── routes/             # API and web routes
├── storage/            # Storage for logs and compiled files
├── tests/              # Test cases
├── .env.example        # Environment variable example file
├── package.json        # Node.js dependencies
├── composer.json       # PHP dependencies
└── README.md           # Project documentation
```

---

## 🛠️ Installation

### Prerequisites

* PHP >= 8.1
* Composer
* Node.js >= 16
* MySQL or any other supported database

### Backend Setup (Laravel)

1. **Clone the repository:**

   ```bash
   git clone https://github.com/emirbaycan/portfolio-react-laravel.git
   cd portfolio-react-laravel
   ```

2. **Install PHP dependencies:**

   ```bash
   composer install
   ```

3. **Copy and configure the environment file:**

   ```bash
   cp .env.example .env
   ```

   Update the `.env` file with your database credentials and other necessary configurations.

4. **Generate application key:**

   ```bash
   php artisan key:generate
   ```

5. **Run migrations (and seeders if available):**

   ```bash
   php artisan migrate --seed
   ```

6. **Start the Laravel development server:**

   ```bash
   php artisan serve
   ```

   The backend API will be accessible at `http://localhost:8000`.

### Frontend Setup (React)

1. **Navigate to the `resources/js` directory:**

   ```bash
   cd resources/js
   ```

2. **Install Node.js dependencies:**

   ```bash
   npm install
   ```

3. **Start the React development server:**

   ```bash
   npm run dev
   ```

   The frontend will be accessible at `http://localhost:5173`.

---

## ⚙️ Configuration

* **API Base URL:** Ensure that the React application communicates with the correct Laravel API endpoint. Update the API base URL in your frontend configuration files as needed.

* **CORS:** Configure Laravel's CORS settings in `config/cors.php` to allow requests from your frontend domain.

---

## 🧪 Testing

### Backend Tests

```bash
php artisan test
```

### Frontend Tests

If you have set up testing frameworks like Jest or React Testing Library:

```bash
npm run test
```

---

## 📦 Deployment

### Backend Deployment

1. **Set up your production environment with PHP, Composer, and a web server (e.g., Nginx or Apache).**

2. **Clone the repository and install dependencies:**

   ```bash
   git clone https://github.com/emirbaycan/portfolio-react-laravel.git
   cd portfolio-react-laravel
   composer install --optimize-autoloader --no-dev
   ```

3. **Set up the `.env` file and generate the application key:**

   ```bash
   cp .env.example .env
   php artisan key:generate
   ```

4. **Run migrations:**

   ```bash
   php artisan migrate --force
   ```

5. **Set appropriate permissions for storage and bootstrap cache:**

   ```bash
   chmod -R 775 storage
   chmod -R 775 bootstrap/cache
   ```

### Frontend Deployment

1. **Navigate to the `resources/js` directory:**

   ```bash
   cd resources/js
   ```

2. **Build the React application:**

   ```bash
   npm run build
   ```

3. **Serve the compiled assets:**

   The compiled assets will be located in the `public` directory. Ensure your web server serves these static files correctly.

---

## 🤝 Contributing

Contributions are welcome! Please fork the repository and submit a pull request for any enhancements or bug fixes.

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

---

## 📬 Contact

For any inquiries or feedback, please reach out to [emirbaycan](https://github.com/emirbaycan).
