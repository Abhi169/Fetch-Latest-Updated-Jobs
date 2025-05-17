# Fetch-Latest-Updated-Jobs
A RESTful API that provides real-time job listings with support for filtering by country, job type, remote roles, and keyword search. Updated daily with 2000+ new jobs — perfect for job boards, career apps, and market research.

# 🔍 Jobs API

A fast, flexible, and developer-friendly RESTful API that delivers **real-time job listings** across regions, companies, and job types. Updated **daily with 2000+ new jobs**, this API is ideal for job boards, career websites, and analytics platforms.

---

## 🚀 Features

- ✅ Fetch latest job listings with pagination and sorting.
- 🌍 Filter jobs by country.
- 🧑‍💻 Filter by job type (Full Time, Part Time, Internship).
- 🔎 Search jobs by keyword or technology (Node.js, Java, C++, etc.).
- 🆔 Retrieve specific jobs by unique ID.
- 🌐 Supports remote job filtering.
- ⚡ JSON responses with structured and clean data.
- 🛡️ Input validation and error handling included.

---

## 📦 Available Endpoints

### `GET /api/jobs`
Fetch the latest job listings.  
**Query Parameters:**
- `limit` – Number of results (default: 10, max: 100)
- `skip` – Number of items to skip
- `sortBy` – Sort field: `createdAt` or `updatedAt`
- `order` – `asc` or `desc`

---

### `GET /api/job?id=...`
Fetch a job by its **unique ID**.

---

### `GET /api/country?country=...`
Fetch jobs available in a **specific country**.

---

### `GET /api/jobtype?jobtype=...`
Filter jobs by **job type**: `Full Time`, `Part Time`, `Internship`, etc.

---

### `GET /api/remote?remote=true|false`
Fetch **remote jobs** based on boolean value.

---

### `GET /api/jobSearch?search=...`
Search for jobs using **keywords or technologies**, like `Java`, `C++`, `Node`, `Frontend`, `Fullstack`, etc.

---

## 🧪 Sample Response

```json
{
  "title": "Frontend Developer",
  "company": {
    "name": "Example Company",
    "website_url": "https://example.com"
  },
  "location": "Remote, India",
  "job_type": "Full Time",
  "experience_level": "Mid",
  "application_url": "https://example.com/careers/frontend",
  "createdAt": "2025-05-03T11:29:25.387Z"
}
```
---

## ⚠️ Error Handling

**400** Bad Request – Invalid parameters

**404** Not Found – No matching jobs

**500** Internal Server Error – Unexpected server error

---

## 📈 Use Cases

### Job board platforms

### Career portals

### Developer dashboards

### Market research and analytics tools

---

## 📬 Feedback

Have suggestions or feedback to improve this API?
Reach out or open an issue! Your input is appreciated.

---
