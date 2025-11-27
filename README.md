# 🛠️ User Configuration Manager (Python)

This project is a simple configuration manager built in Python that allows users to manage customizable settings such as theme, language, and notifications. It includes functionality to **add**, **update**, **delete**, and **view** user preferences in a clean and structured way.

This project was completed as part of the **FreeCodeCamp – Scientific Computing with Python Certification**.

---

## 📌 Features

### ✔ Add new settings  
- Automatically converts key and value to lowercase  
- Prevents adding duplicate settings  

### ✔ Update existing settings  
- Converts key and value to lowercase  
- Ensures the setting exists before updating  

### ✔ Delete settings  
- Only deletes if the key exists  
- Standardized lowercase validation  

### ✔ View settings  
- Displays all settings in a clean formatted list  
- Capitalizes setting names for readability  
- Shows a friendly message if no settings exist  

---

## 📂 Functions Included

### `add_setting(settings, setting_tuple)`  
Adds a new key/value pair to the settings dictionary.

### `update_setting(settings, setting_tuple)`  
Updates an existing setting.

### `delete_setting(settings, key)`  
Deletes a setting by key.

### `view_settings(settings)`  
Displays all settings in a formatted output.

---

## 🧪 Example Usage

```python
settings = {}

print(add_setting(settings, ("Theme", "Dark")))
print(add_setting(settings, ("Language", "English")))
print(update_setting(settings, ("theme", "light")))
print(delete_setting(settings, "language"))

print(view_settings(settings))
