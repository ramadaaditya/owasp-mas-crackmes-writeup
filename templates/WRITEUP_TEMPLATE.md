# [Challenge Name] — Write-up

> **Spoiler warning:** this page contains solution details.
>
> Official challenge: [OWASP MAS Crackmes](https://mas.owasp.org/crackmes/)

## Status

- **Platform:** Android / iOS / native binary
- **Challenge/version:** 
- **Difficulty (personal estimate):** 
- **Date tested:** YYYY-MM-DD
- **Result:** Not started / In progress / Solved / Re-tested

## 1. Objective

Describe the challenge goal in your own words. Do not copy long passages from the official page.

## 2. Environment

| Item | Value |
|---|---|
| Host OS | |
| Device/emulator + OS | |
| Architecture / API level | |
| Challenge version/source | |
| SHA-256 | |
| Tool versions | |

## 3. Initial observations

- Expected behavior:
- Observed behavior:
- Relevant logs/errors:
- Questions/hypotheses:

## 4. Static analysis

Document the path from entry point to the relevant check.

### Entry points and relevant code

- File/class/function:
- Why it matters:
- Evidence:

### Native code (if applicable)

- Library / symbol / function:
- Calling convention or JNI boundary:
- Evidence:

## 5. Dynamic analysis

Explain setup, baseline, instrumentation/debugger steps, and observations.

```bash
# Add reproducible commands here; remove secrets and machine-specific paths.
```

### Observations

| Action | Expected | Actual | Interpretation |
|---|---|---|---|
| | | | |

## 6. Root cause / challenge mechanism

Explain what mechanism prevents the intended success path or protects the secret. Separate evidence from assumptions.

## 7. Solution

**Approach:** static analysis / debugger / Frida / patching / symbolic execution / other

### Steps

1. 
2. 
3. 

### Script or patch (optional)

Explain each important part. Keep scripts minimal and challenge-specific.

```javascript
// Example placeholder only — replace with your own tested script.
```

### Verification

- [ ] Reproduced from a clean install/session
- [ ] Positive case confirmed
- [ ] Negative case tested
- [ ] Works with the documented challenge version
- [ ] Expected output/result recorded

**Result / flag / secret:** `REDACTED OR ADD YOUR VERIFIED RESULT`

## 8. Alternative approaches

Compare other approaches, their trade-offs, and why you chose this one.

## 9. Lessons learned

- What concept did this challenge teach?
- What was surprising?
- What would you investigate next?

## 10. References

- [Official MAS Crackmes](https://mas.owasp.org/crackmes/)
- [OWASP MASTG](https://mas.owasp.org/MASTG/)
- Relevant documentation, source files, or articles:
  - 

## Appendix: Evidence

Add sanitized screenshots/logs under `assets/screenshots/<challenge>/` and link them here.
