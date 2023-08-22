# Code Reviews

[The Secret Society of Code Reviewers at Microsoft](https://www.youtube.com/watch?v=MLU8AwfIe8U)

> Today, his focus is less on scrutinizing individual lines of code and more on assessing the performance, efficiency and identifying issues like cross-team and cross-group dependencies.

## Purpose of a code review

- Track the application state through the app
- Proper code review speed: ~200-400 lines of code per hour
- Code reviewer:
  - Devil’s advocate, but not an adversary.
  - Deeper knowledge of code section than you so that you can learn. Security expert for security concerns, a11y advocate for accessibility concerns, etc.

## How to code review

- Find defects - Find bugs in a quick inspection pass
  - Performance
  - Security
  - Backwards compatibility
- Code Quality - Follow style guide. If not in style guide, follow precedent set in code. To change that, create ADR to get buy-in, fix all instances, then proceed.
  - Maintainability
  - Readability
  - Uniformity
  - Grokability
- Knowledge Transfer
  - Enables new developers to learn the codebase
  - If a picture is worth a thousand words, then an example is worth a million.
  - Learn common solutions, like error handling, and style guide standards
- Mutual Responsibility
  - When people feel they have ownership and authorship, they look after the codebase better.
  - Perfect opportunity for everyone to play “forest ranger” and limit what is allowed to come into your codebase, and what is allowed to stay.
  - As the code reviewer, you are the gatekeeper. You let it in. As the responsible party, if a bug is introduced, you are equally responsible for fixing it.
  - From Dave’s experience, he felt more comfortable with a code change based more on who reviewed it than who wrote it.
- Misc
  - Generating new ideas for patents
  - generating ideas for new products or solutions that transcend the specific code being reviewed.
  - Collaborative and quality benefits of pair programming at the finalization where more minds are better than one.

## How NOT to code review

- No nit-picking: Do not debate the style guide in a code review
- Ping Pong
  - Iterative code review where it goes back and forth between the reviewer and author.
  - If it takes multiple passes to get it right, someone isn’t paying attention.
  - Pair on it, or table it until issues have been addressed.
- Inconsistency
  - If one code reviewer covers performance, and the other covers robustness, neither one is giving you a comprehensive review
- Design changes at review time: Just no.
- Ghosting
  - Code reviews should be the highest priority; must be seen as time well spent and not as an interruption or an intrusion.
  - Completing a code review frees up multiple devs, not just the author
  - Keep MRs small, a few pages at most, to enable a thorough review and to avoid having other devs ghost your MR.
  - “Throwing a fat code manifesto over the wall and expecting a quick answer isn’t fair”

## Additional links and resources

[5 Traits of a Bad Code Reviewer](https://medium.com/@ms_lizzie/5-traits-of-a-bad-code-reviewer-598da8e6dc19)

When doing a code review, check both technical implementation and code’s compliance with requirements. Be attentive, as you are responsible for your review. Don’t waste time arguing about best practices — there are more opinions than one. Consider current project status and suggest massive changes only if there is time to make them. And of course, always be polite.

[Code Review Guidelines | GitLab](https://docs.gitlab.com/ee/development/code_review.html#acceptance-checklist)

This guide contains advice and best practices for performing a code review, and having your code reviewed.
