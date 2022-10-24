---
created: 2022-09-01T09:09:56-07:00
updated: 2022-09-01T09:11:13-07:00
---
Re: getting FedRAMP approved, [[John Blessing]] posted this in the [[Palantir Alumni Slack Community]] \#chatter channel on 2022-09-01 in response to a question from [[Daniel Bardenstein]]:

> Here is the key realization: There are no strict technical requirements, it's primarily a question of fulfilling NIST 800-53 security controls through a combination of technical implementations, policy, and process. Even at Palantir, many of the pieces we built policy around rather than attempting to automate
> 
>    short version though is:  
> 
> -   figure out why you're doing this. It was literally thousands of hours of engineering time for Palantir (but we also had a complex product and little compliance experience). If it's a customer, what's the level at which you need to be approved (low, moderate, high). That will determine the set of controls
> -   Figure out if you're going JAB (joint authorization board) or agency approval. JAB is typically more stringent and takes much longer (backlog was 1-2 years when I last checked a couple years ago), but their approval is mostly accepted across the whole gov. In either case, you need actual federal customers seeking to use your product, otherwise you're at the back of the line
> -   Find a 3PAO (third party audit org) that you can work with. They'll be the people you have to convince of the adequacy of your controls. If they don't have a technical bone in their collective body, tech solutions are going to be a hard sell.
> -   Build your compliance package. That largely means control responses to the subset of [NIST 800-53](https://csrc.nist.gov/publications/detail/sp/800-53/rev-5/final) controls applicable for your security baseline
> -   iterate
> -   get audited
> -   Audit gets  reviewed by the FedRAMP authorization authority selected in step 2 (this too requires iteration and explaining things to non-technical people. Here is where paying for a good 3PAO who can defend your solution / their assessment really pays)
> -   profit?