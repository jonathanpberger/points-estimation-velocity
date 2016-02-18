layout: true
class: middle

  <div class="my-header">
    <!-- <img src="images/logo_tiny.png" style="height: 30px;"/> -->
  </div>
  <div class="my-footer">
    <span class=left>2U Core Practices</span>
    <span class=right>Points, Estimation, & Velocity</span>
  </div>

---
class: center

# Hi! :-)

---

# Writing Well-formed User Stories

---

## Writing Well-Formed User Stories

Convention Over Configuration is one of core principles


-  of the Rails approach to software development, and delivers enormous value.

---

# Convention Over Configuration

means that Rails makes assumptions about what you want to do and how you’re going to do it, rather than requiring you to specify every little thing…

---


# Oddly

we tend not to apply the same perspective to project planning

???

- on almost every project, the team re-invents the wheel
- “how should we write and format our stories?”.
- rigorous story-writing is one of the most common areas for low-cost, high-gain improvement.

---


## Write every story in Gherkin.

???

I don’t care whether or not you use cucumber: use Gherkin. Which is to say, every story should be in “Given / When / Then” form. This is the cheapest and easiest way to apply Convention Over Configuration to your user stories, and can have a HUGE benefit for your team.

---
```
Scenario: User adds item to cart
  Given I'm a logged-in User
  When I go to the Item page
  And I click "Add item to cart"
  Then the quantity of items in my cart should go up
  And my subtotal should increment
  And the warehouse inventory should decrement
```
---

Every feature story should include an “As a / I want to / Because…” block, which illustrates the motivation behind a story. Compelling the product team to specify the motivation behind a story help illuminate what exactly the requirement is, as well as providing guidance to the developers. Some people prefer “So That…” instead of “Because“, but in most cases “Because” helps drive out motivation—the Final Cause—whereas “So that” may only drive out the Effective Cause, which is less useful for understanding the story. (Thanks to Sam Coward for this insight.)
Feature: Shopping Cart
  As a Shopper
  I want to put items in my shopping cart
  Because I want to manage items before I check out
Every story title should include the word “should”. NEVER use the word “can”, which camouflages desired behavior. E.g. It’s unclear whether the story “User can delete comment” is a feature or a bug. “User should be able to delete comment” or “User should not be able to delete comment” are much clearer: the former is a feature, the latter a bug. Don’t make me guess.
When a story feels a little fishy, check that these bases are covered. If any are missing, fix then before you do anything else. The answer will often be driven out in the process of working the story into Well Formed shape.

---


Benefits
Well Formed stories truly drive out the feature from the user’s perspective; this catches 80% of weird edge cases while the whole team is together, in context, and in planning mode, instead of having to interrupt-drive the PM. Well Formed stories make it impossible to camouflage large stories as small stories by elision. Because the story has to be written out step-by-step, all the complexity might otherwise be hidden is forced out into the open. And when you find yourself with conditionals or switches? That’s a new scenario! Now all stories are forced into roughly the same size. Another side-effect is that once one story ~= one scenario, the amount of work to be done can be roughly gauged spatially, by looking at how much of your wall is covered by index cards. For bonus points, use the story title as your git commit, e.g. the story “User should be able to recommend a product” becomes the git commit “User is able to recommend a product”, and your git log tells the narrative of your project.

---


How did this start?
Once apon a time, J (the anchor) made N (a very bright, technical Product Manager) write stories in Gherkin. Most stories weren’t 100% ready to be pasted into cucumber, but it usually didn’t take too much work to get them there. The team would discuss in IPM, and then devs could copy-and-paste stories right into Cucumber. This doesn’t work for every PM, but even in the worst case, teams with less than tech-savvy PMs see real benefits from writing their stories at the right level of granularity. Once I was exposed to a team where we wrote Gherkin all the time, anything else felt like broken process.
