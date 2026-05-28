# Express API Gen Actions

A VS Code extension for generating modular Express.js CRUD API action structures automatically.

Repository:

[vs-code-ext-express-api-gen-actions Repository](https://github.com/keshavsoft/vs-code-ext-express-api-gen-actions?utm_source=chatgpt.com)

---

# Features

* Generate Express API actions automatically
* Generate CRUD endpoint structure
* Create modular backend architecture
* Auto-create route files
* Organized controller/service pattern
* JSON-based backend support
* Faster API development
* Reduce boilerplate Express code

---

# Generated Folder Structure

Example generated structure:

```txt id="jlwm1"
Api/
   V1/
      Journals/

         Alter/
         Config/
         Delete/
         Insert/
         ShowAll/

         end-points.js

      routes.js

routes.js
```

---

# Folder Explanation

| Folder/File     | Purpose                   |
| --------------- | ------------------------- |
| `ShowAll`       | Read all records          |
| `Insert`        | Insert new record         |
| `Alter`         | Update existing record    |
| `Delete`        | Delete record             |
| `Config`        | API configuration         |
| `end-points.js` | Defines Express endpoints |
| `routes.js`     | Connects routers          |

---

# CRUD Actions

The extension generates CRUD API actions automatically.

| Action    | HTTP Method | Purpose         |
| --------- | ----------- | --------------- |
| `ShowAll` | GET         | Read all data   |
| `Insert`  | POST        | Create new data |
| `Alter`   | PUT/PATCH   | Update data     |
| `Delete`  | DELETE      | Remove data     |

---

# API Architecture

```txt id="’wini2"
Browser / Frontend
        ↓
Endpoint
        ↓
routes.js
        ↓
end-points.js
        ↓
controller.js
        ↓
service.js
        ↓
JSON/File Storage
```

# Generated Endpoints

Final endpoints become:

```txt id="’wini6"
GET    Api/V1/Journals/ShowAll
POST   Api/V1/Journals/Insert
PUT    Api/V1/Journals/Alter
DELETE Api/V1/Journals/Delete
```

---

# Example JSON Storage

## Data/Journals.json

```json id="’wini11"
[
  {
    "id": 1,
    "title": "Daily Entry",
    "amount": 500
  },
  {
    "id": 2,
    "title": "Office Expense",
    "amount": 1200
  }
]
# Benefits

* Faster Express API creation
* Clean architecture
* Organized backend structure
* Reusable API modules
* Automatic route generation
* Easier maintenance

---

# Example Workflow

## Generate Journals API

Generated structure:

```txt id="’wini14"
Api/
   V1/
      Journals/
         ShowAll/
         Insert/
         Alter/
         Delete/
```

---

# Technologies

* Node.js
* Express.js
* Express Router
* JSON Storage
* CRUD APIs
* Modular Backend Architecture

---

# Repository

[vs-code-ext-express-api-gen-actions GitHub Repository](https://github.com/keshavsoft/vs-code-ext-express-api-gen-actions?utm_source=chatgpt.com)
