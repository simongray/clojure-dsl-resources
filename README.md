Clojure DSL resources
=====================
This is a curated list of mostly mature and/or actively developed Clojure resources relevant for dealing with domain-specific languages, in particular parsing and data transformation with/of DSLs. The list is currently being expanded as I explore this area more thoroughly. Suggestions are welcome in the form of pull requests or Github issues. I try to steer around abandonware, though.

> If you're interested in graphs and data modelling, be sure to check out [clojure-graph-resources](https://github.com/simongray/clojure-graph-resources) too.

Domain-specific languages
-------------------------
Lisp dialects traditionally make heavy use of macros to rewrite source code at compile time, opening the DSL floodgates. Somewhat unique to Clojure is a strong emphasis on using the core data literals to form DSLs. In either case, a supposed DSL could just as easily be considered a creative use of existing language features or a particularly well-designed API.

### Data-based DSLs
* [weavejester/hiccup](https://github.com/weavejester/hiccup): Hiccup is a library for representing HTML in Clojure.
  - [lambdaisland/hiccup](https://github.com/lambdaisland/hiccup): Enlive-backed Hiccup implementation; behaves closer to how Hiccup works in Reagent.
* [noprompt/garden](https://github.com/noprompt/garden): Garden is a library for rendering CSS in Clojure and ClojureScript.
* [BrianChevalier/radiant](https://github.com/BrianChevalier/radiant): Write full featured CSS as Clojure data structures, inline.
* [stathissideris/dali](https://github.com/stathissideris/dali): Build SVG graphics using a Hiccup-like DSL.
* [cgrand/enlive](https://github.com/cgrand/enlive): A selector-based (à la CSS) templating and transformation system for Clojure.
* [seancorfield/honeysql](https://github.com/seancorfield/honeysql): SQL as Clojure data structures.
* [yetanalytics/flint](https://github.com/yetanalytics/flint): A Clojure(Script) DSL for creating SPARQL query and update strings.
* [cljfx/cljfx](https://github.com/cljfx/cljfx): Declarative, functional, extensible wrapper of JavaFX inspired by the better parts of react and re-frame
* [lambdaisland/regal](https://github.com/lambdaisland/regal): Regal lets you manipulate regular expressions as data.
* [AbhinavOmprakash/luna](https://github.com/AbhinavOmprakash/luna): Wield the power of regex with the readability of English.
* [riverford/datagrep](https://github.com/riverford/datagrep): grep for data, for quick and dirty filtering at the repl.
* [QikLiang/GraphQL-format.clj](https://github.com/QikLiang/GraphQL-format.clj): For building GraphQL queries and transforming the output data in a declaritive format in the style of [Meander](https://github.com/noprompt/meander).
* [plumatic/schema](https://github.com/plumatic/schema): A Clojure(Script) library for declarative data description and validation.
* [metosin/malli](https://github.com/metosin/malli): Data-driven Schemas for Clojure/Script.
* [green-coder/minimallist](https://github.com/green-coder/minimallist): A minimalist data driven data model library, inspired by Clojure Spec and Malli.
* [kwrooijen/gungnir](https://github.com/kwrooijen/gungnir): A fully featured, data-driven database library for Clojure.
* [oakes/edna](https://github.com/oakes/edna): A Clojure library for making music with edn data.
* [oakes/odoyle-rules](https://github.com/oakes/odoyle-rules): A rules engine for Clojure and ClojureScript.
  - [oakes/odoyle-rum](https://github.com/oakes/odoyle-rum): What if we used a rules engine to manage all the state of a frontend UI? Can a rules engine replace reframe?
* [frankiesardo/minikusari](https://github.com/frankiesardo/minikusari): minikusari is a minimal rule engine built on top of Datascript (and can work with Datomic or Datahike).
* [yonatane/bytegeist](https://github.com/yonatane/bytegeist): Define binary encoding using plain data.
* [zen-lang/zen](https://github.com/zen-lang/zen): Zen is a framework to unify Data DSLs, make them composable and take model driven design to the next level.
* [sbocq/cronit](https://github.com/sbocq/cronit): A Clojure library to iterate over time points defined by a cron like expression.
* [mauricioszabo/spock](https://github.com/mauricioszabo/spock): Wrappers of SWI and TuProlog in Clojure.
* **datalog**: See the relevant section in [simongray/clojure-graph-resources](https://github.com/simongray/clojure-graph-resources#datalog) for a list of libraries.

### Data matching/transformation DSLs
Most of these could also be considered data-based DSLs, but I think they deserve a category of their own.

* [noprompt/meander](https://github.com/noprompt/meander): A library that empowers you to write transparent data transformation code that allows you to plainly see the input and output of these transformations.
* [juji-io/editscript](https://github.com/juji-io/editscript): A library designed to diff and patch Clojure data structures.
* [disalvjn/faconne](https://github.com/disalvjn/faconne): Data Restructuring DSL.
* [HealthSamurai/ironhide](https://github.com/HealthSamurai/ironhide): A runtime agnostic bidirectional data-driven transformation domain-specific language for fun and profit.
* [escherize/tracks](https://github.com/escherize/tracks): Allows the user to create transformations declaratively.
* [redplanetlabs/specter](https://github.com/redplanetlabs/specter): Specter rejects Clojure's restrictive approach to immutable data structure manipulation, instead exposing an elegant API to allow any sort of manipulation imaginable.
* [xapix-io/matchete](https://github.com/xapix-io/matchete): 
Yet another pattern matching library for Clojure(Script).
* [bsless/impedance](https://github.com/bsless/impedance): Fast, declarative Clojure map transforms to solve impedance mismatch.
* [TristeFigure/derrida](https://github.com/TristeFigure/derrida): Destructuring "Destructuring".

### Traditional Lisp DSLs
* [clojure/core.logic](https://github.com/clojure/core.logic): Offers Prolog-like relational programming, constraint logic programming, and nominal logic programming for Clojure.
* [quil/quil](https://github.com/quil/quil): Clojure/ClojureScript library for creating interactive drawings and animations.
* [overtone/overtone](https://github.com/overtone/overtone): Overtone is an Open Source toolkit for designing synthesizers and collaborating with music.
* [ctford/leipzig](https://github.com/ctford/leipzig): A music composition library for Clojure and Clojurescript.
  - [ctford/klangmeister](https://github.com/ctford/klangmeister): A musical scratchpad. Klangmeister uses Leipzig for all of its music composition.
* [cerner/clara-rules](https://github.com/cerner/clara-rules): Clara is a forward-chaining rules engine written in Clojure(Script) with Java interoperability.
  - [clyfe/clara-eav](https://github.com/clyfe/clara-eav): ClaraEAV is a thin layer over Clara-Rules API that simplifies working with EAV triplets.
* [lspector/Clojush](https://github.com/lspector/Clojush): The Push programming language and the PushGP genetic programming system implemented in Clojure.
* [adam-james-v/svg-clj](https://github.com/adam-james-v/svg-clj): DSL for compiling SVG elements with Clojure(script).
* [google/clojure-turtle](https://github.com/google/clojure-turtle): A Clojure library that implements the Logo programming language in a Clojure context.
* [farrellm/scad-clj](https://github.com/farrellm/scad-clj): OpenSCAD DSL in Clojure.
* [athos/JiSE](https://github.com/athos/JiSE): JiSE is a Clojure DSL library that compiles a Java-like language into JVM bytecode at macroexpansion time.
* [daveyarwood/alda-clj](https://github.com/daveyarwood/alda-clj): A Clojure library for live-coding music with Alda.

### Text-based DSLs
Some DSLs are based on text, but work on Clojure data.

* [clj-holmes/shape-shifter](https://github.com/clj-holmes/shape-shifter): Transforms a string pattern into clojure spec.
* [gga/json-path](https://github.com/gga/json-path): An implementation of the JsonPath spec for Clojure.

Data-oriented configuration
---------------------------
In most Clojure software there is a guiding principle of _data > functions > macros_. It has resulted in a convention of using mostly data structures to configure the behaviour of systems. This practice has also led to frequent repurposing of data structures. In many cases, the repurposing crosses into a grey zone somewhere between a DSL and idiomatic use.

* [pedestal/pedestal](https://github.com/pedestal/pedestal): Pedestal is a set of libraries written in Clojure that aims to bring both the language and its principles to server-side development.
* [metosin/reitit](https://github.com/metosin/reitit): A fast, data-driven router for Clojure(Script).
* [juxt/bidi](https://github.com/juxt/bidi): Bidirectional URI routing.
* [juxt/yada](https://github.com/juxt/yada): Yada is a web library. Whereas bidi is based on routes as data, yada is based on resources as data.

### Honourable mentions
These libraries are not really data-oriented, but can be considered popular mini-DSLs in their own right.

* [weavejester/compojure](https://github.com/weavejester/compojure): Compojure is a small routing library for Ring that allows web applications to be composed of small, independent parts.

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
* [green-coder/html-to-hiccup](https://github.com/green-coder/html-to-hiccup): An html->hiccup conversion function in pure CLJC.
* [yogthos/markdown-clj](https://github.com/yogthos/markdown-clj): A markdown parser that compiles to both Clojure and ClojureScript.
* [askonomm/clarktown](https://github.com/askonomm/clarktown): A zero-dependency Markdown parser.
* [kiranshila/cybermonday](https://github.com/kiranshila/cybermonday): Cybermonday provides a Clojure(Script) interface to working with markdown as a hiccup AST.
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
* [borkdude/sci](https://github.com/borkdude/sci): Configurable Clojure interpreter suitable for scripting and Clojure DSLs.
* [clojure/tools.reader](https://github.com/clojure/tools.reader): A complete Clojure reader and an EDN-only reader.
* [clojure/tools.analyzer](https://github.com/clojure/tools.analyzer): An analyzer for host agnostic Clojure code, written in Clojure and producing AST in EDN.
* [borkdude/edamame](https://github.com/borkdude/edamame): Configurable EDN/Clojure parser with location metadata.
* [clj-commons/rewrite-clj](https://github.com/clj-commons/rewrite-clj): rewrite-clj is a library offering mechanisms to easily rewrite Clojure/EDN documents in a whitespace- and comment-preserving way.
  - [clj-commons/rewrite-cljs](https://github.com/clj-commons/rewrite-cljs): This library is a ClojureScript port of rewrite-clj.
  - [lread/rewrite-cljc-playground](https://github.com/lread/rewrite-cljc-playground): Working towards rewrite-cljc. Still conservatively pre-alpha, will release on clojars after moving to clj-commons.
* [oakes/parinferish](https://github.com/oakes/parinferish): A Clojure and ClojureScript library that parses code and optionally applies parinfer(ish) to it.
  - See [oakes/html-soup](
https://github.com/oakes/html-soup) for an example of a library that uses parinferish as a parser.
* [carocad/parcera](https://github.com/carocad/parcera): Grammar-based Clojure(script) parser.
* [echeran/kalai](https://github.com/echeran/kalai): A source-to-source transpiler to convert Clojure to multiple target languages (Rust, C++, Java, ...).

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
