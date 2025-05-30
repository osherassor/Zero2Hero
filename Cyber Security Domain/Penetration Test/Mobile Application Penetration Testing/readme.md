## 📱 Mobile Application Penetration Testing

### 📲 Goals & Scope
- Identify vulnerabilities in Android and iOS mobile apps
- Evaluate communication security, local storage security, and runtime protections
- Ensure applications comply with OWASP MASVS (Mobile App Security Verification Standard)

---

### 🧱 Mobile Application Architectures

Different development models impact the security posture and the types of vulnerabilities:

#### 📱 Native Applications
- **Definition**: Apps developed using platform-specific languages (Java/Kotlin for Android, Swift/Objective-C for iOS)
- **Security Considerations**:
  - Direct access to OS-level APIs
  - Vulnerable to insecure storage, debug features, misuse of system permissions
  - Static and dynamic analysis are both crucial

#### 🌐 WebView-based Applications
- **Definition**: Embed a web browser view within a native wrapper
- **Technology**: HTML, JavaScript, CSS (remote or local)
- **Security Considerations**:
  - Susceptible to web vulnerabilities like XSS or insecure `addJavascriptInterface`
  - Weak SSL/TLS validation, mixed content issues
  - Can be tested with a combination of web and mobile tools

#### ⚛ Hybrid Frameworks
- **React Native**:
  - Cross-platform development using JavaScript and native UI bindings
  - Vulnerable to exposed bridges and logic flaws in both JS and native code
- **Flutter**:
  - Uses Dart, compiles to native code with a reactive UI model
  - Runtime manipulation more difficult, but still susceptible to insecure logic or improper storage
- **Cordova / Ionic**:
  - Rely on WebViews with native plugin access
  - Expose both mobile and web attack surfaces

| Architecture     | Language/Framework      | Attack Surfaces                      | Notes                                      |
|------------------|--------------------------|---------------------------------------|---------------------------------------------|
| Native           | Java, Kotlin, Swift      | OS APIs, Local Storage, Permissions   | Decompilation and runtime analysis critical |
| WebView          | HTML/JS + Native Shell   | XSS, insecure JS interfaces, TLS      | Web + mobile hybrid threats                 |
| React Native     | JavaScript + Native Bindings | Bridge exposure, logic flaws     | Needs Frida/Objection + JS review          |
| Flutter          | Dart (compiled to native) | Channel injection, secure storage     | Binary-level inspection needed              |

---

### ⚙️ Environment Setup

#### 🔧 Android
- Rooted device or emulator
- Tools: `adb`, `jadx`, `Frida`, `objection`, `MobSF`, `apktool`, `Ghidra`

#### 🍏 iOS
- Jailbroken device or simulator with decrypted IPA
- Tools: `Frida`, `class-dump`, `Cycript`, `Hopper`, `idevicesyslog`, `MobSF`

---

### 🔍 Static Analysis (SAST)
- Decompile APK or IPA and review:
  - Android: `AndroidManifest.xml`, hardcoded credentials, exported components
  - iOS: `Info.plist`, exposed URL schemes, ATS settings
- Check for:
  - Insecure cryptographic usage
  - Root/jailbreak detection logic
  - Debuggable flags and insecure logs

---

### 🏃 Dynamic Analysis (DAST)
- Proxy traffic with Burp or mitmproxy
- Bypass SSL pinning (Frida, Objection)
- Hook runtime functions to monitor behavior:
  - Login, session tokens
  - API request/response logic
  - Local storage manipulation

---

### 🧠 Business Logic Testing
- Attempt authentication/authorization bypass
- Test for IDOR and insecure session management
- Manipulate intents, deep links, URL schemes

---

### 🔐 Local Storage Security
- Inspect:
  - Android: `SharedPreferences`, SQLite, internal storage
  - iOS: `NSUserDefaults`, Plist files, CoreData, Keychain
- Detect sensitive data stored in plaintext:
  - Access tokens, PII, credentials
- Analyze encryption logic (e.g., AES key handling)

---

### 🛰 Communication Security
- Enforce HTTPS and strong TLS settings
- Test for:
  - Certificate pinning bypass
  - Token leakage in headers or query parameters
  - Unencrypted traffic

---

### 🧩 Reverse Engineering & Tampering
- Use jadx, Hopper, Frida to inspect and manipulate code
- Patch APKs (smali), bypass controls (e.g., root detection)
- Run custom Frida scripts to hook functions like:
  - `checkRootAccess()`, `isEmulator()`, `verifySignature()`

---

### 🛑 OWASP Mobile Top 10 (2023)
| ID   | Name                               |
|------|------------------------------------|
| M1   | Improper Platform Usage            |
| M2   | Insecure Data Storage              |
| M3   | Insecure Communication             |
| M4   | Insecure Authentication            |
| M5   | Insufficient Cryptography          |
| M6   | Insecure Authorization             |
| M7   | Client Code Quality Issues         |
| M8   | Code Tampering                     |
| M9   | Reverse Engineering                |
| M10  | Extraneous Functionality           |

---

### 📦 Deliverables
- Summary of findings (mapped to OWASP & MASVS)
- Burp logs, Frida scripts, APK modifications
- Screenshots and reproduction steps
- Severity ranking with CVSS or custom scoring
- Remediation guidance and architectural suggestions
- Executive summary and technical appendix

---

### 📚 Reference Standards
- **OWASP MASVS**: https://owasp.org/www-project-mobile-app-security/
- **OWASP Mobile Testing Guide**: https://owasp.org/www-project-mobile-security-testing-guide/
