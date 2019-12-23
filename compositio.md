# Compositio de SE
## Process
### The Waterfall Process Model

criticism:

* Building software is by nature an iterative social learning process
* Change may cause confusion 
* Hard to state all requirements explicitly at the beginning of the project
* A working version of the program will not be available until late in the project time-span.

### Evolutionary Process Model

develop _increasingly_, _iteratively_.

* incremental
* prototyping (an initial version to demonstrate concepts, try design options and probe problems and solutions) (considers the difficulty to express their real requirements) (throw-away: to discard the prototype)
* spiral (each loop in the spiral represents a phase; no fixed phases such as specification or design - loops in the spiral are chosen depending on what is required)

### SEI CMM
classifies software processes as initial, repeatable, defined, managed and optimising; appropriate for large systems developed by large teams of engineers.

### Agile
adaptive rather than predictive, people-oriented rather than process-oriented. Principles:

* Highest priority is to satisfy the customer through early and continuous delivery of valuable software.
* Welcome changing requirements, even late in development.
* Deliver working software frequently.
* Working software is the primary measure of progress.
* At regular intervals, the team reflects on how to become more effective.

## xUnit Test
### Result Verification
* State verification: to inspect the state of the system in comparison with the expected.
* Behabior verification: to capture indirect outputs of SUT

## Testing

### Coverage
* White-box: control-flow coverage, data-flow coverage.
* Black-box: requirement coverage

### S, P and T
* __S__ the expected behavior
* __P__ behavior exposed by system implementation
* __T__ behavior detected by test cases

Black-box: __T__ \subset __S__

White-vox: __T__ \subset __P__ 
### control flow testing (wb)

* Predicate Coverage (Condition Coverage) Decompose each decision into atomic conditions -> Draw the flow graph with nodes of conditions -> Find paths that cover all branches (of every atomic condition) -> Choose input data that will result in the selected paths. 

* Multiple Condition Coverage: Find paths that cover all combinations of conditions

### Cyclomatic complexity
Cyclomatic complexity = number of edges - number of nodes + 2 = number of decisions + 1 = number of regions

### data flow testing (wb)
* data flow anomaly: dd, ur, du (d!r). Find DU chain
* data flow graph: definitions and c-use s as node, p-uses as edge

### Equivalence Partitioning (bb)
* weak & strong: whether to cover all combinations
* general & robust: whether to consider invalid input

### Boundary Value Analysis (bb)

## Good Codes
### Defensive programming
assume nothing, make more checks

Experience has shown that writing assertions while programming is one of the quickest and most effective ways to detect and correct bugs.

Error handling: return a neutral/previous/closest value and log a warning

### Self-documenting codes

Never optimize code unless you’ve proved that it is a bottleneck to acceptable program function. 

One function, one action. 

Avoid magic numbers: `login2`, `return 3`

### Comment
write enough and not more. Explain Why, Not How

file comment: avoid listing everything, version or mod history

## Refactoring

Preserves the external software behavior, improves the internal software structure.

### Creating template methods
Separate common behavior from specialized parts
### Optimizing class hierarchies
specialize/generalize
### Incorporating composition relationships
Favor composition over inheritance (classes should achieve polymorphic behavior and code reuse by their composition (by containing instances of other classes that implement the desired functionality) rather than inheritance from a base or parent class.)

## Design Principles
* Keep It Simple Stupid
* Modularity (Development can be more easily planned. Software increments can be defined and delivered. Changes can be more easily accommodated. Testing and debugging. 
Long-term maintenance can be conducted without serious side effects.
)
* Separation of Concern
* Design for Change
* Design for Reuse

## Architecture
Architecture is (mostly) orthogonal to functionality. 

## Requirements Analysis
* 泳道图
* 数据流图（DFD）（顶层：只有一个加工，系统与环境的关系。加工细化得到子图。）（子图-父图输入输出一致：平衡）
* 判定表和判定树
* UML
* 需求应当明确、完整、一致、可追溯

## Operations



