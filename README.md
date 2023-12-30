# A Lightweight WordPress Project Skeleton

This is a lightweight WordPress skeleton for your next WordPress web application. It aims to provide a clean and organized structure for managing WordPress projects, making it easier to develop, deploy, and maintain WordPress websites.

> Uses [wp-env-app](https://github.com/devuri/wp-env-app/)

### Environment Variables Setup

To get started, create a `.env` file in the root directory of your project.
In this file, define the environment variables you wish to use as configuration constants, update the database credentials and other settings as needed.

```shell
WP_HOME='https://example.com'
WP_SITEURL="${WP_HOME}"

WP_ENVIRONMENT_TYPE='production'
DEVELOPER_ADMIN='0'

MEMORY_LIMIT='256M'
MAX_MEMORY_LIMIT='256M'

DB_NAME=wp_dbName
DB_USER=root
DB_PASSWORD=
DB_HOST=localhost
DB_PREFIX=wp_
```

> Full list of [Environment Variables](https://devuri.github.io/wp-env-config/env/)

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
├── pubkey              # Public key used for encryption or verification purposes
│   └── samplekey.pub   # Example key b75b666f-ac11-4342-b001-d2546f1d3a5b.pub
├── storage             # Storage directory for backups, cache, and logs
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
