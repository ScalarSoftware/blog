---
layout: post
title:  "The Benefits of using Pipelines as code"
author: alex
categories: [ Pipelines, CI, CD ]
image: assets/images/pipeline.png
featured: false
hidden: false
---

Development teams that work with Continuous Integration/Delivery systems are used to the frustration that comes with managing delivery pipelines. Pipelines as code eliminate the management portion because the pipeline definition will be stored in a centralized place where everyone can view and make changes to it in a simple way. Manually keeping track of how a delivery pipeline is defined is a lot of work and changes can easily be forgotten.

## What is Pipelines as code?

Pipelines as code are best defined as a practice where you write your deployment pipeline as code and store it in a version control system. This means that the history of the pipeline is tracked and stored in a centralized place. Using Pipelines as code eliminates the manual creation and management of a delivery pipeline that was traditionally done in Continuous Integration/Deployment tools.

## What are the benefits of Pipelines as code?

Traditionally, when teams would try to create a new deployment pipeline, it would have to be manually configured in a Continuous Integration/Delivery tool to work. Pipelines as code allow you to write your delivery pipeline with code which means you can easily store and collaborate on it without having to make manual edits inside of the tool. When you update your pipeline with code, the CI/CD tool will automatically pick up the pipeline changes without any manual intervention. This is a big step up from having to manually make changes from inside the tool.

When your pipeline is stored in a version control system, that means you're able to track the history of the delivery pipeline. In the past, it was common for a change to get made to a pipeline causing it to break which would block the development team. Since the delivery pipeline is tracked, you don't have to worry about rogue changes being made because the pipeline can go through a code review process. If a change to the delivery pipeline breaks it then it can easily be reverted which was difficult to do in the past because delivery pipelines were manually managed and updated.

Since the delivery pipeline is stored in a version control system, it won't get lost and the state will always be consistent. If your CI/CD tool crashes and loses data, you can easily restore the delivery pipeline because it's stored in a version control system. If the delivery pipeline wasn't stored in a version control system, it would be difficult to restore because you would have to manually create it again which can take a long time especially if you don't remember how it's configured.

## What are the disadvantages of Pipelines as code?

The only disadvantage is the learning curve involved when starting to write delivery pipelines. Writing a delivery pipeline isn't something most people have experience with and can be tricky at first. The upside is that there are a lot of resources and examples online that can help you when starting off. Once you get the hang of writing delivery pipelines, you can re-use some of the components across projects by creating a library.

## Conclusion

Development teams should start implementing Pipelines as code as soon as possible because it removes a lot of the complexity and overhead when creating delivery pipelines. Being able to track and store your changes is the biggest benefit and it saves your development team time.
