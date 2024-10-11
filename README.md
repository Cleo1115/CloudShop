# CloudShop

## Overview
CloudShop is a cloud and React-based software marketplace platform designed to facilitate software purchasing. The platform provides an enhanced user experience by integrating responsive UI design using AntD and incorporating advanced features like file upload capabilities.

## Key Features
- **Software Purchasing Platform:** React-based client-side application for seamless software purchasing.
- **User Authentication:** Secure token-based authentication system using JWT for registration, search, and browsing software.
- **Advanced Product Search:** Utilizes ElasticSearch deployed on Google Compute Engine to provide powerful search functionalities.
- **Payment Processing:** Integrates Stripe API for streamlined billing and checkout processes.

## Frontend
- **React.js:** Handles the UI logic and rendering, providing a dynamic and responsive user experience.
- **Ant Design (AntD):** Used for designing a responsive and visually appealing user interface.

## Backend
- **Go:** Manages backend services, including user registration, authentication, and checkout workflows.
- **JWT (JSON Web Tokens):** Provides secure and efficient user authentication.
- **Google App Engine:** Hosts the Go microservices for scalable cloud hosting.

## Services
- **ElasticSearch:** Provides advanced search capabilities for the platform, hosted on Google Compute Engine.
- **Stripe API:** Facilitates efficient payment processing and financial transactions.

## Deployment
- **Backend and Services:** Go microservices are deployed on Google App Engine, with ElasticSearch on Google Compute Engine.

## Technical Stack

```mermaid
graph TD
    A[CloudShop Platform]
    B[Frontend: React & Ant Design] --> A
    C[Backend: Go & JWT Authentication] --> A
    D[Services: ElasticSearch & Stripe API] --> A
    E[Deployment: Hosting Platforms] --> A
    F[On Google Cloud] --> E
    G[Google App Engine] --> F
    H[Google Compute Engine] --> F

    classDef bigText fill:#ffffff,stroke:#3c6e71,stroke-width:1px,font-size:24px;
    classDef mainNode fill:#d9f2e6,stroke:#3c6e71,stroke-width:3px,font-size:28px;
    classDef frontendNode fill:#edf6f9,stroke:#457b9d,stroke-width:2px,font-size:24px;
    classDef backendNode fill:#ffddd2,stroke:#e63946,stroke-width:2px,font-size:24px;
    classDef servicesNode fill:#f4a261,stroke:#e76f51,stroke-width:2px,font-size:24px;
    classDef deploymentNode fill:#e9c46a,stroke:#2a9d8f,stroke-width:2px,font-size:24px;

    class A mainNode;
    class B frontendNode;
    class C backendNode;
    class D servicesNode;
    class E deploymentNode;
    class F,G,H bigText;




