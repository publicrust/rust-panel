# Rust-Panel: Task List and Project Description

## Project Goal
To create an open, secure, and user-friendly server management panel. Rust-Panel provides data encryption, transparent architecture, and blockchain-based authentication.

---

## Main Tasks

### Backend (C#):
1. **Basic Project Structure:**
   - Create an API framework using .NET (ASP.NET Core).
   - Configure interaction with the file system and processes.

2. **Authentication:**
   - Login/password with hashing (e.g., bcrypt).
   - Optional blockchain-based login support (TON/ETH): token generation, signature verification.

3. **Data Encryption:**
   - Module for generating unique keys for each server.
   - Implement file encryption/decryption "on the fly."
   - Encrypted log storage.

4. **Server Management:**
   - Start, stop, and restart processes.
   - Command input via terminal (WebSocket/SignalR implementation).
   - Log processes: capture stdout/stderr.

5. **File Manager API:**
   - CRUD operations (create, read, update, delete files).
   - Support for working with encrypted directories.

6. **Extension Support:**
   - Create a plugin system.
   - API for templates and additional modules.

---

### Frontend (React):
1. **React Application Structure:**
   - Set up the project with routing (React Router).
   - Integrate Redux or Context for global state management.

2. **Authentication:**
   - Login form: username/password.
   - Blockchain login support (TON/ETH).

3. **Dashboard:**
   - Display a list of servers: status, actions (start, stop, restart).
   - Real-time server logs (WebSocket/SignalR).

4. **File Manager:**
   - Interface for file management: upload, delete, edit.
   - Encryption/decryption process indication.

5. **Extension System:**
   - Marketplace for templates and modules.
   - Ability to install custom add-ons.

---

### General Tasks:
1. **Documentation:**
   - API documentation (Swagger, Postman).
   - Guides for installation, configuration, and development (ReadMe, Wiki).

2. **Versioning and Branching System:**
   - Set up Git Flow.
   - Branch separation: main, develop, feature.

3. **Security:**
   - Implement brute-force protection.
   - Regular code reviews (static analysis).

---

## Problem the Project Solves
Most existing hosting services:
- Store user data unencrypted, making it vulnerable to leaks.
- Lack transparency: users are unaware of who has access to their files.
- Limit the ability to modify or extend the panel.

**Solution:** Rust-Panel:
- Encrypts all server data, with access restricted to the owner.
- Fully open-source code, visible and auditable by the community.
- Extensible architecture: templates, plugins, blockchain integration.

---

## Development Stages (Roadmap):
1. **MVP (Minimum Viable Product):**
   - Core functions: server management, encryption, terminal.
   - Basic authentication.

2. **Blockchain Integration:**
   - Authentication via TON/ETH.
   - Key and seed phrase storage without hosting involvement.

3. **Extension Support:**
   - Template and plugin marketplace.
   - Interface customization options.

4. **Infrastructure Expansion:**
   - Cluster and load balancing support.
   - FTP access with 2FA.

---

## Conclusion
Rust-Panel addresses critical issues of security and transparency in hosting solutions. The project is focused on the community, open-source code, and ease of use. We invite everyone to contribute to the development and help create the next generation of hosting panels.

