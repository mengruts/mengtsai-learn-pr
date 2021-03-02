# Title

Improve Azure Netapp Files Performance of your EDA/HPC Applications by using best practice.

## Role(s)

administrator, functional-consultant, solution-architect, student, technology-manager

## Level

200

## Product(s)

Azure NetApp Files

## Prerequisites

- Learner should unserstand the concepts of storage hierarchy of Azure NetApp Files, including NetApp accounts, Capacity Pool and Volumes. 
- Ability to set up Azure NetApp Files and create a Volume.
- Ability to mount the Azure NetApp Files Volume from a Virtual Machine.

## Summary

You will learn how to improve Azure Netapp Files Performance of your EDA/HPC Applications by using best practice.

## Learning objectives

By the end of this module, the learner should be able to:
1. List the best practices which would be able to improve Azure Netapp Files performance.
2. Describe the performance impact of the best practices on FIO and EDA Benchmarking suite. 

## Chunk your content into subtasks

Identify the subtasks of *module title*

| Subtask | What part of the introduction scenario does this subtask satisfy? | How will you assess it: **Exercise or Knowledge check**? | Which learning objective(s) does this help meet? | Does the subtask have enough learning content to justify an entire unit? If not, which other subtask will you combine it with? |
| ---- | ---- | ---- | ---- | ---- |
| Overall suggestions | Provide architecture and overall performance suggestion of running EDA/HPC applications using Azure NetApp Files as storage solution | Kownledge Check | 1 | yes |
| List Performance tips | Discuss performance impact of actimeo & nocto, sysctl, nconnect, NFS version, rsize/wsize | Kownledge Check | 1 | yes |
| Describe Benchmarking results | Verify performance results using FIO and SPEC EDA Benchmarking suite| Knowledge Check | 2 | yes |

## Outline the units

1. **Introduction**

    Suppose you are a member of a manufacturer or semiconductor company, tasked with designing their new products or IC Chips which needs a lot of CAE (Computer Aided Engineering) or EDA (Electronic Design Automation) simulation. You do not have sufficient capacity on premises for this project and so will be using Azure for those HPC simulation needs. Management would like this project to be completed in a timely and cost-effective manner. You choose Azure NetApp Files (ANF) as the back-end storage solution as it provides an on-premises-like experience and performance. You will need list performance pracices of running your HPC applications in Azure.

5. **Performance tips: actimeo & nocto, sysctl, nconnect, NFS version, rsize/wsize, etc.**
    - Learn what these 2 mount options are, and performance impact of EDA simulation
        - Explanation of actimeo and nocto, and suitable scenarios to apply
        - A figure to show perfomance impact when applying on EDA workloads
        - Provide a reference for furthur study
    - Learn sysctl practice to improve performance
        - sysctl example for Azure Dv4/Ev4.
        - Provide a reference for furthur study
    - Learn how "nconnect" mount options's performance impact of EDA simulation.
        - Learn why "nconnect" could improve performance, and it's dependencies and limitation.
        - Example on applying "ncoonect" on Centos/Redhat.
    - rsize/wsize and Others
8. **Benchmarking results**
    - Summarize options which could significanttly or have minor/no impact of an EDA applications 
        - A table to show FIO test resutls on above 3 options, to show it's a generic and fundametal options to improve IOPS and throughput. 
        - A figure to show EDA benchamrking test results on above 3 options.
        - 3 figures to show performance impact of NFS 3/4.1, TCP/UDP and # of MTU.

    **Knowledge check**


**Learn practical performance tuning tips.**

(Multiple choice question)

1. Check the option(s) which can improve overall performance when running EDA applications on ANF:

- Use 'nconnect' mount options.

- Use NFS 4.1 instead of NFS 3.0

- Use 'actimeo and nocto' mount options.

- Fine-tune sysctl.

**Summary**
You learn some generic generic performance tips when running your HPC applications in Azure.

## Notes

Azure NetApp Files Product page:
https://azure.microsoft.com/en-us/services/netapp/ 

Azure NetApp Files documentation, how-to guides, and pricing:
https://docs.microsoft.com/en-us/azure/azure-netapp-files/
