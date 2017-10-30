# Typelevel Search Engine Optimisation with Idris - @janschultecom

Talk description:
> Programming languages with dependent types like Idris, Agda or Coq are usually put into the context of safety & security, where they are used for theorem-proving in order to avoid disastrous bugs. The increased complexity and effort is undeniably justified by the risk of human lives. But having a strong type-system may also be useful in other situations, e.g. where high revenue is at stake. One such use-case is search engine optimisation (SEO). Flaws in SEO can easily affect the page rankings and take weeks or months to correct, consequently causing high revenue losses. In a proof of concept we'll see how Google's SEO guidelines for URLs could be encoded using the Idris type system and thereby force the developer to do the right thing from a SEO point of view

Main goal:
> 

Intro:
  * What is SEO
    * Rule 1: Simple to understand URLs
    * Rule 2: Avoid having deep nesting directory URLs
    * Rule 3: Complete directory structure
  * Avoid SEO problems is hard
  * Proof of concept using dependent types in Idris
  

## Building a routing DSL in Idris

  * Routing DSL
    * Examples from Spring & Play
    * Idris routing DSL similar to play
    * If follow SEO compliance must compiles, not else.
    
- Idris introduction
- Live coding: Building the Routing DSL in Idris
  * Kinda TDD with proofs
  * All is a type and yo proof types
  * Proofs are the Idris tests
  * You enter idris in console and then :e and enters inside the Idris Editor (vim)

