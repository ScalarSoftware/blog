---
layout: post
title:  "Should a Startup use a Platform as a service?"
author: alex
categories: [ PaaS, Cloud ]
image: assets/images/paas.jpg
featured: false
hidden: false
---

Startups want to focus on product development after validating their MVP and acquiring new customers. Startups will initially have small development teams and these teams need to be as productive as possible.

I’ve talked to many startup founders and employees and what I’ve noticed one of their main focuses is to release new features as efficiently as possible. When a startup is ready to release a new feature, they don’t want to spend their time on creating or managing infrastructure, they want everything to work correctly. Creating and maintaining infrastructure requires a specific skill set which a startup might not have in their early stages. Outsourcing infrastructure concerns to a cloud provider can seem attractive to a smaller company.

Startups shouldn’t focus on managing infrastructure because it’s not productive for them. This is why a Platform as a service (Paas) is the best option for startups looking to focus on product development, adding value to their customers, and maintaining a good uptime.

## What is PaaS?

Microsoft defines a Platform as a service (PaaS) as a complete development and deployment environment in the cloud, with resources that enable you to deliver everything from simple cloud-based apps to sophisticated, cloud-enabled enterprise applications. You purchase the resources you need from a cloud service provider on a pay-as-you-go basis and access them over a secure Internet connection.[[1]](https://azure.microsoft.com/en-ca/overview/what-is-paas/){:target="_blank"}

## What are the benefits of using a PaaS?

The reason a PaaS is good for startups is that it allows them to focus on product development without having to worry about the underlying infrastructure in production. This allows small development teams to be extremely efficient when releasing new features. Using a PaaS means you don’t have to have an understanding of how infrastructure is set up and operated you can easily deploy your code to production.

Using a PaaS mean you get a service level agreement (SLA) from the cloud provider which offers good uptime for the end user. Looking at Google App Engine, they are promising a 99.95% uptime in their SLA. This means you will experience a total of 4.5 hours of downtime in an entire year. It will be difficult for a startup that doesn’t have experience running infrastructure in production to achieve this level of uptime. This SLA is high and the majority of companies don’t meet that when running their own infrastructure. This means your initial customers will be happy with the stability of your service. Startups shouldn’t focus on maintaining this SLA because focusing on product development is a better use of time.

Using a PaaS will also save you money because you only pay for the resources that you’re using. This allows you to be more efficient when spending money on infrastructure when you need to scale your application. 

Popular PaaS providers follow security best practices when managing their infrastructure. This is something else you don’t need to worry about if you run your application on a PaaS. Not having to worry about infrastructure security is another benefit of using a PaaS and you get world-class security support and updates included in the product. 

PaaS providers offer integrations to other products within the same cloud provider. Whether you’re using Google Cloud Platform (GCP) or Amazon Web Services  (AWS), both providers offer great integration to other services in their platforms. This can help you when your products start to grow and require different solutions to your problems. The main disadvantage to seamless integration is vendor lock-in which I will discuss in the disadvantages section.

## What are the disadvantages of using a PaaS?
While there are a lot of great benefits of using a PaaS, there are also many disadvantages that you need to be aware of. One of the biggest disadvantages when using a PaaS is vendor lock-in. Vendor lock-in when you’re using a specific product that can’t be migrated off of that platform. This typically happens when using proprietary technology which is common with PaaS products. This might not be an issue when initially using a PaaS but can be a problem when the company starts to grow and has requirements that are no longer compatible with that PaaS.

PaaS providers sometimes don’t provide their services in all regions which means your performance might suffer depending on where your customers are located. This is common with all cloud products since they will offer the majority of their products to the regions with the most demand. If you find yourself in a situation where a product isn’t available in a certain region, you can always email the support team to ask them if there are plans to release it to a specific region.

If your customers are large or have a lot of regulations, sometimes you won’t be able to use a cloud provider because certain companies and industries have rules around how data is stored and where applications can be hosted. Some large enterprise companies still prefer to have software hosted within their data centers which will prevent you from using a cloud provider.

As your development team starts to grow the requirements will change or you might need a different solution. Migrating off of a PaaS is a lot of work since it provides solutions to many different problems out of the box which you end up needing to recreate. This will require a lot of time and expertise.

## Should a Startup use a Paas?

In conclusion, using a PaaS product does solve a lot of problems for startups but also has disadvantages as your team starts to grow and requirements start to change. One major advantage is that you don’t need to focus on the underlying infrastructure when deploying your code to production while the biggest disadvantage is vendor lock-in.

We recommend that startups initially go with a PaaS provider when starting off so they can focus on delivering value to their customers without too much effort. This will make your application more reliable which is good for a startup because it helps improve the user experience. Achieving a 99.95% SLA is difficult with a small team and is better left done by the cloud provider that’s an expert in this area. 

As your company starts to grow, a PaaS might not solve all of your needs and you might need to reevaluate the platform. This can be a lot of work but ultimately there are more advantages to using a PaaS then there are disadvantages. Startup founders should strive to reduce complexity while providing great experiences to their customers. 

## Notes

[1] [https://azure.microsoft.com/en-ca/overview/what-is-paas/](https://azure.microsoft.com/en-ca/overview/what-is-paas/){:target="_blank"}
