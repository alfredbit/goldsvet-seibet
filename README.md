Goldsvet Open Source

This version comes with support for:
- Laravel 8
- PHP 7.3
- Node.js 16
- PM2
- Redis

Also includes plugin support for:
- Sports Betting
- Crypto Competitions
- Stock Competitions

> **Note:** Games are available here 📩 **Telegram:** [@n0_Signall](https://t.me/n0_Signall)

---

# Key Features
- **1320 games available**, including 100 from PragmPlay.
- **GeoIP2 support** (manually enabled).

---

# Setup Instructions
Here’s a guide for setting up the project on a typical aaPanel or virtualmin server. It can be adapted for other environments.

# 1. Server Setup Requirements
- Apache, MySQL
- PHP 7.3 *(Composer required)*
- Laravel 8
- Node.js 16 & PM2
- php imagemagick

### 2. Installation Steps
1. **Enable SSL:** Force SSL for your domain.
2. **Create Database:** Set up a MySQL database for the app.
3. **Clone the Repository:** Pull the latest code from GitHub.
4. **Install Dependencies:**
   ```bash
   composer install
   npm install
5.	Environment Configuration: Copy .env.example to .env and update with your environment variables.
Bash
cp .env.example .env
php artisan key:generate
6.	Migrate Database:
execute the .sql file on phpmyadmin
Bash
php artisan migrate

## 🎮 Additional Content / Game Assets

If you need the full package with over **50 GB of games and assets**, feel free to reach out directly:

📩 **Telegram:** [@n0_Signall](https://t.me/n0_Signall)

PM2 Commands for WebSockets
Tip: Check out the full PM2 Commands Guide for managing Node.js processes.
Inside the PTWEBSOCKET folder, use the following commands: 
Bash
pm2 start Arcade.js --watch
pm2 start Server.js --watch
pm2 start Slots.js --watch
To start all services at once: 
Bash
pm2 start Arcade.js --watch && pm2 start Server.js --watch && pm2 start Slots.js --watch
Troubleshooting 
If you run into issues, try clearing caches: 
Bash
php artisan cache:clear
php artisan config:clear
php artisan route:clear
Common Errors 
•	404 Errors: Ensure your .htaccess file is properly set up. 

