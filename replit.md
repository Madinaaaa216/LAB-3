# HashMap Lab (C)

## Overview
A C-based laboratory assignment implementing a **HashMap (Hash Table) ADT** with linear probing for collision resolution and dynamic resizing.

## Tech Stack
- **Language**: C (standard library)
- **Compiler**: GCC
- **Environment**: Replit (NixOS)

## Key Files
- `hashmap.h` — Header defining `HashMap` and `Pair` structs and function prototypes
- `hashmap.c` — Implementation file where student exercises live (DO NOT auto-complete)
- `main.c` — Word-counter demo application using the HashMap
- `test.c` / `test.sh` — Automated test suite

## Running the Project
```bash
gcc main.c hashmap.c -o main && ./main
```

## Running Tests
```bash
bash test.sh
```

## Student Exercises (in hashmap.c)
1. `createMap` — Initialize the HashMap
2. `insertMap` — Insert key-value pairs with linear probing
3. `searchMap` — Search for a key
4. `eraseMap` — Lazy deletion (set key to NULL)
5. `firstMap` / `nextMap` — Iterator functions
6. `enlarge` — Double capacity and rehash all elements

## Notes
- Keys are strings (`char*`)
- Collision resolution: linear probing
- Array is circular
- Lazy deletion: invalid entries have `key == NULL`
- `current` index starts at -1
