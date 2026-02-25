# LeaseSeal

**Verified lease documents. Tamper-evident. Auditable. Dispute-resistant.**

LeaseSeal turns leases (PDFs, scans, exports) into verifiable artifacts with a clear source of truth.

## Repository structure

```
LeaseSeal/
├── LeaseSealBackEnd/    # Java 21 + Spring Boot 4 API
├── LeaseSealFrontEnd/   # React 19 + TypeScript + Vite
└── README.md            # (you are here)
```

## Prerequisites

- Java 21 (LTS)
- Maven (or use the included `mvnw` wrapper)
- Node.js 20+
- npm 10+

## Running the backend

```bash
cd LeaseSealBackEnd
./mvnw spring-boot:run
```

The API starts on `http://localhost:8080` by default.

### Running backend tests

```bash
cd LeaseSealBackEnd
./mvnw test
```

## Running the frontend

```bash
cd LeaseSealFrontEnd
npm install
npm run dev
```

The dev server starts on `http://localhost:5173` by default.

### Building for production

```bash
cd LeaseSealFrontEnd
npm run build
```

Output goes to `LeaseSealFrontEnd/dist/`.

## Tech stack

| Layer    | Technology                    |
|----------|-------------------------------|
| Backend  | Java 21, Spring Boot 4, JPA   |
| Frontend | React 19, TypeScript, Vite    |
| Database | PostgreSQL (planned)          |
| Infra    | Docker (planned)              |
