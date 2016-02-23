layout: true
class: middle

  <div class="my-header">
    <!-- <img src="images/logo_tiny.png" style="height: 30px;"/> -->
  </div>
  <div class="my-footer">
    <span class=left>2U Core Practices</span>
    <span class=right>User-Centered Storywriting</span>
  </div>

---
class: center

# Hi! :-)

---

2U Core Practice Talks

# User-centered Story Writing

February 2016

---

subj: what are core practice talks?

# What are Core Practice Talks?

- a place to share best practices and context about agile concepts
- we'll repeat talks as necessary to keep room size conversational
- WIP / experimenting w format

---
.f3[What are Core Practice Talks? (cont.)]

- an opportunity to ask questions and deliberate
- let us know what you want to hear about
- success criteria: more debate, more and more ppl feel comfortable giving them

---

class: center

.f1[User Centered <br /> Story Writing]

---
# Agenda

1. Types of stories
2. Writing Well-formed User Stories
3. User-Centered Design

---

# I. Types of stories

1. (Feature) Stories
2. Bugs
3. Chores

---

## (Feature) Stories

- A story is the smallest amount of work that has user-facing value
- A story card is a placeholder for a conversation
- Stories should follow I.N.V.E.S.T. principles

???

- let's take these in reverse order

---
### I.N.V.E.S.T.

|                 |                                                                                                 |
| ------          | ------                                                                                          |
| **Independent** | Stories should be self-contained, without inherent dependency on another story.                 |
| **Negotiable**  | Stories, until started, can always be changed and rewritten.                                    |
| **Valuable**    | Stories must deliver value to the end user.                                                     |
| **Estimatable** | You must always be able to estimate the size of a user story.                                   |
| **Small**       | Stories should not be so big as to become impossible to estimate or prioritize.                 |
| **Testable**    | The user story must provide the necessary information to make test-driven development possible. |

???
- rubric for writing stories
- this can help update our backlogs
- note what stories aren't: feature requests divorced from user value, or descriptions of UI

---

### Stories are **placeholders for conversations**
- Stories are not valuable (holy?) in and of themselves
- Delay detail until the Last Responsible Moment to avoid waste
- Conversations are *interactive* among the team (use the comments to conduct / memorialize conversation)
- Use the storycard (description) to memorialize decisions

???

- once upon a time, these really were index cards on wall (we're still doing that here)
- this is a point about how teams and stories relate to each other
- so let's step back and talk about what we're doing here


---
name: think-make-check
class: contain
background-image: url(images/think-make-check.png)


???
### Think-Make-Check


---
name: sawtooth
background-image: url(images/sawtooth.jpg)
class: contain

???

### Minimizing Risk
- risk is Unvalidated Work
- why is story-writing helpful?
- it breaks work down into more validate-able chunks

---
class: center

### User-facing value

![](images/skateboard.jpg)

???

- this is a story about user-facing value
- try to deliver small increments, even if they're not what was originally asked for, if
- they build to the "final" goal
- they deliver learnings cheaply

---

### F.U.E.P.
- user flows / features must progress through FUEP when being built
- effort is a hockey stick shape
- coverage is a long tail shape

???

This can be a tool for prioritizing


---

### Splitting Stories

- In Gherkin, "If" and "Or" are clues to split the story

---

## Bugs

- *un*pointed (because the points were already assigned and spent)
- should represent work the PM thought was already done / had already accepted
- Bugs represent software regressions
- not the same as support tickets (e.g. “fix this user’s permissions in the db”)
- Written by anyone, prioritized by Product
- "it's a bug if it was created here"

???

- unpointed bugs affect velocity; that's good. We want to drive the conversation

---

## Chores

- *un*pointed
- technical tasks w/o user-facing value (e.g. "switch from MySQL to Postgres")
- something that has to be done and cannot be accepted by the PM
- written and prioritized by Engineers
- "things the client doesn't know to ask for"
- "something we're gonna do whether the PM likes it or not

???

- not things the client asked for
- we should make them care. "You can stick w/ this new version, but we'll move faster if we spend a few days upgrading rails"
- this all ties into tech debt: how to manage it, how to advise clients?
- refactoring can be a feature, it's not always a chore (eg refactoring on open-source)

---

### Spikes
- *un*pointed (it's a type of chore)
- spike when you don't know enough to estimate a story
- a spike is "narrow and deep" research
- the outcome of a spike is an estimated story
- you *can* write untested code
- you *must* throw the code away

---

## What about Technical Teams?

- 2U has some exceptional teams ({Financial, } Data Warehouse, DevOps)
- "User-facing Value" gets a little sketchy
- Stories for one team might look more like Chores for another. That's ok.

???

- "The constitution isn't a suicide pact"
- these principles serve our teams, not the other way around


---


# II. Writing Well-Formed User Stories

1. Gherkin
2. Motivation
3. Should

???

- Ok, so how do we do it?

---

## Convention over configuration

???

- on almost every project, the team re-invents the wheel
- “how should we write and format our stories?”
- rigorous story-writing is one of the most common areas for low-cost, high-gain improvement.

---


## Write every story in Gherkin

The magic words are:

- Given,
- When,
- And,
- Then

???

- Gherkin != cucumber
- cheapest and easiest way to apply Convention Over Configuration to your user stories

---

## Gherkin Example

```Cucumber
Scenario: User adds item to cart
  Given I'm a logged-in User
  When I go to the Item page
  And I click Add item to cart
  Then the quantity of items in my cart should go up
  And my subtotal should increment
  And the warehouse inventory should decrement
```


---

## Motivation block

```Cucumber
As a [ROLE]
I want to [DO A THING]
Because [MOTIVATION]
```


???

- helps illuminate what exactly the requirement is
- provides guidance to the developers
- "because" vs "so that"

---

## Motivation block example

```Cucumber
Feature: Shopping Cart
  As a Shopper
  I want to put items in my shopping cart
  Because I want to manage items before I check out
```

---

## Story Titles

- Every story title should include the word “should”.
- NEVER use the word “can”, which camouflages desired behavior.
- E.g. It’s unclear whether the story “User can delete comment” is a feature or a bug. “User should be able to delete comment” or “User should not be able to delete comment” are much clearer: the former is a feature, the latter a bug. Don’t make me guess.

???

- When a story feels a little fishy, check that these bases are covered.
- If any are missing, fix then before you do anything else.
- The answer will often be driven out in the process of working the story into Well Formed shape.


---


## Benefits of Well Formed stories
- drive out the feature from the user’s perspective
- catches weird edge cases
- do it while the whole team is together, in context, and in planning mode, instead of having to interrupt

???

---

- Well Formed stories make it impossible to camouflage large stories as small stories by elision.
- Because the story has to be written out step-by-step, all the complexity might otherwise be hidden is forced out into the open.
- And when you find yourself with conditionals or switches?
- That’s a new scenario! Now all stories are forced into roughly the same size.
- Another side-effect is that once one story ~= one scenario, the amount of work to be done can be roughly gauged spatially,
- by looking at how much of your wall is covered by index cards.

---

## Bonus Points: stories & Git commits

- For bonus points, use the story title as your git commit,
- e.g. the story “User should be able to recommend a product” becomes the git commit “User is able to recommend a product”,
- and your git log tells the narrative of your project.

---


## the payoff
- Once apon a time, J (the anchor) made N (a very bright, technical Product Manager) write stories in Gherkin.
- Most stories weren’t 100% ready to be pasted into cucumber, but it usually didn’t take too much work to get them there.
- The team would discuss in IPM, and then devs could copy-and-paste stories right into Cucumber.
- This doesn’t work for every PM, but even in the worst case, teams with less than tech-savvy PMs see real benefits from writing their stories at the right level of granularity.
- Once I was exposed to a team where we wrote Gherkin all the time, anything else felt like broken process.

---

# III. User-Centered Design


---

# Thanks!

---

# Questions?
