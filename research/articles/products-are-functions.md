# Products Are Functions — Ryan Singer

## Source
- **Title:** Products Are Functions (4 Aug 2018)
- **Speaker / author:** Ryan Singer (ex-Basecamp, creator of Shape Up)
- **URL:** https://www.feltpresence.com/functions/ (now redirects to https://ryansinger.co/functions/)
- **Type:** article
- **Notes on source quality:** Full text read. Short article. The x / f() / y diagrams are images; their content is described by alt text and surrounding prose (for example "Function before Basecamp", "Requirements for a new function to replace the wall calendar"), so the exact wording inside the diagrams was not available.

## Summary
Singer argues that a product is best described as a function. The user starts in a situation x, applies a product f(), and ends in a situation y. This describes what the product does for the customer, not a bundle of features. The designer does not get to choose x or y; both are empirical facts about the customer. So x and y are the real requirements, and f() is the only variable. The Basecamp "calendar" story shows the payoff: by finding the real x and y, the team built a "Dot Grid" that was 10x cheaper than a full calendar. For idea validation, this forces a founder to name the before-situation and after-situation in the customer's terms, and to compare against the status quo, not an ideal.

## Key ideas and frameworks
- **Product as function f(x) = y:** x is the user's circumstance before. f() is the product. y is the resulting circumstance. Describe products as transformations, not as categories like "project management".
- **Status quo is also a function:** Before Basecamp, the f() was email and spreadsheets. They are fine until the workload or team gets too big; then they give a bad y. Basecamp takes the same x and gives a different y.
- **x and y are requirements; f() is the variable:** The designer cannot define x (it is empirical) or dictate y (it is only a valid target if the user would pay for it). Requirements should be defined independent of the solution, as tests for fitness.
- **Feature requests have no requirements in them:** "I want a calendar in Basecamp" names an f() with no x or y. You do not know what to build.
- **Detective work on the current function:** Ask what they use today (a calendar painted on the wall), and what situation made it fail (she got a client call while away from the office and could not see room bookings).
- **Solve for f():** With y = "See room availability when I'm away from the office", the problem becomes resource scheduling, not "calendar". That opened booking-style options and led to the Dot Grid: dots on a month grid, click a day to see events. 10x faster and cheaper than any full calendar concept.
- **Better or worse = compare outputs:** Judge a design by comparing its y to the status quo's y. Designers often compare "up" to an ideal that is never reached instead of "down" to the baseline.
- **Time and causality:** Customers decide in situations to achieve outcomes, not on likes and dislikes. Think about what happens before and after use. This counters design by fashion and personal taste.
- **Value is the difference in outcome:** (from the article's final diagram alt text) value is the gap between the old y and the new y.

## Strong quotes
> "Products are easier to reason about when you think of them as functions. They transform an input situation into an output situation."

> "The designer doesn't get to define x: that's empirical. And they don't get to dictate y either. A given y is only a worthwhile target if it's worth paying for in the eyes of the user — also empirical."

> "Most designers set requirements for f() by describing what f() should be, which is a circularity."

> "Very often designers are comparing "up" to an ideal solution (which is never reached), rather than "down" to the status quo."

> "Customers make decisions in situations to achieve outcomes, rather than purely based on likes and dislikes."

## Questions this source makes you ask about an idea
**Defining x (the starting situation)**
- Describe the customer's situation right before they would use your product. Where are they, what just happened, what are they trying to do?
- What do they use today to handle this? Name the actual tool or workaround (email, a spreadsheet, a wall calendar, a person).
- When exactly does that current tool break down? Describe one real moment when it failed someone.
- How do you know this x exists? Did you observe it, or did you imagine it?

**Defining y (the outcome)**
- What is different in the customer's situation after using your product? Say it in their words, not in feature terms.
- Would they pay to get from their current y to your y? How do you know?
- If your product is "team collaboration" or "productivity", what is the precise before/after it produces instead?

**Solving for f()**
- Is your product idea a requirement, or is it a solution someone asked for ("I want a calendar")? What is the x and y behind that request?
- Now that you know x and y, what are three completely different f()s that could produce the same y? Is your idea the cheapest?
- What is your "Dot Grid": the stripped-down version that produces the same y at a tenth of the cost?
- Does your spec describe what the product should be, or what outcome it must produce? Could you test a design against it without knowing the design?

**Judging better or worse**
- Compared to the status quo (not to your ideal), how much better is the outcome? Can you show the difference?
- If you put the old tool and your product side by side in the same x, what does each produce?
- Which parts of your design come from taste or fashion, and which come from a specific outcome the user needs?

## Red flags / failure modes
- The idea is described as a category or feature bundle ("an AI calendar", "a collaboration tool") with no before/after situation.
- Requirements are written as a description of the solution, so there is no way to test if a design fits.
- The founder takes a customer feature request at face value and builds it, without asking what situation broke and what outcome they want.
- Success is judged against an imagined perfect product, not against what people use today.
- Design debates are about what is "good" in the abstract or what is trendy, not about the outcome in a specific situation.
- No cheaper alternative f() was considered once x and y were known.
