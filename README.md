# MLGit_Test_Repo_N1

A Test Repo for MLGit.

### Descriptions

- Python
- Absolute Imports

### Naming Scheme

- `<module name or module acronym>_dummy_<type>_<n>` for each identifier.

### Circular Imports

> Circular Imports

```
a <-> b [one import at runtime]
c <-> d [both imports at runtime]
```

> Triple Circular Imports

```
   a
 /   \
b --- c
```

> Diamond Circular Imports

```
   a
 / | \
b  |  c
 \ | /
   d
```

### Import Graph

> Graph

- (1) `outer_module_producer_a.py`:
- (2) `outer_module_consumer_a.py`: (7)
- (3) `app/app.py`: (4), (5), (7)
- (4) `app/definitions.py`:
- (5) `app/externals_modules.py`: (os), (math), (6)
- (6) `app/utils.py`:
- (7) `app/subdirectory_1/inner_module_producer_a.py`: (sys), (os), (9)
- (8) `app/subdirectory_1/inner_module_consumer_a.py`: (sys), (os), (1)
- (9) `app/subdirectory_2/inner_module_circular_import_a.py`: (10)
- (10) `app/subdirectory_2/inner_module_circular_import_b.py`: (9)
