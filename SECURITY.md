# Security policy -- Groundskeeper

RSJ Software Ltd makes Groundskeeper. This policy says how to report a security problem, what we do with it, and how
quickly. How Groundskeeper is built and checked, and what has not been done yet, is on the
[Security and trust](https://groundskeeper.rsjsoftware.com/security) page.

## Reporting a problem

Email **security@rsjsoftware.com**, or use **Report a vulnerability** on this repository's Security tab. Please do not
open a public issue or post about it until it is fixed.

Please include, as far as you can:

- what the problem is and what someone could do with it;
- how to reproduce it, or a proof of concept;
- the Groundskeeper version (Settings -> About, or `GET /api/version`);
- any fix or workaround you suggest.

## What happens next

1. We acknowledge your report within **3 working days** (2 for a Critical one).
2. We confirm whether it is a security problem, and agree its severity with you.
3. We fix it, aiming for the times below, and tell you before the fix is released.
4. We publish the fix. Fixes that affect a school's own systems are listed in the release notes. Critical and High
   problems also get a GitHub security advisory on this repository. With your permission we credit you.

If we cannot meet a target, we tell you why and when we expect to.

## Target times by severity

| Severity | What it means | Fix or workaround released |
|---|---|---|
| **Critical** | Someone with no account could take control of the Groundskeeper server or the PCs running the RSJ Agent, read the school's data, or get past sign-in. | within **7 days** |
| **High** | Someone with an account, or a foothold on the network, could do much more than they should: become an administrator, read stored passwords or keys, or reach other systems. | within **30 days** |
| **Medium** | A real problem that is harder to reach or does less harm. | within **90 days** |
| **Low** | Hardening, or a minor information leak. | in a planned release, or we explain why we will not change it |

These are targets, not contractual promises. RSJ Software is one person; we say this so that you can judge the times,
not to excuse missing them.

## Supported versions

Groundskeeper has one release line. Fixes go into the next release, and we do not patch older versions. Please check you
are on the latest release before reporting, in case it is already fixed.

## Scope

In scope: the Groundskeeper server, the RSJ Agent and its Groundskeeper module, the Windows installer and updater, the
licence server at `api.rsjsoftware.com`, and the websites under `rsjsoftware.com`.

Out of scope: the services Groundskeeper connects to (for example Microsoft 365, Meraki, Veeam) and a school's own
network. Please report those to their makers. Also out of scope: denial-of-service testing, social engineering, and
testing against a school's server without that school's permission.

## Safe harbour

If you act in good faith, stay within this policy, avoid harming people and data, and give us reasonable time to fix
the problem before you disclose it, we will not take legal action against you. Look at no more data than you need to
show the problem, and do not keep it.

## Disclosure

We ask for up to **90 days** from your report, or until a fix is released if that is sooner, before details are made
public. We are happy to agree a different date with you.

## Bug bounty

There is no paid bug bounty. We are grateful for every report and will credit you if you would like that.
