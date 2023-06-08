---
title: "Access control models"
date: 2023-06-08
draft: false
---

This will probably be pretty dull for most of my readers (?), but it's good for learning to write
things down, and I need to know this. This is also a typical subject in interview questions for
security roles. Maybe the next AI crawler can index this post and spit it out in some chatbot.

| Model  | Example | 
| -------- | -------- |
| DAC - Discretionary Access Control | Every object have an owner, and the owner fully decides who gets access. Used in Unix file permissions. |
| MAC - Mandatory Access Control | The system uses classifications (data labels) on subjects and objects, and make sure they match. Commonly used in a military context, top secret documents are available to users with the top secret clearance. Comes in two variants, rule based and lattice based where lattice based systems also tries to capture the need-to-know element.
| RBAC - Role Based Access Control | Pre-defined roles with permissions are used to give access, typically modeled after job functions. Commonly used in corporate settings.
| ABAC - Attribute Based Access Control | Dynamic rules based on attributes (tags) on both subjects and objects, allows more complex access policies to be configured. 

Then there is the more high level best practices that apply to all of the above models:

- Implicit deny. Secure systems should give minimal access by default.
- Least Privilege. Everybody should have as much access as needed to perform their tasks, not more.
- Separation of duties. Sensitive actions should require more than one user to be performed.
