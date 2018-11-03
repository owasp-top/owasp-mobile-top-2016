### Welcome to the OWASP Mobile Top 10 2016


OWASP Mobile Top 10 2016 List :

![M1-Improper Platform Usage](https://www.owasp.org/index.php/Mobile_Top_10_2016-M1-Improper_Platform_Usage)

This category covers misuse of a platform feature or failure to use platform security controls. It might include Android intents, platform permissions, misuse of TouchID, the Keychain, or some other security control that is part of the mobile operating system. There are several ways that mobile apps can experience this risk. 

![M2-Insecure Data Storage](https://www.owasp.org/index.php/Mobile_Top_10_2016-M2-Insecure_Data_Storage)

This new category is a combination of M2 + M4 from Mobile Top Ten 2014. This covers insecure data storage and unintended data leakage. 

![M3-Insecure Communication](https://www.owasp.org/index.php/Mobile_Top_10_2016-M3-Insecure_Communication)

This covers poor handshaking, incorrect SSL versions, weak negotiation, cleartext communication of sensitive assets, etc.

![M4-Insecure Authentication](https://www.owasp.org/index.php/Mobile_Top_10_2016-M4-Insecure_Authentication)

This category captures notions of authenticating the end user or bad session management. This can include:

* Failing to identify the user at all when that should be required
* Failure to maintain the user's identity when it is required
* Weaknesses in session management 

![M5-Insufficient Cryptography](https://www.owasp.org/index.php/Mobile_Top_10_2016-M5-Insufficient_Cryptography)

The code applies cryptography to a sensitive information asset. However, the cryptography is insufficient in some way. Note that anything and everything related to TLS or SSL goes in M3. Also, if the app fails to use cryptography at all when it should, that probably belongs in M2. This category is for issues where cryptography was attempted, but it wasn't done correctly. 

![M6-Insecure Authorization](https://www.owasp.org/index.php/Mobile_Top_10_2016-M6-Insecure_Authorization)

This is a category to capture any failures in authorization (e.g., authorization decisions in the client side, forced browsing, etc.). It is distinct from authentication issues (e.g., device enrolment, user identification, etc.).

If the app does not authenticate users at all in a situation where it should (e.g., granting anonymous access to some resource or service when authenticated and authorized access is required), then that is an authentication failure not an authorization failure.

![M7-Poor Code Quality](https://www.owasp.org/index.php/Mobile_Top_10_2016-M7-Poor_Code_Quality)

This was the "Security Decisions Via Untrusted Inputs", one of our lesser-used categories. This would be the catch-all for code-level implementation problems in the mobile client. That's distinct from server-side coding mistakes. This would capture things like buffer overflows, format string vulnerabilities, and various other code-level mistakes where the solution is to rewrite some code that's running on the mobile device. 

![M8-Code Tampering](https://www.owasp.org/index.php/Mobile_Top_10_2016-M8-Code_Tampering)

This category covers binary patching, local resource modification, method hooking, method swizzling, and dynamic memory modification.

Once the application is delivered to the mobile device, the code and data resources are resident there. An attacker can either directly modify the code, change the contents of memory dynamically, change or replace the system APIs that the application uses, or modify the application's data and resources. This can provide the attacker a direct method of subverting the intended use of the software for personal or monetary gain.

![M9-Reverse Engineering](https://www.owasp.org/index.php/Mobile_Top_10_2016-M9-Reverse_Engineering)

This category includes analysis of the final core binary to determine its source code, libraries, algorithms, and other assets. Software such as IDA Pro, Hopper, otool, and other binary inspection tools give the attacker insight into the inner workings of the application. This may be used to exploit other nascent vulnerabilities in the application, as well as revealing information about back end servers, cryptographic constants and ciphers, and intellectual property. 

![M10-Extraneous Functionality](https://www.owasp.org/index.php/Mobile_Top_10_2016-M10-Extraneous_Functionality)

Often, developers include hidden backdoor functionality or other internal development security controls that are not intended to be released into a production environment. For example, a developer may accidentally include a password as a comment in a hybrid app. Another example includes disabling of 2-factor authentication during testing. 
