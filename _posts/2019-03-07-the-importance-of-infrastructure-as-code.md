---
layout: post
title:  "The Importance of Infrastructure as code"
author: alex
categories: [ IaC, DevOps ]
image: assets/images/iac.png
featured: true
hidden: false
date: 2019-03-07 1:54:00 -0500
---

Infrastructure as code (IaC) is a recent practice that solves inconsistencies between environments. If your application environments aren’t identical, you run into the risk of having production outages. IaC will streamline all of your environment configuration so you don’t have to worry about differences in configuration between your production environments. IaC is a deterministic way of creating infrastructure.

## What is Infrastructure as code 

Infrastructure as Code (IaC) is the management of infrastructure (networks, virtual machines, load balancers, and connection topology) in a descriptive model, using the same versioning as DevOps team uses for source code. Like the principle that the same source code generates the same binary, an IaC model generates the same environment every time it is applied. IaC is a key DevOps practice and is used in conjunction with continuous delivery.[[2]](https://docs.microsoft.com/en-us/azure/devops/learn/what-is-infrastructure-as-code){:target="_blank"}

## What are the benefits of IaC?

There are plenty of reasons why IaC is important and beneficial for your team. Below we will outline a few reasons why.

### Improved Collaboration

IaC will be stored in a centralized version control system where everyone can view and make changes to it. The benefit of this is that you don’t need to worry track how a specific environment was created, it will be stored in the version control system for everyone to see. You can also track who made changes to the environments and why which is something that wasn’t intuitive in the past.

If a team wants to make a change, they can create a change that can then be reviewed by the team. This is important because everyone can be involved in the code review process and it encourages team members to make changes. This also makes sure that more than 1 person on the team is aware of how the environment is configured.

### Increased Efficiency

Once you define all of the resources you want to create, the IaC tool can launch these resources. In the past, teams would manually configure all of their environments or write complex scripts which were time-consuming. IaC will allow you to create libraries that can be used across different projects. This ends up saving the development team time as they grow and need to launch new environments. IaC promotes DevOps practices for your team.

### Improved Governance

IaC makes it easy to involve your security team in the process. They can easily provide ways to secure your environment based on corporate policy and compliance. These requirements can then be added to a library that can be used across all projects. The security team can also be involved in the code review process so they can provide feedback on the configurations from a security perspective.

### Tracked Changes

If someone makes a rogue change to the environment that isn’t tracked in the IaC, then the next time it gets run, the change will be reverted to prevent the environment to be in a state that isn’t consistent from what’s defined in the IaC. IaC tools track how the environment is configured with a state that’s stored in a centralized place. This will prevent inconsistencies between environments.

### Decreased Cost

Since IaC will make your team more productive, they can spend more time working on high-value tasks due to the productivity increase that IaC introduced. You will also be able to track all of the infrastructures that exists in your environment making it easier to audit and delete resources that don’t need to be used. 

## How to get Started

First, you need to decide which IaC tool you want to use. This will be entirely dependent on which cloud provider you’re using and how your infrastructure is configured. My suggestion is that you compare each tool to see which one is a good fit for your use-case.

Once you decide on which tool you want to use, you can then start writing IaC for any new resources you need to launch. Involving your team in this process is highly recommended as it’s important to create enablement around the creation of infrastructure.  

### What do I do with existing infrastructure?

This is something that I hear often from individuals looking to get started with IaC. The good news is that certain IaC tools like Terraform allow you to import pre-existing resources in your cloud environment. Not having to start from scratch is a huge benefit for teams. The only caveat with this approach is that you need to fully understand how your environment is configured for this to work properly. In the future, some tools might provide ways to automatically detect how an environment is configured but you can’t do that today.

## Conclusion

IaC will save your company money, make your team more productive, and will promote collaboration. Your team won’t have to worry about inconsistencies between environments and your team can focus more on development. IaC provides a lot of benefits for your company and it promotes DevOps principles, which is why your team should start implementing this practice today.

## Notes

[1] [https://docs.microsoft.com/en-us/azure/devops/learn/_img/infrastructureascode_600x300-3.png](https://docs.microsoft.com/en-us/azure/devops/learn/_img/infrastructureascode_600x300-3.png){:target="_blank"}

[2] [https://docs.microsoft.com/en-us/azure/devops/learn/what-is-infrastructure-as-code](https://docs.microsoft.com/en-us/azure/devops/learn/what-is-infrastructure-as-code){:target="_blank"}
