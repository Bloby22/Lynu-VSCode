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

## 🛡 License

Majest is released under the **MIT License**. Keep it open, keep it fast.
