Programming languages
=====================

Context and Problem Statement
-----------------------------
There are many programming languages, or combinations of programming languages, that could be chosen to implement this application. Front-end, back-end, training, future development, feature availability, speed and support – all characteristics of programming languages that make this decision one of the most significant.

Considered Options
------------------
C++, Javascript, Java, Python, Ruby, Rust, Typescript were all considered options for reasons including JFS has experience using these languages or JFS developers think new languages could present a viable and beneficial opportunity for our tool.

Decision
--------
While JFS developers have some experience with C++, it is dated and its features can be performed by other languages that have additional benefits.
Java: is a very good language with a lot of industry experience and capabilities but industry appears to be moving on (first it was onto python, now several others as well). 
JFS developers have plenty of experience with Javascript, as does the industry. It is a very common language that is sure to be more than capable but is losing industry support.
Python has been gaining popularity, especially in administrative applications. However for unknown reasons, it has been abandoned by some larger systems.
JFS developers have limited Ruby experience but have reported positives in terms ongoing support. However, it is also reported that Ruby can be slow but it is not clear how significant of a downside that is for this application.
JFS developers have no experience with Rust but continue to propose it as the language of the future. Reported benefits are performance comparable to C++, while maintaining firm memory control and interaction with a developer-loved packager, Cargo. Rust also is easily suitable for multiple platforms as it compiles to native machine code.
Typescript is another new language that JFS developers have no experience with but continue to report as a language of the future. Essentially, it is explained as a Javascript replacement but with better features. Additionally, there appears to be support for porting directly from Javascript to Typescript. A link is apparent in that Typescript seems to be gaining popularity in an inversely proportional rate that Javascript is losing popularity.
The decision has been made to prioritize longevity without the need to retool to a new language and runtime over compile time. Therefore, the JFS healthcare tool will utilize Typescript for a front-end language and Rust on the back-end of the architecture. 

Consequences
------------
Using two new languages will mean significant learning curves for the JFS developers, as well as training expenses. However, this investment is an up-front, one-time cost. The slow compiles times are acceptable when providing better runtime performance. A fast customer experience is prioritized over the JFS developer experience during project integration. Support for both languages is an unknown during initial product stages. However, this is projected to improve over time as the language becomes more seasoned and communities expand. Initial development is expected to greatly assisted by the direct porting of Javascript to Typescript. If necessary, JFS developers could even code in Javascript and utilize this coding function. 
