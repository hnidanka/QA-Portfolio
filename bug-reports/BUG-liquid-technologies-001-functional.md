# [BUG-liquid-technologies-001]

**ID:** BUG-liquid-technologies-001  
**Summary:** JSON Schema converter fails to generate results and returns response status 503  
**Status:** New 🟢  
**Author:** Sofiia Hnidan  
**Type:** Functional  
**Severity:** Blocker  
**Priority:** High

---

### 🌐 Environment
* **Browsers:** 
  * Safari Version 17.6 (19618.3.11.11.5)
  * Chrome Version 145.0.7632.160 (Official Build, arm64)
  * Firefox 148.0 (aarch64)
    
---

### Preconditions
* **Browsers:** Navigate to: https://www.liquid-technologies.com/online-json-to-schema-converter
* **"Copy JSON file structure to clipboard:**  
[
    {
        ""id"": ""69d2584b7ab8c4c2f320b507"",
        ""name"": ""enterprise Chief Shoals Trafficway"",
        ""idBoard"": ""69d2389ed168a9a46174b960"",
        ""idCard"": ""69d253cfbc47dfc785442daa"",
        ""pos"": 665,
        ""checkItems"": []
    }
]"

---

### 👣 Steps to Reproduce
1. Paste the copied JSON structure into the **JSON Input Area**.
3. Check the **"Data Security Warning"** checkbox.
4. Click the **"Generate Schema"** button.
5. Observe the loading icon and wait for the process to finish.
6. Scroll down to browse the schema conversion result.

### ❌ Actual Result
* JSON Sheme is not generated.
* The server responds with a **503 Service Unavailable** error in the **Network** tab.
* Console logs: `Failed to load resource: the server responded with a status of 503 ()`.

### ✅ Expected Result
JSON Sheme is generated
---

### 🖼️ Attachment
![Bug Screenshot nr 1]: https://i.ibb.co/DHs9MxZ6/Screenshot-2026-04-05-at-19-55-05.png  
![Bug Screenshot nr 2]: https://i.ibb.co/mVJpcTrX/Screenshot-2026-04-05-at-19-56-26.png

