# Apartment Management System

A backend-based apartment management system built with Java and Spring Boot, designed to support common rental business scenarios such as apartment information management, room management, lease agreements, appointments, users, fees, labels, and related resources.

## Project Structure

This project uses a multi-module Maven architecture:

- `common`  
  Common utilities and shared configurations.

- `model`  
  Entity models and shared data structures.

- `web`  
  Web layer module.
  - `web-admin` : backend services for the admin side
  - `web-app` : reserved module for app-side services

## Tech Stack

- Java 17
- Spring Boot 3
- Maven
- MyBatis-Plus
- MySQL
- JWT
- Knife4j / OpenAPI
- EasyCaptcha
- MinIO
- Alibaba Cloud SMS SDK

## Main Features

- Apartment information management
- Room information management
- Lease agreement management
- Viewing appointment management
- User management
- Fee and payment configuration
- Facility and label management
- Image / graph resource management
- Authentication and API documentation support

## Backend Architecture

The project follows a layered backend design:

- **Controller layer** for handling REST API requests
- **Service layer** for business logic
- **Mapper layer** for database operations
- **VO layer** for request/response data transfer

This structure helps improve readability, maintainability, and scalability.

公寓管理系统

技术栈： Java 17, Spring Boot 3, Maven, MyBatis-Plus, MySQL, JWT, Knife4j, MinIO

设计并开发基于 Spring Boot 的公寓管理系统后端，采用 Maven 多模块架构拆分 common、model、web 等模块，提高项目可维护性与代码复用性。
实现管理员端业务模块，覆盖公寓信息、房间信息、租约管理、预约看房、用户信息、费用配置、标签配置、图片资源等核心租赁场景。
基于 MyBatis-Plus 完成数据持久层开发，结合 Mapper、Service、VO 分层设计，提升业务代码组织性与数据库操作效率。
集成 JWT 登录认证、图形验证码、API 文档（Knife4j/OpenAPI）等功能，增强系统安全性与接口可测试性。
支持对象存储与短信服务相关能力扩展，引入 MinIO 与阿里云短信依赖，为图片上传和通知类业务预留实现基础。
