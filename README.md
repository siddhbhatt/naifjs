# NaifJs, a simple state-machine based dialog manager

NaifJs is a simple state-machine based (task-oriented) 
dialog manager micro-framework for nodejs developers.

The package consists in: 
- A run-time dialog engine as a library to be embedded in production conversational apps 
- A micro-framework to create and test dialogues in dev environment (`naif` command line program)


## [Concepts](doc/concepts.md)

Naifjs is based on a specific conceptual model and a domain specific language (DSL) I conceived,
implementing multi-turn contextual dialogues as "state machines". 

Following paragraph introduce main concepts and naming conventions:

- Dialog system
  - [Stateful multi-turn dialogues](doc/concepts.md#introduction--stateful-multi-turn-dialogues)
  - [Architecture](doc/concepts.md#architecture)

- State-machine based dialog manager 
  - [Dialogue as a state-machine](doc/concepts.md#dialogue-as-a-state-machine)
  - [State tracker](doc/concepts.md#state-tracker)

- What is a dialog unit
  - [Dialog Unit](doc/concepts.md#dialog-unit)
  - [Coding a dialogue with a javascript domain specific language](doc/concepts.md#coding-a-dialogue-with-a-javascript-domain-specific-language)
  - [Requests and responses](doc/concepts.md#requests-and-responses)

- Application 
  - [Dialog application](doc/concepts.md#dialog-application)
  - [Sessions](doc/sessions.md)



## Installation

The package contains command line interface program `naif`, so you must install the npm package as global:

- use npm package manager repo

  ```
  $ npm install -g naifjs
  ```

- or download this github repo:

  ```
  $ git clone https://github.com/solyarisoftware/naifjs
  $ cd naifjs && npm link
  ``` 

## Application Programming interface and command line tools 


### [API library](doc/API.md)

NaifJs act as an API library of functions to be called by a main nodejs program. 
See: 

- [API cheat sheet](doc/API.md): list of available functions 
- [Application examples](examples/README.md) some application examples 
- [Documentation content index](doc/index.md) some application examples 
- [Workflow](doc/workflow.md) design/development phases 


### [`naif` command line interface tools](doc/CLI.md)

- [`naif`](doc/CLI.md#naif): is the main command line program 
- [`naif init`](doc/CLI.md#naif-init): initializes project directory 
- [`naif generate`](doc/CLI.md#naif-generate): generate the code skeleton of a dialog unit 
- [`naif show`](doc/CLI.md#naif-show): for a given project, lists all dialog units and relative states 
- [`naif shell`](doc/CLI.md#naif-shell): test a dialog unit using the command line interface 
- [`naif telegram`](doc/CLI.md#naif-telegram): test a dialog unit, setting up on the fly a telegram bot for the purpose


## Discussion 

- [Pros and cons](doc/discussion.md#pros-and-cons)
- [Food for thought](doc/discussion.md#food-for-thought)
- [BackStory](doc/discussion.md#backstory)
- [Acknowledgments](doc/discussion.md#acknowledgments)


## How to contribute

Please feel free to contact me for any proposal/discussion. 
There are many areas of improvement!

- [How to contribute](doc/contributing.md).<br>
- [To do](doc/todo.md)


## Caveat

Currently the project is just a proof of concept. Not ready for production.
<br>The software made is just a prototype in alpha stage. 


## License 

[MIT](LICENSE.md) (c) Giorgio Robino

---

[top](#) | [index](doc/index.md)
