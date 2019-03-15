---
layout: post
title:  "Why most companies don't need Kubernetes"
author: alex
categories: [ Kubernetes, DevOps ]
image: assets/images/kubernetes.png
featured: true
hidden: false
date: 2019-03-15 11:25:00 -0500
---

Kubernetes has gained a lot of popularity recently in the industry and a lot of people are considering using it in production. Before you consider using Kubernetes, you need to understand what your use-case is so you can determine if Kubernetes is a good fit for your organization.

While I am a fan of Kubernetes and the problems it solves but I don’t think most companies have a proper use-case for using it. If you’re able to keep things as simple as possible, I would recommend doing that instead of introducing a complex system.

## Why should you avoid Kubernetes?

Below I will outline a few reasons why your company should avoid using Kubernetes.

### Kubernetes is complex

Kubernetes introduces a lot of complexity for development teams. The reason why this is a problem is that your development team has to spend the time to learn another tool. Creating and operating a cluster is complex and isn’t something that most people know how to do. Kubernetes also has a lot of moving pieces which is why it isn’t something you can learn overnight.

### Your applications are simple

If you have a small number of applications that don’t receive a lot of traffic, then you should look at alternatives. Kubernetes becomes useful when you're following a microservices pattern and have many different services with similar configurations.

### You run everything in the cloud

If you already run everything in the cloud, I don’t see the advantage of using Kubernetes. Kubernetes is great for companies that are looking to use their on-prem infrastructure as well as cloud infrastructure to create a hybrid cloud. This is typically done by companies that need to maintain a high level of availability for their applications. Unless you’re running a highly critical application that needs to provide a high uptime for users, it doesn’t make sense.

### Kubernetes is hard to secure

Securing a cluster is a complex task that requires a special set of expertise. Kubernetes has a lot of gotchas when it comes to security so I would suggest using something that’s simpler to secure.

### Kubernetes introduces overhead

Although Kubernetes can save your company money and make your development team more productive in the long-run, you need to make a large upfront investment when starting out. You will need to teach your teams how to use Kubernetes and you will need to build a dedicated team of experts to maintain and operate your Kubernetes cluster. Kubernetes itself doesn’t provide the best developer experience which is why there are plenty of tools that have been created to help turn Kubernetes into a platform. Turning Kubernetes into a platform also introduces a lot of overhead.

## What are the alternatives?

For companies that have simple applications, I suggest using a [Platform as a service (PaaS)](https://scalarsoftware.com/blog/should-a-startup-use-paas/){:target="_blank"}. There are plenty of container-based PaaS tools that all of the cloud providers offer. If you decide that you don’t want to use containers, there are still plenty of options to choose from. Each cloud provider will have some sort of PaaS offering so you will need to do research to see which one is the best fit for your team and application.

## What if I need Kubernetes?

If you found a use-case where you need to use Kubernetes, I would suggest that you look at the managed Kubernetes services that exist. Google Cloud offers GKE, Amazon offers EKS, and Azure offers AKS. Rancher offers RKS which makes it easier to create clusters. These tools will make your Kubernetes experience smoother.

## What about self-healing features?

While the auto-scaling and auto-healing features of Kubernetes are great, you don’t need to use it to get this functionality. There are plenty of different tools out there that also come with these capabilities that are simpler to use than Kubernetes.

## The future of Kubernetes

I believe that Kubernetes will become easier to work within the future. The managed Kubernetes services being offered by cloud providers have already made a big impact on the developer community. With tools like Knative, I could see cloud providers move to a more serverless approach with Kubernetes. There are plenty of tools in the ecosystem that is trying to simplify the Kubernetes user-experience to make it accessible to everyone.

## Conclusion

Unless you have a compelling use-case on why Kubernetes will provide a better user experience for your customers, you shouldn’t introduce it. The complexity and overhead don’t make sense for most companies. There are plenty of great platforms that can solve your business problem without introducing a lot of complexity for your development teams.

## Links

[0] [https://kubernetes.io/images/kubernetes-horizontal-color.png](https://kubernetes.io/images/kubernetes-horizontal-color.png){:target="_blank"}
