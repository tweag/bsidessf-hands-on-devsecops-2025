![BSides San Francisco](BSidesSF_2025_MobileHeader_1080x440.jpg "BSides SF 2025")


# Shifting Left: A Hands-on Introductory Guide to DevSecOps

The following repository contains training material on shifting security left for our 2025 workshop at BSides SF.

This workshop is held at `BSides SF` on `April 26th 2025` at `12:30pm - 2:30pm`.

Sign up is available at: https://bsidessf.regfox.com/2025

## Workshop Outline

This two hour workshop on Shifting Left guides BSides SF participants through integrating security tooling into a GitHub Actions based DevSecOps CI/CD pipeline.

BSides SF attendees will learn about setting up basic CI/CD processes that incorporate security using both open source and commercial tool

Here we provide an introduction to the workshop and the team running it. We will also cover some basics around how to ask for help and the tools we will be using across the two hour session.

## Pre-setup Phase

In order to fully participate in this workshop you will need a GitHub account. You can obtain this by signing up at http://www.github.com. If you are a student, you can sign up for a student account. 

Students will be able to sign up for a .edu account which comes with some added bonuses, such as being able to setup private repositories for free. You can learn more here: https://education.github.com/pack

Once your account is setup, you will need to `Fork` and `Clone` this repository or spin up a Codespace environment. 

Read more about forking and cloning here: https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo

## Working In The Repository - Scanning Codebase

Here we cover some repository scanning methodologies, including scanning for secrets and vulnerability detection in codebases. This will be demonstrated using tools like GitHub's dependabot and GoDaddy's Tartufo.

### Part 1 - The First Hour: DevSecOps Basics

1. Secrets scanning. Our first task will be to demonstrate how secret scanning can be performed on some vulnerable source code. This includes examples of using open source tools Tartufo, TruffleHog, Horusec and GitHub's native secret scanning capabilities. [Module 1:Secrets Scanning](https://github.com/tweag/bsidessf-hands-on-devsecops-2025/tree/main/src#module-1secrets-scanning)

2. Handling secrets in the SCM. GitHub includes a secrets storage mechanism, that allows you to safely store API keys, passwords and other senstivie data securely within the SCM. These credentials can then be pulled out for usage at deployment time e.g. via GitHub Actions. Here BSides SF students learn the basics of GitHub's features and how to leverage GitHub native secret storage mechanisms. We will demonstrate how to pull repository level secrets into the CI/CD pipeline and show how GitHub ensures these do not leak [Module 2: Handling secrets in GitHub](https://github.com/tweag/bsidessf-hands-on-devsecops-2025/tree/main/src#module-2handling-secrets-in-github)

3. Detecting security vulnerabilities within the source code. BSides SF students are introduced to the concept of detecting security vulnerabilities in the git repository. A general overview of techniques and approaches is given using open source and GitHub native tools.[Module 3:Detecting Security vulnerabilities](https://github.com/tweag/bsidessf-hands-on-devsecops-2025/tree/main/src#module-3handling-secrets-in-github)

4. Vulnerable dependency detection. Here we look at GitHub's dependabot, which provides a mechanism for analyzing the dependencies associated with a project and understanding if they contain security vulnerabilities. A walkthrough of dependabot is performed. [Module 4:Vulnerable dependencies](https://github.com/tweag/bsidessf-hands-on-devsecops-2025/tree/main/src#module-4vulnerable-dependencies) 

### Part 2 - The Second Hour: Digging Deeper

5. Static analysis in more detail. GitHub's GHAS (GitHub Advanced Security) contains a native SAST tool built on CodeQL and some newer AI features that allow you to Autofix issues. This section of the class walks through how it works and how it can be integrated into GitHub actions. This section of the talk will also cover the Open Source Horusec tool and how it can be used in the same capacity.[Module 5:Static Analysis](https://github.com/tweag/bsidessf-hands-on-devsecops-2025/tree/main/src#module-5static-analysis)

6. Rule sets and pull request gating mechanisms. The penultimate topic covered is how rule sets and PR gating mechanisms can leverage SAST tools to block pull requests that fail security checks.[Module 6:Branch protection rules](https://github.com/tweag/bsidessf-hands-on-devsecops-2025/tree/main/src#module-6rulesets)

7. SBOMs - Software Bill of Material. GitHub dependency featurescan be used to extract a Software Bill of Materials from your application repositories. [Module 7:SBOMs Software Bill of Materials](https://github.com/tweag/bsidessf-hands-on-devsecops-2025/tree/main/src#module-7sboms-software-bill-of-materials)

## Q and A

This course wraps up with a Q and A session..

