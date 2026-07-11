# LRU Cache Simulator

[![Live Demo](https://img.shields.io/badge/Live-Demo-success?style=for-the-badge)](https://lru-cache-livid.vercel.app/)
[![Hosted on Vercel](https://img.shields.io/badge/Hosted%20on-Vercel-black?style=for-the-badge&logo=vercel)](https://lru-cache-livid.vercel.app/)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-yellow?style=for-the-badge&logo=javascript)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![HTML5](https://img.shields.io/badge/HTML5-orange?style=for-the-badge&logo=html5)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-blue?style=for-the-badge&logo=css3)](https://developer.mozilla.org/en-US/docs/Web/CSS)

## 🌐 Live Demo

🚀 **Try the application here:**

https://lru-cache-livid.vercel.app/

---

## 📖 Overview

The **LRU Cache Simulator** is a modern and interactive web application designed to visualize how the **Least Recently Used (LRU) Cache** algorithm works internally.

The project demonstrates the complete working of an LRU cache using:

- **HashMap** for O(1) lookup.
- **Doubly Linked List** for O(1) insertion and deletion.
- Real-time cache visualization.
- Step-by-step cache updates.
- Hit/Miss tracking and cache statistics.

This project helps students and developers understand one of the most frequently asked data structures in technical interviews.

---

## ✨ Features

### 🔹 Dynamic Cache Visualization
- Visual representation of cache nodes.
- Displays the order of recently used and least recently used items.
- Automatically updates after every operation.

### 🔹 HashMap Visualization
- Shows key-to-node mapping.
- Demonstrates how O(1) lookup is achieved.

### 🔹 Interactive Operations
Users can perform:

- `PUT(key, value)`
- `GET(key)`
- Change cache capacity dynamically.
- Reset the cache.

### 🔹 Operation Logs
- Displays every operation performed.
- Shows cache hits and misses.
- Useful for understanding cache behavior.

### 🔹 Statistics Dashboard
Tracks:

- Total Requests
- Cache Hits
- Cache Misses
- Hit Rate Percentage

### 🔹 Responsive UI
- Desktop support
- Tablet support
- Mobile support

### 🔹 Premium User Interface
- Glassmorphism design
- Smooth animations
- Gradient effects
- Dark mode inspired color palette

---

## 🧠 How LRU Cache Works

The **Least Recently Used (LRU)** caching strategy removes the item that has not been accessed for the longest time when the cache becomes full.

### Example

Assume cache capacity = **3**

| Operation | Cache State |
|-----------|------------|
| PUT(1,A) | 1 |
| PUT(2,B) | 2 → 1 |
| PUT(3,C) | 3 → 2 → 1 |
| GET(1) | 1 → 3 → 2 |
| PUT(4,D) | 4 → 1 → 3 |

Since key **2** was the least recently used item, it gets removed.

---

## ⚙️ Internal Data Structures

### 1. HashMap

Stores:

```text
key -> Node reference
