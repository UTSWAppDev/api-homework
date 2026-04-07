# APIs and FHIR – Python Homework Exercise
## MS Health Informatics · Application Development · UT Southwestern Medical Center

---

## Overview

This repository contains a guided Jupyter notebook that introduces Master of Science in Health Informatics students to **REST APIs** and **FHIR** (Fast Healthcare Interoperability Resources) using Python.

By the end of the exercise students will be able to:

- Explain what a REST API is and what a **resource URI** represents
- Send **GET**, **POST**, **PUT**, and **DELETE** HTTP requests using the Python `requests` library
- Parse and work with **JSON** responses
- Retrieve, create, update, and delete **FHIR Patient** resources on a sandbox FHIR R4 server

---

## Concepts Covered

### REST APIs

**REST** (Representational State Transfer) is an architectural style that leverages standard HTTP methods to exchange data between a client and a server. A REST API exposes a set of **resource URIs** — unique addresses that identify pieces of data. Clients interact with those resources using the following HTTP methods:

| Method   | Action                                |
|----------|---------------------------------------|
| `GET`    | Retrieve a resource                   |
| `POST`   | Create a resource        |
| `PUT`    | Update a resource    |
| `DELETE` | Remove a resource                     |

### JSON

**JSON** (JavaScript Object Notation) is the most common data format used in REST APIs. It represents structured data as human-readable key-value pairs and is natively supported by Python's standard library (`json` module) as well as the `requests` library (`.json()` method).

### FHIR

**FHIR** (Fast Healthcare Interoperability Resources, pronounced "fire") is an HL7 standard for exchanging healthcare information electronically. It models every type of clinical data — patients, observations, medications, appointments — as a **resource** with a well-defined structure and its own REST URI.

For example, a Patient resource lives at:

```
https://<fhir-server>/Patient/<id>
```

This exercise uses the publicly accessible **SMART Health IT FHIR R4 sandbox** (`https://r4.smarthealthit.org`) which allows unauthenticated read and write operations for learning purposes.

---

## Files

| File | Description |
|------|-------------|
| `api_homework.ipynb` | Main Jupyter notebook with all exercises |
| `README.md` | This file |
| `index.html` | Course landing page |
| `styles.css` | Stylesheet for the landing page |

---

## Getting Started

### Running the Notebook

#### Codespaces
Create new Codespace
Open the `api_homework.ipynb` and begin following the instructions in the notebook

#### Running locally

```bash
# Clone the repository (if you haven't already)
git clone https://github.com/UTSWAppDev/api-homework.git
cd api-homework

# Install dependencies
pip install notebook requests

# Launch Jupyter
jupyter notebook api_homework.ipynb
```

Then follow the cells from top to bottom, reading the explanations and executing the code.

---

## External APIs Used

| API | Documentation |
|-----|---------------|
| Joke API (`official-joke-api.appspot.com/random_joke`) | -------------|
| SMART Health IT FHIR R4 Sandbox (`r4.smarthealthit.org`) | https://docs.smarthealthit.org/ |

---

## Additional Resources

- [HL7 FHIR R4 Specification](https://hl7.org/fhir/R4/)
- [SMART on FHIR](https://docs.smarthealthit.org/)
- [Python `requests` library](https://requests.readthedocs.io/)
- [JSON specification](https://www.json.org/)
