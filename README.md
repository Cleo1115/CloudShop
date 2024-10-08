# CloudShop

## Overview
CloudShop is a cloud and React-based software marketplace platform designed to facilitate software purchasing. The platform provides an enhanced user experience by integrating responsive UI design using AntD and incorporating advanced features like file upload capabilities.

## Key Features
- **Software Purchasing Platform:** React-based client-side application for seamless software purchasing.
- **User Authentication:** Secure token-based authentication system using JWT for registration, search, and browsing software.
- **Advanced Product Search:** Utilizes ElasticSearch deployed on Google Compute Engine to provide powerful search functionalities.
- **Payment Processing:** Integrates Stripe API for streamlined billing and checkout processes.

## Technical Stack

```mermaid
graph TD
    A[CloudShop Platform] --> B[Frontend]
    A --> C[Backend]
    A --> D[Services]
    A --> E[Deployment]

    B --> F[React.js]
    B --> G[Ant Design]

    C --> H[Go]
    C --> I[JWT for Authentication]
    C --> J[Google App Engine]

    D --> K[ElasticSearch on Google Compute Engine]
    D --> L[Stripe API for Payment Processing]

    E --> N[Backend Microservices on Google App Engine]

    subgraph Frontend
        F
        G
    end

    subgraph Backend
        H
        I
        J
    end

    subgraph Services
        K
        L
    end

    subgraph Deployment
        M
        N
    end


