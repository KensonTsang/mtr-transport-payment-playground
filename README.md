# MTR Payment Backend Service

A high-performance C++17 backend service designed for MTR (Mass Transit Railway) station payments, supporting gate entry, fare deduction, and card top-ups. Built using modern C++ with RESTful APIs, modular architecture, and full containerization support.

---

## 🚀 Tech Stack

| Component          | Description                                |
|--------------------|--------------------------------------------|
| **C++17**          | Modern language features and performance   |
| **[oatpp](https://github.com/oatpp/oatpp)** | Lightweight and efficient REST framework |
| **[Boost.DI](https://github.com/boost-experimental/di)** | Dependency injection container |
| **[libpqxx](https://github.com/jtv/libpqxx)** | PostgreSQL driver for C++     |
| **[Catch2](https://github.com/catchorg/Catch2)** | Unit testing framework        |
| **[nlohmann/json](https://github.com/nlohmann/json)** | JSON serialization/deserialization |
| **[Conan](https://conan.io/)** | C++ package manager           |
| **CMake**          | Build configuration system                 |
| **Docker**         | Containerization for consistent builds     |
| **Kubernetes**     | (Planned) Cloud-native deployment          |

---

## 📦 Features

- Card top-up API (Oyster card / Debit card)
- Fare deduction & gate entry validation
- Integration with multiple banking APIs (JSON, XML, Protobuf)
- Dependency injection with testability in mind
- PostgreSQL for transactional data persistence
- CI/CD-ready Docker image

---

## 📁 Project Structure

```bash
.
├── CMakeLists.txt
├── docker/
├── src/
│   ├── api/            # REST controllers
│   ├── core/           # Business logic (DDD-style services)
│   ├── db/             # PostgreSQL access using libpqxx
│   ├── di/             # Dependency injection setup (Boost.DI)
│   └── main/           # Application entrypoint
├── include/
├── tests/
├── conanfile.txt
└── README.md
