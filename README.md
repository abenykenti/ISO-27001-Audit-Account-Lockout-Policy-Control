# SecureAuth-AD ISO 27001 Compliance Audit Report

## Audit Overview
**Audit Focus:**  
ISO 27001 Audit – Account Lockout Policy Control

**Objective:**  
Evaluate the Active Directory system based on ISO 27001 controls to assess the implementation and effectiveness of account lockout mechanisms.

---

## 1. Scope Definition
The audit focuses on user access management, particularly on the secure logon procedures as defined in **ISO 27001 Annex A.9.4.2** (Secure Logon Procedures).

---

## 2. Audit Focus: A.9.4.2 Control

### Control Family: Annex A.9
**Control:** A.9.4.2 (Secure Logon Procedures)

### Evaluation Against ISO 27001 A.9.4.2 Requirements:
- **Requirement:** Systems must implement appropriate user authentication controls, including managing failed login attempts.
- **Expected Control:** Failed login attempts should trigger an account lockout to prevent unauthorized access.

---

## 3. Audit Findings
The review revealed that the **Active Directory environment lacks a Group Policy** to lock user accounts after repeated failed login attempts.

### Key Findings:
- **Risk Exposure:** The absence of this control significantly increases the risk of unauthorized access due to brute force or other attack methods.
- **Compliance Impact:** This represents a non-compliance with ISO 27001's A.9.4.2 control, indicating a critical security gap.

---

## 4. Recommendations

To mitigate the risks and align with ISO 27001 standards:

- **Policy Implementation:**  
  Configure a Group Policy to **lock accounts after 5 failed login attempts**, with a reset after **30 minutes**.
  
- **Regular Audits:**  
  Perform regular audits to verify that the policy is functioning correctly and is properly documented.

---

## 5. Conclusion
The lack of an account lockout policy represents **non-compliance** with **ISO 27001 A.9.4.2**. Immediate corrective actions are necessary to mitigate potential security risks and ensure compliance with the ISO standard.

---


