# Title

Choose the best Service Level of Azure NetApp Files for your HPC applications.

## Role(s)

administrator, functional-consultant, solution-architect, student, technology-manager

## Level

100

## Product(s)

Azure NetApp Files

## Prerequisites

- Learner should unserstand the concepts of storage hierarchy of Azure NetApp Files, including NetApp accounts, Capacity Pool and Volumes. 

## Summary

Choose the best Service Level of Azure NetApp Files based on your throughput requirements including cost considerations.

## Learning objectives

By the end of this module, the learner should be able to choose the best Service Level of Azure NetApp Files for HPC applications.

## Chunk your content into subtasks

Identify the subtasks of *module title*

| Subtask | What part of the introduction scenario does this subtask satisfy? | How will you assess it: **Exercise or Knowledge check**? | Which learning objective(s) does this help meet? | Does the subtask have enough learning content to justify an entire unit? If not, which other subtask will you combine it with? |
| ---- | ---- | ---- | ---- | ---- |
| Service Level intro | Map throghput requirements to ANF's Service Level | Knowledge Check | 1 | yes |
| Cost-effective Analysis | Examples on choosing most cost-effective Service Level based on throughput requirements | Knowledge Check | 1 | yes |

## Outline the units

1. **Introduction**

    Suppose you are a member of a manufacturer or semiconductor company, tasked with designing their new products or IC Chips which needs a lot of CAE (Computer Aided Engineering) or EDA (Electronic Design Automation) simulation. You do not have sufficient capacity on premises for this project and so will be using Azure for those HPC simulation needs. Management would like this project to be completed in a timely and cost-effective manner. You choose Azure NetApp Files (ANF) as the back-end storage solution as it provides an on-premises-like experience and performance. You will need to choose the most suitable Service Level of Azure NetApp Files based on your throughput requirements including cost considerations.

1. **Understand ANF performance regarding to service level and volume quota.**
    - Understand 2 key factors affecting ANF's performance.
        - A figure to visualize the performace regarding to service level and volume quota
        - An example on how to configure ANF to the expected throughput
        - An example on how to calculate expected throughput from IOPS and IO sizes.
        - Reminder of real-world performance is impacted by multi-factors
    **Knowledge check**
    
3. **Cost-effective Analysis to choose suitable Service Level**
    - Examples on choosing most cost-effective Service Level based on throughput requirements
        - Ex1: Have specific throughput requirements
        - Ex2: Have spesific IOPS requirements
        - Online ANF performance calculator
    **Knowledge check**

**Learn how to choose proper service lebel and volume quota when running your HPC applications on Azure NetApp Files.**

(Single choice question)

1.  What's the top-down order of Azure NetApp Files storage hierarchy:

- ANF Account -> ANF Container -> Volume

- Capacity Pool -> ANF Account -> Volume

- ANF Account -> Capacity Pool -> Volume

- ANF Account -> Capacity Pool -> Storage Target

(Single choice question)

2. When resizing ANF Volume quota to reflect different HPC applications performance requirements, what actions need to be done to make the change effective?

- umount and mount the Volumes.

- Reboot all VMs connecting to Volumes.

- None of above, ANF will just affect performance change almost immediately.


**Cost-effective Analysis to choose suitable Service Level**

(Single choice question)

1. A specfic HPC application need at least 50TiB size of file storage, and need to ensure 3,000MiB/sec in throughput. With below knowledge, which of the following ANF Service Level and volume quota sould be configured?

- Ultra + 25TiB

- Premium + 50TiB

- Standard + 100Tib

2. A specfic HPC application need at least 20TiB size of file storage, and need to ensure 120,000 in IOPS with 8KiB 50/50 random read/write. With below knowledge, which of the following ANF Service Level and volume quota sould be configured?

- Ultra + 25TiB

- Premium + 50TiB

- Standard + 100Tib


**Summary**

Choose suitable Service Level of Azure NetApp Files based on your throughput requirements including cost considerations.

## Notes

Azure NetApp Files Product page:
https://azure.microsoft.com/en-us/services/netapp/ 

Azure NetApp Files documentation, how-to guides, and pricing:
https://docs.microsoft.com/en-us/azure/azure-netapp-files/
