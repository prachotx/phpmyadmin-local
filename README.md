# phpMyAdmin Docker Control Script

If you love using **XAMPP** or **Laragon** for quick local development,  
you’ll definitely enjoy this project. 🚀  

This is a **Docker-based local development environment** that works just like XAMPP/Laragon,  
but with the power and flexibility of Docker Compose.  

It comes with:
- **MySQL** as the database
- **phpMyAdmin** as the database management tool
- A simple control script (`phpmyadmin`) so you can start/stop/restart the environment from anywhere in your terminal.

---

## ⚙️ Installation

1. **Clone this repository**
   ```bash
   git clone https://github.com/your-username/phpmyadmin-local.git
   cd phpmyadmin-local
2. Create a bin directory inside your home (if it doesn’t exist yet)
   ```bash
   mkdir -p ~/bin
3. **Copy the script**
   ```bash
   cp ./bin/phpmyadmin ~/bin/
4. **Make it executable**
   ```bash
   chmod +x ~/bin/phpmyadmin
5. **Add ~/bin to your PATH**
   ```bash
   export PATH=$PATH:~/bin
6. **Reload your shell configuration**
   ```bash
   source ~/.bashrc

---

## ▶️ Usage

From anywhere in your terminal:
  ```bash
  phpmyadmin start     # Start phpMyAdmin + MySQL
  phpmyadmin stop      # Stop containers
  phpmyadmin restart   # Restart containers
  ```
Access phpMyAdmin in your browser: [http://localhost:8080](http://localhost:8080)

---

## 🐳 Example Output
  ```bash
  $ phpmyadmin start
  [+] Running 2/2
  ✔ Container my_mysql        Started
  ✔ Container my_phpmyadmin   Started
  ```

---

## 🛠️ Requirements
- [Docker](https://docs.docker.com/get-docker/)
- [Docker Compose](https://docs.docker.com/compose/)
