Overview:-
--------------------
AuthGate is an Authentication as a Service (SaaS) solution designed to simplify user authentication and authorization for multi-tenant applications. It provides a secure, scalable, and easy-to-integrate authentication system with OAuth 2.0 support.
-------------------------------------------------------------------------------------------------------------------------------
Features:-
--------------------
OAuth 2.0 Authentication: Secure user authentication flow.
Multi-Tenant Support: Manage multiple tenants with isolated data.
Easy Integration: Simple setup for frontend and backend applications.
Extensible: Supports future enhancements like MFA and additional SSO providers.
Installation
Prerequisites
Node.js
MongoDB
Backend (NestJS)
-------------------------------------------------------------------------------------------------------------------------------
Clone the repository:-
--------------------
---->bash:
git clone https://github.com/ahadlyy/AuthGate.git
Navigate to the backend directory:

---->bash:
cd AuthGate/backend
Install dependencies:

---->bash:
npm install
Configure environment variables:

---->Copy .env.example to .env and update the values.
Run the server:

---->bash:
npm run start

Frontend (Angular)
Navigate to the frontend directory:

---->bash:
cd AuthGate/frontend

-Install dependencies:

---->bash:
npm install
Run the application:

---->bash:
ng serve

-------------------------------------------------------------------------------------------------------------------------------
Usage:-
--------------------
---->Tenant Registration
Tenants register by providing name, email, phone, and address.
Upon registration, tenants can add projects and configure callback URLs.
---->User Authentication
Users visit the tenant's application and click "Sign Up with AuthGate".
AuthGate handles the authentication flow and redirects users back to the tenant application with an authorization code.
Tenant's backend exchanges the authorization code for an access token from AuthGate.
-------------------------------------------------------------------------------------------------------------------------------
API Documentation:-
--------------------
POST /api/auth/register: Register a new tenant.
POST /api/auth/login: Authenticate a user.
GET /api/auth/callback: Handle OAuth callback.
Refer to the API Documentation for detailed endpoint information.
-------------------------------------------------------------------------------------------------------------------------------
Contribution:-
--------------------
Fork the repository.
Create a new branch (git checkout -b feature-branch).
Commit your changes (git commit -m 'Add new feature').
Push to the branch (git push origin feature-branch).
Open a pull request.
Future Work
Multi-Factor Authentication (MFA)
Support for additional SSO providers
Performance optimizations
-------------------------------------------------------------------------------------------------------------------------------
