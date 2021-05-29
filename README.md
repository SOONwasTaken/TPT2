# TPT2
This is where my TPT2 scripts will be housed and updated.

# Current Scripts
Scripts below are most currently updated versions

## T1 Presser Scripts
Because Factory Packages do not currently support T1 Pressers (due to the Hammer recipe being implemented), I've decided to make a few scripts to make them. 

There are 3 scripts, Presser_Main, Presser_Chip, Presser_Hammer. Maximum required lines is 22. The Chip and Hammer scripts are helper scripts with precise values, so there's no **need to edit those**.

### Usage:
- Import package into Facility AI.
- Change the `Impulse` key to whatever you want (Default is `p`).
- Change `Pressers_To_Make` to however many you want.
- Go into the Factory, enable the AI using F4, and press the `Impulse` key.

### Possible Changes / Optimizations:
- ~~Debugging.~~ (Credit: Xenos6666, d0sboots, and Coco)
- ~~Pressers materials are made 1 at a time.~~ (Updated as of v. 2.0)
- Parallel processing.
- Script creates `Pressers_To_Make + 1` pressers due to loop being treated as `while(Pressers_Made <= Pressers_To_Make)`.
- Produces leftovers (Hammer Rods and T1 Cables).

### Import Codes:
These are import codes for all 3 scripts, as well as an `Import All`.
#### Import All:

Minimum Requirements|Import Code
:-:|:-
22 Lines|DFByZXNzZXJfTWFpbgEAAAAFa2V5LnABAAAAEnRvd24ud2luZG93Lmlzb3Blbghjb25zdGFudAQHZmFjdG9yeREAAAARZ2xvYmFsLmRvdWJsZS5zZXQIY29uc3RhbnQEDVByZXNzZXJzX01hZGUIY29uc3RhbnQDAAAAAAAAAAARZ2xvYmFsLmRvdWJsZS5zZXQIY29uc3RhbnQEEFByZXNzZXJzX1RvX01ha2UIY29uc3RhbnQDAAAAAAAACEAPZmFjdG9yeS5wcm9kdWNlCGNvbnN0YW50BARkdXN0CGNvbnN0YW50AgEAAAARYXJpdGhtZXRpYy5kb3VibGUIY29uc3RhbnQDAAAAAAAAFEAIY29uc3RhbnQEASoRZ2xvYmFsLmRvdWJsZS5nZXQIY29uc3RhbnQEEFByZXNzZXJzX1RvX01ha2UIY29uc3RhbnQEBG92ZW4RZ2VuZXJpYy53YWl0dW50aWwPY29tcGFyaXNvbi5ib29sFmZhY3RvcnkubWFjaGluZS5hY3RpdmUIY29uc3RhbnQEBG92ZW4IY29uc3RhbnQEAj09CGNvbnN0YW50AQAPZmFjdG9yeS5wcm9kdWNlCGNvbnN0YW50BAVpbmdvdAhjb25zdGFudAIBAAAAEWFyaXRobWV0aWMuZG91YmxlCGNvbnN0YW50AwAAAAAAABBACGNvbnN0YW50BAEqEWdsb2JhbC5kb3VibGUuZ2V0CGNvbnN0YW50BBBQcmVzc2Vyc19Ub19NYWtlCGNvbnN0YW50BAdwcmVzc2VyEWdlbmVyaWMud2FpdHVudGlsD2NvbXBhcmlzb24uYm9vbBZmYWN0b3J5Lm1hY2hpbmUuYWN0aXZlCGNvbnN0YW50BAdwcmVzc2VyCGNvbnN0YW50BAI9PQhjb25zdGFudAEAD2ZhY3RvcnkucHJvZHVjZQhjb25zdGFudAQFaW5nb3QIY29uc3RhbnQCAQAAABFnbG9iYWwuZG91YmxlLmdldAhjb25zdGFudAQQUHJlc3NlcnNfVG9fTWFrZQhjb25zdGFudAQIcmVmaW5lcnkRZ2VuZXJpYy53YWl0dW50aWwPY29tcGFyaXNvbi5ib29sFmZhY3RvcnkubWFjaGluZS5hY3RpdmUIY29uc3RhbnQECHJlZmluZXJ5CGNvbnN0YW50BAI9PQhjb25zdGFudAEAD2ZhY3RvcnkucHJvZHVjZQhjb25zdGFudAQFY2FibGUIY29uc3RhbnQCAQAAABFnbG9iYWwuZG91YmxlLmdldAhjb25zdGFudAQQUHJlc3NlcnNfVG9fTWFrZQhjb25zdGFudAQIcmVmaW5lcnkRZ2VuZXJpYy53YWl0dW50aWwPY29tcGFyaXNvbi5ib29sFmZhY3RvcnkubWFjaGluZS5hY3RpdmUIY29uc3RhbnQECHJlZmluZXJ5CGNvbnN0YW50BAI9PQhjb25zdGFudAEAE2dlbmVyaWMuZXhlY3V0ZXN5bmMIY29uc3RhbnQEDFByZXNzZXJfQ2hpcBNnZW5lcmljLmV4ZWN1dGVzeW5jCGNvbnN0YW50BAxQcmVzc2VyX0NoaXATZ2VuZXJpYy5leGVjdXRlc3luYwhjb25zdGFudAQOUHJlc3Nlcl9IYW1tZXINZmFjdG9yeS5jcmFmdAhjb25zdGFudAQPbWFjaGluZS5wcmVzc2VyCGNvbnN0YW50AgEAAAAIY29uc3RhbnQDAAAAAAAA8D8RZ2xvYmFsLmRvdWJsZS5zZXQIY29uc3RhbnQEDVByZXNzZXJzX01hZGURYXJpdGhtZXRpYy5kb3VibGURZ2xvYmFsLmRvdWJsZS5nZXQIY29uc3RhbnQEDVByZXNzZXJzX01hZGUIY29uc3RhbnQEASsIY29uc3RhbnQDAAAAAAAA8D8OZ2VuZXJpYy5nb3RvaWYIY29uc3RhbnQCDQAAABFjb21wYXJpc29uLmRvdWJsZRFnbG9iYWwuZG91YmxlLmdldAhjb25zdGFudAQNUHJlc3NlcnNfTWFkZQhjb25zdGFudAQCIT0RZ2xvYmFsLmRvdWJsZS5nZXQIY29uc3RhbnQEEFByZXNzZXJzX3RvX21ha2UMZ2VuZXJpYy5zdG9wCGNvbnN0YW50BAxQcmVzc2VyX21haW4

