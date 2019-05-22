# cloudreach-azure-compliance-blueprint
Blueprint for deploying a compliance-ready Azure solution

### NOTE TO CLOUDREACHERS

The document will be built following the table of contents' listing. This is a work in progress.....Code will follow and suggestions are welcome for areas missed, regulatory regimens overlooked and any other relevant items that may occur to you.


### Contents


* Introduction
* Common Regulations
* Regulatory and Compliance Workflow
* Building a Compliance-sensitive Azure solution
  - Identify the business process
  - Identify the client’s compliance and regulatory exposures
  - Understand the on-premises technology service layer from a compliance POV
  - Designing the Azure Solution for compliance
* Microsoft PCI/DSS Example
* Azure Compliance Technologies
* Azure Management Groups
* Azure Policies
* Azure Monitor
* Azure Secure DevOps
* Compliance Solution High Level Design



### Introduction

All organizations have security and access control requirements and all solutions should employ security best practices.

Specific firms however, such as finance and banking or any organization which performs credit card transactions, have particular needs beyond baseline security driven by regulatory and compliance requirements.  For example, if customers purchase shoes via a company website, the information generated is subject to the PCI (and perhaps PII) regulatory regimen.

The material in this blueprint is offered to help you build a solution using Azure platform technologies designed to address compliance and regulatory challenges.

### Common Regulations

These are the regulations you’re most likely to encounter during a client engagement. It’s important to understand, if only at a high-level, what the regulations cover to better inform architectural decisions.

![Common Regulations](https://mlabshare.blob.core.windows.net/malbshare/Regulations_Listing.png)

### More Information

[Sarbanes Oxley](https://bit.ly/1Jhbio3)
[PCI/DSS](https://bit.ly/1ONAycB)
[PII](https://bit.ly/2WeREd7)
[GDPR](https://bit.ly/1lmrNJz)
[Calif. Consumer Privacy Act](https://bit.ly/2wedkY1)


### Regulatory and Compliance Workflow

Within most organizations, the compliance workflow is performed using some variation of this process. The key elements of compliance are:

- Data gathering
- Remediation
- Demonstration (of controls)
- Attestation (i.e., reporting to auditors)

![Compliance Workflow Overview](https://mlabshare.blob.core.windows.net/malbshare/Compliance-High-Level-Overview.png)


### Building a Compliance-sensitive Azure solution


### One.)Identify the business process

Compliance exposures flow from business process - i.e., from the business workflow and the types of data that moves through a business. In the example, credit card data, including personally identifiable information (PII), is stored and acted upon by company personal.  This makes the business information systems subject to PII regulations.

The first step in designing an architecture for this client was detailing the busines process from a technology point of view.  This is accomplished via interviews with both business and technology stakeholders (e.g., not IT alone).


![Credit Card Processor Example](https://mlabshare.blob.core.windows.net/malbshare/Credit-Card-Processor-Data-Workflow.png)


### Two.) Identify the client’s compliance and regulatory exposures

Following on from the information gathered during the business process review phase is the creation of a compliance exposure map. In this context, "compliance exposure" refers to the regulatory and compliance regimens the client is subject to based on the type of data gathered and manipulated. Returning to the credit card processing example, we can map specific regulations to platforms used.  This will inform architectural choices for the cloud landing zone.

![Compliance Mapping](https://mlabshare.blob.core.windows.net/malbshare/Compliance-Exposures-Mapping-Example.png)


### Three.) Understand the on-premises technology service layer from a compliance POV

All Gaul is divided into three parts, one of which the Belgae inhabit, the Aquitani another, those who in their own language are called Celts, in our Gauls, the third. All these differ from each other in language, customs and laws. The river Garonne separates the Gauls from the Aquitani; the Marne and the Seine separate them from the Belgae. Of all these, the Belgae are the bravest...


### Four.) Designing the Azure Solution for compliance

All Gaul is divided into three parts, one of which the Belgae inhabit, the Aquitani another, those who in their own language are called Celts, in our Gauls, the third. All these differ from each other in language, customs and laws. The river Garonne separates the Gauls from the Aquitani; the Marne and the Seine separate them from the Belgae. Of all these, the Belgae are the bravest...
