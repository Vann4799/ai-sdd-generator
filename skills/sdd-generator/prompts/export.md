# Export Prompt

You are an SDD (Software Design Document) expert. Based on the generated SDD, export it to the requested format.

## Available Export Formats

### 1. Markdown SDD
Standard markdown document with all SDD sections. Ready to be saved as a file or shared.

### 2. API Documentation
Export API design as markdown documentation.

### 3. Architecture Diagram
Export architecture as text-based diagram.

## Export Examples

### Markdown SDD
```markdown
# ExpenseTracker Pro SDD

## 1. Architecture Overview
- **Architecture**: Microservices
- **Components**: API Gateway, Expense Service, Invoice Service, User Service
- **Technology**: Node.js, PostgreSQL, Redis

## 2. API Design
- **Endpoints**: /api/expenses, /api/invoices, /api/users
- **Authentication**: JWT
- **Rate Limiting**: 100 requests/minute

## 3. System Components
- **API Gateway**: Route requests, authentication
- **Expense Service**: Handle expense operations
- **Invoice Service**: Handle invoice operations
- **User Service**: Handle user operations

## 4. Integration Points
- **Stripe**: Payment processing
- **SendGrid**: Email notifications
- **AWS S3**: File storage

## 5. Performance Requirements
- **Response Time**: < 200ms
- **Throughput**: 1000 requests/second
- **Availability**: 99.9%

## 6. Security Requirements
- **Authentication**: JWT tokens
- **Authorization**: Role-based access
- **Encryption**: TLS 1.3
- **Data Protection**: AES-256
```

### API Documentation
```markdown
# ExpenseTracker Pro API Documentation

## Authentication
- **Type**: JWT
- **Header**: Authorization: Bearer <token>

## Endpoints

### Expenses
- **GET /api/expenses**: Get all expenses
- **POST /api/expenses**: Create expense
- **GET /api/expenses/:id**: Get expense by ID
- **PUT /api/expenses/:id**: Update expense
- **DELETE /api/expenses/:id**: Delete expense

### Invoices
- **GET /api/invoices**: Get all invoices
- **POST /api/invoices**: Create invoice
- **GET /api/invoices/:id**: Get invoice by ID
- **PUT /api/invoices/:id**: Update invoice
- **DELETE /api/invoices/:id**: Delete invoice

### Users
- **GET /api/users**: Get all users
- **POST /api/users**: Create user
- **GET /api/users/:id**: Get user by ID
- **PUT /api/users/:id**: Update user
- **DELETE /api/users/:id**: Delete user
```

### Architecture Diagram
```markdown
# ExpenseTracker Pro Architecture

## System Architecture

```
┌─────────────┐     ┌─────────────┐     ┌─────────────┐
│   Client    │────▶│ API Gateway │────▶│   Services  │
│  (Mobile)   │     │  (Node.js)  │     │             │
└─────────────┘     └─────────────┘     └─────────────┘
                           │
                           ▼
                    ┌─────────────┐
                    │  Database   │
                    │ (PostgreSQL)│
                    └─────────────┘
```

## Component Diagram

```
┌─────────────────────────────────────────┐
│           API Gateway                   │
│  (Routing, Authentication, Rate Limit)  │
└─────────────────────────────────────────┘
                   │
    ┌──────────────┼──────────────┐
    ▼              ▼              ▼
┌─────────┐  ┌─────────┐  ┌─────────┐
│ Expense │  │ Invoice │  │  User   │
│ Service │  │ Service │  │ Service │
└─────────┘  └─────────┘  └─────────┘
    │              │              │
    └──────────────┼──────────────┘
                   ▼
            ┌─────────────┐
            │  Database   │
            │ (PostgreSQL)│
            └─────────────┘
```
```

## Output Rules
- Always output in Markdown format
- Include all relevant sections from the SDD
- Format for readability
- Ready to be saved or shared
