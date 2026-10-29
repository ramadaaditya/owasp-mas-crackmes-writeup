# Mobile Reverse-Engineering Methodology

Use this as a flexible checklist, not a requirement to run every tool.

## 1. Scope and baseline

- Challenge name, official URL, release/version
- SHA-256 of the downloaded artifact
- Device/emulator model, OS/API version, architecture
- Install and launch behavior before instrumentation
- Challenge objective and observable success/failure conditions

## 2. Static analysis

1. Identify file type, architecture, package/bundle metadata.
2. Inspect manifest, permissions, exported components, and network configuration.
3. Search strings, resources, entry points, and validation-related code.
4. Inspect Java/Kotlin/Swift/Objective-C and native libraries as applicable.
5. Trace the validation path from UI/input to the final comparison.
6. Note obfuscation, anti-debugging, root/jailbreak detection, integrity checks, and native boundaries.

Record exact class/function names and evidence. Avoid asserting intent from a string alone.

## 3. Dynamic analysis

1. Establish a baseline without hooks or debugger.
2. Observe relevant logs, UI transitions, and process behavior.
3. Attach debugger/instrumentation only when needed.
4. Hook or trace narrow functions and compare inputs/outputs.
5. Record whether instrumentation changes app behavior.
6. Re-test after removing hooks/patches.

## 4. Solution validation

- State the hypothesis and what evidence supports it.
- Explain the minimal change or runtime intervention.
- Include reproducible commands/scripts and expected output.
- Test a negative case and a positive case.
- Mention limitations, version assumptions, and alternative approaches.

## 5. Evidence hygiene

- Use redacted screenshots/logs.
- Remove usernames, device IDs, tokens, and unrelated personal data.
- Keep large binaries out of Git; link to the official challenge page.
- Distinguish observed facts from interpretation.
