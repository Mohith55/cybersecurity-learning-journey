# Day 24 – File Inclusion Vulnerabilities (LFI & RFI)

## Objective
To understand how file inclusion vulnerabilities can lead
to sensitive data exposure and remote code execution.

## What is File Inclusion?
File inclusion occurs when applications load files dynamically
based on user-controlled input.

## Types
- Local File Inclusion (LFI)
- Remote File Inclusion (RFI)

## Impact
- Source code disclosure
- Credential leakage
- Log file abuse
- Remote Code Execution (RCE)

## Root Causes
- Unsanitized user input
- Insecure file path handling
- Lack of whitelisting
- Mixing code and data

## Key Learning
File inclusion vulnerabilities can directly lead to full system compromise.

## Takeaway
Secure file handling is critical.
Never trust user-controlled file paths.
