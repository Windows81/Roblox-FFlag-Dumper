# rbxfflagdumper

.NET suite for statically analysing and dumping Roblox engine FastFlags

## RbxFFlagDumper.Lib

Simple programmatic dumping of either C++ or Lua defined flags

```c#
List<String> flags = StudioFFlagDumper.DumpAllFlags("versions\\version-xxxxxxxxxxxxxxxx\\");
File.WriteAllText("fflags.txt", String.Join('\n', flags));
```

## RbxFFlagDumper.Cli

Basic command line tool for dumping from a directory containing Roblox Studio

```
Usage: RbxFFlagDumper.Cli.exe [cpp|lua|all] [path to studio folder]
```

## Libraries

Uses [PeNet](https://github.com/secana/PeNet) for aid in static analysis