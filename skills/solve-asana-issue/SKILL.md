---
name: solve-asana-issue
description: When you are asked to solve a issue with asana link given, consider this skill 
---

# Following the instructions
- Read the Issue from asana and build up comprehensive understanding of the issue itself
- You can use any Skills, Tools, Command, Agent, or check any document include source code to figure out root cause of problem
- If you think it's no need to write code, report you conclusion to me
- If you think PR is need, you can carryout a Fix PR

# Caveat: if carry out a Fix PR
- Make sure checkout from develop to your fix branch
- Make sure you write test cover fixed logic and test is passed
- Make PR is target to merge to develop

# Caveat: if fire PR to Github
- Put Asana Issue link in front section if PR description
- Describe root cause and how to fix comprehensively, but not lengthly
- If PR is large, provide advice to reviewer
