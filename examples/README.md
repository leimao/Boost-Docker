# Boost CMake Examples

## Build Examples

```bash
$ cmake -B build
$ cmake --build build --config Release --parallel
```

## Run Examples

### Header-Only Example

```bash
$ echo 1 2 3 | build/header-only/Triple 
3 6 9 
```

### Library-Link Example

```bash
$ build/library-link/SubjectExtraction < library-link/data/jayne.txt 
Will Success Spoil Rock Hunter?
```
