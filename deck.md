layout: true
class: middle

  <div class="my-header">
    <!-- <img src="images/logo_tiny.png" style="height: 30px;"/> -->
  </div>
  <div class="my-footer">
    <span class=left>2U Core Practices</span>
    <span class=right>Estimation, Points, & Velocity</span>
  </div>

---
class: center

# Hi! :-)

---

.f3[Part 1:]

# Team Velocity <br/>is a Speedometer,<br/> not a Tachometer

---

A **tachometer** is an instrument indicating the rotation speed of the engine of a car. You could say it indicates _how hard your engine is working_.

---

A **speedometer** is a gauge that measures and displays the actual speed (aka velocity) of a vehicle. It tells you _how_ _fast (or slow) you are actually moving along_.

---

For any given engineering team in my organization, especially with regards to their product managers and stakeholders, I care much more about monitoring how quickly they are delivering business value (speedometer) than how hard they are working (tachometer).

---

The metaphor of engineering team as motor vehicle is quite useful for explaining this tricky matter of speed versus effort and why it is a vitally important aspect of modern agile.

---

# SUSTAINABLE PACE

---

background-image: url(https://cdn-images-1.medium.com/max/880/1*HkUnhCW4nFCeZux36QbTTg.jpeg)

Let’s first consider effort, _how hard the team is working_. Modern agile teams are supposed to work at a _sustainable pace_. They commit to enough work to operate near maximum efficiency; no more, no less.

---

If someone tries to force a modern agile team to do more work than they are capable of doing responsibly, they resist.

The team says **no**.

---

If you push an engine to its redline it will resist. When it hits maximum RPM, it will not go any further.

The engine says **no**.

---

I find it useful to think about a team’s sustainable pace and redline kind of like engine efficiency metrics of a car’s internal combustion engine. [All engines have a _power band_](https://en.wikipedia.org/wiki/Power_band), the range of operating speeds under which they are able to operate efficiently.

---

Engineering teams have a power band too — the range of work commitment that maximizes delivery of business value while still allowing optimal time for vital activities such as automated testing, addressing technical debt (refactoring), learning, innovation, and maintenance of social cohesion.

Underutilize a team by not giving them enough work and you’ll waste money. Over-utilize a team (redlining?) and you’ll also waste money, plus they’ll eventually break down and fail.

# TORQUE & HORSEPOWER

---

The output of an engine can be measured in [torque](https://en.wikipedia.org/wiki/Torque) (power) and [horsepower](https://en.wikipedia.org/wiki/Horsepower) (rate of work). Engineering teams can be measured that way too. I like to think of _team torque_ as the power to deliver effective & elegant solutions to difficult problems and _team horsepower_ as an idealized measure of how quickly they deliver solutions.

---

Teams with high torque and modest horsepower can tackle difficult problems, just not very quickly. Conversely, teams with modest torque and high horsepower can crank out software at a high rate, as long as the work is not difficult.

---

Teams with superbly high torque and horsepower, like the engines in supercars, are relatively rare, expensive, and require high maintenance costs.

---

That said, the natural output metrics of a team affect but do not guarantee, velocity. Why? For the same reason you wouldn’t take million-dollar supercar on an off-roading excursion or enter it in a tractor-pull.

---

# VELOCITY IS SUBJECT TO EXTERNAL FACTORS

---

External factors matter, sometimes much more than team effort. While a tachometer is a useful indicator of effort, you cannot determine the speed of a vehicle based on the tachometer alone. You need a speedometer because velocity is always subject to _external factors_.

---

External factors that affect the velocity of your car include the incline of the roadway, [rolling resistance](https://en.wikipedia.org/wiki/Rolling_resistance), the effects of tail or head winds ([drag](https://en.wikipedia.org/wiki/Aerodynamic_drag)), and the weight of cargo being transported.

---

What are the external factors that affect an engineering team regardless of their horsepower? Technical debt, the quality of the specifications, tooling, team morale, the list goes on and on…

---

# POINTS

---

In a car, we measure velocity with MPH (miles per hour)or KPH (same, but with kilometers). On a modern agile engineering team we measure _team velocity_ with _points per iteration (PPI?)_ or simply _points_. You might say that points are like miles or kilometers on the speedometer.

---

In [How we estimate user stories](https://medium.com/modern-agile/how-we-estimate-user-stories-f345fd384474#.ocu944r8d), I explained that only user stories that deliver business value get point estimates, in measures of 1, 2 or 4 points. Stories that are too large and/or undefined to estimate are rejected and refined. Everything else (refactoring, fixing defects and developer chores) is either accomplished in the context of a user story, or tracked individually with zero points.

---

# SPRINT VELOCITY IS A TACHOMETER

---

Scrum has you assign points to everything the team does and use the number as the basis for deciding how much work the team should commit to doing during a sprint. Scrum teams have fancy ceremonial procedures like planning poker to decide how many points to assign to a story or task.

---

At best, all that kind of estimation and “velocity” accomplishes is to indicate how hard a Scrum team plans to work for the next two weeks. It does not reflect external factors affecting the team’s actual velocity, and has nil long-term predictive power. You cannot use Scrum’s sprint “velocity” to gain any predictive insight into when milestones will be reached beyond the end of the sprint.

---

Point estimation in Scrum is a _tachometer_. It’s a big part of why I think Scrum is full of _ceremonial bullshit._

---

# MODERN AGILE VELOCITY IS A SPEEDOMETER

---

When your estimation and velocity calculation reflect the rate at which business value is delivered per week rather than effort expended, then team velocity truly does indicate speed and can be used to predict arrival times for future milestones.

---

To recap, here are comprehensive rules for making sure that your velocity is a speedometer:

---

- Mercilessly break down stories into roughly equal units
- All user stories added to the backlog must be estimated by a representative of the engineering team
- Only use 1, 2 and 4 point estimates ([guidelines](https://medium.com/modern-agile/how-we-estimate-user-stories-f345fd384474#.wmy0te9m2))
- Reject any user story that feels larger than 4 points due to size or uncertainty — send it back to product managers for further decomposition and refinement
- Identify change requests masquerading as bugs — treat as user stories.
- Do not ever assign points to work spent on correcting “real bugs” (defects due to programmer error) or addressing technical debt.

---

# IF VELOCITY DROPS THEN IDENTIFY WHAT’S SLOWING DOWN THE TEAM

---

Bottom line, when there’s a problem with the team, no matter what the root cause is, you want to it to be bloody obvious that the problem is happening, _to everyone involved_.

---

Since velocity is the primary metric for the team and the one metric that directly affects product manager’s ability to predict releases accurately, it serves nicely as the team’s primary diagnostic tool.
