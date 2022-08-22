<p align="center">
  <br>
  <img width="400" src="./assets/robot-awesome.svg" alt="logo of awesome-fsm repository">
  <br>
  <br>
</p>

## Awesome Finite State Machines

A curated list of awesome resources related to finite state machines and statecharts. 

The main idea of this repository is to have a nice place when people can rely on nice quality content, such as articles, videos, ebooks, documents, books, etc. A little different from the other awesome type lists that we can find in GitHub about a variety of topics, the idea of this list is to provide a nice and short explanation about concepts first, then show a list of nice content related to that specific concept.

Any comments or suggestions about nice quality content that should be in this repository, please open an issue. 

## Contents

- [Introduction](#introduction)
- [Concepts](#concepts)
	- [Deterministic Finite Automatons (DFAs)](#deterministic-finite-automatons(dfas))
	- [Non-deterministic Finite Automatons (NFAs)](#non-deterministic-finite-automatons(nfas))
	- [Mealy Machines](#mealy-machine)
	- [Moore Machines](#moore-machine)
- [Statecharts](#statecharts)
- [Libraries](#libraries)
	 - [JavaScript](#javascript)
	 - [Java](#java)
	 - [Python](#python)
	 - [Ruby](#ruby)
	 - [Go](#go)
	 - [C++](#c++)

## Introduction

You might have not heard the term "finite state machines" before, but humanity has been using this concept every day for a long time. Not only in the programming world, but in real life too, we have a lot of systems that rely upon the concept of finite state machines.

Finite state machines are a computation model, it consists of a machine with a finite number of states. A finite state machine has a finite number of events, to move from one state to another we have something called transitions. These transitions are triggered after a specific event, each transition expects an input, after its triggered, it will change to a specific state depending on the current state and the event.

We can simplify a finite state machine in 4 parts: 

1. A finite number of states.
2. A finite number of events.
3. An initial state.
4. A transition will be triggered after a specific event and will change to a specific state depending on the current state and the event.

Finite state machines can be used to simulate sequential logic, let's take as an example of a traffic light. 

We know that a traffic light has only 3 possible states: green, yellow, and red. To change from one state to another, we will use it as an input integer representing seconds. When the input is 60, the machine will trigger an event and transition to another state depending on the current state and the event, in our case, the seconds.

<p align="center">
  <img width="400" src="./assets/traffic-light-state-machine-example.png" alt="traffic light finite state machine example">
</p>

We can observe finite state machines not only inside the software development but in our real world as well. You can think about almost anything and use finite state machines for it. By having a finite number of states, it reduces drastically the possibility of having unexpected side-effects in your application, your application will get more consistent, well-written, and maintainable.

### Further Reading

- [Finite-state_machine](https://en.wikipedia.org/wiki/Finite-state_machine)
- [Theory of Computation - Finite State Machines](https://stackabuse.com/theory-of-computation-finite-state-machines/)
- [Finite State Machines](https://www.i-programmer.info/babbages-bag/223-finite-state-machines.html)
- [Elements of Robotics - Finite State Machines](https://link.springer.com/chapter/10.1007/978-3-319-62533-1_4)
- [Finite State Machines](http://www.inf.ufsc.br/~joao.dovicchi/pos-ed/pos/exerc/machines2.pdf)
- [The Rise Of The State Machines](https://www.smashingmagazine.com/2018/01/rise-state-machines/)

## Concepts

In the finite state machine model, we have a few different concepts that it’s very important to learn about. There are two types of finite state machines: deterministic state automaton and non-deterministic state automaton. There are a few differences between those two types. 

A deterministic state automaton is a finite state machine with a  finite number of states and input symbols. A transition is defined in every state for every input symbol. Each input symbol will determine which state the machine will move. A deterministic finite automaton machine can only be in one state at a time, and transition to one state at a time.

A non-deterministic finite automaton has a finite number of states and a finite number of input symbols. In a nondeterministic finite automaton, for each state and input symbol, it can be one or more output states. NFAs can be in one or more states at once.

If you’re wondering, an automaton is the plural of automata. Finite state machines are also known as finite-state automata or finite-state automaton.

### Deterministic Finite Automaton (DFAs)

A deterministic finite automaton finite state machine with a finite number of inputs symbols. For each input symbol, it will determine which state the machine will move.
A deterministic finite automaton machine can only be in one state at a time, and transition to one state at a time.

#### Further Reading

- [Deterministic finite automaton](https://en.wikipedia.org/wiki/Deterministic_finite_automaton)
- [Deterministic Finite Automata (DFAs)](https://lambda.uta.edu/cse5317/notes/node8.html)
- [Deterministic Finite Automata (DFAs)](https://www.cs.uic.edu/~ajayk/c301/CS301-UIC/Lecture-02-DFA.pdf)
- [Deterministic Finite Automata (DFA)](https://www.cs.wcupa.edu/rkline/fcs/dfas.html)
- [Deterministic Finite Automaton](https://www.tutorialspoint.com/automata_theory/deterministic_finite_automaton.htm)
- [Deterministic Finite Automata](http://www.cse.chalmers.se/~coquand/AUTOMATA/o2.pdf)
- [Applications of Deterministic Finite Automata](https://web.cs.ucdavis.edu/~rogaway/classes/120/spring13/eric-dfa.pdf)
- [Deterministic Finite Automata (DFA)](https://cseweb.ucsd.edu/classes/sp15/cse191-e/lec1.html)

### Non-deterministic Finite Automaton (NFAs)

A nondeterministic finite automaton has a finite number of states and a finite number of input symbols. In a nondeterministic finite automaton, for each state and input symbol, it can be one or more output states. NFAs can be in one or more states at once.

#### Further Reading

- [Nondeterministic finite automaton](https://en.wikipedia.org/wiki/Nondeterministic_finite_automaton)
- [Non-deterministic Finite Automata](http://cs.ru.nl/~jrot/TnA2017/lecture3.pdf)
- [Nondeterministic Finite Automata](https://courses.engr.illinois.edu/cs374/sp2017/notes/models/NFAnotes.pdf)
- [Non-deterministic Finite Automaton](https://www.tutorialspoint.com/automata_theory/non_deterministic_finite_automaton.htm)
- [Nondeterministic finite automata](https://cs.uwaterloo.ca/~watrous/CS360/Lectures/03.pdf)
- [Nondeterministic Finite Automata](http://people.seas.harvard.edu/~cs125/fall16/lec12.pdf)
- [Non-deterministic Finite State Machines](http://www.inf.ed.ac.uk/teaching/courses/inf1/cl/notes/Comp3.pdf)
- [Nondeterministic Finite Automata](https://people.cs.clemson.edu/~goddard/texts/theoryOfComputation/3a.pdf)
- [NFA (Non-Deterministic finite automata)](https://www.javatpoint.com/non-deterministic-finite-automata)

### Mealy Machine

A mealy machine is a machine where the output value is determined by the input and the current state. For each input and state in a Mealy machine, one transition is possible.

#### Further Reading

- [Mealy machine](https://en.wikipedia.org/wiki/Mealy_machine)
- [Mealy Machine](https://www.javatpoint.com/automata-mealy-machine)
- [Mealy machine](https://ncatlab.org/nlab/show/Mealy+machine)
- [Mealy machine](https://xlinux.nist.gov/dads/HTML/mealyMachine.html)
- [Mealy state machine](https://www.slideshare.net/arifsiyal7/mealy-state-machine)
- [Inferring Mealy Machines](https://link.springer.com/chapter/10.1007/978-3-642-05089-3_14)
- [Moore and Mealy Machines](https://www.tutorialspoint.com/automata_theory/moore_and_mealy_machines.htm)
- [Mealy and Moore Machines in TOC](https://www.geeksforgeeks.org/mealy-and-moore-machines-in-toc/)

### Moore Machine

A Moore machine is a machine where the output is determined by only its current state. The output depends only on the present state and it's the same output every time the machine enters that state.

#### Further Reading

- [Moore machine](https://en.wikipedia.org/wiki/Moore_machine)
- [Moore Machine](https://www.javatpoint.com/automata-moore-machine)
- [Moore Machine](https://xlinux.nist.gov/dads/HTML/mooreMachine.html)
- [Moore Finite State Machine](https://www.electronics-tutorial.net/finite-state-machines/State-Machine-Fundamentals/Moore-Finite-State-Machine/)
- [Moore and Mealy Machine Design Procedure](http://www2.elo.utfsm.cl/~lsb/elo211/aplicaciones/katz/chapter8/chapter08.doc4.html)

## Statecharts

Sometimes we need something more sophisticated and complex, and that's when a finite state machine cannot help us. 

Statecharts are an extension of traditional finite state machines, the main difference of statecharts is that it can have a hierarchical state, states can contain nested state inside them. The reason for this is simple, not all applications in the world can be described as flat multi numbers of states, sometimes we need to have nested states.

Statecharts also bring us a few extra features such as actions, entry and exit actions, guard conditions, deferred events, etc.

### Further Reading

- [Welcome to Statecharts](https://statecharts.github.io/)
- [Statecharts: A Visual Formalism for Complex Systems](http://www.inf.ed.ac.uk/teaching/courses/seoc/2005_2006/resources/statecharts.pdf)
- [Statecharts](https://help.anylogic.com/index.jsp?topic=%2Fcom.anylogic.help%2Fhtml%2Fstatecharts%2FStatecharts.html)
- [The Statecharts Perspective](http://homepage.cs.uiowa.edu/~fleck/181content/statecharts.pdf)

## Libraries

### JavaScript

* [XState](https://github.com/davidkpiano/xstate)
* [jssm](https://github.com/StoneCypher/jssm) 
* [JavaScript State Machine](https://github.com/jakesgordon/javascript-state-machine)
* [Machina](https://github.com/ifandelse/machina.js)
* [React Automata](https://github.com/MicheleBertoli/react-automata)
* [Robot](https://github.com/matthewp/robot)
* [Stately](https://github.com/fschaefer/Stately.js)
* [Stent](https://github.com/krasimir/stent)
* [fsm-as-promised](https://github.com/vstirbu/fsm-as-promised)
* [redux-machine](https://github.com/mheiber/redux-machine)
* [State Machine](https://github.com/davestewart/javascript-state-machine)
* [redux-dsm](https://github.com/ericelliott/redux-dsm)
* [nanostate](https://github.com/choojs/nanostate)
* [kingly](https://github.com/brucou/kingly)
* [state](https://github.com/steelbreeze/state)
* [finity](https://github.com/nickuraltsev/finity)
* [mood](https://github.com/bredele/mood)
* [maquinaria](https://github.com/tomas2387/maquinaria)
* [Statebot](https://github.com/shuckster/statebot)

### Java

* [squirrel-foundation](https://github.com/hekailiang/squirrel)
* [Spring Statemachine](https://github.com/spring-projects/spring-statemachine)
* [stateless4j](https://github.com/stateless4j/stateless4j)
* [EasyFlow](https://github.com/Beh01der/EasyFlow)
* [StatefulJ](https://github.com/statefulj/statefulj)
* [Easy States](https://github.com/j-easy/easy-states)
* [JState](https://github.com/UnquietCode/JState)
* [Engine](https://github.com/doridori/Engine)
* [Fettle](https://github.com/thehiflyer/Fettle)
* [Yatomata](https://github.com/camelot-framework/yatomata)
* [stateful](https://github.com/zevada/stateful)
* [state-machine](https://github.com/davidmoten/state-machine)

### Python

* [transitions](https://github.com/pytransitions/transitions)
* [django-fsm](https://github.com/viewflow/django-fsm)
* [automat](https://github.com/glyph/automat)
* [state_machine](https://github.com/jtushman/state_machine)
* [xworkflows](https://github.com/rbarrois/xworkflows)
* [django-states2](https://github.com/vikingco/django-states2)
* [python-statemachine](https://github.com/fgmacedo/python-statemachine)
* [machinist](https://github.com/ScatterHQ/machinist)
* [fluidity](https://github.com/nsi-iff/fluidity)
* [automaton](https://github.com/openstack/automaton)
* [pysm](https://github.com/pgularski/pysm)
* [declarative-fsm](https://github.com/thomasquintana/declarative-fsm)
* [automaton](https://github.com/nazavode/automaton)

### Ruby

* [aasm](https://github.com/aasm/aasm)
* [state_machine](https://github.com/pluginaweek/state_machine)
* [statesman](https://github.com/gocardless/statesman)
* [finite_machine](https://github.com/piotrmurach/finite_machine)
* [state_machines](https://github.com/state-machines/state_machines)
* [transitions](https://github.com/troessner/transitions)
* [stateful_enum](https://github.com/amatsuda/stateful_enum)
* [micromachine](https://github.com/soveran/micromachine)
* [workflow](https://github.com/ryan-allen/workflow)
* [stately](https://github.com/rtwomey/stately)
* [motion-state-machine](https://github.com/opyh/motion-state-machine)
* [aquam](https://github.com/emancu/aquam)

### Go

* [fsm](https://github.com/looplab/fsm)
* [transition](https://github.com/qor/transition)
* [stateless](https://github.com/qmuntal/stateless)
* [fsm](https://github.com/ryanfaerman/fsm)
* [stateful](https://github.com/bykof/stateful)
* [ws-machine](https://github.com/aglyzov/ws-machine)
* [fsm](https://github.com/dyrkin/fsm)
* [statemachine-go](https://github.com/Gurpartap/statemachine-go)
* [go-sm](https://github.com/calebwin/go-sm)
* [go-fsm](https://github.com/theckman/go-fsm)
* [go-fsm](https://github.com/igorrius/go-fsm)

### Shell

* [Statebot-sh](https://github.com/shuckster/statebot-sh)

### C++

* [hsm](https://github.com/erikzenker/hsm)
* [msm](https://www.boost.org/doc/libs/1_73_0/libs/msm/doc/HTML/index.html)
* [sml](https://boost-experimental.github.io/sml/index.html)
* [Statechart](https://www.boost.org/doc/libs/1_73_0/libs/statechart/doc/index.html)

### Swift

* [hsm](https://github.com/sergebouts/hsm)

## Contributing

Your contributions are welcome! If you have any content that can contribute to our list, please open a PR.

- - -

If there are any questions about this list or about any other topic, please contact me on Twitter  [@leonardomso](https://twitter.com/leonardomso) and I'll gladly answer it.
