# Title

Choose the suitable Service Level of Azure NetApp Files for your HPC applications.

## Role(s)

administrator, functional-consultant, solution-architect, student, technology-manager

## Level

100

## Product(s)

Azure NetApp Files

## Prerequisites

Concepts of Storage hierarchy of Azure NetApp Files
Ability to Set up Azure NetApp Files and create an NFS volume.

## Summary

Choose suitable Service Level of Azure NetApp Files based on your throughput requirements including cost considerations.

## Learning objectives

1. Understand Service Level and Throughput Limits of Azure NetApp Files

2. Cost-effective Analysis to choose suitable Service Level  

## Chunk your content into subtasks

Identify the subtasks of *module title*

| Subtask | What part of the introduction scenario does this subtask satisfy? | How will you assess it: **Exercise or Knowledge check**? | Which learning objective(s) does this help meet? | Does the subtask have enough learning content to justify an entire unit? If not, which other subtask will you combine it with? |
| ---- | ---- | ---- | ---- | ---- |
| Service Level intro | Map throghput requirements to ANF's Service Level | Knowledge Check | 1 | yes |
| Service Level Cost-effective Analysis |  | TODO | TODO | TODO |
| TODO | TODO | TODO | TODO | TODO |

## Outline the units

1. **Introduction**

    Suppose you are a member of a manufacturer or semiconductor company, tasked with designing their new products or IC Chips which needs a lot of CAE (Computer Aided Engineering) or EDA (Electronic Design Automation) simulation. You do not have sufficient capacity on premises for this project and so will be using Azure for those HPC simulation needs. Management would like this project to be completed in a timely and cost-effective manner. You choose Azure NetApp Files (ANF) as the back-end storage solution as it provides an on-premises-like experience and performance. You will need to figure out what is the ANF hierarchy and performance considerrating while architecting with your HPC Applications, and learn some generic performance tips running your HPC applications in Azure.

1. **Understand ANF's storage hierarchy**
    - Understand relationships among ANF account, service level, and volumn quota.
        - A figure to visualize the relationships.
        - Elaborate the limitation and range of size of service level and volumn quota.
2. **Understand ANF performance regarding to service level and volume quota.**
    - Understand 2 key factors affecting ANF's performance.
        - A fiture to visualize the performace regarding to service level and volume quota
        - An example on how to configure ANF to the expected throughput
        - An example on how to calculate expected throughput from IOPS and IO sizes.
        - Reminder of real-world performance is impacted by multi-factors
3. **[Hands-on] Create an ANF Volume**
    - Real exercise based on the storage hierarchy concept from previous unit
        - A figure to visulize the ANF storage hiearchy as handsd-on practice
        - Refer to Azure Doc for step-by-step tutorial to 1. create the storage hierarchy and 2. mount the Volumne from a VM
        - Examine using "df -h" and explanation "no-reject=write" principle
4. **Examining ANF's Scalability**
    - Take standard EDA workload benchamrking reviewing ANF's real-world scalability 
        - Information regarding the SPEC EDA benchmarking tools, and EDA workloads to be generated
        - A figure to show relationship of the response time and EDA operations/sec, and linear growth when adding # of volumes
        - A table to show achieved operations/sec (throughput) ANF could achieve for user to determine right architecture.
5. **Performance tips (actimeo and nocto)**
    - Learn what these 2 mount options is, and performance impact of EDA simulation
        - Exaplnation of actimeo and nocto, and suitable scenarios to apply
        - A figure to show perfomance impact when applying on EDA workloads
        - Provide a reference for furthur study
6. **Performance tips (sysctl)**
    - Learn sysctl practice to improve performance
        - sysctl example for Azure Dv4/Ev4.
        - Provide a reference for furthur study
7. **Performance tips (nconnect)**
    - Learn how "nconnect" mount options's performance impact of EDA simulation.
        - Learn why "nconnect" could improve performance, and it's dependencies and limitation.
        - Example on applying "ncoonect" on Centos/Redhat.
8. **Performance tips (conclusion)**
    - Summarize options which could significanttly or have minor/no impact of an EDA applications 
        - A table to show FIO test resutls on above 3 options, to show it's a generic and fundametal options to improve IOPS and throughput. 
        - A figure to show EDA benchamrking test results on above 3 options.
        - 3 figures to show performance impact of NFS 3/4.1, TCP/UDP and # of MTU.

    **Knowledge check**

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

3. When resizing ANF Volume quota to reflect different HPC applications performance requirements, what actions need to be done to make the change effective?

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

**Summary**

After the knowledge learned in the moduel, you have understood the ANF storage hierarchy and how to mount Volumes from VMs. You know how to design ANF service level and volume quota to fullfill your HPC Applications performance requirements in a cost-effective way. You also learn some generic generic performance tips when running your HPC applications in Azure.

## Notes

Azure NetApp Files Product page:
https://azure.microsoft.com/en-us/services/netapp/ 

Azure NetApp Files documentation, how-to guides, and pricing:
https://docs.microsoft.com/en-us/azure/azure-netapp-files/
