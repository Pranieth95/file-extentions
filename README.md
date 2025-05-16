# File Types for Offensive Security

A categorized list of file types that are highly valuable during different phases of offensive security assessments, including reconnaissance, enumeration, exploitation, and post-exploitation.

Categories
1. Source Code and Scripts
Files that may reveal application logic, hardcoded credentials, or debugging artifacts.

*.php, *.py, *.js, *.rb, *.asp, *.aspx, *.jsp, *.c, *.cpp, *.cs, *.sh, *.bat

2. Configuration Files
Often contain sensitive environment variables, database credentials, and third-party API keys.

.env, .ini, .conf, .yaml, .yml, .toml, web.config, app.config, settings.py, .htaccess

3. Credential and Database Files
Can expose database schemas, user credentials, or session tokens.

*.sql, *.db, *.sqlite, .pgpass, .my.cnf, id_rsa, *.pem, *.p12, *.kdbx

4. Static Web Files
Useful for mapping application structure and discovering hidden paths or sensitive endpoints.

index.html, robots.txt, sitemap.xml, crossdomain.xml, .well-known/

5. JavaScript and Client-side Files
Often include hidden endpoints, tokens, or business logic vulnerable to manipulation.

*.js, *.map, main.bundle.js, vendor.js, webpack.config.js

6. Stylesheets and Layout Files
Helpful for fingerprinting front-end technologies or identifying CMS themes and versions.

*.css, *.scss, *.less

7. Backup and Temporary Files
Commonly left behind and may leak original source code, configuration, or sensitive data.

*.bak, *.old, *.orig, *.backup, *.1, *.tmp

8. Log and Report Files
Expose internal errors, system paths, and stack traces that aid in identifying weaknesses.

*.log, *.err, *.out, *.report, debug.log

9. Uploadable / Executable Files
Used in testing file upload vulnerabilities, remote code execution (RCE), or LFI scenarios.

*.php, *.asp, *.jsp, *.exe, *.sh, *.pl, *.py, *.cgi, *.jar, *.war

10. Compressed Archives
Commonly used to store source code, old backups, or confidential documents.

*.zip, *.rar, *.7z, *.tar, *.gz, *.bz2, *.tgz, *.tar.gz, *.iso

11. Certificates and Keys
Often include private keys or internal SSL/TLS certificates.

*.crt, *.key, *.pem, *.cer, *.pfx, *.p12

12. Office and Document Files
Can contain metadata, hidden comments, or macro-based payloads.

*.docx, *.xlsx, *.pptx, *.odt, *.rtf, *.csv, *.pdf

13. Media Files
Sometimes used to hide data or malicious code via steganography or metadata injection.

*.jpg, *.jpeg, *.png, *.gif, *.bmp, *.svg, *.ico, *.webp

14. Web Service and API Descriptors
These files can help identify SOAP or REST interfaces and may expose misconfigured endpoints.

*.wsdl, *.xsd, *.asmx, *.wadl, *.graphql

# Usage Recommendations

- Use with tools like ffuf, dirsearch, gobuster, or feroxbuster to discover sensitive files or hidden endpoints.

- Append variations such as .bak, .1, .old, .tmp to detect forgotten or backup files.

- Effective for: LFI/RFI exploitation, Directory and file brute-forcing, File upload vulnerability testing, Credentials and key discovery

# Disclaimer

This list is intended for authorized penetration testing, security research, and educational purposes only. Ensure you have proper legal authorization before testing any system.