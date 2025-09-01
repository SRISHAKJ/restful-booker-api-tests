**Restful Booker API Test**

[![API Tests](https://github.com/SRISHAKJ/restful-booker-api-tests/actions/workflows/api-tests.yml/badge.svg)]

**Overview**
This project contains automated API tests for the [Restful Booker API](https://restful-booker.herokuapp.com/).  
It uses **Postman** for request design, **Newman** for CLI execution, and **GitHub Actions** for CI/CD integration.  

**Tech Stack**
- Postman (Collections & Environments)
- Newman (CLI test runner)
- GitHub Actions (CI/CD)
- htmlextra reporter (detailed HTML reports)

**View Detailed Test report**
[Click here to view report](https://github.com/SRISHAKJ/restful-booker-api-tests/blob/main/report.html)

**How to Run Locally**
Clone the repo and run the following:
```bash
npm install -g newman newman-reporter-htmlextra
newman run "Restful Booker API Tests.postman_collection.json" \
  -e "Restful Booker Env.postman_environment.json" \
  -r htmlextra --reporter-htmlextra-export report.html




