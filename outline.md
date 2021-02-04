# Title

Using Azure NetApp Files and Performance tips for HPC Applications.

## Role(s)

branch=master#role)
administrator, functional-consultant, solution-architect, student, technology-manager

## Level

100

## Product(s)

Azure NetApp Files

## Prerequisites

Ability to deploy Virtual Machine in Azure

## Summary

*Add the summary [(Summary guidance)](https://review.docs.microsoft.com/en-us/learn-docs/docs/id-guidance-introductory-summaries)*

## Learning objectives

*Add numbered Learning Objectives [(Learning objective guidance)](https://review.docs.microsoft.com/en-us/learn-docs/docs/id-guidance-learning-objectives)*
1. Learn how to choose proper service lebel and volume quota when running your HPC applications on Azure NetApp Files.

2. Learn how to create and configure ANF, and mount an ANF volume.

3. Learn practical performance tuning tips.

## Chunk your content into subtasks

Identify the subtasks of *module title*

| Subtask | What part of the introduction scenario does this subtask satisfy? | How will you assess it: **Exercise or Knowledge check**? | Which learning objective(s) does this help meet? | Does the subtask have enough learning content to justify an entire unit? If not, which other subtask will you combine it with? |
| ---- | ---- | ---- | ---- | ---- |
| TODO | TODO | TODO | TODO | TODO |
| TODO | TODO | TODO | TODO | TODO |
| TODO | TODO | TODO | TODO | TODO |

## Outline the units

*Add more units as needed for your content*

1. **Introduction**

    Suppose you are a member of a manufacturer or semiconductor company, tasked with designing their new products or IC Chips which needs a lot of CAE (Computer Aided Engineering) or EDA (Electronic Design Automation) simulation. You do not have sufficient capacity on premises for this project and so will be using Azure for those HPC simulation needs. Management would like this project to be completed in a timely and cost-effective manner. You choose Azure NetApp Files (ANF) as the back-end storage solution as it provides an on-premises-like experience and performance. You will need to figure out what is the ANF hierarchy and performance considerrating while architecting with your HPC Applications, and learn some generic performance tips running your HPC applications in Azure.

1. **Learning-content unit title**

    List the content that will enable the learner to *subtask*:

    - Understand ANF's storage hierarchy.
        - Information needed to accomplish the enabling objective
        - Information needed to accomplish the enabling objective
    - Understand ANF performance regarding to service level and volume quota.
        - Information needed to accomplish the enabling objective
        - Information needed to accomplish the enabling objective
    - [Hands-on] Create an ANF Volume
        - Information needed to accomplish the enabling objective
        - Information needed to accomplish the enabling objective
    - Examining ANF's Scalability
        - Information needed to accomplish the enabling objective
        - Information needed to accomplish the enabling objective
    - Performance tips (actimeo and nocto)
        - Information needed to accomplish the enabling objective
        - Information needed to accomplish the enabling objective
    - Performance tips (sysctl)
        - Information needed to accomplish the enabling objective
        - Information needed to accomplish the enabling objective
    - Performance tips (nconnect)
        - Information needed to accomplish the enabling objective
        - Information needed to accomplish the enabling objective
    - Performance tips (conclusion)
        - Information needed to accomplish the enabling objective
        - Information needed to accomplish the enabling objective


    **Knowledge check**

    What types of questions will test *learning objective*? *[(Knowledge check guidance)](https://review.docs.microsoft.com/en-us/learn-docs/docs/id-guidance-knowledge-check)*


**Learn how to choose proper service lebel and volume quota when running your HPC applications on Azure NetApp Files.**

(Single choice question)
1.  What's the top-down order of Azure NetApp Files storage hierarchy:

- ANF Account -> ANF Container -> Volume

- Capacity Pool -> ANF Account -> Volume

- ANF Account -> Capacity Pool -> Volume

- ANF Account -> Capacity Pool -> Storage Target

(Single choice question)
2. A specfic HPC application need at least 50TiB size of file storage, and need to ensure 3,000MiB/sec in throughput. With below knowledge, which of the following ANF Service Level and volume quota sould be configured?

- Ultra + 25TiB

- Premium + 50TiB

- Standard + 100Tib

(Single choice question)
3. When resizing your ANF Volume quota to reflect different HPC applications performance requirements, what actions need to be done to make the change effective?

- umount and mount the Volumes.

- Reboot all VMs connecting to Volumes.

- None of above, ANF will just affect performance change almost immediately.

**Learn practical performance tuning tips.**
(Multiple choice question)
4. Check the option(s) which can improve overall performance when running EDA applications on ANF:

- Use 'nconnect' mount options.

- Use NFS 4.1 instead of NFS 3.0

- Use 'actimeo and nocto' mount options.

- Fine-tune value of rsize and wsize.

- Fine-tune sysctl.

1. **Summary**

After the knowledge learned in the moduel, you have understood the ANF storage hierarchy and how to mount Volumes from VMs. You know how to design ANF service level and volume quota to fullfill your HPC Applications performance requirements in a cost-effective way. You also learn some generic generic performance tips when running your HPC applications in Azure.

## Notes

Azure NetApp Files Product page:
https://azure.microsoft.com/en-us/services/netapp/ 

Azure NetApp Files documentation, how-to guides, and pricing:
https://docs.microsoft.com/en-us/azure/azure-netapp-files/
