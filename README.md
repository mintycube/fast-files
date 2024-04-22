# Fast Files (ff)

## Description

ff is a bash script which is a combination of 'mkdir' and 'touch'. It can create directory structures and files simultaneously and lists the created objects using eza, lsd, or ls.

## Dependencies

- bash
- [eza](https://github.com/eza-community/eza) (optional)
- [lsd](https://github.com/lsd-rs/lsd) (optional)

## Usage

```bash
  ff [path file or folder]
 --help : prints usage info
```

## Examples

### Single file

```bash
ff file
```

```
 file
```

### Single directory

```bash
ff dir/
```

```
 dir
```

### Multiple files

```bash
ff file1 file2 file3
```

```
 file1
 file2
 file3
```

### Multiple directories

```bash
ff dir1/ dir2/ dir3/
```

```
 dir1
 dir2
 dir3
```

### File in a directory

```bash
ff dir/file
```

```
dir
└── file
```

### Directory in a directory

```bash
ff dir1/dir2/
```

```
dir1
└── dir2
```

### Multiple files in multiple directories

```bash
ff dir1/dir2/file1 dir3/file2
```

```
dir1
└── dir2
    └── file1
dir3
└── file2
```

### If your shell supports brace expansion e.g bash, zsh, fish

```bash
ff dir1/{dir2/{file1,file2}.txt,dir3/file3.txt}
```

```
dir1
├── dir2
│   ├── file1.txt
│   └── file2.txt
└── dir3
    └── file3.txt
```

## Related Projects

[Advanced New File](https://github.com/tanrax/terminal-AdvancedNewFile)
