# A Lightweight WordPress Project Skeleton

This is a lightweight WordPress skeleton for your next WordPress web application. It aims to provide a clean and organized structure for managing WordPress projects, making it easier to develop, deploy, and maintain WordPress websites.

> Uses [wp-env-app](https://github.com/devuri/wp-env-app/)

## Folder Structure

Here's an overview of the directory structure used:

```
├── public              # Web server root directory
│   ├── app             # WordPress core files (excluded from version control)
│   │   ├── mu-plugins  # Must-use plugins directory
│   │   ├── plugins     # WordPress plugins directory
│   │   ├── uploads     # WordPress uploads directory
│   │   ├── templates   # Custom themes directory
│   │   └── themes      # WordPress themes directory
│   ├── wp              # WordPress core files (excluded from version control)
│   ├── .htaccess       # Web server configuration file
│   ├── index.php       # WordPress entry point
│   └── wp-config.php   # WordPress configuration file
├── publickeys          # Public key used for encryption or verification purposes
│   └── samplekey.pub   # Example key b75b666f-ac11-4342-b001-d2546f1d3a5b.pub
├── storage             # Storage directory for backups, cache, and logs
│   ├── .backups        # Backup directory
│   ├── cache           # Cache directory
│   └── logs            # Logs directory
│       └── wp-errors   # WordPress error logs
├── vendor              # Composer dependencies directory
├── .env                # Environment configuration file
├── app.php             # Application configuration file
├── bootstrap.php       # Bootstrap file
├── composer.json       # Composer configuration file
└── config.php          # Project configuration file overrides framework constants.

```
