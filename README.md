# 📊 API Testing with Postman & Newman - FakeREST API

This project contains a collection of **Postman API tests** for the [FakeREST API](https://fakerestapi.azurewebsites.net/), along with instructions to run them using **Newman**, Postman's CLI tool.

---

## 📌 Project Structure

```
├── postman/
│   ├── FakeREST.postman_collection.json     # Main Postman collection
│   └── FakeREST.postman_environment.json    # Postman environment file (optional)
├── reports/
│   └── newman/                              # Newman reports (auto-generated)
├── README.md                                # Project documentation
```

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/fakerest-api-testing.git
cd fakerest-api-testing
```

### 2. Install Dependencies

Make sure you have **Node.js** and **npm** installed. Then install Newman globally:

```bash
npm install -g newman
```

---

## ▶️ Running Tests

### Run Collection via Newman

```bash
newman run postman/FakeREST.postman_collection.json
```

### Run with Environment File

```bash
newman run postman/FakeREST.postman_collection.json -e postman/FakeREST.postman_environment.json
```

### Generate HTML Report (Optional)

Install the Newman HTML reporter:

```bash
npm install -g newman-reporter-html
```

Run with HTML reporting:

```bash
newman run postman/FakeREST.postman_collection.json \
    -r html --reporter-html-export reports/newman/report.html
```

---

## ✅ Test Coverage

The collection includes tests for:

- 🗂️ **Activities**
- 👤 **Authors****
- 📚 **Books**
- 📷 **Cover Photos**
- 👤 **Users**

---

## 📄 Resources

- [FakeREST API Docs](https://fakerestapi.azurewebsites.net/index.html)
- [Postman](https://www.postman.com/)
- [Newman CLI](https://www.npmjs.com/package/newman)

---

## 📬 Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you'd like to change.

---

## 📝 License

This project is licensed under the MIT License.

