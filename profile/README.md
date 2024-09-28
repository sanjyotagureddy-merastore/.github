# MeraStore E-commerce Platform

Welcome to the MeraStore e-commerce platform! This README provides an overview of the project, its components, and how to get started with development and deployment.

## Overview

MeraStore is a modern, scalable e-commerce platform built using microservices architecture. The platform is designed to be flexible, maintainable, and extensible, with separate services handling different aspects of the e-commerce experience.

> ⚠️ **Warning: Self-Learning Project**
>  <p>Please note that this project is intended solely as a self-learning exercise and is not meant for production use or as a commercial website. It is designed to serve as a testing ground for various techniques, methodologies, and approaches. The primary purpose of this project is to experiment and learn, and as such, it may not adhere to best practices or industry standards. <br><br>
> The implementations and design choices are based on exploration and experimentation, and may or may not align with industry best practices or standards. This project should be used as a reference for educational purposes only. For any real-world applications, please adhere to established best practices and seek professional advice.

## Table of Contents

1. [Features](#features)
2. [Architecture](#architecture)
3. [Components](#components)
   - [Microservices](#microservices)
   - [Shared Libraries](#shared-libraries)
   - [Common Libraries](#common-libraries)
   - [Frontend](#frontend)
   - [Infrastructure](#infrastructure)
   - [Documentation](#documentation)
   - [Monitoring and Logging](#monitoring-and-logging)
   - [Testing](#testing)
   - [Analytics](#analytics)
   - [Feature Flags](#feature-flags)
4. [Getting Started](#getting-started)
   - [Prerequisites](#prerequisites)
   - [Setup](#setup)
   - [Running the Application](#running-the-application)
5. [Deployment](#deployment)
6. [Contributing](#contributing)
7. [License](#license)
8. [Contact](#contact)

## Features

- **User Management**: Authentication and authorization for users.
- **Product Management**: Listings, categories, and product details.
- **Inventory Management**: Stock levels and warehouse operations.
- **Order Management**: Processing orders, payments, and tracking.
- **Cart Management**: Shopping carts and wishlists.
- **Payment Processing**: Handling transactions and payment gateways.
- **Shipping**: Delivery logistics and tracking.
- **Authentication/Authorization**: Secure access and permissions.

## Architecture

The MeraStore platform is built using a microservices architecture. Each microservice is responsible for a specific domain of the e-commerce platform, allowing for scalability and independent deployment. Key components include:

- **Microservices**: Individual services handling distinct functionality.
- **Shared Libraries**: Reusable code across microservices.
- **Frontend**: User interface for interacting with the platform.
- **Infrastructure**: Configuration and deployment scripts.

## Components

### Microservices

- **[user-service](https://github.com/sanjyotagureddy-merastore/user-service)**: Manages user profiles, authentication, and authorization.
- **[product-service](https://github.com/sanjyotagureddy-merastore/product-service)**: Handles product listings, categories, and attributes.
- **[inventory-service](https://github.com/sanjyotagureddy-merastore/inventory-service)**: Manages inventory levels and stock movements.
- **[order-service](https://github.com/sanjyotagureddy-merastore/order-service)**: Processes orders and payments.
- **[cart-service](https://github.com/sanjyotagureddy-merastore/cart-service)**: Manages shopping carts and wishlists.
- **[payment-service](https://github.com/sanjyotagureddy-merastore/payment-service)**: Handles payment transactions.
- **[shipping-service](https://github.com/sanjyotagureddy-merastore/shipping-service)**: Manages shipping and delivery logistics.
- **[auth-service](https://github.com/sanjyotagureddy-merastore/auth-service)**: Provides authentication and authorization functionalities.

### Shared Libraries

- **[shared-kernel](https://github.com/sanjyotagureddy-merastore/shared-kernel)**: Common functionalities and utilities shared across microservices.
- **[api-gateway](https://github.com/sanjyotagureddy-merastore/api-gateway)**: Unified entry point for all microservices.
- **[auth-library](https://github.com/sanjyotagureddy-merastore/auth-library)**: Shared authentication and authorization logic.
- **[http-client-library](https://github.com/sanjyotagureddy-merastore/http-client-library)**: Common HTTP client configurations.

### Common Libraries

- **[crypto-library](https://github.com/sanjyotagureddy-merastore/crypto-library)**: Cryptographic utilities for secure data handling.
- **[serialization-library](https://github.com/sanjyotagureddy-merastore/serialization-library)**: Handles data serialization and deserialization.
- **[logging-library](https://github.com/sanjyotagureddy-merastore/logging-library)**: Centralized logging setup.
- **[caching-library](https://github.com/sanjyotagureddy-merastore/caching-library)**: Provides caching mechanisms.
- **[configuration-library](https://github.com/sanjyotagureddy-merastore/configuration-library)**: Manages configuration settings.
- **[validation-library](https://github.com/sanjyotagureddy-merastore/validation-library)**: Provides validation logic.
- **[error-handling-library](https://github.com/sanjyotagureddy-merastore/error-handling-library)**: Centralized error handling.
- **[rate-limiting-library](https://github.com/sanjyotagureddy-merastore/rate-limiting-library)**: Implements rate limiting.
- **[health-check-library](https://github.com/sanjyotagureddy-merastore/health-check-library)**: Health check mechanisms.
- **[authorization-library](https://github.com/sanjyotagureddy-merastore/authorization-library)**: Manages authorization and permissions.
- **[telemetry-library](https://github.com/sanjyotagureddy-merastore/telemetry-library)**: Collects and reports telemetry data.
- **[i18n-library](https://github.com/sanjyotagureddy-merastore/i18n-library)**: Handles internationalization and localization.

### Frontend

- **[frontend](https://github.com/sanjyotagureddy-merastore/frontend)**: User interface code for the e-commerce platform.

### Infrastructure

- **[infra-config](https://github.com/sanjyotagureddy-merastore/infra-config)**: Infrastructure configuration and scripts.
- **[docker-images](https://github.com/sanjyotagureddy-merastore/docker-images)**: Docker images for microservices and components.
- **[ci-cd-pipelines](https://github.com/sanjyotagureddy-merastore/ci-cd-pipelines)**: CI/CD configurations for automated build and deployment.

### Documentation

- **[docs](https://github.com/sanjyotagureddy-merastore/docs)**: Project documentation, setup guides, and usage instructions.

### Monitoring and Logging

- **[monitoring](https://github.com/sanjyotagureddy-merastore/monitoring)**: Configurations for monitoring tools.
- **[secrets-management](https://github.com/sanjyotagureddy-merastore/secrets-management)**: Tools and configurations for managing secrets.

### Testing

- **[testing](https://github.com/sanjyotagureddy-merastore/testing)**: Automated testing tools and scripts.

### Analytics

- **[analytics](https://github.com/sanjyotagureddy-merastore/analytics)**: Setup and configurations for analytics tools.

### Feature Flags

- **[feature-flags](https://github.com/sanjyotagureddy-merastore/feature-flags)**: Tools for managing feature flags and toggles.

## Getting Started

### Prerequisites

Before you start, ensure you have the following installed:

- **Docker**: For containerization and running microservices.
- **Docker Compose**: For managing multi-container Docker applications.
- **Node.js**: For running frontend development tools.
- **.NET SDK**: For building and running .NET microservices.

### Setup

1. Download the [setup-mera-store.ps1](https://gist.github.com/sanjyotagureddy/7a6f8959aacc1dc6112346a7db271846/raw/setup-mera-store.ps1) and execute in powershell or cmd
