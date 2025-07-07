
# Day 24 – Custom Connectors: Consume External APIs in Power Apps

---

## 📝 Overview

Custom connectors in Power Platform allow you to connect your apps and flows to external APIs. This is especially useful when no built-in connector exists or when you want to securely access your company’s RESTful services.

Today you’ll learn how to create a custom connector using an OpenAPI (Swagger) definition or a manual setup, and then use it in Power Apps or Power Automate.

---

## 🧭 Step-by-Step Guide

### ✅ Step 1: Prepare the API Info

1. Get the **Base URL** of the API (e.g., `https://api.example.com`)
2. Obtain documentation or a **Swagger/OpenAPI file**
3. Ensure you have any required:
   - **API keys**
   - **OAuth 2.0 credentials**
   - **Authentication headers**

---

### ✅ Step 2: Create the Custom Connector

1. Go to [https://make.powerapps.com](https://make.powerapps.com)
2. Click **Custom connectors > + New custom connector**
3. Choose one:
   - **Import an OpenAPI file**
   - **Create from blank**
4. Fill in:
   - **Connector name**
   - **Host and Base URL**
   - **Authentication method**

---

### ✅ Step 3: Define Actions

1. Go to the **Definition** tab
2. Click **+ New action**
3. Set:
   - **Summary** (e.g., Get Weather)
   - **Operation ID** (unique name)
   - **Request parameters** (e.g., city, zip code)
   - **Response format** (JSON output)
4. Test with sample values or import from the Swagger file

---

### ✅ Step 4: Test the Connector

1. Save and click **Test**
2. Enter required inputs
3. Review the API response
4. Make sure it returns the expected result (JSON or values)

---

### ✅ Step 5: Use in Power Apps or Power Automate

**In Power Apps:**
1. Go to **Data > Add data**
2. Search for and add your custom connector
3. Use it like any other data source:
   ```powerfx
   MyConnector.GetWeather("Dallas")
   ```

**In Power Automate:**
1. Add an action
2. Search for your custom connector
3. Pass input parameters and map outputs

---

## 🔎 What You Should Try Today

- Create a custom connector to a public API (e.g., weather, currency, news)
- Test GET and POST actions
- Use the connector in a Power App or a scheduled flow

---

## 🔁 Navigation

⬅️ [**Go to Day 23: Power Virtual Agents & Copilot Studio – build your first chatbot**](/PowerPlatform/Power%20Platform%2030%20days/Day23.md)  
➡️ [**Go to Day 25: PDF generation, emails, and attachments using Power Automate**](/PowerPlatform/Power%20Platform%2030%20days/Day25.md)
