# JSON Parser in Java 

An LL(1) predictive parser for parsing JsonObjects and JsonArrays using Recursive Descendent Parsing(RDP) technique.

## Motivation
There are already very efficient and useful libraries for parsing Json data. The main aim of this project is to demonstrate the working of RDP technique by designing a parser for raw json data.

## Parser Grammar
Terminals - string_val
Non-Terminals - JsonObject,JsonArray,JsonValue,Pair,LastPair,Key,LastValue
JsonObject -> {} | { PairLastPair }
Pair -> string_val:JsonValue
LastPair -> NULL | ,PairLastPair
JsonArray -> [] | [JsonValueLastValue]
LastValue -> NULL | ;JsonValueLastValue
JsonValue -> string_val | JsonObject | JsonArray

## Installation
This is a python 2.7 program and uses the default imports available with python 2.7. No extra installations required.

## Test
The driver package contains code as well as sample input files, for testing the classes and their methods.

## License
The MIT License (MIT)
Copyright (c) 2016 DiaMuggles

