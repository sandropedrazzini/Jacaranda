The Jacaranda Framework
============
[![GitHub license](https://img.shields.io/badge/license-Apache%202-blue.svg)](https://raw.githubusercontent.com/apache/opennlp/master/LICENSE)

The Jacaranda Framework is a free Java framework realized at the University of Applied Sciences of Southern Switzerland (SUPSI) with the intention to provide an easy and customizable design for the implementation of different finite-state machines (FSM). 
The added value in respect to other implementations is the framework character of the system, which offers different flexible and customizable parts (hot spots) through which the user not only can change, as usual, the content of the finite-state machine updating the input document with different states and arcs relations, but also customize it in different ways, including type of arcs, kind of output, way of traversing, etc., creating its own instance of the desired FSM. The framework has been used as backbone for some commercial systems. 

One of them is the CanooNet German Language Portal, a web-based application for the German language, including a morphological analyzer, a spell checker, a dictionary, and a thesaurus. The system has been recently integrated into Leo.org, the most important German-English dictionary on the web. 

## Documentation

The documentation includes different single documents, as well as the javadoc generated API internal documentation. 

The documents are the following:
- [Brief introduction](./documentation/introduction/introduction.md) to the project in general,  finite-state machines and motivations for the framework.
- Framework architecture overview, with some insides into the implementation
- How to write an application. Cookbook for the application developer, including the explanations of two different delivered applications.
- How to use an application. Quick guide for the application user, i.e. the user who needs to embed a Jacaranda application within its own application code.
- Advanced features of the framework. Explanations on how the application developer can extend some functionalities of the framework.
- For test infected only. A brief explanation on how the tests have been conceived and how they can be extended.
- References. A list of references used for the design and implementation of the system, not cited in the rest of the documentation.
- [The Jacaranda Picture Show](./documentation/show/show.md). An informal explanation of the "shaken Jacaranda" algorithm.
                           
## The Framework Name

The name of the framework, Jacaranda, comes from the name of the impressing trees that I had the chance to admire every day on the streets of Pretoria, South Africa, during my two months sabbatical period around October 2000 at the local university, where I had the opportunity to design and implement the software.
    
![alt text](./documentation/show/images/overview.JPEG "Overview")

The Jacaranda tree is originally native of South America, specifically Argentina. The botanical name is Jacaranda mimosifolia of the family Bignoniaceae. The tree has adapted well to the warmer parts of southern Africa and today the main concentrations are in the region around Pretoria and Johannesburg.
Although the Jacaranda tree is not indigenous to South Africa, it has become synonymous with Pretoria so that the city is often referred to as the Jacaranda city. The large number of Jacarandas along the streets of Pretoria burst into lilac every October, turning the city into a spectacle that defies description.

Jacaranda is also the name of the radio channel (FM 94.2) I was used to hear during breakfast time in Pretoria (I like such kinds of routines...).

The algorithm that I use to prepare the input data for the framework starts from the bottom of a trie structure, i.e. a particular tree structure, removing every redundant node, when possible, and reducing the trie structure into a finite-state machine structure. I developed the algorithm some years ago and I called it "shaken trie", because of its characteristic of making the leaves of the trie falling down during the process of shaking. The similarity goes well with a shaken Jacaranda losing blooms in October.
But I am not only romantic. As a matter of fact the framework has been fully implemented in Java, and the first "J" of Jacaranda is there to confirm it...
