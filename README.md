**Project: Secure Digital Communication Platform with Nextcloud, Zammad, and Monitoring**

**Introduction**

**What is Secure Digital Communication (SDK)?**

Secure Digital Communication (SDK) offers a safe, simple, and secure way to send sensitive and classified information between various actors in the public sector. The goal is to increase security and efficiency for digital collaboration and information exchange, thereby providing better conditions for taking care of individuals who need support. Every day, vast amounts of information are exchanged between actors in the public sector. Often, this involves sensitive or classified information such as care plans, treatment plans, work ability assessments, and extracts from the criminal record. In the absence of safer alternatives, fax, mail, or couriers are used today, especially in healthcare, schools, and social services.
SDK is a digital infrastructure that enables public actors to exchange sensitive and classified information digitally in a safe, secure, and efficient manner. Private contractors with publicly funded assignments can also connect to SDK.

**Benefits of SDK**

**- Security:** Personal or sensitive information is not spread to unauthorized parties.

**- Efficiency:** Faster processing and decision-making.

**- Traceability:** Ensures traceability regardless of which organization sends the information.

**- Compatibility:** Messages sent via SDK can contain free text and attachments in various formats. They are addressed to functional addresses within the connected participant organizations, such as social services within a municipality, a department at an authority, or a health center within a region. It is not possible to send messages directly to individuals.

**- Integration:** SDK lacks its own user interface, meaning the staff using SDK creates and receives messages in the software chosen by the organization to send messages.
For more information on SDK, visit sdk.digg.se.

**Project Overview**

This project sets up a secure communication platform integrating Nextcloud for file sharing and collaboration, Zammad for ticketing and customer support, and a monitoring stack using Prometheus and Grafana. The setup is designed to cater to the needs of the public sector, ensuring a reliable and secure infrastructure for digital communication.

SDK
├── Monitoring
│   ├── .gitkeep
│   ├── docker-compose.yml
│   ├── grafana.ini
│   ├── prometheus.yml
│   └── README.md
├── nextcloud
│   ├── customer1
│   │   ├── .env
│   │   ├── docker-compose.yml
│   │   ├── nginx.conf
│   │   └── README.md
│   ├── customer2
│   │   ├── .env
│   │   ├── docker-compose.yml
│   │   ├── nginx.conf
│   │   └── README.md
│   ├── .gitkeep
│   └── README.md
├── zammad
│   ├── docker-compose.yml
│   ├── nginx.conf
│   └── README.md
├── .gitlab-ci.yml
└── README.md


