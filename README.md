# MLGit_Test_Repo_N1

A Test Repo for MLGit.

### Descriptions

- Python
- Absolute Imports

### Naming Scheme

- `<module acronym>_dummy_<type>_<n>` for each identifier.

### Imports

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
