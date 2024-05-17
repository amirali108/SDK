**Welcome to Nextcloud**

Nextcloud is an open-source content collaboration platform that empowers teams to securely share, manage, and synchronize data across multiple devices. Engineered for privacy and control, Nextcloud is the ideal solution for organizations seeking to maintain sovereignty over their data. With a comprehensive suite of features tailored for file sharing, communication, and collaboration, Nextcloud facilitates efficient workflow management in a secure environment.

Getting Started
Learn more in the Nextcloud documentation.

Upgrading
For upgrading instructions, see the Nextcloud upgrade guide.



**Step-by-Step Installation of Nextcloud for Customer1**

**1-Setup Directories and Files:**

mkdir -p /nextcloud/customer1

cd /nextcloud/customer1

nano .env  # Add environment variables

nano docker-compose.yml  # Add Docker Compose configuration

nano nginx.conf  # Add Nginx configuration

nano .gitlab-ci.yml  # Add GitLab CI/CD configuration


**2-Run Docker Compose:**

cd /nextcloud/customer1

docker-compose up -d

**3-Configure Nginx:**

sudo ln -s /nextcloud/customer1/nginx.conf /etc/nginx/sites-available/nextcloud_customer1

sudo ln -s /etc/nginx/sites-available/nextcloud_customer1 /etc/nginx/sites-enabled/

sudo systemctl reload nginx




