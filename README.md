# Keylogger (educational)

A keystroke-logging demo written to learn how input capture, log rotation, and
remote log delivery work at a systems level: `keylogger.py` hooks keyboard
events, batches them, and can ship them to a webhook.

## ⚠️ Authorized use only

This exists to study the mechanism, not to monitor anyone without consent.
Run it only on a machine you own or are explicitly authorized to test on.
Installing or running monitoring software on a device without the owner's
permission is illegal in most jurisdictions (e.g. unauthorized wiretapping /
computer-intrusion statutes in the US). Treat this the same way you'd treat
any other pentesting tool: scoped, authorized, and never pointed at a system
or person without consent.

## Run it

```bash
pip install pynput requests
python3 keylogger.py
```

Requires `pynput` (and optionally `requests` for webhook delivery). See the
header of `keylogger.py` for configuration.
