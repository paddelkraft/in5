---
layout: book
title: Secure Coding in five minutes
published: 2016-04-30
coverimage: img/cover-secure-coding.png
featured: true 
preface: |
    Security issues are increasingly important in the IT world, both for developers and users. 
    Burying your head in the sand is just as counterproductive as being paranoid. 
    Instead we should keep the discussion alive as to what is a reasonable level of 
    security within our organization, our projects and for ourselves as indi- viduals. 
    At the same time there are of course practical steps we can take that can achieve a 
    lot through relatively little sacrifice. <br><br>
    This publication can serve as a basis for internal discussion about how you and your 
    colleagues can develop security within your organization
---
### Intro: 

## Morning meeting at Acme Inc.

![](../img/morning-meeting.png)

**Anna, Scrum Master:** Sorry to start the day with a bit of unpleasantness, but
Janne at Delta-Q called me late yesterday. He says
there was a hitch last week with the online store we’re
working on. Now he knows what the problem is.
Judging by the e-mails coming in from customers, it
seems that personal information and passwords
have been leaking ...

**Jonas, developer:** Oh no!

**Anna:** Now he wants to meet the people working on the site.
He believes that either we’ve left something open, or
else it’s even worse ...

**Simon, developer:** Are you saying that he believes that we ...?
Anna is grim-faced. She nods gravely.

***

## Have you thought through security?
Hand on heart – what’s your own approach to security?  

* Do you avoid taking risky short cuts when writing code?
* Do you refrain from using templates or routines in your application whose origin you’re uncertain of?
* Have you made a rational risk analysis and considered what threats and security issues it is sensible 
  to take into account? Have you thought through what an inexperienced or destructive user might do with 
  your system, and do you have a reliable process for restoring it?
* Have you or someone else backed everything up, so that you can confidently
  and safely restore your working environment after a crash?
  If not, the following pages may serve as food for thought ...

***

## Optimum security levels are based on a trade-off

Total security is an unobtainable fantasy: there are no absolute measures of
safety of the sort “if you do this, absolutely nothing can happen.” That’s how
it is with everything in life. Compare, for example, your life as a road-user
– it is built around your daily application of a balanced risk assessment
where, for instance, you weigh up the protection afforded by your bicycle
helmet against the dangers posed by drunk drivers.

Similarly, your life as a software developer or computer user must be
based on a balanced risk assessment where you make trade-offs:

* between efficiency and security
* between freedom of action and a sense of security
* between cost and the value of your work
* between fast, temporary solutions and time-consuming, robust
  solutions.

> **You do not have to solve all the security problems in your product, but you must**  
> <ul><li>Understand the risks you take</li><li>understand that you are taking them</li><ul>

***

### Safe suggestion #1:

## Take responsibility

**When we write robust and intelligible code, we get fewer security
problems. Unfortunately, most developers will probably agree that
they often have to hand over products that they are not entirely
happy with – a consequence of the fact that management prioritises
speed of production over long-term freedom from problems.**

With luck, the worst thing that happens is that a colleague smirks at your
clumsy code or groans at your substandard structure when debugging the
code later on. If you are unlucky, it’ll be worse – you might, for instance,
have created a vulnerability that someone with malicious intent can exploit.

Here we can gain inspiration from the Software Craftsmanship movement
and stress the importance of professional responsibility. Developers with
professional pride should not have to accept deadlines so tight that there’s
insufficient time to do a good job!

![](../img/team-hug.png)

> **Software Craftsmanship**  
> The Software Craftsmanship movement aims to promote professionality in the field of 
> software development, focusing on wellcrafted
> software, knowledge sharing and cooperation. 
>    
> **Read more at** (http://manifesto.softwarecraftsmanship.org)[http://manifesto.softwarecraftsmanship.org]

***

### Safe suggestion #2:

## Never trust data

Studies have shown that 60–80 % of all attacks are possible because
we do not validate that the data is in the correct format, even if it was
input directly by the user. The principle is never to trust data that
comes from somewhere other than our own system and that we can
keep track of.

All data input must therefore be validated in some way. One principle is to
locate any defects or abnormalities, but then you constantly have to add
new rules as the intruders become more skilful. It is actually better to
define what authentic and accurate data should look like.

Also remember that even if you validate data on the client
side, you need to revalidate it on the server side. A
malicious user can circumvent validation in clients and
send bad data straight to the server.

**Some simple examples:**
* If you have a field where you have to fill in a phone
  number, check that it does not contain any characters
  other than those that a phone number can contain.
* Many fields can be checked in terms of reasonable values.
  Input of quantities should be positive and e.g. heights could
  be checked for plausability; a person is probably not 10 meters
  tall.
* Some fields have to allow non-standard characters. For example,
  a surname might be O’Neil, which contains a character that
  some systems do not handle well. Make sure you store data in
  a sensible format so that problems do not arise.

>Examples of vulnerabilities
>  <ul><li>Web forms where the hacker, for example, can enter JavaScript instead of his surname (and can thereby create CrossSite Scripting).
> </li>
> <li>When the user enters SQL code to dump data in a field where
>   you can search for products (so-called SQL injection).</li></ul>

![](../img/detective.png)

