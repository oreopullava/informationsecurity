<h1>A01:2021 – Broken Access Control</h1>
https://owasp.org/Top10/A01_2021-Broken_Access_Control/

- Broken access control affects 94% of applications, leading to unauthorized access, data exposure, and privilege escalation through vulnerabilities like URL tampering and insecure direct object references (IDOR).

- Prevention includes enforcing access control through server-side mechanisms, applying "deny by default" policies, securing APIs, and conducting thorough testing to detect and mitigate access control failures.

<h1>A05:2021 – Security Misconfiguration</h1>
https://owasp.org/Top10/A05_2021-Security_Misconfiguration/

Vulnerabilities: Applications may be at risk if they lack security hardening,  unnecessary features enabled, default accounts/passwords, expose detailed error messages, disable security features, or have outdated components and insecure configurations.

Prevention: Implement secure, repeatable installation processes with hardened environments, remove unnecessary features, regularly update security configurations, use segmentation, and automate verification of security settings across all environments.  

<h1>A06:2021 – Vulnerable and Outdated Components</h1>
https://owasp.org/Top10/A06_2021-Vulnerable_and_Outdated_Components/

Vulnerabilities: use outdated, unsupported, or unpatched components, lack visibility into versioning and dependencies, fail to regularly scan for vulnerabilities, or delay patching and upgrades.

Prevention: Implement a patch management process, remove unused components, inventory versions and dependencies, monitor vulnerability databases, use secure sources for components, and ensure continuous monitoring and timely updates.

<h1>A03:2021 – Injection</h1>
https://owasp.org/Top10/A03_2021-Injection/

Vulnerabilities: Applications can be attacked if they don't properly check or clean user data. This happens when unsafe queries or commands are used, allowing harmful data to interfere with the system. Common types of these attacks include SQL, NoSQL, and command injections.

Prevention: To prevent this, use safe APIs or tools like ORM to handle queries, validate user input on the server, escape special characters in queries, and add limits to SQL queries to prevent large-scale data leaks.

a) <img width="406" alt="image" src="https://github.com/user-attachments/assets/4610a00f-ebcb-4344-b394-87481511d311">

even when trying different ports, it won't open any other than 8080

