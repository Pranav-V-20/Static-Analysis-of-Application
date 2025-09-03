
# Static Analysis of VulnHub Mobile Application with MobSF

This project demonstrates how to perform **static analysis** on the [Dawn-Vulnerable-Bank](https://github.com/dawn/DAWN-Vulnerable-Bank) Android application using [Mobile Security Framework (MobSF)](https://github.com/MobSF/Mobile-Security-Framework-MobSF).

---

## 🔧 MobSF Installation (using Podman)

First, pull the latest MobSF container image:

```bash
podman pull docker.io/opensecurity/mobile-security-framework-mobsf:latest
````

---

## ▶️ Running MobSF

Start MobSF on port `8000`:

```bash
docker run -it --rm -p 8000:8000 opensecurity/mobile-security-framework-mobsf:latest
```

Access the MobSF web interface:

* URL: [http://localhost:8000](http://localhost:8000)
* **Username:** `mobsf`
* **Password:** `mobsf`

<img width="1816" height="1018" alt="Screenshot 2025-09-03 234046" src="https://github.com/user-attachments/assets/67fff25e-dfe0-4efd-891c-57e7faf83642" />

---

## 📱 Target Application

For this analysis, we used the **Vulnub app** from the Dawn-Vulnerable-Bank repository:

👉 [Dawn-Vulnerable-Bank on GitHub](https://github.com/dawn/DAWN-Vulnerable-Bank)

<img width="1823" height="1017" alt="Screenshot 2025-09-03 234127" src="https://github.com/user-attachments/assets/88c34638-af05-40c5-bdff-8a11820d60ed" />

---

## 🧪 Static Analysis Process

1. Download the vulnerable APK from the Dawn-Vulnerable-Bank repository.
2. Log in to MobSF.
3. Upload the APK for static analysis.
4. Review the findings:

   * Insecure storage
   * Hardcoded secrets
   * Weak crypto
   * Exported activities
   * Other vulnerabilities flagged by MobSF

---

## 📊 Results

MobSF generated a detailed report highlighting multiple security issues in the Dawn-Vulnerable-Bank app. These findings can be used for further **penetration testing** and **dynamic analysis**.

---

## 🚀 Next Steps

* Extend the analysis with **dynamic testing** in MobSF.
* Exploit identified vulnerabilities in a controlled environment.
* Document remediation strategies for secure mobile app development.

---

## ⚠️ Disclaimer

This project is for **educational purposes only**. Do not use MobSF or the vulnerable application against systems you do not own or have explicit permission to test.

```
