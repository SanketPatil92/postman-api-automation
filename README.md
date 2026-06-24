# 🚀 DummyJSON API Test Automation Suite

A robust, automated API testing framework designed to validate foundational e-commerce backend workflows using **Postman**. This suite implements end-to-end integration flows across user authentication, product search capabilities, and dynamic shopping cart modifications.

---

## 🎯 Key Features & Test Coverage

The test collection maximizes validation stability across multiple functional areas, executing **70 micro-assertions** with a 100% pass rate:

* **🔐 Authentication Workflows (`/auth`)**
    * Simulates dynamic user login sequences (`POST /auth/login`).
    * Extracts bearer authentication tokens programmatically to authorize subsequent user requests (`GET /auth/me`).
* **📦 Product Catalog Verification (`/products`)**
    * Validates data contract models for retrieval endpoints (All Products vs Single Product).
    * Ensures deep payload integrity (type assertions verifying positive integers, non-empty strings, and required fields).
    * Implements edge-case error boundary assertions for invalid product resource IDs.
* **🛒 Cart State Lifecycle (`/carts`)**
    * Validates operations for items added to shopping carts (`POST`).
    * Assures real-time calculations work properly (verifying totals change appropriately based on item mutation).
    * Validates structural payload updates via `PUT`/`PATCH` methods.

---

## 📊 Latest Execution Summary

```text
Run Status: SUCCESS
Iterations: 1
Total Tests: 70
Failures: 0
Avg Response Time: 144 ms
