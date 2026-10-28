<h1 id="anta-security-advisory-report" align="center">🛡️ ANTA Security Advisory Report 🛡️</h1>

**Table of Contents:**

- [Advisory Assessment Summary](#advisory-assessment-summary)
- [Security Advisory Details](#security-advisory-details)
  - [Security Advisory 0147](#sa-0147)
  - [Security Advisory 0156](#sa-0156)
  - [Security Advisory 0158](#sa-0158)
  - [Security Advisory 0162](#sa-0162)
  - [Security Advisory 0174](#sa-0174)
  - [Security Advisory 0146](#sa-0146)
  - [Security Advisory 0154](#sa-0154)
  - [Security Advisory 0160](#sa-0160)
  - [Security Advisory 0163](#sa-0163)
  - [Security Advisory 0164](#sa-0164)
  - [Security Advisory 0165](#sa-0165)
  - [Security Advisory 0166](#sa-0166)
  - [Security Advisory 0168](#sa-0168)
  - [Security Advisory 0171](#sa-0171)
  - [Security Advisory 0173](#sa-0173)
  - [Security Advisory 0117](#sa-0117)
  - [Security Advisory 0140](#sa-0140)
  - [Security Advisory 0142](#sa-0142)
  - [Security Advisory 0149](#sa-0149)
  - [Security Advisory 0150](#sa-0150)
  - [Security Advisory 0151](#sa-0151)
  - [Security Advisory 0152](#sa-0152)
  - [Security Advisory 0153](#sa-0153)
  - [Security Advisory 0155](#sa-0155)
  - [Security Advisory 0157](#sa-0157)
  - [Security Advisory 0159](#sa-0159)
  - [Security Advisory 0161](#sa-0161)
  - [Security Advisory 0167](#sa-0167)
  - [Security Advisory 0169](#sa-0169)
  - [Security Advisory 0170](#sa-0170)
  - [Security Advisory 0172](#sa-0172)
  - [Security Advisory 0175](#sa-0175)
  - [Security Advisory 0176](#sa-0176)
  - [Security Advisory 0177](#sa-0177)
  - [Security Advisory 0178](#sa-0178)
- [Run Overview](#run-overview)

## 📊 Advisory Assessment Summary <a id="advisory-assessment-summary"></a>

| Security Advisory | Severity | Devices | 🛑&nbsp;Affected | ❓&nbsp;Inconclusive | 🛡️&nbsp;Mitigated | ✅&nbsp;Not&nbsp;Affected | ❗&nbsp;Error | ⏭️&nbsp;Skipped |
| :- | :- | :- | :- | :- | :- | :- | :- | :- |
| [Security Advisory 0147](#sa-0147) | 🔴&nbsp;Critical | 8 | 8 | 0 | 0 | 0 | 0 | 0 |
| [Security Advisory 0156](#sa-0156) | 🔴&nbsp;Critical | 8 | 0 | 0 | 0 | 8 | 0 | 0 |
| [Security Advisory 0158](#sa-0158) | 🔴&nbsp;Critical | 8 | 0 | 0 | 0 | 8 | 0 | 0 |
| [Security Advisory 0162](#sa-0162) | 🔴&nbsp;Critical | 8 | 0 | 8 | 0 | 0 | 0 | 0 |
| [Security Advisory 0174](#sa-0174) | 🔴&nbsp;Critical | 8 | 0 | 0 | 0 | 8 | 0 | 0 |
| [Security Advisory 0146](#sa-0146) | 🟠&nbsp;High | 8 | 0 | 0 | 0 | 8 | 0 | 0 |
| [Security Advisory 0154](#sa-0154) | 🟠&nbsp;High | 8 | 0 | 0 | 0 | 8 | 0 | 0 |
| [Security Advisory 0160](#sa-0160) | 🟠&nbsp;High | 8 | 0 | 0 | 0 | 8 | 0 | 0 |
| [Security Advisory 0163](#sa-0163) | 🟠&nbsp;High | 8 | 0 | 0 | 0 | 8 | 0 | 0 |
| [Security Advisory 0164](#sa-0164) | 🟠&nbsp;High | 8 | 0 | 0 | 0 | 8 | 0 | 0 |
| [Security Advisory 0165](#sa-0165) | 🟠&nbsp;High | 8 | 0 | 0 | 0 | 8 | 0 | 0 |
| [Security Advisory 0166](#sa-0166) | 🟠&nbsp;High | 8 | 0 | 0 | 0 | 8 | 0 | 0 |
| [Security Advisory 0168](#sa-0168) | 🟠&nbsp;High | 8 | 0 | 0 | 0 | 8 | 0 | 0 |
| [Security Advisory 0171](#sa-0171) | 🟠&nbsp;High | 8 | 0 | 0 | 0 | 8 | 0 | 0 |
| [Security Advisory 0173](#sa-0173) | 🟠&nbsp;High | 8 | 0 | 0 | 0 | 8 | 0 | 0 |
| [Security Advisory 0117](#sa-0117) | 🟡&nbsp;Medium | 8 | 0 | 0 | 0 | 8 | 0 | 0 |
| [Security Advisory 0140](#sa-0140) | 🟡&nbsp;Medium | 8 | 0 | 0 | 0 | 8 | 0 | 0 |
| [Security Advisory 0142](#sa-0142) | 🟡&nbsp;Medium | 8 | 0 | 0 | 0 | 8 | 0 | 0 |
| [Security Advisory 0149](#sa-0149) | 🟡&nbsp;Medium | 8 | 0 | 0 | 0 | 8 | 0 | 0 |
| [Security Advisory 0150](#sa-0150) | 🟡&nbsp;Medium | 8 | 0 | 0 | 0 | 8 | 0 | 0 |
| [Security Advisory 0151](#sa-0151) | 🟡&nbsp;Medium | 8 | 0 | 0 | 0 | 8 | 0 | 0 |
| [Security Advisory 0152](#sa-0152) | 🟡&nbsp;Medium | 8 | 8 | 0 | 0 | 0 | 0 | 0 |
| [Security Advisory 0153](#sa-0153) | 🟡&nbsp;Medium | 8 | 0 | 0 | 0 | 8 | 0 | 0 |
| [Security Advisory 0155](#sa-0155) | 🟡&nbsp;Medium | 8 | 0 | 0 | 0 | 8 | 0 | 0 |
| [Security Advisory 0157](#sa-0157) | 🟡&nbsp;Medium | 8 | 0 | 0 | 0 | 8 | 0 | 0 |
| [Security Advisory 0159](#sa-0159) | 🟡&nbsp;Medium | 8 | 8 | 0 | 0 | 0 | 0 | 0 |
| [Security Advisory 0161](#sa-0161) | 🟡&nbsp;Medium | 8 | 0 | 0 | 0 | 8 | 0 | 0 |
| [Security Advisory 0167](#sa-0167) | 🟡&nbsp;Medium | 8 | 0 | 0 | 0 | 8 | 0 | 0 |
| [Security Advisory 0169](#sa-0169) | 🟡&nbsp;Medium | 8 | 0 | 0 | 0 | 8 | 0 | 0 |
| [Security Advisory 0170](#sa-0170) | 🟡&nbsp;Medium | 8 | 0 | 0 | 0 | 8 | 0 | 0 |
| [Security Advisory 0172](#sa-0172) | 🟡&nbsp;Medium | 8 | 0 | 0 | 0 | 8 | 0 | 0 |
| [Security Advisory 0175](#sa-0175) | 🟡&nbsp;Medium | 8 | 0 | 0 | 0 | 8 | 0 | 0 |
| [Security Advisory 0176](#sa-0176) | 🟡&nbsp;Medium | 8 | 0 | 0 | 0 | 8 | 0 | 0 |
| [Security Advisory 0177](#sa-0177) | 🟡&nbsp;Medium | 8 | 0 | 0 | 0 | 8 | 0 | 0 |
| [Security Advisory 0178](#sa-0178) | 🟡&nbsp;Medium | 8 | 0 | 0 | 0 | 8 | 0 | 0 |

## 🔐 Security Advisory Details <a id="security-advisory-details"></a>

### Security Advisory 0147 <a id="sa-0147"></a>

> **Severity:** 🔴 Critical\
> **URL:** <https://www.arista.com/en/support/advisories-notices/security-advisory/24515-security-advisory-0147>
>
> Multiple vulnerabilities have been discovered in OpenSSH before version 10.4, which is shipped with multiple Arista products. One vulnerability (CVE-2026-60001) affects the server-side SSH daemon (sshd). The remaining three vulnerabilities (CVE-2026-60002, CVE-2026-59995, CVE-2026-59996) affect the client-side SSH, Secure File Transfer Protocol (SFTP), and Secure Copy Protocol (SCP) utilities, respectively.
>
> | Vulnerability | Severity | Description |
> | :- | :- | :- |
> | CVE-2026-60002 | 🔴&nbsp;Critical | SSH client issue when connecting to a malicious or compromised server. |
> | CVE-2026-59995 | 🟡&nbsp;Medium | SFTP client issue when connecting to an untrusted server. |
> | CVE-2026-59996 | 🟡&nbsp;Medium | SCP remote-to-remote client issue involving an untrusted server. |
> | CVE-2026-60001 | 🟡&nbsp;Medium | OpenSSH server issue affecting accepted SSH connections. |
>

#### 🔎 Device Findings

| Device | Vulnerability | Result | Findings | Remediations |
| :- | :- | :- | :- | :- |
| s1-brdr1 | 🟡&nbsp;CVE-2026-59995 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected and openssh-clients '9.9p1' is affected. | Upgrade EOS to a fixed release when one is published.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-brdr1 | 🟡&nbsp;CVE-2026-59996 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected and openssh-clients '9.9p1' is affected. | Upgrade EOS to a fixed release when one is published.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-brdr1 | 🟡&nbsp;CVE-2026-60001 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected, openssh-server '9.9p1' is affected, and the SSH feature is enabled. | Upgrade EOS to a fixed release when one is published.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-brdr1 | 🔴&nbsp;CVE-2026-60002 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected and openssh-clients '9.9p1' is affected. | Downgrade to EOS 4.35.6M or later in the 4.35 train.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-brdr2 | 🟡&nbsp;CVE-2026-59995 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected and openssh-clients '9.9p1' is affected. | Upgrade EOS to a fixed release when one is published.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-brdr2 | 🟡&nbsp;CVE-2026-59996 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected and openssh-clients '9.9p1' is affected. | Upgrade EOS to a fixed release when one is published.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-brdr2 | 🟡&nbsp;CVE-2026-60001 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected, openssh-server '9.9p1' is affected, and the SSH feature is enabled. | Upgrade EOS to a fixed release when one is published.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-brdr2 | 🔴&nbsp;CVE-2026-60002 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected and openssh-clients '9.9p1' is affected. | Downgrade to EOS 4.35.6M or later in the 4.35 train.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-leaf1 | 🟡&nbsp;CVE-2026-59995 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected and openssh-clients '9.9p1' is affected. | Upgrade EOS to a fixed release when one is published.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-leaf1 | 🟡&nbsp;CVE-2026-59996 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected and openssh-clients '9.9p1' is affected. | Upgrade EOS to a fixed release when one is published.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-leaf1 | 🟡&nbsp;CVE-2026-60001 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected, openssh-server '9.9p1' is affected, and the SSH feature is enabled. | Upgrade EOS to a fixed release when one is published.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-leaf1 | 🔴&nbsp;CVE-2026-60002 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected and openssh-clients '9.9p1' is affected. | Downgrade to EOS 4.35.6M or later in the 4.35 train.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-leaf2 | 🟡&nbsp;CVE-2026-59995 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected and openssh-clients '9.9p1' is affected. | Upgrade EOS to a fixed release when one is published.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-leaf2 | 🟡&nbsp;CVE-2026-59996 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected and openssh-clients '9.9p1' is affected. | Upgrade EOS to a fixed release when one is published.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-leaf2 | 🟡&nbsp;CVE-2026-60001 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected, openssh-server '9.9p1' is affected, and the SSH feature is enabled. | Upgrade EOS to a fixed release when one is published.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-leaf2 | 🔴&nbsp;CVE-2026-60002 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected and openssh-clients '9.9p1' is affected. | Downgrade to EOS 4.35.6M or later in the 4.35 train.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-leaf3 | 🟡&nbsp;CVE-2026-59995 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected and openssh-clients '9.9p1' is affected. | Upgrade EOS to a fixed release when one is published.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-leaf3 | 🟡&nbsp;CVE-2026-59996 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected and openssh-clients '9.9p1' is affected. | Upgrade EOS to a fixed release when one is published.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-leaf3 | 🟡&nbsp;CVE-2026-60001 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected, openssh-server '9.9p1' is affected, and the SSH feature is enabled. | Upgrade EOS to a fixed release when one is published.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-leaf3 | 🔴&nbsp;CVE-2026-60002 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected and openssh-clients '9.9p1' is affected. | Downgrade to EOS 4.35.6M or later in the 4.35 train.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-leaf4 | 🟡&nbsp;CVE-2026-59995 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected and openssh-clients '9.9p1' is affected. | Upgrade EOS to a fixed release when one is published.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-leaf4 | 🟡&nbsp;CVE-2026-59996 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected and openssh-clients '9.9p1' is affected. | Upgrade EOS to a fixed release when one is published.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-leaf4 | 🟡&nbsp;CVE-2026-60001 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected, openssh-server '9.9p1' is affected, and the SSH feature is enabled. | Upgrade EOS to a fixed release when one is published.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-leaf4 | 🔴&nbsp;CVE-2026-60002 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected and openssh-clients '9.9p1' is affected. | Downgrade to EOS 4.35.6M or later in the 4.35 train.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-spine1 | 🟡&nbsp;CVE-2026-59995 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected and openssh-clients '9.9p1' is affected. | Upgrade EOS to a fixed release when one is published.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-spine1 | 🟡&nbsp;CVE-2026-59996 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected and openssh-clients '9.9p1' is affected. | Upgrade EOS to a fixed release when one is published.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-spine1 | 🟡&nbsp;CVE-2026-60001 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected, openssh-server '9.9p1' is affected, and the SSH feature is enabled. | Upgrade EOS to a fixed release when one is published.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-spine1 | 🔴&nbsp;CVE-2026-60002 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected and openssh-clients '9.9p1' is affected. | Downgrade to EOS 4.35.6M or later in the 4.35 train.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-spine2 | 🟡&nbsp;CVE-2026-59995 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected and openssh-clients '9.9p1' is affected. | Upgrade EOS to a fixed release when one is published.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-spine2 | 🟡&nbsp;CVE-2026-59996 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected and openssh-clients '9.9p1' is affected. | Upgrade EOS to a fixed release when one is published.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-spine2 | 🟡&nbsp;CVE-2026-60001 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected, openssh-server '9.9p1' is affected, and the SSH feature is enabled. | Upgrade EOS to a fixed release when one is published.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-spine2 | 🔴&nbsp;CVE-2026-60002 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected and openssh-clients '9.9p1' is affected. | Downgrade to EOS 4.35.6M or later in the 4.35 train.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |

### Security Advisory 0156 <a id="sa-0156"></a>

> **Severity:** 🔴 Critical\
> **URL:** <https://www.arista.com/en/support/advisories-notices/security-advisory/24712-security-advisory-0156>
>
> On affected EOS releases with DHCP relay active, unvalidated replies may provide clients with malicious network configuration.
>
> | Vulnerability | Severity | Description |
> | :- | :- | :- |
> | CVE-2026-73437 | 🔴&nbsp;Critical | DHCP relay may forward replies from sources that are not configured helper addresses. |
>

#### 🔎 Device Findings

| Device | Vulnerability | Result | Findings | Remediations |
| :- | :- | :- | :- | :- |
| s1-brdr1 | 🔴&nbsp;CVE-2026-73437 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the DHCP relay is disabled. | - |
| s1-brdr2 | 🔴&nbsp;CVE-2026-73437 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the DHCP relay is disabled. | - |
| s1-leaf1 | 🔴&nbsp;CVE-2026-73437 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the DHCP relay is disabled. | - |
| s1-leaf2 | 🔴&nbsp;CVE-2026-73437 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the DHCP relay is disabled. | - |
| s1-leaf3 | 🔴&nbsp;CVE-2026-73437 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the DHCP relay is disabled. | - |
| s1-leaf4 | 🔴&nbsp;CVE-2026-73437 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the DHCP relay is disabled. | - |
| s1-spine1 | 🔴&nbsp;CVE-2026-73437 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the DHCP relay is disabled. | - |
| s1-spine2 | 🔴&nbsp;CVE-2026-73437 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the DHCP relay is disabled. | - |

### Security Advisory 0158 <a id="sa-0158"></a>

> **Severity:** 🔴 Critical\
> **URL:** <https://www.arista.com/en/support/advisories-notices/security-advisory/24714-security-advisory-0158>
>
> On affected EOS releases, configured gNPSI authentication or tracing may permit code execution or credential disclosure.
>
> | Vulnerability | Severity | Description |
> | :- | :- | :- |
> | CVE-2026-73456 | 🔴&nbsp;Critical | An unauthenticated gNPSI client may execute arbitrary code and gain administrative control. |
> | CVE-2026-73457 | 🟡&nbsp;Medium | Explicit gNPSI authentication tracing may log client credentials in clear text. |
>

#### 🔎 Device Findings

| Device | Vulnerability | Result | Findings | Remediations |
| :- | :- | :- | :- | :- |
| s1-brdr1 | 🔴&nbsp;CVE-2026-73456 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNPSI exposed authentication mode is disabled. | - |
| s1-brdr1 | 🟡&nbsp;CVE-2026-73457 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNPSI transport is disabled. | - |
| s1-brdr2 | 🔴&nbsp;CVE-2026-73456 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNPSI exposed authentication mode is disabled. | - |
| s1-brdr2 | 🟡&nbsp;CVE-2026-73457 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNPSI transport is disabled. | - |
| s1-leaf1 | 🔴&nbsp;CVE-2026-73456 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNPSI exposed authentication mode is disabled. | - |
| s1-leaf1 | 🟡&nbsp;CVE-2026-73457 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNPSI transport is disabled. | - |
| s1-leaf2 | 🔴&nbsp;CVE-2026-73456 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNPSI exposed authentication mode is disabled. | - |
| s1-leaf2 | 🟡&nbsp;CVE-2026-73457 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNPSI transport is disabled. | - |
| s1-leaf3 | 🔴&nbsp;CVE-2026-73456 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNPSI exposed authentication mode is disabled. | - |
| s1-leaf3 | 🟡&nbsp;CVE-2026-73457 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNPSI transport is disabled. | - |
| s1-leaf4 | 🔴&nbsp;CVE-2026-73456 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNPSI exposed authentication mode is disabled. | - |
| s1-leaf4 | 🟡&nbsp;CVE-2026-73457 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNPSI transport is disabled. | - |
| s1-spine1 | 🔴&nbsp;CVE-2026-73456 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNPSI exposed authentication mode is disabled. | - |
| s1-spine1 | 🟡&nbsp;CVE-2026-73457 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNPSI transport is disabled. | - |
| s1-spine2 | 🔴&nbsp;CVE-2026-73456 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNPSI exposed authentication mode is disabled. | - |
| s1-spine2 | 🟡&nbsp;CVE-2026-73457 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNPSI transport is disabled. | - |

### Security Advisory 0162 <a id="sa-0162"></a>

> **Severity:** 🔴 Critical\
> **URL:** <https://www.arista.com/en/support/advisories-notices/security-advisory/24718-security-advisory-0162>
>
> A vulnerability in the gRPC Network Security Interface (gNSI) Certz service on Arista EOS-based products allows an authenticated user to escalate its privilege to execute arbitrary OS commands via a crafted Certz Rotate request. The Bootz service is also affected.
>
> | Vulnerability | Severity | Description |
> | :- | :- | :- |
> | CVE-2026-73447 | 🔴&nbsp;Critical | gNSI Certz and Bootz command injection permitting authenticated privilege escalation. |
>

#### 🔎 Device Findings

| Device | Vulnerability | Result | Findings | Remediations |
| :- | :- | :- | :- | :- |
| s1-brdr1 | 🔴&nbsp;CVE-2026-73447 | ❓&nbsp;Inconclusive | The assessment is inconclusive and the device may be affected. Indications: EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected. Unresolved: initial Bootz CertzProfile certificate contents is historical state. | Upgrade to EOS 4.36.1F or later in the 4.36 train.<br>Refer to the advisory to determine whether the unresolved condition applies, for newly fixed releases, and for current mitigation guidance. |
| s1-brdr2 | 🔴&nbsp;CVE-2026-73447 | ❓&nbsp;Inconclusive | The assessment is inconclusive and the device may be affected. Indications: EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected. Unresolved: initial Bootz CertzProfile certificate contents is historical state. | Upgrade to EOS 4.36.1F or later in the 4.36 train.<br>Refer to the advisory to determine whether the unresolved condition applies, for newly fixed releases, and for current mitigation guidance. |
| s1-leaf1 | 🔴&nbsp;CVE-2026-73447 | ❓&nbsp;Inconclusive | The assessment is inconclusive and the device may be affected. Indications: EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected. Unresolved: initial Bootz CertzProfile certificate contents is historical state. | Upgrade to EOS 4.36.1F or later in the 4.36 train.<br>Refer to the advisory to determine whether the unresolved condition applies, for newly fixed releases, and for current mitigation guidance. |
| s1-leaf2 | 🔴&nbsp;CVE-2026-73447 | ❓&nbsp;Inconclusive | The assessment is inconclusive and the device may be affected. Indications: EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected. Unresolved: initial Bootz CertzProfile certificate contents is historical state. | Upgrade to EOS 4.36.1F or later in the 4.36 train.<br>Refer to the advisory to determine whether the unresolved condition applies, for newly fixed releases, and for current mitigation guidance. |
| s1-leaf3 | 🔴&nbsp;CVE-2026-73447 | ❓&nbsp;Inconclusive | The assessment is inconclusive and the device may be affected. Indications: EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected. Unresolved: initial Bootz CertzProfile certificate contents is historical state. | Upgrade to EOS 4.36.1F or later in the 4.36 train.<br>Refer to the advisory to determine whether the unresolved condition applies, for newly fixed releases, and for current mitigation guidance. |
| s1-leaf4 | 🔴&nbsp;CVE-2026-73447 | ❓&nbsp;Inconclusive | The assessment is inconclusive and the device may be affected. Indications: EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected. Unresolved: initial Bootz CertzProfile certificate contents is historical state. | Upgrade to EOS 4.36.1F or later in the 4.36 train.<br>Refer to the advisory to determine whether the unresolved condition applies, for newly fixed releases, and for current mitigation guidance. |
| s1-spine1 | 🔴&nbsp;CVE-2026-73447 | ❓&nbsp;Inconclusive | The assessment is inconclusive and the device may be affected. Indications: EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected. Unresolved: initial Bootz CertzProfile certificate contents is historical state. | Upgrade to EOS 4.36.1F or later in the 4.36 train.<br>Refer to the advisory to determine whether the unresolved condition applies, for newly fixed releases, and for current mitigation guidance. |
| s1-spine2 | 🔴&nbsp;CVE-2026-73447 | ❓&nbsp;Inconclusive | The assessment is inconclusive and the device may be affected. Indications: EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected. Unresolved: initial Bootz CertzProfile certificate contents is historical state. | Upgrade to EOS 4.36.1F or later in the 4.36 train.<br>Refer to the advisory to determine whether the unresolved condition applies, for newly fixed releases, and for current mitigation guidance. |

### Security Advisory 0174 <a id="sa-0174"></a>

> **Severity:** 🔴 Critical\
> **URL:** <https://www.arista.com/en/support/advisories-notices/security-advisory/24730-security-advisory-0174>
>
> On affected EOS releases, an unauthenticated client may achieve arbitrary code execution when P4Runtime uses no mutual TLS, or when request accounting is active without gNSI Authz RPC authorization.
>
> | Vulnerability | Severity | Description |
> | :- | :- | :- |
> | CVE-2026-73453 | 🔴&nbsp;Critical | An unauthenticated P4Runtime client may achieve arbitrary code execution. |
>

#### 🔎 Device Findings

| Device | Vulnerability | Result | Findings | Remediations |
| :- | :- | :- | :- | :- |
| s1-brdr1 | 🔴&nbsp;CVE-2026-73453 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the P4Runtime feature is disabled. | - |
| s1-brdr2 | 🔴&nbsp;CVE-2026-73453 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the P4Runtime feature is disabled. | - |
| s1-leaf1 | 🔴&nbsp;CVE-2026-73453 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the P4Runtime feature is disabled. | - |
| s1-leaf2 | 🔴&nbsp;CVE-2026-73453 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the P4Runtime feature is disabled. | - |
| s1-leaf3 | 🔴&nbsp;CVE-2026-73453 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the P4Runtime feature is disabled. | - |
| s1-leaf4 | 🔴&nbsp;CVE-2026-73453 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the P4Runtime feature is disabled. | - |
| s1-spine1 | 🔴&nbsp;CVE-2026-73453 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the P4Runtime feature is disabled. | - |
| s1-spine2 | 🔴&nbsp;CVE-2026-73453 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the P4Runtime feature is disabled. | - |

### Security Advisory 0146 <a id="sa-0146"></a>

> **Severity:** 🟠 High\
> **URL:** <https://www.arista.com/en/support/advisories-notices/security-advisory/24500-security-advisory-0146>
>
> Arista Networks is providing this security update in response to the gRPC-Go security vulnerabilities published as GHSA-hrxh-6v49-42gf. Arista products are affected solely by the HTTP/2 Rapid Reset denial-of-service bypass, in which an unauthenticated remote attacker can exploit unthrottled HTTP/2 stream resets to bypass rate-limiting controls, consume excessive CPU resources, and cause a denial of service.
>
> | Vulnerability | Severity | Description |
> | :- | :- | :- |
> | GHSA-hrxh-6v49-42gf | 🟠&nbsp;High | HTTP/2 Rapid Reset denial-of-service rate-limit bypass in affected gRPC servers. |
>

#### 🔎 Device Findings

| Device | Vulnerability | Result | Findings | Remediations |
| :- | :- | :- | :- | :- |
| s1-brdr1 | 🟠&nbsp;GHSA-hrxh-6v49-42gf | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNMI feature is disabled, the gRIBI feature is disabled, and the TerminAttr feature is disabled. | - |
| s1-brdr2 | 🟠&nbsp;GHSA-hrxh-6v49-42gf | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNMI feature is disabled, the gRIBI feature is disabled, and the TerminAttr feature is disabled. | - |
| s1-leaf1 | 🟠&nbsp;GHSA-hrxh-6v49-42gf | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNMI feature is disabled, the gRIBI feature is disabled, and the TerminAttr feature is disabled. | - |
| s1-leaf2 | 🟠&nbsp;GHSA-hrxh-6v49-42gf | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNMI feature is disabled, the gRIBI feature is disabled, and the TerminAttr feature is disabled. | - |
| s1-leaf3 | 🟠&nbsp;GHSA-hrxh-6v49-42gf | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNMI feature is disabled, the gRIBI feature is disabled, and the TerminAttr feature is disabled. | - |
| s1-leaf4 | 🟠&nbsp;GHSA-hrxh-6v49-42gf | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNMI feature is disabled, the gRIBI feature is disabled, and the TerminAttr feature is disabled. | - |
| s1-spine1 | 🟠&nbsp;GHSA-hrxh-6v49-42gf | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNMI feature is disabled, the gRIBI feature is disabled, and the TerminAttr feature is disabled. | - |
| s1-spine2 | 🟠&nbsp;GHSA-hrxh-6v49-42gf | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNMI feature is disabled, the gRIBI feature is disabled, and the TerminAttr feature is disabled. | - |

### Security Advisory 0154 <a id="sa-0154"></a>

> **Severity:** 🟠 High\
> **URL:** <https://www.arista.com/en/support/advisories-notices/security-advisory/24710-security-advisory-0154>
>
> On affected EOS releases with authenticated BFD sessions configured, a crafted packet can cause BFD sessions to go down and may trigger undesirable routing changes.
>
> | Vulnerability | Severity | Description |
> | :- | :- | :- |
> | CVE-2026-73458 | 🟠&nbsp;High | A crafted packet may bring down operational authenticated BFD sessions. |
>

#### 🔎 Device Findings

| Device | Vulnerability | Result | Findings | Remediations |
| :- | :- | :- | :- | :- |
| s1-brdr1 | 🟠&nbsp;CVE-2026-73458 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the BFD authentication is disabled. | - |
| s1-brdr2 | 🟠&nbsp;CVE-2026-73458 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the BFD authentication is disabled. | - |
| s1-leaf1 | 🟠&nbsp;CVE-2026-73458 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the BFD authentication is disabled. | - |
| s1-leaf2 | 🟠&nbsp;CVE-2026-73458 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the BFD authentication is disabled. | - |
| s1-leaf3 | 🟠&nbsp;CVE-2026-73458 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the BFD authentication is disabled. | - |
| s1-leaf4 | 🟠&nbsp;CVE-2026-73458 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the BFD authentication is disabled. | - |
| s1-spine1 | 🟠&nbsp;CVE-2026-73458 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the BFD authentication is disabled. | - |
| s1-spine2 | 🟠&nbsp;CVE-2026-73458 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the BFD authentication is disabled. | - |

### Security Advisory 0160 <a id="sa-0160"></a>

> **Severity:** 🟠 High\
> **URL:** <https://www.arista.com/en/support/advisories-notices/security-advisory/24716-security-advisory-0160>
>
> On affected EOS releases, crafted IS-IS packets may disrupt adjacencies, link-state data, or graceful restart.
>
> | Vulnerability | Severity | Description |
> | :- | :- | :- |
> | CVE-2026-73446 | 🟠&nbsp;High | A crafted IS-IS hello may tear down an adjacency on a broadcast interface. |
> | CVE-2026-73459 | 🟠&nbsp;High | A crafted IS-IS LSP may purge a legitimate LSP from the link-state database. |
> | CVE-2026-73460 | 🟡&nbsp;Medium | A malformed IS-IS LSP may terminate graceful restart prematurely. |
>

#### 🔎 Device Findings

| Device | Vulnerability | Result | Findings | Remediations |
| :- | :- | :- | :- | :- |
| s1-brdr1 | 🟠&nbsp;CVE-2026-73446 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the IS-IS feature is disabled. | - |
| s1-brdr1 | 🟠&nbsp;CVE-2026-73459 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the IS-IS feature is disabled. | - |
| s1-brdr1 | 🟡&nbsp;CVE-2026-73460 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the IS-IS graceful restart is disabled. | - |
| s1-brdr2 | 🟠&nbsp;CVE-2026-73446 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the IS-IS feature is disabled. | - |
| s1-brdr2 | 🟠&nbsp;CVE-2026-73459 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the IS-IS feature is disabled. | - |
| s1-brdr2 | 🟡&nbsp;CVE-2026-73460 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the IS-IS graceful restart is disabled. | - |
| s1-leaf1 | 🟠&nbsp;CVE-2026-73446 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the IS-IS feature is disabled. | - |
| s1-leaf1 | 🟠&nbsp;CVE-2026-73459 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the IS-IS feature is disabled. | - |
| s1-leaf1 | 🟡&nbsp;CVE-2026-73460 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the IS-IS graceful restart is disabled. | - |
| s1-leaf2 | 🟠&nbsp;CVE-2026-73446 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the IS-IS feature is disabled. | - |
| s1-leaf2 | 🟠&nbsp;CVE-2026-73459 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the IS-IS feature is disabled. | - |
| s1-leaf2 | 🟡&nbsp;CVE-2026-73460 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the IS-IS graceful restart is disabled. | - |
| s1-leaf3 | 🟠&nbsp;CVE-2026-73446 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the IS-IS feature is disabled. | - |
| s1-leaf3 | 🟠&nbsp;CVE-2026-73459 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the IS-IS feature is disabled. | - |
| s1-leaf3 | 🟡&nbsp;CVE-2026-73460 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the IS-IS graceful restart is disabled. | - |
| s1-leaf4 | 🟠&nbsp;CVE-2026-73446 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the IS-IS feature is disabled. | - |
| s1-leaf4 | 🟠&nbsp;CVE-2026-73459 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the IS-IS feature is disabled. | - |
| s1-leaf4 | 🟡&nbsp;CVE-2026-73460 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the IS-IS graceful restart is disabled. | - |
| s1-spine1 | 🟠&nbsp;CVE-2026-73446 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the IS-IS feature is disabled. | - |
| s1-spine1 | 🟠&nbsp;CVE-2026-73459 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the IS-IS feature is disabled. | - |
| s1-spine1 | 🟡&nbsp;CVE-2026-73460 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the IS-IS graceful restart is disabled. | - |
| s1-spine2 | 🟠&nbsp;CVE-2026-73446 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the IS-IS feature is disabled. | - |
| s1-spine2 | 🟠&nbsp;CVE-2026-73459 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the IS-IS feature is disabled. | - |
| s1-spine2 | 🟡&nbsp;CVE-2026-73460 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the IS-IS graceful restart is disabled. | - |

### Security Advisory 0163 <a id="sa-0163"></a>

> **Severity:** 🟠 High\
> **URL:** <https://www.arista.com/en/support/advisories-notices/security-advisory/24719-security-advisory-0163>
>
> On affected EOS releases, an authenticated OpenConfig gRPC request using mutual TLS and request authorization may use privilege level zero and the wrong AAA command-authorization method list.
>
> | Vulnerability | Severity | Description |
> | :- | :- | :- |
> | CVE-2026-73461 | 🟠&nbsp;High | OpenConfig gRPC requests may be authorized using the wrong AAA privilege level. |
>

#### 🔎 Device Findings

| Device | Vulnerability | Result | Findings | Remediations |
| :- | :- | :- | :- | :- |
| s1-brdr1 | 🟠&nbsp;CVE-2026-73461 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNMI mTLS request authorization is disabled. | - |
| s1-brdr2 | 🟠&nbsp;CVE-2026-73461 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNMI mTLS request authorization is disabled. | - |
| s1-leaf1 | 🟠&nbsp;CVE-2026-73461 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNMI mTLS request authorization is disabled. | - |
| s1-leaf2 | 🟠&nbsp;CVE-2026-73461 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNMI mTLS request authorization is disabled. | - |
| s1-leaf3 | 🟠&nbsp;CVE-2026-73461 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNMI mTLS request authorization is disabled. | - |
| s1-leaf4 | 🟠&nbsp;CVE-2026-73461 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNMI mTLS request authorization is disabled. | - |
| s1-spine1 | 🟠&nbsp;CVE-2026-73461 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNMI mTLS request authorization is disabled. | - |
| s1-spine2 | 🟠&nbsp;CVE-2026-73461 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNMI mTLS request authorization is disabled. | - |

### Security Advisory 0164 <a id="sa-0164"></a>

> **Severity:** 🟠 High\
> **URL:** <https://www.arista.com/en/support/advisories-notices/security-advisory/24720-security-advisory-0164>
>
> On affected platforms running Arista EOS, a running gNMI server may fail to correctly enforce a gNSI Pathz policy containing a group rule and a user rule for the same path, allowing an authenticated user unauthorized access to restricted gNMI paths.
>
> | Vulnerability | Severity | Description |
> | :- | :- | :- |
> | CVE-2026-73439 | 🟠&nbsp;High | gNMI Pathz may incorrectly combine user and group permissions for the same path. |
>

#### 🔎 Device Findings

| Device | Vulnerability | Result | Findings | Remediations |
| :- | :- | :- | :- | :- |
| s1-brdr1 | 🟠&nbsp;CVE-2026-73439 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNSI Pathz service is disabled. | - |
| s1-brdr2 | 🟠&nbsp;CVE-2026-73439 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNSI Pathz service is disabled. | - |
| s1-leaf1 | 🟠&nbsp;CVE-2026-73439 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNSI Pathz service is disabled. | - |
| s1-leaf2 | 🟠&nbsp;CVE-2026-73439 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNSI Pathz service is disabled. | - |
| s1-leaf3 | 🟠&nbsp;CVE-2026-73439 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNSI Pathz service is disabled. | - |
| s1-leaf4 | 🟠&nbsp;CVE-2026-73439 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNSI Pathz service is disabled. | - |
| s1-spine1 | 🟠&nbsp;CVE-2026-73439 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNSI Pathz service is disabled. | - |
| s1-spine2 | 🟠&nbsp;CVE-2026-73439 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNSI Pathz service is disabled. | - |

### Security Advisory 0165 <a id="sa-0165"></a>

> **Severity:** 🟠 High\
> **URL:** <https://www.arista.com/en/support/advisories-notices/security-advisory/24721-security-advisory-0165>
>
> On affected EOS releases, a crafted gNSI Credentialz request may modify account properties beyond the administrator's intent.
>
> | Vulnerability | Severity | Description |
> | :- | :- | :- |
> | CVE-2026-73454 | 🟠&nbsp;High | A crafted gNSI Credentialz request may unintentionally elevate account privileges. |
>

#### 🔎 Device Findings

| Device | Vulnerability | Result | Findings | Remediations |
| :- | :- | :- | :- | :- |
| s1-brdr1 | 🟠&nbsp;CVE-2026-73454 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNSI Credentialz service is disabled. | - |
| s1-brdr2 | 🟠&nbsp;CVE-2026-73454 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNSI Credentialz service is disabled. | - |
| s1-leaf1 | 🟠&nbsp;CVE-2026-73454 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNSI Credentialz service is disabled. | - |
| s1-leaf2 | 🟠&nbsp;CVE-2026-73454 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNSI Credentialz service is disabled. | - |
| s1-leaf3 | 🟠&nbsp;CVE-2026-73454 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNSI Credentialz service is disabled. | - |
| s1-leaf4 | 🟠&nbsp;CVE-2026-73454 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNSI Credentialz service is disabled. | - |
| s1-spine1 | 🟠&nbsp;CVE-2026-73454 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNSI Credentialz service is disabled. | - |
| s1-spine2 | 🟠&nbsp;CVE-2026-73454 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNSI Credentialz service is disabled. | - |

### Security Advisory 0166 <a id="sa-0166"></a>

> **Severity:** 🟠 High\
> **URL:** <https://www.arista.com/en/support/advisories-notices/security-advisory/24722-security-advisory-0166>
>
> On affected EOS releases with gNMI enabled, a malicious authenticated client may execute arbitrary code with root privileges.
>
> | Vulnerability | Severity | Description |
> | :- | :- | :- |
> | CVE-2026-73464 | 🟠&nbsp;High | A crafted authenticated gNMI request may execute arbitrary code with root privileges. |
>

#### 🔎 Device Findings

| Device | Vulnerability | Result | Findings | Remediations |
| :- | :- | :- | :- | :- |
| s1-brdr1 | 🟠&nbsp;CVE-2026-73464 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNMI feature is disabled. | - |
| s1-brdr2 | 🟠&nbsp;CVE-2026-73464 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNMI feature is disabled. | - |
| s1-leaf1 | 🟠&nbsp;CVE-2026-73464 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNMI feature is disabled. | - |
| s1-leaf2 | 🟠&nbsp;CVE-2026-73464 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNMI feature is disabled. | - |
| s1-leaf3 | 🟠&nbsp;CVE-2026-73464 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNMI feature is disabled. | - |
| s1-leaf4 | 🟠&nbsp;CVE-2026-73464 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNMI feature is disabled. | - |
| s1-spine1 | 🟠&nbsp;CVE-2026-73464 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNMI feature is disabled. | - |
| s1-spine2 | 🟠&nbsp;CVE-2026-73464 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNMI feature is disabled. | - |

### Security Advisory 0168 <a id="sa-0168"></a>

> **Severity:** 🟠 High\
> **URL:** <https://www.arista.com/en/support/advisories-notices/security-advisory/24724-security-advisory-0168>
>
> On affected EOS releases, enabled OpenConfig services may log sensitive request or response content.
>
> | Vulnerability | Severity | Description |
> | :- | :- | :- |
> | CVE-2026-2380 | 🟠&nbsp;High | OpenConfig requests and responses containing sensitive values may be written to local or accounting logs. |
>

#### 🔎 Device Findings

| Device | Vulnerability | Result | Findings | Remediations |
| :- | :- | :- | :- | :- |
| s1-brdr1 | 🟠&nbsp;CVE-2026-2380 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNMI feature is disabled, the RESTCONF feature is disabled, and the NETCONF feature is disabled. | - |
| s1-brdr2 | 🟠&nbsp;CVE-2026-2380 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNMI feature is disabled, the RESTCONF feature is disabled, and the NETCONF feature is disabled. | - |
| s1-leaf1 | 🟠&nbsp;CVE-2026-2380 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNMI feature is disabled, the RESTCONF feature is disabled, and the NETCONF feature is disabled. | - |
| s1-leaf2 | 🟠&nbsp;CVE-2026-2380 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNMI feature is disabled, the RESTCONF feature is disabled, and the NETCONF feature is disabled. | - |
| s1-leaf3 | 🟠&nbsp;CVE-2026-2380 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNMI feature is disabled, the RESTCONF feature is disabled, and the NETCONF feature is disabled. | - |
| s1-leaf4 | 🟠&nbsp;CVE-2026-2380 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNMI feature is disabled, the RESTCONF feature is disabled, and the NETCONF feature is disabled. | - |
| s1-spine1 | 🟠&nbsp;CVE-2026-2380 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNMI feature is disabled, the RESTCONF feature is disabled, and the NETCONF feature is disabled. | - |
| s1-spine2 | 🟠&nbsp;CVE-2026-2380 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNMI feature is disabled, the RESTCONF feature is disabled, and the NETCONF feature is disabled. | - |

### Security Advisory 0171 <a id="sa-0171"></a>

> **Severity:** 🟠 High\
> **URL:** <https://www.arista.com/en/support/advisories-notices/security-advisory/24727-security-advisory-0171>
>
> On affected EOS releases, crafted OSPFv2 packets may disrupt authenticated broadcast adjacencies or restart OSPF segment routing.
>
> | Vulnerability | Severity | Description |
> | :- | :- | :- |
> | CVE-2026-73435 | 🟠&nbsp;High | Crafted authenticated OSPFv2 packets may disrupt adjacencies and cause packet loss. |
> | CVE-2026-73436 | 🟡&nbsp;Medium | Crafted OSPFv2 packets may restart the OSPF process when segment routing is enabled. |
>

#### 🔎 Device Findings

| Device | Vulnerability | Result | Findings | Remediations |
| :- | :- | :- | :- | :- |
| s1-brdr1 | 🟠&nbsp;CVE-2026-73435 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the OSPFv2 routing process configuration is not configured. | - |
| s1-brdr1 | 🟡&nbsp;CVE-2026-73436 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the OSPFv2 segment routing is disabled. | - |
| s1-brdr2 | 🟠&nbsp;CVE-2026-73435 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the OSPFv2 routing process configuration is not configured. | - |
| s1-brdr2 | 🟡&nbsp;CVE-2026-73436 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the OSPFv2 segment routing is disabled. | - |
| s1-leaf1 | 🟠&nbsp;CVE-2026-73435 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the OSPFv2 routing process configuration is not configured. | - |
| s1-leaf1 | 🟡&nbsp;CVE-2026-73436 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the OSPFv2 segment routing is disabled. | - |
| s1-leaf2 | 🟠&nbsp;CVE-2026-73435 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the OSPFv2 routing process configuration is not configured. | - |
| s1-leaf2 | 🟡&nbsp;CVE-2026-73436 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the OSPFv2 segment routing is disabled. | - |
| s1-leaf3 | 🟠&nbsp;CVE-2026-73435 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the OSPFv2 routing process configuration is not configured. | - |
| s1-leaf3 | 🟡&nbsp;CVE-2026-73436 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the OSPFv2 segment routing is disabled. | - |
| s1-leaf4 | 🟠&nbsp;CVE-2026-73435 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the OSPFv2 routing process configuration is not configured. | - |
| s1-leaf4 | 🟡&nbsp;CVE-2026-73436 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the OSPFv2 segment routing is disabled. | - |
| s1-spine1 | 🟠&nbsp;CVE-2026-73435 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the OSPFv2 routing process configuration is not configured. | - |
| s1-spine1 | 🟡&nbsp;CVE-2026-73436 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the OSPFv2 segment routing is disabled. | - |
| s1-spine2 | 🟠&nbsp;CVE-2026-73435 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the OSPFv2 routing process configuration is not configured. | - |
| s1-spine2 | 🟡&nbsp;CVE-2026-73436 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the OSPFv2 segment routing is disabled. | - |

### Security Advisory 0173 <a id="sa-0173"></a>

> **Severity:** 🟠 High\
> **URL:** <https://www.arista.com/en/support/advisories-notices/security-advisory/24729-security-advisory-0173>
>
> On affected Arista EOS releases with OSPFv3 configured, a peer can send a crafted packet that causes the OSPFv3 process to restart unexpectedly.
>
> | Vulnerability | Severity | Description |
> | :- | :- | :- |
> | CVE-2026-73455 | 🟠&nbsp;High | A crafted OSPFv3 packet may cause the OSPFv3 process to restart unexpectedly. |
>

#### 🔎 Device Findings

| Device | Vulnerability | Result | Findings | Remediations |
| :- | :- | :- | :- | :- |
| s1-brdr1 | 🟠&nbsp;CVE-2026-73455 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the OSPFv3 routing process is disabled and the OSPFv3 legacy IPv6 routing process is disabled. | - |
| s1-brdr2 | 🟠&nbsp;CVE-2026-73455 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the OSPFv3 routing process is disabled and the OSPFv3 legacy IPv6 routing process is disabled. | - |
| s1-leaf1 | 🟠&nbsp;CVE-2026-73455 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the OSPFv3 routing process is disabled and the OSPFv3 legacy IPv6 routing process is disabled. | - |
| s1-leaf2 | 🟠&nbsp;CVE-2026-73455 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the OSPFv3 routing process is disabled and the OSPFv3 legacy IPv6 routing process is disabled. | - |
| s1-leaf3 | 🟠&nbsp;CVE-2026-73455 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the OSPFv3 routing process is disabled and the OSPFv3 legacy IPv6 routing process is disabled. | - |
| s1-leaf4 | 🟠&nbsp;CVE-2026-73455 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the OSPFv3 routing process is disabled and the OSPFv3 legacy IPv6 routing process is disabled. | - |
| s1-spine1 | 🟠&nbsp;CVE-2026-73455 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the OSPFv3 routing process is disabled and the OSPFv3 legacy IPv6 routing process is disabled. | - |
| s1-spine2 | 🟠&nbsp;CVE-2026-73455 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the OSPFv3 routing process is disabled and the OSPFv3 legacy IPv6 routing process is disabled. | - |

### Security Advisory 0117 <a id="sa-0117"></a>

> **Severity:** 🟡 Medium\
> **URL:** <https://www.arista.com/en/support/advisories-notices/security-advisory/21394-security-advisory-0117>
>
> On affected platforms running Arista EOS with a gNMI transport enabled, running the gNOI File TransferToRemote RPC with credentials for a remote server may cause these remote-server credentials to be logged or accounted on the local EOS device or possibly on other remote accounting servers (i.e. TACACS, RADIUS, etc).
>
> | Vulnerability | Severity | Description |
> | :- | :- | :- |
> | CVE-2025-0936 | 🟡&nbsp;Medium | gNOI TransferToRemote credential exposure through OpenConfig accounting or tracing. |
>

#### 🔎 Device Findings

| Device | Vulnerability | Result | Findings | Remediations |
| :- | :- | :- | :- | :- |
| s1-brdr1 | 🟡&nbsp;CVE-2025-0936 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is outside the affected releases. | - |
| s1-brdr2 | 🟡&nbsp;CVE-2025-0936 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is outside the affected releases. | - |
| s1-leaf1 | 🟡&nbsp;CVE-2025-0936 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is outside the affected releases. | - |
| s1-leaf2 | 🟡&nbsp;CVE-2025-0936 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is outside the affected releases. | - |
| s1-leaf3 | 🟡&nbsp;CVE-2025-0936 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is outside the affected releases. | - |
| s1-leaf4 | 🟡&nbsp;CVE-2025-0936 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is outside the affected releases. | - |
| s1-spine1 | 🟡&nbsp;CVE-2025-0936 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is outside the affected releases. | - |
| s1-spine2 | 🟡&nbsp;CVE-2025-0936 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is outside the affected releases. | - |

### Security Advisory 0140 <a id="sa-0140"></a>

> **Severity:** 🟡 Medium\
> **URL:** <https://www.arista.com/en/support/advisories-notices/security-advisory/24074-security-advisory-0140>
>
> A user with local eos-admin privileges on affected Arista EOS (Extensible Operating System) platforms where secure boot is enabled can bypass Secure Boot Software Image (SWI) verification through the use of a specially crafted file.
>
> | Vulnerability | Severity | Description |
> | :- | :- | :- |
> | CVE-2026-10040 | 🟡&nbsp;Medium | Secure Boot Software Image verification bypass. |
>

#### 🔎 Device Findings

| Device | Vulnerability | Result | Findings | Remediations |
| :- | :- | :- | :- | :- |
| s1-brdr1 | 🟡&nbsp;CVE-2026-10040 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is outside the affected releases. | - |
| s1-brdr2 | 🟡&nbsp;CVE-2026-10040 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is outside the affected releases. | - |
| s1-leaf1 | 🟡&nbsp;CVE-2026-10040 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is outside the affected releases. | - |
| s1-leaf2 | 🟡&nbsp;CVE-2026-10040 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is outside the affected releases. | - |
| s1-leaf3 | 🟡&nbsp;CVE-2026-10040 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is outside the affected releases. | - |
| s1-leaf4 | 🟡&nbsp;CVE-2026-10040 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is outside the affected releases. | - |
| s1-spine1 | 🟡&nbsp;CVE-2026-10040 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is outside the affected releases. | - |
| s1-spine2 | 🟡&nbsp;CVE-2026-10040 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is outside the affected releases. | - |

### Security Advisory 0142 <a id="sa-0142"></a>

> **Severity:** 🟡 Medium\
> **URL:** <https://www.arista.com/en/support/advisories-notices/security-advisory/24111-security-advisory-0142>
>
> On affected platforms running Arista EOS (Extensible Operating System) configured with next-hop redirection features—such as Policy-Based Routing (PBR), Border Gateway Protocol (BGP) Flowspec, Traffic Policy, DirectFlow, or Segment Security—certain specific classes of IP packets requiring exception handling may bypass the configured redirection action. Instead of being redirected to the designated next hop, these packets may be handled via fallback software forwarding paths, which can result in the packets being routed according to the system's standard forwarding information.
>
> | Vulnerability | Severity | Description |
> | :- | :- | :- |
> | CVE-2026-12546 | 🟡&nbsp;Medium | Next-hop redirection bypass for packets requiring exception handling. |
>

#### 🔎 Device Findings

| Device | Vulnerability | Result | Findings | Remediations |
| :- | :- | :- | :- | :- |
| s1-brdr1 | 🟡&nbsp;CVE-2026-12546 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the next-hop redirection path using Policy-Based Routing configuration is not configured, the next-hop redirection path using BGP FlowSpec configuration is not configured, the next-hop redirection path using Traffic Policy configuration is not configured, the next-hop redirection path using DirectFlow configuration is not configured, and the next-hop redirection path using Segment Security configuration is not configured. | - |
| s1-brdr2 | 🟡&nbsp;CVE-2026-12546 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the next-hop redirection path using Policy-Based Routing configuration is not configured, the next-hop redirection path using BGP FlowSpec configuration is not configured, the next-hop redirection path using Traffic Policy configuration is not configured, the next-hop redirection path using DirectFlow configuration is not configured, and the next-hop redirection path using Segment Security configuration is not configured. | - |
| s1-leaf1 | 🟡&nbsp;CVE-2026-12546 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the next-hop redirection path using Policy-Based Routing configuration is not configured, the next-hop redirection path using BGP FlowSpec configuration is not configured, the next-hop redirection path using Traffic Policy configuration is not configured, the next-hop redirection path using DirectFlow configuration is not configured, and the next-hop redirection path using Segment Security configuration is not configured. | - |
| s1-leaf2 | 🟡&nbsp;CVE-2026-12546 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the next-hop redirection path using Policy-Based Routing configuration is not configured, the next-hop redirection path using BGP FlowSpec configuration is not configured, the next-hop redirection path using Traffic Policy configuration is not configured, the next-hop redirection path using DirectFlow configuration is not configured, and the next-hop redirection path using Segment Security configuration is not configured. | - |
| s1-leaf3 | 🟡&nbsp;CVE-2026-12546 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the next-hop redirection path using Policy-Based Routing configuration is not configured, the next-hop redirection path using BGP FlowSpec configuration is not configured, the next-hop redirection path using Traffic Policy configuration is not configured, the next-hop redirection path using DirectFlow configuration is not configured, and the next-hop redirection path using Segment Security configuration is not configured. | - |
| s1-leaf4 | 🟡&nbsp;CVE-2026-12546 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the next-hop redirection path using Policy-Based Routing configuration is not configured, the next-hop redirection path using BGP FlowSpec configuration is not configured, the next-hop redirection path using Traffic Policy configuration is not configured, the next-hop redirection path using DirectFlow configuration is not configured, and the next-hop redirection path using Segment Security configuration is not configured. | - |
| s1-spine1 | 🟡&nbsp;CVE-2026-12546 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the next-hop redirection path using Policy-Based Routing configuration is not configured, the next-hop redirection path using BGP FlowSpec configuration is not configured, the next-hop redirection path using Traffic Policy configuration is not configured, the next-hop redirection path using DirectFlow configuration is not configured, and the next-hop redirection path using Segment Security configuration is not configured. | - |
| s1-spine2 | 🟡&nbsp;CVE-2026-12546 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the next-hop redirection path using Policy-Based Routing configuration is not configured, the next-hop redirection path using BGP FlowSpec configuration is not configured, the next-hop redirection path using Traffic Policy configuration is not configured, the next-hop redirection path using DirectFlow configuration is not configured, and the next-hop redirection path using Segment Security configuration is not configured. | - |

### Security Advisory 0149 <a id="sa-0149"></a>

> **Severity:** 🟡 Medium\
> **URL:** <https://www.arista.com/en/support/advisories-notices/security-advisory/24705-security-advisory-0149>
>
> On affected physical EOS platforms, combined 802.1X and RADIUS proxy dynamic authorization may prevent local sessions from being disconnected.
>
> | Vulnerability | Severity | Description |
> | :- | :- | :- |
> | CVE-2026-73449 | 🟡&nbsp;Medium | RADIUS proxy processing may prevent dynamic authorization from reaching local 802.1X sessions. |
>

#### 🔎 Device Findings

| Device | Vulnerability | Result | Findings | Remediations |
| :- | :- | :- | :- | :- |
| s1-brdr1 | 🟡&nbsp;CVE-2026-73449 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the 802.1X dynamic authorization authenticator is disabled. | - |
| s1-brdr2 | 🟡&nbsp;CVE-2026-73449 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the 802.1X dynamic authorization authenticator is disabled. | - |
| s1-leaf1 | 🟡&nbsp;CVE-2026-73449 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the 802.1X dynamic authorization authenticator is disabled. | - |
| s1-leaf2 | 🟡&nbsp;CVE-2026-73449 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the 802.1X dynamic authorization authenticator is disabled. | - |
| s1-leaf3 | 🟡&nbsp;CVE-2026-73449 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the 802.1X dynamic authorization authenticator is disabled. | - |
| s1-leaf4 | 🟡&nbsp;CVE-2026-73449 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the 802.1X dynamic authorization authenticator is disabled. | - |
| s1-spine1 | 🟡&nbsp;CVE-2026-73449 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the 802.1X dynamic authorization authenticator is disabled. | - |
| s1-spine2 | 🟡&nbsp;CVE-2026-73449 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the 802.1X dynamic authorization authenticator is disabled. | - |

### Security Advisory 0150 <a id="sa-0150"></a>

> **Severity:** 🟡 Medium\
> **URL:** <https://www.arista.com/en/support/advisories-notices/security-advisory/24706-security-advisory-0150>
>
> On affected physical EOS platforms using 802.1X authentication with per-supplicant ACL authorization, transient or stale state may permit traffic without the intended ACL policy.
>
> | Vulnerability | Severity | Description |
> | :- | :- | :- |
> | CVE-2026-75944 | 🟡&nbsp;Medium | A stale supplicant ACL may be applied after re-authentication and an AclAgent restart. |
> | CVE-2026-75943 | 🔵&nbsp;Low | A removed or timed-out supplicant may briefly send traffic without ACL enforcement. |
> | CVE-2026-75945 | 🔵&nbsp;Low | A supplicant may remain authorized after all 802.1X hosts are cleared. |
> | CVE-2026-77191 | 🔵&nbsp;Low | An authenticated supplicant may briefly send traffic before its assigned ACL is enforced. |
>

#### 🔎 Device Findings

| Device | Vulnerability | Result | Findings | Remediations |
| :- | :- | :- | :- | :- |
| s1-brdr1 | 🔵&nbsp;CVE-2026-77191 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the 802.1X controlled authenticator is disabled. | - |
| s1-brdr1 | 🔵&nbsp;CVE-2026-75943 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the 802.1X controlled authenticator is disabled. | - |
| s1-brdr1 | 🟡&nbsp;CVE-2026-75944 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the 802.1X controlled authenticator is disabled. | - |
| s1-brdr1 | 🔵&nbsp;CVE-2026-75945 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the 802.1X controlled authenticator is disabled. | - |
| s1-brdr2 | 🔵&nbsp;CVE-2026-77191 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the 802.1X controlled authenticator is disabled. | - |
| s1-brdr2 | 🔵&nbsp;CVE-2026-75943 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the 802.1X controlled authenticator is disabled. | - |
| s1-brdr2 | 🟡&nbsp;CVE-2026-75944 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the 802.1X controlled authenticator is disabled. | - |
| s1-brdr2 | 🔵&nbsp;CVE-2026-75945 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the 802.1X controlled authenticator is disabled. | - |
| s1-leaf1 | 🔵&nbsp;CVE-2026-77191 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the 802.1X controlled authenticator is disabled. | - |
| s1-leaf1 | 🔵&nbsp;CVE-2026-75943 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the 802.1X controlled authenticator is disabled. | - |
| s1-leaf1 | 🟡&nbsp;CVE-2026-75944 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the 802.1X controlled authenticator is disabled. | - |
| s1-leaf1 | 🔵&nbsp;CVE-2026-75945 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the 802.1X controlled authenticator is disabled. | - |
| s1-leaf2 | 🔵&nbsp;CVE-2026-77191 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the 802.1X controlled authenticator is disabled. | - |
| s1-leaf2 | 🔵&nbsp;CVE-2026-75943 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the 802.1X controlled authenticator is disabled. | - |
| s1-leaf2 | 🟡&nbsp;CVE-2026-75944 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the 802.1X controlled authenticator is disabled. | - |
| s1-leaf2 | 🔵&nbsp;CVE-2026-75945 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the 802.1X controlled authenticator is disabled. | - |
| s1-leaf3 | 🔵&nbsp;CVE-2026-77191 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the 802.1X controlled authenticator is disabled. | - |
| s1-leaf3 | 🔵&nbsp;CVE-2026-75943 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the 802.1X controlled authenticator is disabled. | - |
| s1-leaf3 | 🟡&nbsp;CVE-2026-75944 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the 802.1X controlled authenticator is disabled. | - |
| s1-leaf3 | 🔵&nbsp;CVE-2026-75945 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the 802.1X controlled authenticator is disabled. | - |
| s1-leaf4 | 🔵&nbsp;CVE-2026-77191 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the 802.1X controlled authenticator is disabled. | - |
| s1-leaf4 | 🔵&nbsp;CVE-2026-75943 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the 802.1X controlled authenticator is disabled. | - |
| s1-leaf4 | 🟡&nbsp;CVE-2026-75944 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the 802.1X controlled authenticator is disabled. | - |
| s1-leaf4 | 🔵&nbsp;CVE-2026-75945 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the 802.1X controlled authenticator is disabled. | - |
| s1-spine1 | 🔵&nbsp;CVE-2026-77191 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the 802.1X controlled authenticator is disabled. | - |
| s1-spine1 | 🔵&nbsp;CVE-2026-75943 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the 802.1X controlled authenticator is disabled. | - |
| s1-spine1 | 🟡&nbsp;CVE-2026-75944 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the 802.1X controlled authenticator is disabled. | - |
| s1-spine1 | 🔵&nbsp;CVE-2026-75945 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the 802.1X controlled authenticator is disabled. | - |
| s1-spine2 | 🔵&nbsp;CVE-2026-77191 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the 802.1X controlled authenticator is disabled. | - |
| s1-spine2 | 🔵&nbsp;CVE-2026-75943 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the 802.1X controlled authenticator is disabled. | - |
| s1-spine2 | 🟡&nbsp;CVE-2026-75944 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the 802.1X controlled authenticator is disabled. | - |
| s1-spine2 | 🔵&nbsp;CVE-2026-75945 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the 802.1X controlled authenticator is disabled. | - |

### Security Advisory 0151 <a id="sa-0151"></a>

> **Severity:** 🟡 Medium\
> **URL:** <https://www.arista.com/en/support/advisories-notices/security-advisory/24707-security-advisory-0151>
>
> On affected 755 and 758 Series platforms, restarting or inserting a secondary switch card may cause shared IPv4 or IPv6 SVI ingress ACLs to stop functioning.
>
> | Vulnerability | Severity | Description |
> | :- | :- | :- |
> | CVE-2026-73451 | 🟡&nbsp;Medium | A shared SVI ingress ACL may stop functioning after a secondary switch-card event. |
>

#### 🔎 Device Findings

| Device | Vulnerability | Result | Findings | Remediations |
| :- | :- | :- | :- | :- |
| s1-brdr1 | 🟡&nbsp;CVE-2026-73451 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because platform 'cEOSLab' is outside the affected platform scope. | - |
| s1-brdr2 | 🟡&nbsp;CVE-2026-73451 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because platform 'cEOSLab' is outside the affected platform scope. | - |
| s1-leaf1 | 🟡&nbsp;CVE-2026-73451 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because platform 'cEOSLab' is outside the affected platform scope. | - |
| s1-leaf2 | 🟡&nbsp;CVE-2026-73451 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because platform 'cEOSLab' is outside the affected platform scope. | - |
| s1-leaf3 | 🟡&nbsp;CVE-2026-73451 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because platform 'cEOSLab' is outside the affected platform scope. | - |
| s1-leaf4 | 🟡&nbsp;CVE-2026-73451 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because platform 'cEOSLab' is outside the affected platform scope. | - |
| s1-spine1 | 🟡&nbsp;CVE-2026-73451 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because platform 'cEOSLab' is outside the affected platform scope. | - |
| s1-spine2 | 🟡&nbsp;CVE-2026-73451 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because platform 'cEOSLab' is outside the affected platform scope. | - |

### Security Advisory 0152 <a id="sa-0152"></a>

> **Severity:** 🟡 Medium\
> **URL:** <https://www.arista.com/en/support/advisories-notices/security-advisory/24708-security-advisory-0152>
>
> On affected EOS releases with login authentication and a password-capable SSH or Telnet service enabled, crafted passwords may create orphan sessions and exhaust authentication resources.
>
> | Vulnerability | Severity | Description |
> | :- | :- | :- |
> | CVE-2026-19641 | 🟡&nbsp;Medium | A crafted password may exhaust pending authentication sessions and prevent legitimate logins. |
>

#### 🔎 Device Findings

| Device | Vulnerability | Result | Findings | Remediations |
| :- | :- | :- | :- | :- |
| s1-brdr1 | 🟡&nbsp;CVE-2026-19641 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected, the AAA login authentication is enabled, and the AAA password-based management service is enabled. | Upgrade to EOS 4.36.1F or later in the 4.36 train.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-brdr2 | 🟡&nbsp;CVE-2026-19641 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected, the AAA login authentication is enabled, and the AAA password-based management service is enabled. | Upgrade to EOS 4.36.1F or later in the 4.36 train.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-leaf1 | 🟡&nbsp;CVE-2026-19641 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected, the AAA login authentication is enabled, and the AAA password-based management service is enabled. | Upgrade to EOS 4.36.1F or later in the 4.36 train.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-leaf2 | 🟡&nbsp;CVE-2026-19641 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected, the AAA login authentication is enabled, and the AAA password-based management service is enabled. | Upgrade to EOS 4.36.1F or later in the 4.36 train.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-leaf3 | 🟡&nbsp;CVE-2026-19641 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected, the AAA login authentication is enabled, and the AAA password-based management service is enabled. | Upgrade to EOS 4.36.1F or later in the 4.36 train.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-leaf4 | 🟡&nbsp;CVE-2026-19641 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected, the AAA login authentication is enabled, and the AAA password-based management service is enabled. | Upgrade to EOS 4.36.1F or later in the 4.36 train.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-spine1 | 🟡&nbsp;CVE-2026-19641 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected, the AAA login authentication is enabled, and the AAA password-based management service is enabled. | Upgrade to EOS 4.36.1F or later in the 4.36 train.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-spine2 | 🟡&nbsp;CVE-2026-19641 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected, the AAA login authentication is enabled, and the AAA password-based management service is enabled. | Upgrade to EOS 4.36.1F or later in the 4.36 train.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |

### Security Advisory 0153 <a id="sa-0153"></a>

> **Severity:** 🟡 Medium\
> **URL:** <https://www.arista.com/en/support/advisories-notices/security-advisory/24709-security-advisory-0153>
>
> On affected Arista EOS releases, specialized non-standard agent tracing may write plaintext private keys, user passwords, or TACACS+ shared keys to agent logs.
>
> | Vulnerability | Severity | Description |
> | :- | :- | :- |
> | CVE-2026-73465 | 🟡&nbsp;Medium | Private keys may be written in plaintext to ConfigAgent logs when risky tracing is enabled. |
> | CVE-2026-73466 | 🟡&nbsp;Medium | User passwords may be written in plaintext to Aaa logs when risky tracing is enabled. |
> | CVE-2026-73467 | 🟡&nbsp;Medium | TACACS+ shared keys may be written in plaintext to Aaa logs when risky tracing is enabled. |
>

#### 🔎 Device Findings

| Device | Vulnerability | Result | Findings | Remediations |
| :- | :- | :- | :- | :- |
| s1-brdr1 | 🟡&nbsp;CVE-2026-73465 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the agent tracing risk for ConfigAgent private keys is disabled. | - |
| s1-brdr1 | 🟡&nbsp;CVE-2026-73466 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the agent tracing risk for Aaa user passwords is disabled. | - |
| s1-brdr1 | 🟡&nbsp;CVE-2026-73467 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the agent tracing risk for Aaa TACACS+ shared keys is disabled. | - |
| s1-brdr2 | 🟡&nbsp;CVE-2026-73465 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the agent tracing risk for ConfigAgent private keys is disabled. | - |
| s1-brdr2 | 🟡&nbsp;CVE-2026-73466 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the agent tracing risk for Aaa user passwords is disabled. | - |
| s1-brdr2 | 🟡&nbsp;CVE-2026-73467 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the agent tracing risk for Aaa TACACS+ shared keys is disabled. | - |
| s1-leaf1 | 🟡&nbsp;CVE-2026-73465 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the agent tracing risk for ConfigAgent private keys is disabled. | - |
| s1-leaf1 | 🟡&nbsp;CVE-2026-73466 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the agent tracing risk for Aaa user passwords is disabled. | - |
| s1-leaf1 | 🟡&nbsp;CVE-2026-73467 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the agent tracing risk for Aaa TACACS+ shared keys is disabled. | - |
| s1-leaf2 | 🟡&nbsp;CVE-2026-73465 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the agent tracing risk for ConfigAgent private keys is disabled. | - |
| s1-leaf2 | 🟡&nbsp;CVE-2026-73466 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the agent tracing risk for Aaa user passwords is disabled. | - |
| s1-leaf2 | 🟡&nbsp;CVE-2026-73467 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the agent tracing risk for Aaa TACACS+ shared keys is disabled. | - |
| s1-leaf3 | 🟡&nbsp;CVE-2026-73465 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the agent tracing risk for ConfigAgent private keys is disabled. | - |
| s1-leaf3 | 🟡&nbsp;CVE-2026-73466 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the agent tracing risk for Aaa user passwords is disabled. | - |
| s1-leaf3 | 🟡&nbsp;CVE-2026-73467 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the agent tracing risk for Aaa TACACS+ shared keys is disabled. | - |
| s1-leaf4 | 🟡&nbsp;CVE-2026-73465 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the agent tracing risk for ConfigAgent private keys is disabled. | - |
| s1-leaf4 | 🟡&nbsp;CVE-2026-73466 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the agent tracing risk for Aaa user passwords is disabled. | - |
| s1-leaf4 | 🟡&nbsp;CVE-2026-73467 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the agent tracing risk for Aaa TACACS+ shared keys is disabled. | - |
| s1-spine1 | 🟡&nbsp;CVE-2026-73465 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the agent tracing risk for ConfigAgent private keys is disabled. | - |
| s1-spine1 | 🟡&nbsp;CVE-2026-73466 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the agent tracing risk for Aaa user passwords is disabled. | - |
| s1-spine1 | 🟡&nbsp;CVE-2026-73467 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the agent tracing risk for Aaa TACACS+ shared keys is disabled. | - |
| s1-spine2 | 🟡&nbsp;CVE-2026-73465 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the agent tracing risk for ConfigAgent private keys is disabled. | - |
| s1-spine2 | 🟡&nbsp;CVE-2026-73466 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the agent tracing risk for Aaa user passwords is disabled. | - |
| s1-spine2 | 🟡&nbsp;CVE-2026-73467 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the agent tracing risk for Aaa TACACS+ shared keys is disabled. | - |

### Security Advisory 0155 <a id="sa-0155"></a>

> **Severity:** 🟡 Medium\
> **URL:** <https://www.arista.com/en/support/advisories-notices/security-advisory/24711-security-advisory-0155>
>
> On affected EOS releases, a crafted packet may restart DHCP relay when DHCP relay, snooping, or server matching uses Option 82.
>
> | Vulnerability | Severity | Description |
> | :- | :- | :- |
> | CVE-2026-19655 | 🟡&nbsp;Medium | A crafted DHCP Option 82 packet may restart the DHCP relay service. |
>

#### 🔎 Device Findings

| Device | Vulnerability | Result | Findings | Remediations |
| :- | :- | :- | :- | :- |
| s1-brdr1 | 🟡&nbsp;CVE-2026-19655 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the DHCP Option 82 exposure is disabled. | - |
| s1-brdr2 | 🟡&nbsp;CVE-2026-19655 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the DHCP Option 82 exposure is disabled. | - |
| s1-leaf1 | 🟡&nbsp;CVE-2026-19655 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the DHCP Option 82 exposure is disabled. | - |
| s1-leaf2 | 🟡&nbsp;CVE-2026-19655 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the DHCP Option 82 exposure is disabled. | - |
| s1-leaf3 | 🟡&nbsp;CVE-2026-19655 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the DHCP Option 82 exposure is disabled. | - |
| s1-leaf4 | 🟡&nbsp;CVE-2026-19655 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the DHCP Option 82 exposure is disabled. | - |
| s1-spine1 | 🟡&nbsp;CVE-2026-19655 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the DHCP Option 82 exposure is disabled. | - |
| s1-spine2 | 🟡&nbsp;CVE-2026-19655 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the DHCP Option 82 exposure is disabled. | - |

### Security Advisory 0157 <a id="sa-0157"></a>

> **Severity:** 🟡 Medium\
> **URL:** <https://www.arista.com/en/support/advisories-notices/security-advisory/24713-security-advisory-0157>
>
> On affected EOS releases, VRRP authentication may be bypassed, replayed, or exposed in logs depending on configuration.
>
> | Vulnerability | Severity | Description |
> | :- | :- | :- |
> | CVE-2026-73443 | 🟡&nbsp;Medium | VRRPv2 IP-AH advertisements may be captured and replayed indefinitely. |
> | CVE-2026-73444 | 🟡&nbsp;Medium | VRRPv2 IP-AH authentication may be bypassed by an adjacent attacker. |
> | CVE-2026-73442 | 🔵&nbsp;Low | Peer VRRP authentication credentials may be written to agent trace logs. |
>

#### 🔎 Device Findings

| Device | Vulnerability | Result | Findings | Remediations |
| :- | :- | :- | :- | :- |
| s1-brdr1 | 🟡&nbsp;CVE-2026-73444 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the VRRP version 2 IP-AH authentication is disabled. | - |
| s1-brdr1 | 🟡&nbsp;CVE-2026-73443 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the VRRP version 2 IP-AH authentication is disabled. | - |
| s1-brdr1 | 🔵&nbsp;CVE-2026-73442 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the VRRP feature is disabled. | - |
| s1-brdr2 | 🟡&nbsp;CVE-2026-73444 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the VRRP version 2 IP-AH authentication is disabled. | - |
| s1-brdr2 | 🟡&nbsp;CVE-2026-73443 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the VRRP version 2 IP-AH authentication is disabled. | - |
| s1-brdr2 | 🔵&nbsp;CVE-2026-73442 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the VRRP feature is disabled. | - |
| s1-leaf1 | 🟡&nbsp;CVE-2026-73444 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the VRRP version 2 IP-AH authentication is disabled. | - |
| s1-leaf1 | 🟡&nbsp;CVE-2026-73443 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the VRRP version 2 IP-AH authentication is disabled. | - |
| s1-leaf1 | 🔵&nbsp;CVE-2026-73442 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the VRRP feature is disabled. | - |
| s1-leaf2 | 🟡&nbsp;CVE-2026-73444 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the VRRP version 2 IP-AH authentication is disabled. | - |
| s1-leaf2 | 🟡&nbsp;CVE-2026-73443 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the VRRP version 2 IP-AH authentication is disabled. | - |
| s1-leaf2 | 🔵&nbsp;CVE-2026-73442 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the VRRP feature is disabled. | - |
| s1-leaf3 | 🟡&nbsp;CVE-2026-73444 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the VRRP version 2 IP-AH authentication is disabled. | - |
| s1-leaf3 | 🟡&nbsp;CVE-2026-73443 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the VRRP version 2 IP-AH authentication is disabled. | - |
| s1-leaf3 | 🔵&nbsp;CVE-2026-73442 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the VRRP feature is disabled. | - |
| s1-leaf4 | 🟡&nbsp;CVE-2026-73444 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the VRRP version 2 IP-AH authentication is disabled. | - |
| s1-leaf4 | 🟡&nbsp;CVE-2026-73443 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the VRRP version 2 IP-AH authentication is disabled. | - |
| s1-leaf4 | 🔵&nbsp;CVE-2026-73442 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the VRRP feature is disabled. | - |
| s1-spine1 | 🟡&nbsp;CVE-2026-73444 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the VRRP version 2 IP-AH authentication is disabled. | - |
| s1-spine1 | 🟡&nbsp;CVE-2026-73443 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the VRRP version 2 IP-AH authentication is disabled. | - |
| s1-spine1 | 🔵&nbsp;CVE-2026-73442 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the VRRP feature is disabled. | - |
| s1-spine2 | 🟡&nbsp;CVE-2026-73444 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the VRRP version 2 IP-AH authentication is disabled. | - |
| s1-spine2 | 🟡&nbsp;CVE-2026-73443 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the VRRP version 2 IP-AH authentication is disabled. | - |
| s1-spine2 | 🔵&nbsp;CVE-2026-73442 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the VRRP feature is disabled. | - |

### Security Advisory 0159 <a id="sa-0159"></a>

> **Severity:** 🟡 Medium\
> **URL:** <https://www.arista.com/en/support/advisories-notices/security-advisory/24715-security-advisory-0159>
>
> Malformed network packets can cause the IGMP snooping agent to terminate unexpectedly and temporarily disrupt multicast traffic management.
>
> | Vulnerability | Severity | Description |
> | :- | :- | :- |
> | CVE-2026-73462 | 🟡&nbsp;Medium | Malformed network packets can cause the IGMP snooping agent to terminate unexpectedly. |
>

#### 🔎 Device Findings

| Device | Vulnerability | Result | Findings | Remediations |
| :- | :- | :- | :- | :- |
| s1-brdr1 | 🟡&nbsp;CVE-2026-73462 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected. | Upgrade to EOS 4.36.2F or later in the 4.36 train.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-brdr2 | 🟡&nbsp;CVE-2026-73462 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected. | Upgrade to EOS 4.36.2F or later in the 4.36 train.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-leaf1 | 🟡&nbsp;CVE-2026-73462 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected. | Upgrade to EOS 4.36.2F or later in the 4.36 train.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-leaf2 | 🟡&nbsp;CVE-2026-73462 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected. | Upgrade to EOS 4.36.2F or later in the 4.36 train.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-leaf3 | 🟡&nbsp;CVE-2026-73462 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected. | Upgrade to EOS 4.36.2F or later in the 4.36 train.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-leaf4 | 🟡&nbsp;CVE-2026-73462 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected. | Upgrade to EOS 4.36.2F or later in the 4.36 train.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-spine1 | 🟡&nbsp;CVE-2026-73462 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected. | Upgrade to EOS 4.36.2F or later in the 4.36 train.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |
| s1-spine2 | 🟡&nbsp;CVE-2026-73462 | 🛑&nbsp;Affected | The device is affected because EOS version '4.36.0.1F-47425148.43601F (engineering build)' is affected. | Upgrade to EOS 4.36.2F or later in the 4.36 train.<br>Refer to the advisory for newly fixed releases and current mitigation guidance. |

### Security Advisory 0161 <a id="sa-0161"></a>

> **Severity:** 🟡 Medium\
> **URL:** <https://www.arista.com/en/support/advisories-notices/security-advisory/24717-security-advisory-0161>
>
> On affected EOS releases with MLAG dual-primary heartbeat and errdisable-all configured, forged heartbeat packets may interrupt traffic.
>
> | Vulnerability | Severity | Description |
> | :- | :- | :- |
> | CVE-2026-73450 | 🟡&nbsp;Medium | Forged MLAG dual-primary heartbeat packets may errdisable interfaces and interrupt traffic. |
>

#### 🔎 Device Findings

| Device | Vulnerability | Result | Findings | Remediations |
| :- | :- | :- | :- | :- |
| s1-brdr1 | 🟡&nbsp;CVE-2026-73450 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the MLAG dual-primary heartbeat with errdisable-all action is disabled. | - |
| s1-brdr2 | 🟡&nbsp;CVE-2026-73450 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the MLAG dual-primary heartbeat with errdisable-all action is disabled. | - |
| s1-leaf1 | 🟡&nbsp;CVE-2026-73450 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the MLAG dual-primary heartbeat with errdisable-all action is disabled. | - |
| s1-leaf2 | 🟡&nbsp;CVE-2026-73450 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the MLAG dual-primary heartbeat with errdisable-all action is disabled. | - |
| s1-leaf3 | 🟡&nbsp;CVE-2026-73450 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the MLAG dual-primary heartbeat with errdisable-all action is disabled. | - |
| s1-leaf4 | 🟡&nbsp;CVE-2026-73450 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the MLAG dual-primary heartbeat with errdisable-all action is disabled. | - |
| s1-spine1 | 🟡&nbsp;CVE-2026-73450 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the MLAG dual-primary heartbeat with errdisable-all action is disabled. | - |
| s1-spine2 | 🟡&nbsp;CVE-2026-73450 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the MLAG dual-primary heartbeat with errdisable-all action is disabled. | - |

### Security Advisory 0167 <a id="sa-0167"></a>

> **Severity:** 🟡 Medium\
> **URL:** <https://www.arista.com/en/support/advisories-notices/security-advisory/24723-security-advisory-0167>
>
> On affected platforms running Arista EOS, an issue with the gRPC Network Security Interface (gNSI) Authz Rotate RPC may cause an incorrect Authz policy which was uploaded in the ongoing RPC stream to become active. This does not affect Bootz.
>
> | Vulnerability | Severity | Description |
> | :- | :- | :- |
> | CVE-2026-73445 | 🟡&nbsp;Medium | gNSI Authz Rotate RPC may activate an unintended policy from an ongoing stream. |
>

#### 🔎 Device Findings

| Device | Vulnerability | Result | Findings | Remediations |
| :- | :- | :- | :- | :- |
| s1-brdr1 | 🟡&nbsp;CVE-2026-73445 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNSI transport is disabled. | - |
| s1-brdr2 | 🟡&nbsp;CVE-2026-73445 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNSI transport is disabled. | - |
| s1-leaf1 | 🟡&nbsp;CVE-2026-73445 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNSI transport is disabled. | - |
| s1-leaf2 | 🟡&nbsp;CVE-2026-73445 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNSI transport is disabled. | - |
| s1-leaf3 | 🟡&nbsp;CVE-2026-73445 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNSI transport is disabled. | - |
| s1-leaf4 | 🟡&nbsp;CVE-2026-73445 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNSI transport is disabled. | - |
| s1-spine1 | 🟡&nbsp;CVE-2026-73445 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNSI transport is disabled. | - |
| s1-spine2 | 🟡&nbsp;CVE-2026-73445 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNSI transport is disabled. | - |

### Security Advisory 0169 <a id="sa-0169"></a>

> **Severity:** 🟡 Medium\
> **URL:** <https://www.arista.com/en/support/advisories-notices/security-advisory/24725-security-advisory-0169>
>
> On affected EOS releases, a race involving multiple gNSI transports may cause an Authz policy rotation to fail silently and retain access revoked by the new policy.
>
> | Vulnerability | Severity | Description |
> | :- | :- | :- |
> | CVE-2026-73463 | 🟡&nbsp;Medium | A gNSI Authz policy rotation may silently retain a stale authorization policy. |
>

#### 🔎 Device Findings

| Device | Vulnerability | Result | Findings | Remediations |
| :- | :- | :- | :- | :- |
| s1-brdr1 | 🟡&nbsp;CVE-2026-73463 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNSI transport is disabled. | - |
| s1-brdr2 | 🟡&nbsp;CVE-2026-73463 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNSI transport is disabled. | - |
| s1-leaf1 | 🟡&nbsp;CVE-2026-73463 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNSI transport is disabled. | - |
| s1-leaf2 | 🟡&nbsp;CVE-2026-73463 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNSI transport is disabled. | - |
| s1-leaf3 | 🟡&nbsp;CVE-2026-73463 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNSI transport is disabled. | - |
| s1-leaf4 | 🟡&nbsp;CVE-2026-73463 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNSI transport is disabled. | - |
| s1-spine1 | 🟡&nbsp;CVE-2026-73463 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNSI transport is disabled. | - |
| s1-spine2 | 🟡&nbsp;CVE-2026-73463 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNSI transport is disabled. | - |

### Security Advisory 0170 <a id="sa-0170"></a>

> **Severity:** 🟡 Medium\
> **URL:** <https://www.arista.com/en/support/advisories-notices/security-advisory/24726-security-advisory-0170>
>
> On affected EOS releases, authenticated gNMI users may retain access beyond their current authorization policy.
>
> | Vulnerability | Severity | Description |
> | :- | :- | :- |
> | CVE-2026-19640 | 🟡&nbsp;Medium | Existing gNMI subscriptions may retain authorization granted before an AAA policy change. |
>

#### 🔎 Device Findings

| Device | Vulnerability | Result | Findings | Remediations |
| :- | :- | :- | :- | :- |
| s1-brdr1 | 🟡&nbsp;CVE-2026-19640 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNMI request authorization is disabled. | - |
| s1-brdr2 | 🟡&nbsp;CVE-2026-19640 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNMI request authorization is disabled. | - |
| s1-leaf1 | 🟡&nbsp;CVE-2026-19640 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNMI request authorization is disabled. | - |
| s1-leaf2 | 🟡&nbsp;CVE-2026-19640 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNMI request authorization is disabled. | - |
| s1-leaf3 | 🟡&nbsp;CVE-2026-19640 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNMI request authorization is disabled. | - |
| s1-leaf4 | 🟡&nbsp;CVE-2026-19640 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNMI request authorization is disabled. | - |
| s1-spine1 | 🟡&nbsp;CVE-2026-19640 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNMI request authorization is disabled. | - |
| s1-spine2 | 🟡&nbsp;CVE-2026-19640 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the gNMI request authorization is disabled. | - |

### Security Advisory 0172 <a id="sa-0172"></a>

> **Severity:** 🟡 Medium\
> **URL:** <https://www.arista.com/en/support/advisories-notices/security-advisory/24728-security-advisory-0172>
>
> On affected EOS releases with OSPFv3 configured, crafted packets may restart the OSPFv3 agent and disrupt routing.
>
> | Vulnerability | Severity | Description |
> | :- | :- | :- |
> | CVE-2026-73438 | 🟡&nbsp;Medium | Crafted packets may restart OSPFv3 and disrupt routing adjacencies. |
>

#### 🔎 Device Findings

| Device | Vulnerability | Result | Findings | Remediations |
| :- | :- | :- | :- | :- |
| s1-brdr1 | 🟡&nbsp;CVE-2026-73438 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the OSPFv3 routing process is disabled and the OSPFv3 legacy IPv6 routing process is disabled. | - |
| s1-brdr2 | 🟡&nbsp;CVE-2026-73438 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the OSPFv3 routing process is disabled and the OSPFv3 legacy IPv6 routing process is disabled. | - |
| s1-leaf1 | 🟡&nbsp;CVE-2026-73438 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the OSPFv3 routing process is disabled and the OSPFv3 legacy IPv6 routing process is disabled. | - |
| s1-leaf2 | 🟡&nbsp;CVE-2026-73438 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the OSPFv3 routing process is disabled and the OSPFv3 legacy IPv6 routing process is disabled. | - |
| s1-leaf3 | 🟡&nbsp;CVE-2026-73438 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the OSPFv3 routing process is disabled and the OSPFv3 legacy IPv6 routing process is disabled. | - |
| s1-leaf4 | 🟡&nbsp;CVE-2026-73438 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the OSPFv3 routing process is disabled and the OSPFv3 legacy IPv6 routing process is disabled. | - |
| s1-spine1 | 🟡&nbsp;CVE-2026-73438 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the OSPFv3 routing process is disabled and the OSPFv3 legacy IPv6 routing process is disabled. | - |
| s1-spine2 | 🟡&nbsp;CVE-2026-73438 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the OSPFv3 routing process is disabled and the OSPFv3 legacy IPv6 routing process is disabled. | - |

### Security Advisory 0175 <a id="sa-0175"></a>

> **Severity:** 🟡 Medium\
> **URL:** <https://www.arista.com/en/support/advisories-notices/security-advisory/24731-security-advisory-0175>
>
> On affected Arista EOS releases with PIM sparse mode configured, a crafted packet can prematurely expire multicast forwarding state and temporarily disrupt multicast traffic.
>
> | Vulnerability | Severity | Description |
> | :- | :- | :- |
> | CVE-2026-73468 | 🟡&nbsp;Medium | A crafted packet may prematurely expire multicast forwarding state on PIM sparse-mode interfaces. |
>

#### 🔎 Device Findings

| Device | Vulnerability | Result | Findings | Remediations |
| :- | :- | :- | :- | :- |
| s1-brdr1 | 🟡&nbsp;CVE-2026-73468 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the PIM sparse-mode interface is disabled. | - |
| s1-brdr2 | 🟡&nbsp;CVE-2026-73468 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the PIM sparse-mode interface is disabled. | - |
| s1-leaf1 | 🟡&nbsp;CVE-2026-73468 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the PIM sparse-mode interface is disabled. | - |
| s1-leaf2 | 🟡&nbsp;CVE-2026-73468 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the PIM sparse-mode interface is disabled. | - |
| s1-leaf3 | 🟡&nbsp;CVE-2026-73468 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the PIM sparse-mode interface is disabled. | - |
| s1-leaf4 | 🟡&nbsp;CVE-2026-73468 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the PIM sparse-mode interface is disabled. | - |
| s1-spine1 | 🟡&nbsp;CVE-2026-73468 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the PIM sparse-mode interface is disabled. | - |
| s1-spine2 | 🟡&nbsp;CVE-2026-73468 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the PIM sparse-mode interface is disabled. | - |

### Security Advisory 0176 <a id="sa-0176"></a>

> **Severity:** 🟡 Medium\
> **URL:** <https://www.arista.com/en/support/advisories-notices/security-advisory/24732-security-advisory-0176>
>
> On affected 7050X4 and 7358X4 platforms running affected EOS releases, traffic received on an interface configured with loose Unicast Reverse Path Forwarding may bypass the intended verification drop.
>
> | Vulnerability | Severity | Description |
> | :- | :- | :- |
> | CVE-2026-73469 | 🟡&nbsp;Medium | Loose uRPF may fail to drop traffic that should not pass source verification. |
>

#### 🔎 Device Findings

| Device | Vulnerability | Result | Findings | Remediations |
| :- | :- | :- | :- | :- |
| s1-brdr1 | 🟡&nbsp;CVE-2026-73469 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the uRPF loose-mode interface is disabled. | - |
| s1-brdr2 | 🟡&nbsp;CVE-2026-73469 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the uRPF loose-mode interface is disabled. | - |
| s1-leaf1 | 🟡&nbsp;CVE-2026-73469 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the uRPF loose-mode interface is disabled. | - |
| s1-leaf2 | 🟡&nbsp;CVE-2026-73469 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the uRPF loose-mode interface is disabled. | - |
| s1-leaf3 | 🟡&nbsp;CVE-2026-73469 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the uRPF loose-mode interface is disabled. | - |
| s1-leaf4 | 🟡&nbsp;CVE-2026-73469 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the uRPF loose-mode interface is disabled. | - |
| s1-spine1 | 🟡&nbsp;CVE-2026-73469 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the uRPF loose-mode interface is disabled. | - |
| s1-spine2 | 🟡&nbsp;CVE-2026-73469 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the uRPF loose-mode interface is disabled. | - |

### Security Advisory 0177 <a id="sa-0177"></a>

> **Severity:** 🟡 Medium\
> **URL:** <https://www.arista.com/en/support/advisories-notices/security-advisory/24733-security-advisory-0177>
>
> On affected Arista EOS releases and platforms with PIM Sparse Mode and active MLAG, malformed messages may repeatedly restart the Pimsm agent and cause a sustained denial of service.
>
> | Vulnerability | Severity | Description |
> | :- | :- | :- |
> | CVE-2026-77190 | 🟡&nbsp;Medium | Malformed PIM sparse-mode messages may repeatedly restart the Pimsm agent and cause a sustained denial of service. |
>

#### 🔎 Device Findings

| Device | Vulnerability | Result | Findings | Remediations |
| :- | :- | :- | :- | :- |
| s1-brdr1 | 🟡&nbsp;CVE-2026-77190 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the PIM sparse-mode interface is disabled. | - |
| s1-brdr2 | 🟡&nbsp;CVE-2026-77190 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the PIM sparse-mode interface is disabled. | - |
| s1-leaf1 | 🟡&nbsp;CVE-2026-77190 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the PIM sparse-mode interface is disabled. | - |
| s1-leaf2 | 🟡&nbsp;CVE-2026-77190 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the PIM sparse-mode interface is disabled. | - |
| s1-leaf3 | 🟡&nbsp;CVE-2026-77190 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the PIM sparse-mode interface is disabled. | - |
| s1-leaf4 | 🟡&nbsp;CVE-2026-77190 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the PIM sparse-mode interface is disabled. | - |
| s1-spine1 | 🟡&nbsp;CVE-2026-77190 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the PIM sparse-mode interface is disabled. | - |
| s1-spine2 | 🟡&nbsp;CVE-2026-77190 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the PIM sparse-mode interface is disabled. | - |

### Security Advisory 0178 <a id="sa-0178"></a>

> **Severity:** 🟡 Medium\
> **URL:** <https://www.arista.com/en/support/advisories-notices/security-advisory/24734-security-advisory-0178>
>
> On affected Arista EOS releases, local or remote SNMPv3 authentication keys may be exposed as one-way hashed localized values in running and sanitized configuration.
>
> | Vulnerability | Severity | Description |
> | :- | :- | :- |
> | CVE-2026-73440 | 🟡&nbsp;Medium | SNMPv3 authentication keys may be exposed as hashed localized values in configuration. |
>

#### 🔎 Device Findings

| Device | Vulnerability | Result | Findings | Remediations |
| :- | :- | :- | :- | :- |
| s1-brdr1 | 🟡&nbsp;CVE-2026-73440 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the SNMPv3 authentication key is disabled. | - |
| s1-brdr2 | 🟡&nbsp;CVE-2026-73440 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the SNMPv3 authentication key is disabled. | - |
| s1-leaf1 | 🟡&nbsp;CVE-2026-73440 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the SNMPv3 authentication key is disabled. | - |
| s1-leaf2 | 🟡&nbsp;CVE-2026-73440 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the SNMPv3 authentication key is disabled. | - |
| s1-leaf3 | 🟡&nbsp;CVE-2026-73440 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the SNMPv3 authentication key is disabled. | - |
| s1-leaf4 | 🟡&nbsp;CVE-2026-73440 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the SNMPv3 authentication key is disabled. | - |
| s1-spine1 | 🟡&nbsp;CVE-2026-73440 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the SNMPv3 authentication key is disabled. | - |
| s1-spine2 | 🟡&nbsp;CVE-2026-73440 | ✅&nbsp;Not&nbsp;Affected | The device is not affected because the SNMPv3 authentication key is disabled. | - |

## 📋 Run Overview <a id="run-overview"></a>

| | |
| :- | :- |
| **ANTA Version** | v1.10.0 |
| **Duration** | 2 seconds (2026-10-28 19:51:29.684+00:00 → 2026-10-28 19:51:32.327+00:00) |
| **Security Advisories Tested** | 35 |
| **Total Devices In Inventory** | 8 |
| **Devices Assessed** | 8 |
| **Devices Unreachable At Setup** | None |
| **Devices Filtered At Setup** | None |
| **Filters Applied** | None |
