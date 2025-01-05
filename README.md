# Frappe-bench-commands-for-developers
This document provides a comprehensive list of Frappe Bench commands for enabling scripts, developer mode, and other useful developer functionalities. 

## Table of Contents  
1. [Enable Developer Mode](#enable-developer-mode)  
2. [Custom Scripts Management](#custom-scripts-management)  
3. [Scheduler Management](#scheduler-management)  
4. [Error Logs](#error-logs)  
5. [Email Notifications](#email-notifications)  
6. [Maintenance Mode](#maintenance-mode)  
7. [Multitenancy](#multitenancy)  
8. [Auto-reloading](#auto-reloading)  
9. [Debugging Tools](#debugging-tools)  
10. [Custom Method Execution](#custom-method-execution)  

---

## Enable Developer Mode  
Enable and disable developer mode to allow customization and advanced features.  

```bash
# Enable Developer Mode
bench set-config developer_mode 1

# Disable Developer Mode
bench set-config developer_mode 0
```

---

## Custom Scripts Management  
Enable or disable client-side custom JavaScript scripts.  

```bash
# Enable Custom Scripts
bench set-config allow_js_scripts true

# Disable Custom Scripts
bench set-config allow_js_scripts false
```

---

## Scheduler Management  
Manage the background job scheduler for your site.  

```bash
# Enable Scheduler
bench enable-scheduler

# Disable Scheduler
bench disable-scheduler
```

---

## Error Logs  
Enable error logging for debugging purposes.  

```bash
# Enable Error Logs
bench set-config log_error true
```

---

## Email Notifications  
Enable or disable system email notifications.  

```bash
# Enable Email Notifications
bench set-config enable_email_notifications true

# Disable Email Notifications
bench set-config enable_email_notifications false
```

---

## Maintenance Mode  
Put the site in maintenance mode or remove it from maintenance mode.  

```bash
# Enable Maintenance Mode
bench set-maintenance-mode on

# Disable Maintenance Mode
bench set-maintenance-mode off
```

---

## Multitenancy  
Enable or disable DNS-based multitenancy for Frappe.  

```bash
# Enable Multitenancy
bench config dns_multitenant on

# Disable Multitenancy
bench config dns_multitenant off
```

---

## Auto-reloading  
Automatically reload assets when changes are made.  

```bash
# Enable Auto-reloading
bench watch
```

---

## Debugging Tools  
Enable or disable debugging tools and methods.  

```bash
# Enable Debugging
bench set-config disable_debugger false

# Disable Debugging
bench set-config disable_debugger true
```

---

## Custom Method Execution  
Execute custom Python methods for debugging or testing purposes.  

```bash
# Execute a Custom Method
bench execute path.to.method
```
Replace `path.to.method` with the full Python path of the method you want to execute.

---

## Notes  
- Use these commands cautiously, especially in a production environment.  
- Always backup your data before making significant changes to the system.  
