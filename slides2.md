---
marp: true
paginate: true
theme: default
---

# Clojure as Your First Language: Shaping a Functional Mindset

# Wendy Randolph

 Dutch Clojure Days 2026
 Amsterdam, Netherlands

---
## Act I : An Unusual Start <!-- (10 min) -->
What Happened
<!-- FRAMING: what happened (events, experience, feelings — your story) -->

<!-- Who here wants to get real technical? ok, Clojure wasn't TECHNICALLY my first programming language. we'll get to that soon enough. ok. so, how did I get here? Before software, there was... -->
- Creative arts; programming was a different kind of hard
<!--
- "you know what you are working with, you can hold them in your hands... the systems are in front of your eyeballs"
- I want to switch careers, become a software developer, Can I build abstract things?
- Make an app > mobile app? > Swift, I guess
 -->
- Started with a puzzle game, not a technical book
<!-- Started with Swift playgrounds, no editor yet, no language docs, no programming theory yet, just make the dude turn around, get gems, start / stop loops
- this is where I first felt the burn of not breaking down problems small enough
- first learned value of taking breaks, from trying to stop a loop... -->
- Deliberate Pivot to Clojure
<!--
- on a recommendation to get to my app goal faster, I started looking into Clojurescript and Clojure, seemed more multi-purpose, beyond "apps"
- breaks: "laying on the floor... listening to the sweet sound of Rich Hickey and Stu Halloway talking about thinking deeply" - not understanding why i need to be thinking so deeply about things - i was working on memorizing basic core functions and writing them correctly - didnt get it all but kept at it
- nevertheless, the thoughtfulness of language leaders drew me in even before I understood the broad concepts or ecosystem of the language
-->
- Community & Resources
<!-- "picked up Learn ClojureScript... clojuredocs.org... Clojure for the Brave and True... Clojure Koans... looking to share my gratitude and enthusiasm, reaching out to Daniel H and Jordan M to thank them for their contributions, they eventually cofound Clojure Camp... this gave me accountability every week for learning, as well as opportunity to shape the operations with my unique perspective" -->
    - counter arg: not everyone has same inclination or access to community
 <!-- Claim: community kept you going → Not every beginner has access to a Clojure Camp, a Strange Loop, a Carol Silva. The community that supported you may not be replicable for someone learning alone. -->
- Early Struggles <!-- (~2 min) -->
<!--
- my biggest hurdles - not clojure-specific.
- counter-arg: so let me argue a point you may think i am making: blank slate = advantage
- it can be a blessing and a curse - No prior experience also means no intuition to fall back on. most engineers ive met have cut their teeth on other languages; growing pains were 'back there'
— but im going thru it when I adopted clojure:
    - short version: "becoming overwhelmed... didn't break it down small enough... didn't even know what 'it' was called"
    - or "becoming overwhelmed with problem bc i was trying to do too much." The blank slate cuts both ways.
    - long version:
        - becoming overhwhelmed with problem bc i was trying to do too much - didnt break it down small enough - how do i break it down? guess i should have thought more deeply
        - what is the abstraction I am struggling with? what is abstraction? twas not a great googler. how do i express what i am having trouble with when I don't even know what "it" is called? e.g., how can i make the app i built available for people to use on the internet - what is that called?
-->
- "More often than not, people thought I dove into the deep end" <!-- (~1 min) -->
<!-- (plant this seed in Act I, pay it off in Act II or III)
- motivation in writing this talk, do people not recommend Clojure as a first programming language? do people recommend "easier" language as a first one?
- poll results surprised me - high % would recommend Clj as 1st language
-->

---

## Act II : The Features That Made It Possible <!-- (10 min) -->
What kept me going
<!--
FRAMING: what kept me going (the specific Clojure features that made it survivable as a beginner: minimal syntax, immutability, purity, REPL)

ANSWERS: "what does this feature do and why did it help me survive?"

"not just a functional language, not just a lisp — our powers combined!"
-->
### Minimal Syntax
<!-- (~2 min) -->
- narrower focus on problem at hand
<!-- without concern of mutations, side effects, types, operations, classes, procedures, objects, ceremony, boilerplate -->
- forces you to express logic concisely
<!-- example -->
- less overhead compared to other (more popular first) languages
<!-- what are other popular first languages? -->
<!-- Winter weather analogy - ralphie from christmas story -->
- counter arg: no visual landmarks
<!-- Claim: minimal syntax → narrower focus on the problem → When everything looks structurally identical (uniform list syntax), there are no visual landmarks. Beginners often rely on visual differentiation to parse what they're reading — Clojure removes that scaffold. (is that true? what about structural editing? could that apply here as a counter to the counter? put it in your own words) -->

### Immutability
<!-- (~2.5 min) -->
- simpler reasoning than reasoning thru when things change in place / state / mutations
<!-- why immutability specifically helps a beginner — mechanics -->
- in other words, leads to simpler, more predictable code, which makes problem-solving easier. don’t have to worry about things changing unexpectedly.
-  write a change-tree function. "that intitial tree is still a magnolia tree"
- counter arg: what about handling real changes?
<!-- Claim: immutability → simpler reasoning → When something genuinely needs to change, beginners may not yet have the vocabulary or patterns to handle it. Immutability defers that complexity — it doesn't eliminate it. (is that true? put it in your own words) -->

---
### Purity
<!-- (~2 min) -->
- predictable behavior, fewer surprises, no side effects
- what you get: can make your code easier to understand, test, and debug
- counter arg: what about when you need to interact with the outside world?
<!-- Claim: purity → predictable behavior, fewer surprises → A beginner working purely in pure functions may struggle when they inevitably need to interact with the outside world — files, databases, APIs. Side effects don't disappear, they just get deferred to the edges. That boundary can be confusing without guidance. (is that true?) -->

### REPL Feedback Loop
<!-- (~2.5 min) -->
- explore problems interactively, one small step at a time, in real time. prove it to yourself
- what the REPL actually does and why it's different from compile-run cycles — mechanics, beginner-specific benefit
-  "eval to comment for everything — what does this evaluate to? what is the shape of my result?"
<!-- concrete REPL habit, specific to you, humanizes the section -->
- "made huge scratch pads — was that weird? it worked for me"
<!-- humor, also a counter argument setup -->
<!-- One way I used my scratch pads: if i figured out some coding problem, explain every piece to myself in english prose as a comment. eval expressions within larger ones to make sure i knew what i was doing. -->
- claim: accelerates learning, encourages experimention
- counter arg: exploratory repl habits can work against building structured software
<!-- Claim: REPL accelerates learning → Exploratory REPL habits can work against building structured software. "Try stuff until it works" is a real risk — and your own note about "made huge scratch pads to test ideas — was that weird?" touches this. It worked for you, but it's worth naming. (is that true?) "I spent a while in my scratchpad. I wasn't sure how to structure a project repo when I thought its probably time I build something already. -->

---

## Act III : What Remains, or The Mindset that Stayed <!-- (10 min) -->
What Stuck
<!--
FRAMING: what stuck (the habits, the transfer, the lasting mindset)

ANSWERS: what thinking habits did those features leave behind?

consider the "what programming teaches you / what functional programming teaches you / what Clojure teaches you" → consider as the internal logic organizing Act III's sub-sections...
-->
- "more often than not, people thought I dove into the deep end" <!-- if planted in Act I, pay it off here: they were right, and here's what I got from it -->
- "naming your problem / work on a problem statement that is true" <!-- (~2 min) -->
<!-- principle of simplicity — what are we DOING? - spreadsheet, IMMUTABILITY INFLUENCE, What state are we in? Robert responding "Florida" :| -->
- "I still think in small feedback loops"
 <!-- REPL: the habit that transferred -->
- "thinking in increments — what do I have? what do I need? what would it take to get there?" <!-- (~2 min) -->
<!-- "what do I have, what do I need" — immutability's influence on how you now think, what is the state of the world right now, thats true now. -->
- Composability as a named transferable habit <!-- (~1.5 min) -->
- "what you avoid — what I don't even have to deal with" — reframed as a gift <!-- (~1.5 min) -->
<!-- type systems, mutability, procedures" → reframe as a gift Clojure gave you: protected from complexity you didn't need yet -->
- counter arg: Tiny job market.
<!-- Claim: Clojure as a deliberate, worthwhile first choice. If someone's goal is employment quickly, starting with Clojure may slow that path. Python or JavaScript get people hired faster. (is that true for those languages) -->
- counter arg: some habits harder to apply in languages that don't support or encourage them
<!-- Claim: these habits transfer to any language → Some of these habits are harder to apply in languages that don't support or encourage them. Immutable-first thinking in a mutable-by-default language requires swimming upstream — it's possible, but not frictionless. (is that true? like what?) -->
- "oh my gosh, clojure is so hard. is it? isn't programming just hard?"
<!-- Claim: "isn't programming just hard?" → This is your own counter argument and it's your strongest one. Worth keeping exactly as you wrote it. -->
- Closing argument: sets you up no matter the language, no matter the problem — "do lots of small things. that makes something big." <!-- (~2 min) -->
<!--  dot matrix throughline made explicit; candidate for your closing line -->