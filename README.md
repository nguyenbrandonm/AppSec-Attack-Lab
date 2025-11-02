# AppSec-Attack-Lab
Utilize OWASP Juice Shop to learn and test tools and techniques related to OWASP Top Ten

## Objective
Use OWASP Juice Shop in Docker to learn and practice a methodical web testing workflow based on GWAPT: recon, enumeration, exploitation, verification, reporting, cleanup.

## Scope
Lab only. Test the Juice Shop instance you control. Do not test systems you do not own or have explicit authorization to test.

## Quick setup
1. Install Docker and Docker Compose.  
2. Run docker pull bkimminich/juice-shop
3. Run docker run --rm -p 127.0.0.1:3000:3000 bkimminich/juice-shop
4. Browse to http://localhost:3000 (on macOS and Windows browse to http://192.168.99.100:3000 if you are using docker-machine instead of the native docker installation)

## Methodology
1. Recon: find endpoints and assets.  
2. Enumerate: parameters, APIs, auth flows, inputs.  
3. Attack: validate vulnerabilities safely and capture evidence.  
4. Verify: reproduce impact and scope.  
5. Report: technical findings and executive summary.  
6. Retest: confirm fixes.

## Skills focused
- Endpoint and parameter discovery.  
- XSS, SQLi, CSRF, auth bypass, IDOR, SSRF basics.  
- DAST workflow with Burp Suite and automation.  
- Container awareness and safe cleanup.  
- Evidence collection and concise reporting.

## Tools
| Phase | Tools |
|---|---|
| Recon | `amass`, `subfinder`, `assetfinder`, `Shodan`, `dnsrecon`, `dig`, `nslookup` |
| Fingerprint | `Wappalyzer`, `retireJS`, `BuiltWith` |
| Port / service scan | `nmap`, `sslscan`, `nikto` |
| Endpoint discovery | `ffuf`, `dirb`, `dirbuster`, `waybackmachine`, `gowitness` |
| Intercept & manual testing | `Burp Suite Pro`, `FoxyProxy`, `Cookie Editor`, `curl` |
| Automated verification | `sqlmap`, `OWASP ZAP` |
| Evidence collection & reporting | `gowitness`, saved Burp logs, `curl`, `waybackmachine` |


## Short exercise list
- Recon and map routes and APIs.  
- Enumerate parameters and fuzz inputs.  
- Validate XSS and SQLi with non-destructive payloads.  
- Test auth, session handling, and RBAC.  
- Inspect container for misconfigurations.  
- Report findings and retest after fixes.

## Safety and cleanup
Keep the lab isolated. Stop and remove containers after testing. Do not reuse lab payloads against production systems without permission.

## Steps
Coming Soon...
