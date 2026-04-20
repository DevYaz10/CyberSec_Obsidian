## The CIA Triad

>The CIA triad is an information security model that is used in consideration throughout creating a security policy.

it consists of:
- Confidentiality: This element is the protection of data from unauthorized access and misuse.
- Integrity: The condition where information is kept accurate and consistent unless authorized changes are made.
- Availability: The information should be available when authorized users need to access it.


## Principles of Privileges

The levels of access given to individuals are determined on two primary factors:
- The individual's **role/function** within the organization
- The sensitivity of the information being stored on the system

2 Concepts of access rights management in an organization:
- Privileged Identity Management (PIM)
- Privileged Access Management (PAM)

>[!Info]
>users should be given the minimum amount of privileges


## Security Models Continued

>[!Info]
>any system or piece of technology storing information is called an information system


### The Bell-LaPadula Model

- **used to achieve confidentiality**, and prevent leakage of sensitive information
- Used in military or anywhere where the information are secret or should be hidden
- "No Write Down, No Read Up" which means you can't read information from a higher security level or write, save, or transfer information of a lower-level system (or individual) 
- ![[Pasted image 20260420222514.png|269]]


### Biba Model 

- arguably the equivalent of the Bell-La Padula model but **for the integrity of the CIA triad**.
- It prevents "low-integrity" users from corrupting "high-integrity" data.
- Used in software development or finance or anywhere where information are critical to modify but disclosed or public 
- "No Read Down, No Write Up" here is the opposite where u can read higher-level data but you can't modify it or transfer data to a higher level, you can't read lower-level data thus you can't read it ig
- ![[Pasted image 20260420223654.png|269]]



## Threat Modelling & Incident Response

### Threat Modelling 

>[!quote] Definition
> Threat modelling is the process of reviewing, improving, and testing the security protocols in place in an organisation's information technology infrastructure and services.


Threat Modelling Process:
1. Identification
2. Preparation
3. Mitigations
4. Review
![[Pasted image 20260420230619.png|212]]

An effective threat model includes:
- Threat intelligence
- Asset identification
- Mitigation capabilities
- Risk assessment

#### STRIDE 

>[!Info] Abrriviation
>**S**poofing identity, **T**ampering with data, **R**epudiation threats, **I**nformation disclosure, **D**enial of Service and **E**levation of privileges

| **Principle**          | **Description**                                                                                                                                                                                                                                               |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Spoofing               | This principle requires you to authenticate requests and users accessing a system. Spoofing involves a malicious party falsely identifying itself as another.<br><br>Access keys (such as API keys) or signatures via encryption helps remediate this threat. |
| Tampering              | By providing anti-tampering measures to a system or application, you help provide integrity to the data. Data that is accessed must be kept integral and accurate.<br><br>For example, shops use seals on food products.                                      |
| Repudiation            | This principle dictates the use of services such as logging of activity for a system or application to track.                                                                                                                                                 |
| Information Disclosure | Applications or services that handle information of multiple users need to be appropriately configured to only show information relevant to the owner.                                                                                                        |
| Denial of Service      | Applications and services use up system resources, these two things should have measures in place so that abuse of the application/service won't result in bringing the whole system down.                                                                    |
| Elevation of Privilege | This is the worst-case scenario for an application or service. It means that a user was able to escalate their authorization to that of a higher level i.e. an administrator. This scenario often leads to further exploitation or information disclosure.    |

### Incident Response

>[!quote] Definition
>A breach of security is known as an *incident*.
>Actions taken to resolve and remediate the threat are known as **Incident Response (IR)**

>An incident is responded to by a **C**omputer **S**ecurity **I**ncident **R**esponse **T**eam (**CSIRT**) which is prearranged group of employees with technical knowledge about the systems and/or current incident.


6 Phases of incident response:

| **Action**      | **Description**                                                                                                                             |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------- |
| Preparation     | Do we have the resources and plans in place to deal with the security incident?                                                             |
| Identification  | Has the threat and the threat actor been correctly identified in order for us to respond to?                                                |
| Containment     | Can the threat/security incident be contained to prevent other systems or users from being impacted?                                        |
| Eradication     | Remove the active threat.                                                                                                                   |
| Recovery        | Perform a full review of the impacted systems to return to business as usual operations.                                                    |
| Lessons Learned | What can be learnt from the incident? I.e. if it was due to a phishing email, employees should be trained better to detect phishing emails. |
