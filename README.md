# 🏰 Majest Framework
> **The Kernel 0 Web Engine.** Built for speed, locked for security, powered by Go & Lua.

Majest is a high-performance web framework designed to end "JavaScript fatigue." By treating **Go as the Hardware (Kernel 0)** and **Lua as the Scripting Layer**, Majest delivers sub-millisecond rendering with a zero-JS footprint.

---

## 🚀 Why Majest?

* **Kernel 0 Security:** Built-in auto-escaping in the Go core. XSS attacks like `alert('hacked')` are physically impossible by design.
* **Raw Performance:** Compiled Go binary execution. No V8 engine overhead, no Python interpreter lag.
* **Zero JS Runtime:** Leverages **HTMX** for reactivity. You get the feel of a Single Page App (SPA) with the simplicity of Multi-Page Architecture (MPA).
* **Resource Efficiency:** Runs on **15-20MB of RAM**. Perfect for low-cost VPS, Raspberry Pi, or edge computing.
* **Pterodactyl Ready:** Deploy instantly using the official Majest Egg.

---

## 🛠 The Architecture

Majest splits the world into two rings:

1.  **The Ring 0 (Go):** Handles routing, security filtering, database pooling, and template compilation. It acts as the "Hardware" that protects the system.
2.  **The User Space (Lua):** Your application logic. Fast, lightweight, and isolated. No more `node_modules` dependency hell.

---

## 📦 Project Structure

```text
.
├── core/                // Go "Kernel" logic (Server, Bridge, Security)
├── internal/            // Internal Lua-to-Go APIs
├── app/                 // User Application Space
│   ├── controllers/     // Logic written in Lua
│   ├── views/           // .gxd templates (HTML + Lua)
│   └── static/          // Minified assets (HTMX, CSS)
├── majest.json          // Framework configuration
└── main.go              // The Entry Point
```

---

## 🏗 Installation (Coming Soon)

Once the first stable build is released on `gxd.bloby.eu`, you will be able to install Majest as a single static binary:

---

## 🎯 Roadmap

- [ ] **Alpha 0.1:** Core Go-Lua bridge with `sync.Pool` implementation.
- [ ] **Security:** Context-aware auto-escaping for all `.gxd` templates.
- [ ] **Deployment:** Official Pterodactyl Egg for one-click hosting.
- [ ] **Edge:** Vercel Runtime integration for Go-based Serverless functions.

---

## 🛡 License

Majest is released under the **MIT License**. Keep it open, keep it fast.
```

Tento formát zajistí, že na GitHubu nebo tvém webu uvidíš krásné nadpisy, tučný text a přehledné bloky kódu. Chceš tam ještě doplnit nějaké specifické **TODO** úkoly, které máš v hlavě?
