# GitHub Advanced Security Technical Documentation

## Need?
  - Enabling Security in the BUILD pipelines is crucial because it helps detect vulnerabilities early in the development cycle, protect sensitive information, and ensure fast, secure delivery of software.

## 🔧 Security Features/Tools Enabled in GitHub
1. **CodeQL**: Static code analysis engine that automatically finds vulnerabilities in Python code.
2. **Dependabot**: Dependency graph scanner that detects vulnerable versions in `requirements.txt` and Docker images.
3. **GitHub Secret Scanning**: Flags hardcoded credentials like AWS access keys, passwords, and tokens.

## 📸 Screenshots Attached
- [GHAS enabled](https://github.com/vijayjirange/python-demoapp/blob/master/GHAS.png)
- [Dependabot output](https://github.com/vijayjirange/python-demoapp/blob/master/dependabot.png)
- [Code Scanning output](https://github.com/vijayjirange/python-demoapp/blob/master/CodeScanning.png)
- [Secret Scanning output](https://github.com/vijayjirange/python-demoapp/blob/master/SecretScanning.png)

## 🔐 Key Benefits of GitHub Advanced Security
1. **Code Scanning (Static Analysis)**  
   - Automatically scans code for security vulnerabilities and coding errors using CodeQL, GitHub’s semantic analysis engine.  
   - Finds flaws like buffer overflows, SQL injection, path traversal, etc.  
   - Results are shown directly in pull requests, making it easy to fix before merging.

2. **Secret Scanning**  
   - Detects hardcoded secrets (API keys, credentials, tokens) accidentally committed to the repo.  
   - Scans both new commits and historical data (if enabled).  
   - GitHub can notify the secret provider to automatically revoke or rotate the exposed secret.

3. **Dependency Review**  
   - Identifies risks from third-party dependencies in pull requests.  
   - Tells you which vulnerabilities would be introduced if merged and suggests safer versions.  
   - Integrates with GitHub’s Advisory Database and Dependabot.