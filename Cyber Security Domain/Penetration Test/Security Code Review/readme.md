## 🧾 Security Code Review (Source Code Analysis)

### 🎯 Purpose & Goals
- Identify security vulnerabilities in source code before production
- Understand the flow of data and control across the application
- Detect insecure coding practices and logic flaws early

### 🛠 Tools & Setup
- **Static Analysis Tools**:
  - [Semgrep](https://semgrep.dev/)
  - [SonarQube](https://www.sonarsource.com/products/sonarqube/)
  - [Checkmarx](https://checkmarx.com/)
  - [Fortify SCA](https://www.microfocus.com/en-us/products/static-code-analyzer-sast/overview)
  - [Brakeman (Ruby)](https://brakemanscanner.org/)
- **Linters**:
  - [ESLint (JavaScript)](https://eslint.org/)
  - [Pylint (Python)](https://pylint.pycqa.org/)
  - [RuboCop (Ruby)](https://github.com/rubocop/rubocop)
- **IDE Plugins**:
  - [Visual Studio Code Security Extensions](https://marketplace.visualstudio.com/)
  - [IntelliJ Security Code Scan Plugins](https://plugins.jetbrains.com/)
- **Source Control Hooks**:
  - [Pre-commit hooks](https://pre-commit.com/)
  - [GitLeaks](https://github.com/gitleaks/gitleaks) for secrets detection

### 🧪 Common Vulnerability Categories to Identify
- Input validation issues: **XSS**, **SQL Injection**, **Command Injection**
- Broken authentication and session management
- Insecure file handling: **Path Traversal**, unrestricted upload
- Cryptographic flaws: hardcoded keys, weak encryption, insecure randomness
- Insecure API/library usage (e.g., outdated or unsafe dependencies)
- Poor error handling & missing security logs
- Race conditions and **Time-of-check to time-of-use (TOCTOU)**
- Business logic errors (e.g., privilege escalation, bypass flows)

### 🔍 Code Analysis Techniques
- **Taint Analysis**: Trace untrusted input to sensitive sinks  
  - [Semgrep Taint Rules](https://semgrep.dev/docs/writing-rules/taint-tracking/)
- **Control Flow Analysis**: Map conditions and branches that affect decision logic
- **Data Flow Tracing**: Understand how data moves across modules and functions
- Manual review:
  - Authentication and Authorization modules
  - File handling
  - Custom cryptography
  - Input parsing

### 🔐 Secure Coding Standards
- [OWASP Secure Coding Practices](https://owasp.org/www-project-secure-coding-practices/)
- [SEI CERT Guidelines](https://wiki.sei.cmu.edu/confluence/display/seccode) (C/C++, Java, etc.)
- Language-specific:
  - [Python Security Guidelines](https://cheatsheetseries.owasp.org/cheatsheets/Python_Security_Cheat_Sheet.html)
  - [Java Secure Coding Guide](https://www.oracle.com/java/technologies/javase/seccodeguide.html)
  - [.NET Secure Coding Guidelines](https://learn.microsoft.com/en-us/dotnet/standard/security/secure-coding-guidelines)

### 🧰 Automation & CI/CD Integration
- Embed scanners into:
  - [GitHub Actions](https://github.com/features/actions)
  - [GitLab CI/CD](https://docs.gitlab.com/ee/ci/)
  - [Jenkins](https://www.jenkins.io/)
- Define fail conditions for high/critical issues
- Schedule periodic full scans to detect regression
- Use security dashboards to track technical debt and fix SLAs

### 📂 Deliverables
- Vulnerability summary table with:
  - Severity
  - CWE reference ([CWE Database](https://cwe.mitre.org/))
  - Affected file/function
- Annotated code snippets
- Fix recommendations using secure coding patterns
- Integration roadmap for DevSecOps teams
- Executive summary for non-technical stakeholders
