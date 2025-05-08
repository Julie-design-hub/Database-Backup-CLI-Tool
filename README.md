# Database-Backup-CLI-Tool
A Python CLI tool to automate backups for MySQL, PostgreSQL &amp; MongoDB with compression, cloud storage (AWS/GCP), and encryption – designed for developers who value simplicity and security. 🚀

**GitHub Repository Description: CLI Database Backup Utility**  

**🔧 Overview**  
This repository hosts a **command-line interface (CLI) tool** for backing up and restoring multiple database types (MySQL, PostgreSQL, MongoDB) with support for local/cloud storage, compression, and scheduling. Designed for developers and sysadmins, it simplifies database management through automation and secure workflows.  

**✨ Key Features**  
- **Multi-DB Support**: Backup/restore for MySQL, PostgreSQL, MongoDB, and SQLite.  
- **Flexible Storage**: Save backups locally or to cloud services (AWS S3, Google Cloud).  
- **Compression**: Reduce backup size with GZIP/TAR.  
- **Scheduling**: Automate backups using cron (Linux/macOS) or Task Scheduler (Windows).  
- **Security**: Encrypt backups and use environment variables for credentials.  
- **Logging & Alerts**: Detailed logs and Slack notifications for backup status.  

**🛠️ Tech Stack**  
- **Language**: Python 3.x  
- **Libraries**: `psycopg2`, `pymysql`, `pymongo`, `boto3` (AWS), `python-dotenv`  
- **Tools**: `mysqldump`, `pg_dump`, `mongodump`  

**🚀 Use Cases**  
- Automated daily backups for small businesses.  
- Disaster recovery for DevOps teams.  
- Secure database migrations.  

**📂 Repository Structure**  
```
db_backup_tool/  
├── main.py                # CLI entry point  
├── db_connectors/         # Database-specific logic  
├── storage/               # Local/cloud storage handlers  
├── utils/                 # Compression, logging  
├── .env.example           # Template for environment variables  
└── README.md              # Setup + usage guide  
```

**Install dependencies:**  
   ```bash  
   pip install -r requirements.txt  
   ```  
**Run a backup:**  
   ```bash  
   python main.py --db mysql --host localhost --user root --output local  
   ```  

**📜 License**  
MIT License - Free for personal and commercial use.  

**🙌 Contributions Welcome!**  
Open issues/PRs for new DB support, cloud providers, or optimizations.  

---  
**Why This Tool?**  
Unlike GUI-based solutions, this lightweight CLI tool prioritizes **scriptability**, **transparency**, and **cross-platform support**—ideal for automation pipelines. Perfect for learning database internals or deploying in production!  



---  
