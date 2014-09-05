# Minerva: a fast and flexible system for deep learning

## Goal ##
Make deep learning a home dish

## How to build ##
1. Put path and configures in "configure.in" (please refer to configure.in.example)
2. "./configure"
3. "cd debug"(or "cd release") and press "make"

## Dev notes ##
### Garbage collection ###
* Operator: `NArray` -> `DagHelper<PhysicalData, PhysicalOp>::FreeOp`
* Node: `Dag::NewDataNode`/`Dag::NewOpNode` -> ? -> `Dag::DeleteNode`
