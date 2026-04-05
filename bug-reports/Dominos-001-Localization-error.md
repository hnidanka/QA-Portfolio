# [BUG-DOMINOS-001]

**ID:** BUG-Dominos-001  
**Summary:** The Ukrainian translation for menu cards is missing  
**Status:** New 🟢  
**Author:** Sofiia Hnidan  
**Type:** Localization  
**Severity:** Minor  
**Priority:** Low

---

### 🌐 Environment
* **Browsers:** 
  * Safari Version 17.6 (19618.3.11.11.5)
  * Chrome Version 145.0.7632.160 (Official Build, arm64)
  * Firefox 148.0 (aarch64)
    
---

### Preconditions
* **Browsers:** Navigate to: https://www.dominospizza.pl

---

### 👣 Steps to Reproduce
1. Click the **'Language switcher'** button in the header.
2. Select **Ukrainian** from the dropdown list.
3. Verify that the URL changes to `https://www.dominospizza.pl/uk-ua`.
4. In the delivery popup (`m-PopupChangePlace__list`), set the option to **'Доставка'**.
5. Fill in the delivery form with valid data (e.g., *City: Szczecin, Street: Monte Cassino, House: 4*).
6. Submit the form and ensure the menu page `../uk-ua/menu/promocje` is loaded.
7. Scroll down and browse all available menu cards.
8. Verify the translations for each card.

### ❌ Actual Result
Certain menu card titles and descriptions remain in **Polish**, even though the global language setting is Ukrainian.

### ✅ Expected Result
All menu card titles, descriptions, and promotional content should be fully translated into **Ukrainian**.

---

### 🖼️ Attachment
![Bug Screenshot] https://i.ibb.co/h1LQVTHS/Screenshot-2026-04-05-at-19-16-56.png


