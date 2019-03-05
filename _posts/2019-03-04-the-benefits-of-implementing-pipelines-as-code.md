---
layout: post
title:  "The Benefits of Implementing Pipelines as code"
author: alex
categories: [ Pipelines, CI, CD ]
image: assets/images/pipeline.png
featured: true
hidden: false
date: 2019-03-04 11:38:52 -0500
---

Development teams that work with Continuous Integration/Delivery (CI/CD) systems are used to the frustration that comes with managing deployment pipelines. Pipelines as code eliminate the management portion because the pipeline definition will be stored in a centralized place where everyone can view and make changes to it in a collaborative way. Manually keeping track of how a deployment pipeline is created is a lot of work and changes can easily be forgotten or lost. There are a variety of tools that allow you to leverage Pipelines as code but we will be focusing on the advantages and disadvantages of this practice.

## What is Pipelines as code?

Pipelines as code are best defined as a practice where you write your deployment pipeline as code and store it in a version control system. This means that the history of the pipeline is tracked and stored in a centralized place. Using Pipelines as code eliminates the manual creation and management of a deployment pipeline that was traditionally done in CI/CD tools.

## What are the benefits of implementing Pipelines as code?

When teams would try to create a new deployment pipeline, it would have to be manually configured in a CI/CD tool to work. Pipelines as code allow you to write your deployment pipeline with code which means you can easily collaborate on it without having to make manual edits inside of the tool. When you update your pipeline, the CI/CD tool will automatically pick up the pipeline changes without any manual intervention. This is a big step up from having to manually make changes from inside the tool.

When your pipeline is stored in a version control system, this means you're able to track the history of changes made to the deployment pipeline. In the past, it was common to make a change to the pipeline causing it to break which would result in the development team being blocked. Since the deployment pipeline is tracked, you don't have to worry about rogue changes being made because the pipeline can go through a code review process where multiple people can review the changes. If a change to the deployment pipeline causes it to break, then it can easily be reverted which was difficult to do in the past because deployment pipelines were manually managed and updated from within the CI/CD tool.

Since the deployment pipeline is stored in a version control system, it won't get lost and the state will always be consistent. If your CI/CD tool crashes and loses data, you can easily restore the deployment pipeline because it's stored in a version control system and the CI/CD tool knows where to find it. If the deployment pipeline wasn't stored in a version control system, it would be difficult to restore because you would have to manually create it again which can take a long time especially if you don't remember how it was configured.

## What are the disadvantages of implementing Pipelines as code?

The only disadvantage is the learning curve involved when starting to write deployment pipelines. Writing a deployment pipeline isn't something most people have experience with and can be tricky at first. The upside is that there are a lot of resources and examples online that can help you when starting off. Once you get the hang of writing deployment pipelines, you can re-use some of the components across projects by creating a library. This reusability will save your development team time in the future.

## Conclusion

Development teams should start implementing Pipelines as code as soon as possible because it removes a lot of the complexity and overhead when creating deployment pipelines. Being able to track and store your changes is the biggest benefit and it makes your development team more productive. Pipelines as code encourage everybody to contribute to the deployment pipeline which was something people avoided doing in the past.

## Notes

[1] [https://developers.redhat.com/blog/2017/09/06/continuous-integration-a-typical-process/](https://developers.redhat.com/blog/2017/09/06/continuous-integration-a-typical-process/){:target="_blank"}