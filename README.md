# Vulnerability Management Program Implementation

In this project, we simulate the implementation of a comprehensive vulnerability management program, from inception to completion.

_**Inception State:**_ the organization has no existing policy or vulnerability management practices in place.

_**Completion State:**_ a formal policy is enacted, stakeholder buy-in is secured, and a full cycle of organization-wide vulnerability remediation is successfully completed.

---

<img width="1000" alt="image" src="https://github.com/user-attachments/assets/cfc5dbcf-3fcb-4a71-9c13-2a49f8bab3e6">

# Technology Utilized
- Tenable (enterprise vulnerability management platform)
- Azure Virtual Machines (Nessus scan engine + scan targets)
- PowerShell & BASH (remediation scripts)

---


# Table of Contents

- [Vulnerability Management Policy Draft Creation](#vulnerability-management-policy-draft-creation)
- [Mock Meeting: Policy Buy-In (Stakeholders)](#step-2-mock-meeting-policy-buy-in-stakeholders)
- [Policy Finalization and Senior Leadership Sign-Off](#step-3-policy-finalization-and-senior-leadership-sign-off)
- [Mock Meeting: Initial Scan Permission (Server Team)](#step-4-mock-meeting-initial-scan-permission-server-team)
- [Initial Scan of Server Team Assets](#step-5-initial-scan-of-server-team-assets)
- [Vulnerability Assessment and Prioritization](#step-6-vulnerability-assessment-and-prioritization)
- [Distributing Remediations to Remediation Teams](#step-7-distributing-remediations-to-remediation-teams)
- [Mock Meeting: Post-Initial Discovery Scan (Server Team)](#step-8-mock-meeting-post-initial-discovery-scan-server-team)
- [Mock CAB Meeting: Implementing Remediations](#step-9-mock-cab-meeting-implementing-remediations)
- [Remediation Round 1: Outdated Wireshark Removal](#remediation-round-1-outdated-wireshark-removal)
- [Remediation Round 2: Insecure Protocols & Ciphers](#remediation-round-2-insecure-protocols--ciphers)
- [Remediation Round 3: Guest Account Group Membership](#remediation-round-3-guest-account-group-membership)
- [Remediation Round 4: Windows OS Updates](#remediation-round-4-windows-os-updates)
- [First Cycle Remediation Effort Summary](#first-cycle-remediation-effort-summary)

---

### Vulnerability Management Policy Draft Creation

This phase focuses on drafting a Vulnerability Management Policy as a starting point for stakeholder engagement. The initial draft outlines scope, responsibilities, and remediation timelines, and may be adjusted based on feedback from relevant departments to ensure practical implementation before final approval by upper management.  
[Draft Policy](https://docs.google.com/document/d/1CLSWm1_9JL1oUqgyNNwtPXW6FzXJ7ddVnSAUQTyqC8I/edit?usp=drive_link)

---

### Step 2) Mock Meeting: Policy Buy-In (Stakeholders)

In this phase, a meeting with the server team introduces the draft Vulnerability Management Policy and assesses their capability to meet remediation timelines. Feedback leads to adjustments, like extending the critical remediation window from 48 hours to one week, ensuring collaborative implementation.

<a href='https://youtu.be/8g6uafc6LjE' target="_"><img width="600" alt="image" src="https://github.com/user-attachments/assets/549d21f4-26c2-412d-9117-d7b6835aedbf"></a>

[YouTube Video: Stakeholder Policy Buy-In Meeting](https://youtu.be/8g6uafc6LjE)

---

### Step 3) Policy Finalization and Senior Leadership Sign-Off

After gathering feedback from the server team, the policy is revised, addressing aggressive remediation timelines. With final approval from upper management, the policy now guides the program, ensuring compliance and reference for pushback resolution.  
[Finalized Policy](https://docs.google.com/document/d/1rvueLX_71pOR8ldN9zVW9r_zLzDQxVsnSUtNar8ftdg/edit?usp=drive_link)
<div style="text-align: center;">
    <img src="https://github.com/user-attachments/assets/9afcdbc1-0493-4af2-9287-1cb9b8f59b40" alt="image" width="400">
</div>

---

### Step 4) Mock Meeting: Initial Scan Permission (Server Team)

The team collaborates with the server team to initiate scheduled credential scans. A compromise is reached to scan a single server first, monitoring resource impact, and using just-in-time Active Directory credentials for secure, controlled access.  

<a href='https://youtu.be/lg068WA4SKM' target="_"><img width="600" alt="image" src="https://github.com/user-attachments/assets/31fe8d0f-636b-475b-8d5a-a2795c183f86"></a>

[YouTube Video: Initial Discovery Scan](https://youtu.be/lg068WA4SKM)

---

### Step 5) Initial Scan of Server Team Assets

In this phase, an insecure Windows Server is provisioned to simulate the server team's environment. After creating vulnerabilities, an authenticated scan is performed, and the results are exported for future remediation steps.  

<img width="635" alt="image" src="https://github.com/user-attachments/assets/937cccbd-36bb-4445-97b9-e915085cda81" style="border: 2px solid black;">

[Scan 1 - Initial Scan](https://drive.google.com/file/d/1RBPVj_azKJMwmRZ8QILlb4hxIjQU3wQ7/view?usp=drive_link)




---

### Step 6) Vulnerability Assessment and Prioritization

We assessed vulnerabilities and established a remediation prioritization strategy based on ease of remediation and impact. The following priorities were set:

1. Third Party Software Removal (Wireshark)
2. Windows OS Secure Configuration (Protocols & Ciphers)
3. Windows OS Secure Configuration (Guest Account Group Membership)
4. Windows OS Updates

---

### Step 7) Distributing Remediations to Remediation Teams

The server team received remediation scripts and scan reports to address key vulnerabilities. This streamlined their efforts and prepared them for a follow-up review.  

<img width="635" alt="image" src="https://github.com/user-attachments/assets/bbf9478f-e1d1-4898-846e-b510ec8c6f72">

[Remediation Email](https://github.com/joshmadakor1/lognpacific-public/blob/main/misc/remediation-email.md)

---

### Step 8) Mock Meeting: Post-Initial Discovery Scan (Server Team)

The server team reviewed vulnerability scan results, identifying outdated software, insecure accounts, and deprecated protocols. The remediation packages were prepared for submission to the Change Control Board (CAB). 

<a href="https://youtu.be/0tjjFewxSNw" target="_"><img width="600" src="https://github.com/user-attachments/assets/03027c66-5f7c-42d0-b6dd-09d053c040b1"/></a>

[Meeting Video](https://youtu.be/0tjjFewxSNw)

---

### Step 9) Mock CAB Meeting: Implementing Remediations

The Change Control Board (CAB) reviewed and approved the plan to remove insecure protocols and cipher suites. The plan included a rollback script and a tiered deployment approach.  

<a href="https://youtu.be/zOFPkTa9kY8" target="_"><img width="600" src="https://github.com/user-attachments/assets/07164e63-fbce-471a-b469-29a6d41b7bb8"/></a>

[Meeting Video](https://youtu.be/zOFPkTa9kY8)

---
### Step 10 ) Remediation Effort

#### Remediation Round 1: Outdated Wireshark Removal

The server team used a PowerShell script to remove outdated Wireshark. A follow-up scan confirmed successful remediation.  
[Wireshark Removal Script](https://github.com/joshmadakor1/lognpacific-public/blob/main/automation/remediation-wireshark-uninstall.ps1)  

<img width="634" alt="image" src="https://github.com/user-attachments/assets/7b4f9ab2-d230-4458-ac0f-c0ff070ae79a">

[Scan 2 - Third Party Software Removal](https://drive.google.com/file/d/1UiwPPTtuSZKk02hiMyXf31pXUIeC5EWt/view?usp=drive_link)


#### Remediation Round 2: Insecure Protocols & Ciphers

The server team used PowerShell scripts to remediate insecure protocols and cipher suites. A follow-up scan verified successful remediation, and the results were saved for reference.  
[PowerShell: Insecure Protocols Remediation](https://github.com/joshmadakor1/lognpacific-public/blob/main/automation/toggle-protocols.ps1)
[PowerShell: Insecure Ciphers Remediation](https://github.com/joshmadakor1/lognpacific-public/blob/main/automation/toggle-cipher-suites.ps1)

<img width="630" alt="image" src="https://github.com/user-attachments/assets/0e96120d-8ec9-4f76-8e42-79c752200010">

[Scan 3 - Ciphersuites and Protocols](https://drive.google.com/file/d/1Qc6-ezQvwReCGUZNtnva0kCZo_-zW-Sm/view?usp=drive_link)


#### Remediation Round 3: Guest Account Group Membership

The server team removed the guest account from the administrator group. A new scan confirmed remediation, and the results were exported for comparison.  
[PowerShell: Guest Account Group Membership Remediation](https://github.com/joshmadakor1/lognpacific-public/blob/main/automation/toggle-guest-local-administrators.ps1)  

<img width="627" alt="image" src="https://github.com/user-attachments/assets/870a3eac-3398-44fe-91c0-96f3c2578df4">

[Scan 4 - Guest Account Group Removal](https://drive.google.com/file/d/1jVgikjfrV1YjOcL3QRT_oUB0Y82w22V7/view?usp=drive_link)


#### Remediation Round 4: Windows OS Updates

Windows updates were re-enabled and applied until the system was fully up to date. A final scan verified the changes  

<img width="627" alt="image" src="https://github.com/user-attachments/assets/870a3eac-3398-44fe-91c0-96f3c2578df4">

[Scan 5 - Post Windows Updates](https://drive.google.com/file/d/1tmDjeHl5uiGitRwWy8kFRi33q-nGi1Zt/view?usp=drive_link)

---

### First Cycle Remediation Effort Summary

The remediation process reduced total vulnerabilities by 80%, from 30 to 6. Critical vulnerabilities were resolved by the second scan (100%), and high vulnerabilities dropped by 90%. Mediums were reduced by 76%. In an actual production environment, asset criticality would further guide future remediation efforts.  

<img width="1920" alt="image" src="https://github.com/user-attachments/assets/51f0aae8-7f36-4d90-b29f-5257e57155f9">

[Remediation Data](https://docs.google.com/spreadsheets/d/1FTtFfZYmFsNLU6pm8nTzsKyKE-d2ftXzX_DPwcnFNfA/edit?gid=0#gid=0)

---

### On-going Vulnerability Management (Maintenance Mode)

After completing the initial remediation cycle, the vulnerability management program transitions into **Maintenance Mode**. This phase ensures that vulnerabilities continue to be managed proactively, keeping systems secure over time. Regular scans, continuous monitoring, and timely remediation are crucial components of this phase. (See [Finalized Policy](https://docs.google.com/document/d/1rvueLX_71pOR8ldN9zVW9r_zLzDQxVsnSUtNar8ftdg/edit?usp=drive_link) for scanning and remediation cadence requirements.)

Key activities in Maintenance Mode include:
- **Scheduled Vulnerability Scans**: Perform regular scans (e.g., weekly or monthly) to detect new vulnerabilities as systems evolve.
- **Patch Management**: Continuously apply security patches and updates, ensuring no critical vulnerabilities remain unpatched.
- **Remediation Follow-ups**: Address newly identified vulnerabilities promptly, prioritizing based on risk and impact.
- **Policy Review and Updates**: Periodically review the Vulnerability Management Policy to ensure it aligns with the latest security best practices and organizational needs.
- **Audit and Compliance**: Conduct internal audits to ensure compliance with the vulnerability management policy and external regulations.
- **Ongoing Communication with Stakeholders**: Maintain open communication with teams responsible for remediation, ensuring efficient coordination.

By maintaining an active vulnerability management process, organizations can stay ahead of emerging threats and ensure long-term security resilience.
Chat

New Conversation

🤓 Explain a complex thing

Explain Artificial Intelligence so that I can explain it to my six-year-old child.


🧠 Get suggestions and create new ideas

Please give me the best 10 travel ideas around the world


💭 Translate, summarize, fix grammar and more…

Translate "I love you" French


GPT-4o Mini
Hello, how can I help you today?
The theory of natural law is based on which of the following?


a.)
Discovered moral truths


b.)
Human-made laws


c.)
Interpretations of existing laws


d.)
Societal norms
GPT-4o Mini
The theory of natural law is based on:
a.) Discovered moral truths
Natural law theory posits that there are inherent moral principles that can be discovered through reason and that these principles guide human conduct and inform the creation of just laws.
Which of the following laws or agencies protect the public from the consequences of risky accounting practices?


a.)
Title VII


b.)
Federal Trade Commission


c.)
Sarbanes-Oxley Act


d.)
Truth in Lending Act
GPT-4o Mini
The law that protects the public from the consequences of risky accounting practices is:
c.) Sarbanes-Oxley Act
The Sarbanes-Oxley Act, enacted in response to financial scandals in the early 2000s, aims to enhance corporate governance and accountability, improve the accuracy of financial reporting, and protect investors from fraudulent accounting practices.
Which of the following is true of criminal law?


a.)
Possible remedies include jail time.


b.)
A preponderance of evidence is necessary for conviction.


c.)
Cases typically occur between private parties.


d.)
Its purpose is to settle individual disputes peacefully.
GPT-4o Mini
The correct statement about criminal law is:
a.) Possible remedies include jail time.
In criminal law, the state prosecutes individuals accused of committing crimes, and if convicted, possible remedies can include incarceration, fines, community service, probation, or other penalties. The standard of proof in criminal cases is "beyond a reasonable doubt," not a preponderance of evidence, which is used in civil cases. Criminal law cases involve the state versus the individual, rather than private parties, and the purpose is to maintain public order and deter crime.
Select the true statement about public law in the U.S.


a.)
It is handed down by authorities with no input from the people.


b.)
It is based on social custom, but is not enforceable by the government.


c.)
It applies to everyone within a jurisdiction.


d.)
It does not allow penalties for violators.
GPT-4o Mini
The true statement about public law in the U.S. is:
c.) It applies to everyone within a jurisdiction.
Public law governs the relationships between individuals and the government, as well as the structure and operation of government itself. It includes areas such as constitutional law, administrative law, and criminal law, and it applies universally to individuals within a certain jurisdiction. The other statements are not accurate reflections of public law.
Statutory law is created by __________.


A.)
the judicial branch


B.)
the legislative branch


C.)
the executive branch


D.)
all three branches of government
GPT-4o Mini
Statutory law is created by:
B.) the legislative branch
Statutory laws are laws enacted by legislatures, both at the federal and state levels. These laws are established through the legislative process, which includes proposal, debate, and voting by elected representatives.
Which of the following is a consideration when choosing a form of business organization?


A.)
The degree of complexity in the business's supply chain


B.)
The number of market competitors


C.)
The size of the company's customer base


D.)
The degree of personal liability a business owner wishes to be exposed to
GPT-4o Mini
The correct consideration when choosing a form of business organization is:
D.) The degree of personal liability a business owner wishes to be exposed to.
When selecting a business structure, factors like personal liability, taxation, management structure, and regulatory requirements are critical. The degree of personal liability can vary significantly among different business forms, such as sole proprietorships, partnerships, and corporations.
Which of the following describes a general partnership?


A.)
An agreement between two or more persons to operate a business and share profits and losses


B.)
An agreement between two or more persons to operate a business, but in which one partner's losses are limited to what he or she initially invested


C.)
A business with a single owner who is fully liable for all debts


D.)
An agreement between two separate businesses to form a new business with a single owner
GPT-4o Mini
The correct description of a general partnership is:
A.) An agreement between two or more persons to operate a business and share profits and losses.
In a general partnership, all partners share responsibility for managing the business and are jointly liable for its debts and obligations.
In which scenario do the different court systems in the U.S. interact properly?


A New Jersey resident is sued by an Iowa resident. After a trial in which the New Jersey resident vigorously defends himself, the Iowa state court finds in favor of the defendant. The Iowa resident then files the same claim in a New Jersey state court, which dismisses the case.


A Colorado man is a defendant in a personal injury lawsuit for an incident that occurred in New Mexico when he was under the influence of marijuana. When hearing the case, the New Mexico judge applies the laws of Colorado, where marijuana is legal, rather than New Mexico law, which criminalizes it.


A convict on death row in Texas sues, claiming that the death penalty violates the prohibition in the Constitution of cruel and unusual punishment. The federal courts refuse to hear the case, because the complaint includes questions of Texas state law.


A West Virginia woman was driving across the country on vacation and caused a traffic accident in Nebraska that resulted in a personal injury tort claim. The case is tried in Nebraska, but the state court judge applies West Virginia law, since that's where the defendant is from.

GPT-4o Mini
The scenario that describes proper interaction between different court systems in the U.S. is:
A convict on death row in Texas sues, claiming that the death penalty violates the prohibition in the Constitution of cruel and unusual punishment. The federal courts refuse to hear the case, because the complaint includes questions of Texas state law.
In this scenario, the federal courts have the discretion to decline to hear cases that primarily involve state law issues, even if there are federal constitutional claims involved. This reflects the federal system of government, where state and federal courts often operate on different issues and legal principles. The other scenarios involve misunderstandings or incorrect applications of law that would not typically occur in appropriate legal practice.
Since corporations are separate legal entities from their shareholders, which of the following is true?


Shareholders are usually not financially accountable for the actions of the corporation, but neither do they own the assets of the corporation.


Shareholders do not need to pay taxes on dividend earnings since corporations are taxed independently.


Under no circumstances can the protection of limited liability be removed from shareholders.


A corporation can only exist for as long as its original owners are present.
GPT-4o Mini
The correct statement is:
Shareholders are usually not financially accountable for the actions of the corporation, but neither do they own the assets of the corporation.
This statement accurately reflects the principle of limited liability, which means that shareholders typically are not personally liable for the corporation's debts and obligations. However, shareholders do not own the corporation's assets directly; rather, the corporation is a separate legal entity that owns its assets. 
The other statements are not accurate:

Shareholders do need to pay taxes on dividend earnings, as dividends are considered personal income.

Protection of limited liability can be removed under certain circumstances, such as in cases of fraud, misconduct, or when courts "pierce the corporate veil."

A corporation can exist independently of its original owners; it continues to exist regardless of changes in ownership or the death of its shareholders.


a b c or d
GPT-4o Mini
Based on your query, the correct answer is:
A: Shareholders are usually not financially accountable for the actions of the corporation, but neither do they own the assets of the corporation.
Feel free to ask if you need clarification or have more questions!
Why do LLCs often have problems borrowing funds for business growth?


Because LLC stock is not transferable. 


Because the members of the LLC are not personally liable for the debts and loans received by the LLC


Because an LLC can only issue stock certificates to members of the company


Because the partners and directors of the LLC do not share responsibility for the debts of the LLC
GPT-4o Mini
LLCs often have problems borrowing funds for business growth primarily for the following reason:
Because the members of the LLC are not personally liable for the debts and loans received by the LLC.
This limited liability protection can make lenders hesitant to extend credit, as they may perceive a higher risk when they can't hold individual members personally accountable for the LLC's debts. 
Let me know if you need further explanation or assistance!
If a breach of contract case is filed in federal court, the court __________.


has subject matter jurisdiction if the claim is for more than $75,000 and no plaintiff lives in the same state as any defendant


has subject matter jurisdiction if the claim is for less than $75,000 and no plaintiff lives in the same state as any defendant


has no subject matter jurisdiction and cannot hear the case


has no subject matter jurisdiction, but can hear the case at its own discretion
GPT-4o Mini
If a breach of contract case is filed in federal court, the court has subject matter jurisdiction if the claim is for more than $75,000 and no plaintiff lives in the same state as any defendant.
This statement describes the requirements for diversity jurisdiction in federal court, which requires that there is diversity of citizenship between the parties (meaning the plaintiffs and defendants are from different states) and that the amount in controversy exceeds $75,000.
Which level of state court would most likely decide a case related to running a red traffic light?


Limited jurisdiction court


General jurisdiction court


Intermediate appellate court


Supreme court
GPT-4o Mini
A case related to running a red traffic light would most likely be decided in a limited jurisdiction court. 
These courts typically handle specific types of cases, such as traffic violations, small claims, and misdemeanors. In many states, traffic violations fall under this category, making limited jurisdiction courts the appropriate venue for such matters.
A 33-year-old business owner is put on trial for negligence.

When in his trial process does voir dire occur?


After the closing arguments


At the beginning, as part of jury selection


After a witness has given testimony, as part of the cross-examination


In the appeals stage
GPT-4o Mini
Voir dire occurs at the beginning, as part of jury selection. This is the process where potential jurors are questioned by the attorneys and the judge to determine their suitability to serve on the jury for a particular case.
Select the true statement about administrative law.


Administrative law can be vetoed by the President, which represents a "check" on the legislative branch.


Administrative regulations created by the agencies can never be changed.


It is produced by private individuals working at the request of the government to manage a social or business activity.


The authority for administrative law at the federal level comes from Congress.
GPT-4o Mini
The true statement about administrative law is:
The authority for administrative law at the federal level comes from Congress.
Congress grants agencies the authority to create regulations, thereby enabling them to implement and enforce specific laws.
only say a b c or d for all 
GPT-4o Mini
d
Select the example where the court has established personal jurisdiction over the defendant.


Frank, an accountant, is suing a client for unpaid bills. The client is located in Mississippi, and Frank lives and works in Virginia. Frank initiates his lawsuit in his home state, because he knows many of the state judges.


Drew is being sued by a man who claims that Drew committed slander by speaking ill of him. Drew lives in Oregon, but the man resides in Texas. Drew has received a summons ordering him to appear in court in Texas to respond to the complaint.


Aisha, a resident of New York, is visited by a process officer at her workplace in New York City and delivered a summons to appear in court in Maryland. The lawsuit against her relates to property damage that occurred in a home she rented in New Jersey, which is owned by a woman from Maryland.


Miguel is being sued by an acquaintance over unpaid debts. Both Miguel and the plaintiff are residents of Colorado. Miguel has not been personally visited by a process server with a summons to appear in court, but he did receive one by certified mail at his home.
GPT-4o Mini
b
ABC Corporation is one of the largest energy companies in the United States, with over $50 million in publicly traded shares. The corporation's unusual accounting practices have disguised the fact that the company has accumulated significant losses over the past five years, making it appear far more profitable than it is. The CEO of ABC Corporation has decided to continue misleading investors by hiding its mounting debt in order to support the company's current market valuation.

How would Deontology analyze this decision?


ABC Corporation is acting unethically because it is intentionally losing money. 


ABC Corporation is acting unethically because it owes a duty to the shareholders, not to its business executives.  


ABC Corporation is acting unethically because the results of its dishonesty are likely to be negative for its employees, for its shareholders, and for society as a whole.


ABC Corporation is acting unethically because it owes a duty to the public as a whole, even if this means losing money. 
GPT-4o Mini
Deontology, a moral philosophy that emphasizes duties and rules, would analyze the decision of ABC Corporation's CEO primarily in terms of the obligations the corporation has to various stakeholders, such as shareholders, employees, and the public. Based on this framework, the most appropriate analysis would be:
ABC Corporation is acting unethically because it owes a duty to the public as a whole, even if this means losing money.
This option aligns with deontological principles, as it emphasizes the duty to act in a way that is honest and transparent, respecting the rights and well-being of the public and stakeholders, rather than focusing solely on the consequences of profit or loss. Deontology holds that certain actions can be considered right or wrong based on adherence to rules or duties, regardless of their outcomes. In this case, deceiving investors breaches the ethical duty of honesty that the corporation owes to the public.
a b c d
GPT-4o Mini
It seems like you are looking for options to choose from based on the earlier response. Here are the options again for clarity:
a) ABC Corporation is acting unethically because it is intentionally losing money.
b) ABC Corporation is acting unethically because it owes a duty to the shareholders, not to its business executives.
c) ABC Corporation is acting unethically because the results of its dishonesty are likely to be negative for its employees, for its shareholders, and for society as a whole.
d) ABC Corporation is acting unethically because it owes a duty to the public as a whole, even if this means losing money.
If you can clarify what you would like to do with these options (e.g., select one, provide reasoning, etc.), I would be happy to assist you further!
Which of the following accurately characterizes the function of the U.S. Supreme Court?


In some years, the Court does not hear any cases whatsoever.


The Court only hears cases sent to it by the District Courts.


The Court selects only a small number of cases to hear on an annual basis.


The Court is required to hear all of the cases that are sent to it by the U.S. Circuit Courts.
GPT-4o Mini
The statement that accurately characterizes the function of the U.S. Supreme Court is:
The Court selects only a small number of cases to hear on an annual basis.
The Supreme Court receives thousands of petitions for cases each year but only hears a small fraction of those, typically around 70-100 cases. The Court is not required to hear any specific case and has discretion over which cases it will take.
The CEO of a multinational retail corporation has decided to raise the minimum wage for its U.S. employees to three times the current federal minimum wage. The CEO explains that the company needs to provide its employees a living wage, regardless of what the law requires.

According to Milton Friedman, did the corporation fulfill its duty?


Yes, because employees will now be able to afford to purchase more of the company's products.


No, because the increase would not be good for the economy. 


No, because the wage hike will drastically increase the corporation's liabilities and likely harm its stock price.


Yes, because the corporation is going beyond what the government requires it to do, in order to advance the public good.
GPT-4o Mini
According to Milton Friedman, the answer would be:
No, because the wage hike will drastically increase the corporation's liabilities and likely harm its stock price.
Friedman argued that the primary responsibility of a corporation is to maximize shareholder value. While he recognized the importance of providing fair wages, he was generally skeptical of actions that would significantly increase costs without corresponding benefits to shareholders. He believed that such actions could ultimately be detrimental to the corporation’s financial health.
Which of the following laws or agencies protects the public from various forms of investment fraud?


Federal Trade Commission


Truth in Lending Act


Civil Rights Act


Securities and Exchange Commission
GPT-4o Mini
The correct answer is Securities and Exchange Commission (SEC). 
The SEC is responsible for protecting investors, maintaining fair and efficient markets, and facilitating capital formation. It oversees the securities industry and enforces laws against market manipulation and investment fraud.
The new CEO of a large coffee corporation makes fighting sexual harassment a cornerstone of the company's culture after a series of embarrassing incidents involving several of the company's managers are leaked to the media. The corporation drafts a new code of ethics with an expanded set of policies related to sexual harassment, creates a series of mandatory workshops for its workforce, and fires the managers involved in the incidents.

Consider what you have learned about the factors that impact corporate culture. What is the ethical strength of the corporation in the example?


Strong, because the corporation must show that it has an ongoing process to discourage wrongdoing in order to avoid legal action.


Weak, because this focus on matters of social justice has no place in capitalism.


Weak, because the CEO should have cracked down on the employees who were leaking information to the media as well.


Strong, because the CEO is setting expectations for ethical behavior and holding violators accountable.
GPT-4o Mini
The ethical strength of the corporation in the example is strong, because the CEO is setting expectations for ethical behavior and holding violators accountable.
By implementing a new code of ethics, organizing mandatory workshops, and taking disciplinary action against the managers involved, the CEO is actively fostering a culture of integrity and accountability. This approach demonstrates a commitment to addressing and preventing sexual harassment, which is essential for promoting a healthy workplace environment.
Select the true statement about the relationship between law, ethics, and business.


Abiding by the law is sufficient for businesses to earn a moral reputation.


It is impossible for a business to behave unethically if it follows the law.


What is ethical in business is not necessarily required by law.


The law ensures ethical conduct in most areas of business.
GPT-4o Mini
The true statement about the relationship between law, ethics, and business is:
What is ethical in business is not necessarily required by law.
This statement recognizes that while laws establish minimum standards for behavior, ethical considerations can go beyond legal requirements. Businesses may choose to adhere to ethical principles that exceed what is mandated by law, demonstrating a commitment to moral standards and social responsibility.
Which of the following is an example of a sole proprietorship?


Matt and Carlene are both owners of a business that sells hand-crafted home goods via the Internet. Although they both own the business, Matt is solely responsible for the business operations.


Gabrielle started a dog-walking company. She sometimes worries about the fact that she has no one to share the potential liabilities of the company with, but she does enjoy retaining 100% of the profits.


Issa and Raymond start a t-shirt printing company that earns a small profit in its first year of operation. They both invested capital in the business to get it up and running, so they are both glad to share in the small profit.


Shawn is a partner in a successful downtown law firm. He has a number of clients that he is exclusively responsible for, so he works very hard to make sure they're happy with his services.

Save & Continue
Report an issue with this question
Here are all the tutorials from Unit 1. Use them as needed throughout the Unit 1 Milestone.
Unit 1 Tutorials
1.1 Foundations of Law
1.1.1 What Is Law? 
1.1.2 Law in Business 
1.1.3 U.S. Positive Law 
1.1.4 Origins of Law 
1.1.5 U.S. Constitution as a Source of Law 
1.1.6 Legislation and Other Sources of Law 
1.2 Business Entities
1.2.1 Business Organizations 
GPT-4o Mini
The example of a sole proprietorship is:
Gabrielle started a dog-walking company. She sometimes worries about the fact that she has no one to share the potential liabilities of the company with, but she does enjoy retaining 100% of the profits.
A sole proprietorship is a business owned and operated by a single individual who retains all profits and is personally liable for all debts and obligations of the business. In this scenario, Gabrielle is the only owner of her dog-walking company, which is characteristic of a sole proprietorship.
Arbitration is a __________ form of alternative dispute resolution.


voluntary, never binding 


involuntary, always binding 


voluntary, often binding 


voluntary, always non-binding 
GPT-4o Mini
Arbitration is a voluntary, often binding form of alternative dispute resolution. 
In arbitration, parties typically agree to submit their disputes to an arbitrator or a panel of arbitrators, and the decision made by the arbitrator is usually binding on the parties, depending on the terms of their agreement. This distinguishes arbitration from other forms of dispute resolution like mediation, which is generally non-binding.
A driver is texting and runs into a pedestrian crossing the road at a crosswalk. The pedestrian suffers a broken leg and is rushed to the hospital.

Is the driver liable for negligence if the pedestrian sues?


Yes, because the driver broke the law by texting while driving.


Yes, because the driver had a duty of care which was breached by texting while driving, and the pedestrian had legally recognizable injuries directly resulting from that breach.


No, because even though the driver was texting while driving, the pedestrian had a duty to look out for possible dangers before entering the crosswalk.


No, because it would be difficult to prove that the driver's texting was the proximate cause of the pedestrian's broken leg.
GPT-4o Mini
The correct answer is:
Yes, because the driver had a duty of care which was breached by texting while driving, and the pedestrian had legally recognizable injuries directly resulting from that breach.
In this scenario, the driver has a legal duty to operate the vehicle with reasonable care, which includes maintaining attention on the road and avoiding distractions like texting. By texting while driving, the driver breached this duty, and the pedestrian's injuries (a broken leg) are a direct result of that breach. This establishes a potential case for negligence, making the driver liable if the pedestrian sues.
GPT-4o Mini
coin image
0
Upgrade




Ask me anything...



Make a Review & Earn Credit ❤
Chat
Ask
Search
Write
Image
ChatFile
Vision
Full Page
Invite & Earn
