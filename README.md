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
graph TD;
    React-->AntD;
    AntD-->UI[Responsive UI];
    React-->Authentication;
    Authentication-->JWT;
    Go-->GAE;
    GAE-->Authentication;
    ElasticSearch-->GCE;
    StripeAPI-->Checkout;
    GAE-->StripeAPI;
    Checkout-->Review;

## Frontend
- **React.js:** Handles the UI logic and rendering.
- **Ant Design (AntD):** Used for designing a responsive and visually appealing user interface.

## Backend
- **Go:** Manages backend services, including user registration, authentication, and checkout workflows.
- **JWT (JSON Web Tokens):** Provides secure and efficient user authentication.
- **Google App Engine:** Hosts the Go microservices for scalable cloud hosting.

## Services
- **ElasticSearch:** Provides advanced search capabilities for the platform, hosted on Google Compute Engine.
- **Stripe API:** Facilitates efficient payment processing and financial transactions.

## Deployment
- **Frontend:** Deployed as a static site on suitable hosting platforms.
- **Backend and Services:** Go microservices are deployed on Google App Engine, with ElasticSearch on Google Compute Engine.
