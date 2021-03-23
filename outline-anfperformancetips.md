# Title

Improve Azure Netapp Files Performance of your EDA/HPC Applications by using best practices

## Role(s)

administrator, functional-consultant, solution-architect, student, technology-manager

## Level

200

## Product(s)

Azure NetApp Files

## Prerequisites

- Learner should understand the concepts of storage hierarchy of Azure NetApp Files, including NetApp accounts, Capacity Pool and Volumes. 
- Ability to set up Azure NetApp Files and create a Volume.
- Ability to mount the Azure NetApp Files Volume from a Virtual Machine.

## Summary

You will learn how to improve Azure NetApp Files Performance of your EDA/HPC Applications by using best practice.

## Learning objectives
By the end of this module, the learner should be able to:
1. List the best practices which would be able to improve Azure NetApp Files performance.
2. Describe the performance impact of the best practices on FIO and EDA Benchmarking suite. 

## Chunk your content into subtasks

Identify the subtasks of *module title*

| Subtask | What part of the introduction scenario does this subtask satisfy? | How will you assess it: **Exercise or Knowledge check**? | Which learning objective(s) does this help meet? | Does the subtask have enough learning content to justify an entire unit? If not, which other subtask will you combine it with? |
| ---- | ---- | ---- | ---- | ---- |
| Introduction | Introduce scenarios, learning objectives and prerequisites | N/A | 1 | yes |
| Overall performance suggestions | Provide architecture and overall performance suggestion | Kownledge Check | 1 | yes |
| List Performance tips | Discuss performance impact of actimeo & nocto, sysctl, nconnect, NFS version, rsize/wsize | Kownledge Check | 1 | yes |
| Benchmarking results | Verify performance results using FIO and SPEC EDA Benchmarking suite| Knowledge Check | 2 | yes |
| Summary | Summarize list of best practices and applicability| Knowledge Check | 2 | yes |

## Outline the units

1. **Introduction**
    - Introduce scenarios, learning objectives and prerequisites

2. **Overall performance suggestions**
    - Provide architecture and overall performance suggestion
        - Architecture of running EDA Applications on Azure NetApp Files 
        - Overall performance suggestion

2. **Performance tips: actimeo & nocto, sysctl, nconnect, NFS version, rsize/wsize, etc.**
    - actimeo & nocto
    - /etc/sysctl.conf
    - nconnect
    - NFS version
    - rsize/wsize
    - Others
3. **Benchmarking results**
    - Describe benchmarking results of FIO and SPEC EDA tools 
        - FIO 
        - SPEC EDA benchamrking
    **Knowledge check**
4. **Summary**
    - Summarize performance best practice  

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
