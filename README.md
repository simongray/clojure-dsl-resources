Clojure DSL resources
=====================
This is a curated list of mostly mature and/or actively developed Clojure resources relevant for dealing with domain-specific languages, in particular parsing and data transformation with/of DSLs. The list is currently being expanded as I explore this area more thoroughly. Suggestions are welcome in the form of pull requests or Github issues. I try to steer around abandonware, though.

> If you're interested in graphs and data modelling, be sure to check out [clojure-graph-resources](https://github.com/simongray/clojure-graph-resources) too.

Domain-specific languages
-------------------------
Lisp dialects traditionally make heavy use of macros to rewrite source code at compile time, opening the DSL floodgates. Somewhat unique to Clojure is a strong emphasis on using the core data literals to form DSLs. In either case, a supposed DSL could just as easily be considered a creative use of existing language features or a particularly well-designed API.

### Data-based DSLs
* [weavejester/hiccup](https://github.com/weavejester/hiccup): Hiccup is a library for representing HTML in Clojure.
* [noprompt/garden](https://github.com/noprompt/garden): Garden is a library for rendering CSS in Clojure and ClojureScript.
* [cgrand/enlive](https://github.com/cgrand/enlive): A selector-based (à la CSS) templating and transformation system for Clojure.
* [seancorfield/honeysql](https://github.com/seancorfield/honeysql): SQL as Clojure data structures.
* [lambdaisland/regal](https://github.com/lambdaisland/regal): Regal lets you manipulate regular expressions as data.
* [riverford/datagrep](https://github.com/riverford/datagrep): grep for data, for quick and dirty filtering at the repl.
* [plumatic/schema](https://github.com/plumatic/schema): A Clojure(Script) library for declarative data description and validation.
* [metosin/malli](https://github.com/metosin/malli): Data-driven Schemas for Clojure/Script.
* [oakes/edna](https://github.com/oakes/edna): A Clojure library for making music with edn data.
* [oakes/odoyle-rules](https://github.com/oakes/odoyle-rules): A rules engine for Clojure and ClojureScript.
* **datalog**: See the relevant section in [simongray/clojure-graph-resources](https://github.com/simongray/clojure-graph-resources#datalog) for a list of libraries.

### Traditional Lisp DSLs
* [clojure/core.logic](https://github.com/clojure/core.logic): Offers Prolog-like relational programming, constraint logic programming, and nominal logic programming for Clojure.
* [quil/quil](https://github.com/quil/quil): Clojure/ClojureScript library for creating interactive drawings and animations.
* [overtone/overtone](https://github.com/overtone/overtone): Overtone is an Open Source toolkit for designing synthesizers and collaborating with music.
* [ctford/leipzig](https://github.com/ctford/leipzig): A music composition library for Clojure and Clojurescript.
  - [ctford/klangmeister](https://github.com/ctford/klangmeister): A musical scratchpad. Klangmeister uses Leipzig for all of its music composition.
* [cerner/clara-rules](https://github.com/cerner/clara-rules): Clara is a forward-chaining rules engine written in Clojure(Script) with Java interoperability.

### Text-based DSLs
Some DSLs are implemented in Clojure, but aren't written as Clojure code.

* [alda-lang/alda](https://github.com/alda-lang/alda): Alda is a text-based programming language for music composition.
  - [daveyarwood/alda-clj](https://github.com/daveyarwood/alda-clj): A Clojure library for live-coding music with Alda.

Data transformation
-------------------
These could also be considered data-based DSLs, but I think they deserve a category of their own.

* [noprompt/meander](https://github.com/noprompt/meander): A library that empowers you to write transparent data transformation code that allows you to plainly see the input and output of these transformations.
* [juji-io/editscript](https://github.com/juji-io/editscript): A library designed to diff and patch Clojure data structures.
* [disalvjn/faconne](https://github.com/disalvjn/faconne): Data Restructuring DSL.
* [HealthSamurai/ironhide](https://github.com/HealthSamurai/ironhide): A runtime agnostic bidirectional data-driven transformation domain-specific language for fun and profit.
* [redplanetlabs/specter](https://github.com/redplanetlabs/specter): Specter rejects Clojure's restrictive approach to immutable data structure manipulation, instead exposing an elegant API to allow any sort of manipulation imaginable.

Parsing
-------
* [Engelberg/instaparse](https://github.com/Engelberg/instaparse): Instaparse aims to be the simplest way to build parsers in Clojure.
* [aphyr/clj-antlr](https://github.com/aphyr/clj-antlr): Clojure bindings for the ANTLR 4 parser library.

### Parser combinators
* [blancas/kern](https://github.com/blancas/kern): A Parser Combinators Library for Clojure.
* [youngnh/parsatron](https://github.com/youngnh/parsatron): Born from Haskell's Parsec library, The Parsatron is a functional parser library.
* [rm-hull/jasentaa](https://github.com/rm-hull/jasentaa): A parser-combinator library for Clojure and ClojureScript.

### Artificial languages
* [davidsantiago/hickory](https://github.com/davidsantiago/hickory): Hickory parses HTML into Clojure data structures, so you can analyze, transform, and output back to HTML.
* [yogthos/markdown-clj](https://github.com/yogthos/markdown-clj): A markdown parser that compiles to both Clojure and ClojureScript.
* [bnbeckwith/orgmode](https://github.com/bnbeckwith/orgmode): A Clojure library designed to parse mode files into clojure data structures.
* [russellwhitaker/uap-clj](https://github.com/russellwhitaker/uap-clj): A Clojure library for extracting browser, operating system, and device information from a raw useragent string.
* [alumbra/alumbra.parser](https://github.com/alumbra/alumbra.parser): An ANTLR4-based GraphQL parser for Clojure.
* [igrishaev/remus](https://github.com/igrishaev/remus): An attentive RSS and Atom feed parser for Clojure. It's built on top of well-known and powerful ROME Tools Java library.
* [zsau/rome-clj](https://github.com/zsau/rome-clj): rome-clj is a Clojure wrapper for ROME, a Java RSS/Atom feed parsing library.
* [zsau/id3](https://github.com/zsau/id3): A simple ID3v2 parser, written in Clojure.
* [l3nz/cli-matic](https://github.com/l3nz/cli-matic): Compact, hands-free [sub]command line parsing library for Clojure.
* [smee/binary](https://github.com/smee/binary): This library is a high performance binary parser combinator.

### Natural languages
Not _technically_ DSLs, but included here to complete the parsing section.

* [simongray/datalinguist](https://github.com/simongray/datalinguist): A Clojure wrapper for Stanford CoreNLP.
* [plandes/clj-nlp-parse](https://github.com/plandes/clj-nlp-parse): A generalized library to deal with natural language.
* [turbopape/postagga](https://github.com/turbopape/postagga): A Library to parse natural language in pure Clojure and ClojureScript. 
* [ekoontz/menard](https://github.com/ekoontz/menard): A Clojure library for generation and parsing expressions from grammars and lexicons.

### Clojure code
* [clj-commons/rewrite-clj](https://github.com/clj-commons/rewrite-clj): rewrite-clj is a library offering mechanisms to easily rewrite Clojure/EDN documents in a whitespace- and comment-preserving way.
  - [clj-commons/rewrite-cljs](https://github.com/clj-commons/rewrite-cljs): This library is a ClojureScript port of rewrite-clj.
  - [lread/rewrite-cljc-playground](https://github.com/lread/rewrite-cljc-playground): Working towards rewrite-cljc. Still conservatively pre-alpha, will release on clojars after moving to clj-commons.
* [oakes/parinferish](https://github.com/oakes/parinferish): A Clojure and ClojureScript library that parses code and optionally applies parinfer(ish) to it.
  - See [oakes/html-soup](
https://github.com/oakes/html-soup) for an example of a library that uses parinferish as a parser.
* [carocad/parcera](https://github.com/carocad/parcera): Grammar-based Clojure(script) parser.

Miscellaneous
-------------
* [clojure/spec.alpha](https://github.com/clojure/spec.alpha): The spec library specifies the structure of data, validates or conforms it, and can generate data based on the spec.
  - [clojure/spec-alpha2](https://github.com/clojure/spec-alpha2):  This library is an evolution from spec.alpha as well as work towards several new features.
* [jkk/formative](https://github.com/jkk/formative): Web forms for Clojure and ClojureScript - rendering, parsing, and validating.
* [agentbellnorm/dativity](https://github.com/agentbellnorm/dativity): Dativity is a stateless, data driven workflow engine library for Clojure and ClojureScript.
* [clojure-lsp/clojure-lsp](https://github.com/clojure-lsp/clojure-lsp): A Language Server for Clojure. Taking a Cursive-like approach of statically analyzing code.

Articles/videos
---------------
* [Growing a DSL with Clojure](http://clojure-doc.org/articles/tutorials/growing_a_dsl_with_clojure.html)
* [Parsing XML in Clojure](http://clojure-doc.org/articles/tutorials/parsing_xml_with_zippers.html)
* [Clojure Macros and Metaprogramming](http://clojure-doc.org/articles/language/macros.html)
* [The Art of Tree Shaping with Clojure Zippers](https://lambdaisland.com/blog/2018-11-26-art-tree-shaping-clojure-zip)
* [Building trees with and without zippers](https://vincent.404.taipei/clojure/building-trees-with-and-without-zippers/)
* [Writing Parser Combinator Library in Clojure](http://troydm.github.io/blog/2016/04/11/writing-parser-combinator-library-in-clojure/)
* [Constructing Clojure private DSLs on top of functions and function combinators](https://gist.github.com/TristeFigure/20dd01b0d3415f34075cfc02a1918106)

Community
---------
* [Clojurians Slack](https://clojurians.slack.com/messages): Where Clojure's most active users seem to hang out.
  - [#parsers](https://clojurians.slack.com/archives/C01BMKFSL14)
