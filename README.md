<p align="center">
  <br>
  <img width="400" src="./assets/robot-awesome.svg" alt="logo of awesome-fsm repository">
  <br>
  <br>
</p>

## Awesome Finite State Machines

A curated list of awesome resources related to finite state machines and statecharts. The idea of this repository is to group a lot of nice content related to state machines and statecharts, articles, videos, books, talks, etc.

Any comments or suggestions to this repository, please open an issue. If you have any good content that's related to state machines and statecharts, please open a PR.

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
- [Videos](#videos)
- [Podcasts](#podcasts)
- [Ebooks](#ebooks)

## Introduction

<p align="center">
  <img width="400" src="./assets/traffic-light-state-machine-example.png" alt="traffic light finite state machine example">
</p>

Finite state machines are a computation model, it consists of a machine with a finite number of states and a few transitions between states. To change from one state to another, the transition expects an input, given a specific input the machine will transition to another state. To be more simple, this is how a finite state machine works in 3 steps: 

1. A finite state machine has a finite number of states.
2. To change from one state to another, it responds to a condition, called input.
3. The action of changing from one state to another is called transition. 

Let’s take as an example of a traffic light. A traffic light can have only 3 states: green, red and yellow. To change from one state to another, we will use it as an input integer representing seconds. When the input is 60, the machine will transition to another state. You can see this example at the beginning of the section. 

We can observe finite state machines not only inside the software development but in our real world as well. You can think about almost anything and use finite state machines for it. By having a finite number of states, it reduces drastically the possibility of having unexpected side-effects in your application, your application will get more consistent, well-written and maintainable. 

### Further Reading

- [Finite-state_machine](https://en.wikipedia.org/wiki/Finite-state_machine)
- [Theory of Computation - Finite State Machines](https://stackabuse.com/theory-of-computation-finite-state-machines/)
- [Finite State Machines](https://www.i-programmer.info/babbages-bag/223-finite-state-machines.html)
- [Elements of Robotics - Finite State Machines](https://link.springer.com/chapter/10.1007/978-3-319-62533-1_4)
- [Finite State Machines](http://www.inf.ufsc.br/~joao.dovicchi/pos-ed/pos/exerc/machines2.pdf)
- [The Rise Of The State Machines](https://www.smashingmagazine.com/2018/01/rise-state-machines/)

## Concepts

In the finite state machine model, we have a few different concepts that it’s very important to learn about. We can classify finite state machines by two types: deterministic state automaton and non-deterministic state automaton. 

If you’re wondering, automaton is the plural of automata. Finite state machines are also know as finite state automata or finite state automaton.

Within the finite state machine model, we have two types of finite state machines that generate output: Mealy state machine and Moore state machine.

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

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse at felis ipsum. Quisque fermentum tellus magna, sed aliquet mi venenatis at. Ut in placerat nisi. Etiam placerat id ligula et sagittis. Phasellus ullamcorper tristique euismod. 

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

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse at felis ipsum. Quisque fermentum tellus magna, sed aliquet mi venenatis at. Ut in placerat nisi. Etiam placerat id ligula et sagittis. Phasellus ullamcorper tristique euismod. 

#### Further Reading

- [Moore machine](https://en.wikipedia.org/wiki/Moore_machine)
- [Moore Machine](https://www.javatpoint.com/automata-moore-machine)
- [Moore Machine](https://xlinux.nist.gov/dads/HTML/mooreMachine.html)
- [Moore Finite State Machine](https://www.electronics-tutorial.net/finite-state-machines/State-Machine-Fundamentals/Moore-Finite-State-Machine/)
- [Moore and Mealy Machine Design Procedure](http://www2.elo.utfsm.cl/~lsb/elo211/aplicaciones/katz/chapter8/chapter08.doc4.html)

## Statecharts

## Libraries

### JavaScript

* [XState](https://github.com/davidkpiano/xstate)
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

## Videos

## Podcasts

## Ebooks

## Contributing

Your contributions are welcome! If you have any content that can contribute to our list, please open a PR.

- - -

If there are any questions about this list or about any other topic, please contact me on Twitter  [@leonardomso](https://twitter.com/leonardomso) and I'll gladly answer it.
