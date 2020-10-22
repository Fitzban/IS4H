# IS4H


In this project we would like to present the aim to generate an application
which could be able to support an user to threat spatial referred informations.
In this context we could sum up the basic operations in:
• the possibility to insert new informations in the application whit the ability to
maintain the spatial disposition oh themselves,
• the possibility to recover informations making queries in an formal
language,
• the possibility to take advantage of inferential mechanisms to increase
contained knowledge.

In order to approach to every person who is not familiar with computer,
we researched a way to allow an user to execute tasks previously listed in a
simply and intuitive way.

The first question that rise spontaneous is how it could absolve this task,
on which existents theories it was possible to build and wich techniques it was
possible to use. The first step consists of find that technique able to give us the
capability to increase knowledge by adding new truths, moreover it was required
to have strong theoretical basis.

In order to maintain spatial reference, it was adopted a spatial model that
allow us to represent an abstraction of reality, a spatial model contain that
worlds in witch interesting informations was truth.
To maintain spatial disposition of the contained worlds, it was important
to have in the model a set of commonsense spatial relations between couple of
contained worlds, these relations allow us to order worlds with respect to fixed
external referent point.

In order to recognise contained modality, it was important to have a third
set of label, these labels it will be used to identify one modality linked on it.
In works like “Representation, Reasoning, and Relational Structures: a
Hybrid Logic Manifesto”, Patrick Blackburn, is presented a relational structure
called Kripke “ possible worlds” and in “Commonsense Spatial Reasoning For
Context-Aware Pervasive Systems”, Stefania Bandini, Alessandro Mosca,
Matteo Palmonari, Department of Computer Science, Systems and
Communication (DISCo) University of Milan Bicocca, is defined a
commonsense spatial model like:
A commonsense spatial model CSM = <P,R> is a relational structure,
where P = {p1, ..., pi} is a finite set of places, and R = {R1, ...,Rn} is a finite nonempty
set of binary conceptual spatial relations, labeled by means of a set of labels N.
Having a model implies necessity to have a formal language that allow us
to talk about the model, from the introduction of commonsense spatial model
like a relational structure become natural to consider the model like a semantic
specification for a modal language.

A great goal in the context of logical research with the aim to create
formal language was obtained trough the creation of hybrid logic, whose
language is adopted in this work. Hybrid logic allow us to refer directly to a
world by naming it whit a nominal symbol, directly in the language it was
encapsulated this functionality by giving the rule that the nominal symbol is
truth on one and only one world of the model.

With the introduction of the so-called “satisfaction operator” @, it
becomes possible to reasoning globally on the universe of places.
It is possible to subdivide commonsense spatial relations in three classes
by their sets formal properties. Orientation relations are transitive, asymmetric
and irreflexive, and whit this kind of relations it is possible to obtain a partial
order on worlds in respect to an external fixed point( i.e., Geographic North and
East respectively for the relation “to be at north of” and “to be at east of”);
containment relations are irreflexive and antisymmetric and permit us to have a
granularity of the world; proximity relations are symmetric and reflexive and
they could be used for reason about the worlds reachability.

Taking advantage on formal properties valid on a relation, it is possible to
implement automatic procedures able to increase the knowledge in one model,
in this way it was possible to reach the first goal of the work.

In order to extract informations from the model using language of the
hybrid logic, it was decided to integrate HLMC software into our application,
HLMC is a software that allow us to know, given a model completely expressed
in an xml file and an hybrid formula expressed in an hlf file, on witch worlds the
given formula is valid.

Manual creation of xml file was not simple especially for big models, to
make it simple it was automatized by the creation of an object able to write an
appropriate xml file for HLMC software creating a model and writing a formula.
The inference engine is able to generate the correct files and to call an HLMC
wrapper able to send results of model checking to the user.

All these features were accessible by a graphical interface that is allow to
get an user friendly use of the application, in fact with simple clicks is possible
to create, complete and check a spatial model.

IS4H was presented in spatial context, however by defining personal
relations is possible to use this application in all of the context in witch modal
logic is used, removing the constraint given by modal label set permit the use of
IS4H in non modal logics.

The architecture of the application was studied in order to permit the
substitution of the use of the graphical interface to put informations whit the use
of interfaces with spatial database (GIS) or distributed sensor (context-aware
application.
