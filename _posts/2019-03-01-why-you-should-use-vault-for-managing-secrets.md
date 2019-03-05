---
layout: post
title:  "Why you Should use Vault for Managing Secrets"
author: alex
categories: [ Vault, Cloud ]
image: assets/images/vault.png
featured: false
hidden: false
date: 2019-03-01 10:49:05 -0500
---

Most development teams are struggling or have struggled to manage secrets at scale. There is a lot of overhead when rotating secrets and it’s a manual process that doesn’t get done right away. The solution for managing secrets is to introduce a tool that can store, audit, revoke, and rotate your secrets.

As development teams start to grow, managing your secrets starts to become complex especially when multiple teams need to access the same secret. Using a centralized secret storage tool like [Vault](https://www.vaultproject.io/){:target="_blank"} will allow multiple teams to access a secret efficiently and securely.

## What is Vault?

Vault is a tool for securely accessing secrets. A secret is anything that you want to tightly control access to, such as API keys, passwords, or certificates. Vault provides a unified interface to any secret, while providing tight access control and recording a detailed audit log.[[1]](https://www.vaultproject.io/docs/what-is-vault/index.html){:target="_blank"}

## The advantages of using Vault

One of the biggest advantages of using Vault is being able to store your secrets in a centralized place that’s encrypted and secured. If you need to update a secret that’s being used in different places, you only need to update it in 1 place. This removes secret management overhead and allows you to rotate secrets more efficiently.

Vault comes with multiple authentication systems. Auth methods are the components in Vault that perform authentication and are responsible for assigning identity and a set of policies to a user.[[2]](https://www.vaultproject.io/docs/auth/){:target="_blank"} What’s nice about Vault is that you can authenticate to it a variety of different ways. One of our personal favorites is using GitHub to authenticate to Vault. This makes it easier to manage user and team permissions for Vault.

Vault allows you to create dynamic secrets. This means that Vault can issue secrets with a Time to live (TTL). What this means is that a secret will only be valid for a certain period of time before it gets revoked. Vault has a feature called [secrets engines](https://www.vaultproject.io/docs/secrets/){:target="_blank"} which allows Vault to issue secrets to specific services dynamically. For example, Vault has a secrets engine that can handle database credentials which will allow Vault to dynamically generate credentials to a specific database for a certain amount of time. We highly recommend this feature as it’s a secure and automated way of handling credentials for certain systems. Since this is audited, you can see who requests a credential to which specific system. Since these credentials have a TTL, credentials being compromised become less of an issue.

One security focused feature that comes with Vault is audit logging which you can enable with 1 command. An audit log will show you if someone accesses or deletes a specific secret. It also shows when someone authenticates to the server. One strategy we’ve used in the past was to ship the audit logs to a centralized logging tool for further analysis. This allows you to indefinitely store the audit logs and lets you create reports on the activity of Vault. Traditionally it’s been difficult to see which secret is being accessed by who and the audit log solves this problem by creating log entries for all user actions.

If you have a server or application that needs to access a specific secret, Vault also provides functionality to solve this problem. Vault introduced the [AppRole](https://www.vaultproject.io/docs/auth/approle.html){:target="_blank"} as a way to provide authentication to specific roles in Vault. This means a system or application can only have access to credentials that you let it have access to by defining a role. 

People might think that Vault is insecure because if someone compromises the Vault server, they should be able to read any secret. This isn’t true since you need to authenticate to Vault to be able to read secrets. Vault also uses an algorithm known as Shamir's Secret Sharing to split the master key into shards. This means that even if you hold a key, you aren’t able to unseal Vault unless you have all of them. This is similar to a Two-man rule but you can have multiple people holding keys. In the past, we've set up clusters to have 6 key holders which are common in large organizations.


## The disadvantages of using Vault

The main disadvantage of using vault is the overhead required to run a vault cluster. The cluster needs to guarantee a certain uptime because applications can go down if they can’t read secrets from it. This means you have to create a robust infrastructure that can scale for your organization. It also needs to be performant so applications can read secrets quickly. The only managed Vault solution that currently exists is [Vault Enterprise](https://www.hashicorp.com/products/vault/enterprise){:target="_blank"}. It’s expensive but does solve the operational concerns for large companies that really heavily on Vault for managing their secrets and require a good SLA.

People might view the unsealing feature of Vault a disadvantage which is understandable. The alternative to having multiple key holders would be to introduce Vault auto unsealing. While this does make it easier to recover Vault when it goes down, some people might view this as a security risk. When evaluating auto unseal, you need to make sure you understand how it works and make sure it gets implemented correctly.

## Conclusion

Vault is a great way to manage secrets for large organizations and development teams. Being able to issue, rotate, and revoke secrets automatically is what makes Vault worthwhile. When using Vault, the manual overhead of managing secrets is eliminated. If your team is having trouble managing secrets, your team should evaluate Vault to see if introducing a secrets management tool will help improve your process.

## Notes

[1] [https://www.vaultproject.io/docs/what-is-vault/index.html](https://www.vaultproject.io/docs/what-is-vault/index.html){:target="_blank"}

[2] [https://www.vaultproject.io/docs/auth/](https://www.vaultproject.io/docs/auth/){:target="_blank"}
