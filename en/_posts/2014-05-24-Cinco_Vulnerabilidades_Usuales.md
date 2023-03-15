---
title: "Five Common Vulnerabilities within an Organization"
date: 2014-05-24
categories: [Ethical Hacking, Vulnerabilities]
tags: [vulnerabilities, ethical hacking]
author: <MH>
comments: false
img_path: /assets/img/postimg/brechas
image: SecurityBreach.jpg
lang: en
lang-ref: cinco-vulns
---

As you may already know, vulnerabilities are always present within organizations and if they are not analyzed or controlled in some way before being exploited, they could represent a serious threat to the information assets of the compromised organization.

There are levels of criticality in vulnerabilities associated with information systems. In the following post, we will discuss 5 vulnerabilities usually classified as low risk but that are important to analyze, as they could represent the first step towards a much larger attack.

## Vulnerability 1: Weak Passwords

An attacker will always look to enter through the weakest or least controlled side of an organization, such as the human factor. Therefore, in terms of credentials, users will always prefer to use passwords that are easy to remember, simple, or associated with an important event or experience such as a birthday or the name of their children. In other cases, they use sequential passwords such as "April2014++", "May2014++", and so on.

**BIG MISTAKE!** Those types of passwords are easy to break using brute force algorithms, dictionary usage, or hybrid mechanisms. Using this type of passwords compromises the information handled by the user at a very high level. It should be noted that if it is a key user in the organization, the information they handle may be very sensitive. Passwords for servers, database accesses, and commercial strategies are some examples.

> The more complex and unrelated to personal matters your password is, the lower the risk of it being broken.
{: .prompt-tip }

![Figura 1](figura1.png)
*Using John The Ripper to obtain the root user's password.*

## Vulnerability 2: Information Disclosure

Speaking of Microsoft products, how many times have you seen the typical yellow error screen that represents an uncontrolled exception in web applications? How many times have you been faced with the ostentatious IIS7 screen when trying to access a web page incorrectly?

![Figura 2](figura2.png)
*Microsoft IIS7 banner*

For a common user, those screens may be insignificant and even incomprehensible, but **for an attacker they could be very useful** within a Footprinting process or data harvesting to later carry out elaborate attacks.

Upon seeing the IIS7 screen, an attacker would automatically think:

- IIS version 7
- Operating system used by the server: Windows Server 2008 (at a minimum)
- Possibly using ASP.Net in Visual or C# as it is the most commercial.

In reality, an attacker would not hesitate to search Google for the types of vulnerabilities that exist for IIS7 or set up a virtual machine with those characteristics and run a vulnerability scanner on it.

**The same thing happens for uncontrolled exceptions**, if one emits an ORA error message, we immediately know that an Oracle DBMS is being used and if it is a weak application we could begin with simple SQL injection tests.

> One must be very careful with the information that is disseminated towards the Internet, you never know who is on the other side.
{: .prompt-tip }

## Vulnerability 3: Unpatched Systems

It is a fact that **systems that do not have the latest software updates are the most likely to become a target of an attack.** While keeping a system updated is considered a good practice, it can sometimes become a complicated task, especially when working in production environments where high availability of applications is required.

For example, if an organization has a web application based on Net Framework 1.1 on WS2000 and upgrades the OS version to WS2008 without testing, problems may arise that affect the availability of the service, since without installing certain hotfixes, Framework 1.1 does not work well with WS2008. Many times, server administrators choose to disable automatic updates because the behavior of an application in response to software updates for a server cannot be predicted. In this regard, other alternatives must be chosen to ensure the availability of services and the security of servers simultaneously.

![Figura 3](figura3.png)
*Windows Update*

## Vulnerability 4: Default Configurations

When an organization acquires a new technology or specialized hardware (firewalls, preventors, etc.), they almost always leave the installation and configuration of the product in the hands of the provider. In theory, this is the most logical thing to do since no one within the organization is a specialist or knowledgeable about the new product.

**In practice, doing this is somewhat risky**. Providers in some cases choose to send untrained personnel for the installation of their products because it generates lower costs, or even outsource the installation. In other cases, providers opt for default installations, as they do not want to risk the installation causing problems in the client's operations. This generates configurations and credentials that everyone knows. Who doesn't know that the default credentials for a Tomcat are admin/admin?

> Always demand customized installations or designate someone to supervise the installation.
{: .prompt-tip }

## Vulnerability 5: Untracked Controls

Within organizations, procedures or controls are always created to align the daily operations of internal collaborators. In many cases, **organizations believe that it is sufficient to define procedures and do not track them to validate if the procedure is being fully complied with**. For example: An organization that performs its own developments must ensure that they are reliable and do not generate security breaches. To achieve this, a secure development procedure or policy must be defined. These will ensure that developments are secured, but what if the developers do not comply with these policies for the sake of practicality or to make the development process more agile?

This could be a real situation for any organization if periodic controls are not carried out to validate that developments comply with the established guidelines.