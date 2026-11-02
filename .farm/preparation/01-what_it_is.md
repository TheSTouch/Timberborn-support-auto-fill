# What it is

Role: intake. Version 2, signed 2026-11-02T19:24:57Z by owner.

# What it is

**Platform Autofill** is a Timberborn mod that adds an Autofill toggle to every drag-placeable block tool (platforms, paths, overhangs). When active, dragging across a height change automatically inserts support columns underneath, stacking from largest to smallest (TriplePlatform → DoublePlatform → Platform) to minimise block count. Live previews show the supports before placement is committed.

## Built with

| Component | Detail |
|---|---|
| Language | C# 9, targeting .NET Framework 4.7.2 |
| Runtime integration | Harmony 2.4.1 (NuGet, runtime provided by the HarmonyLib mod) |
| Game references | Timberborn 1.0.13.1+ managed DLLs (not redistributed; path set via `TIMBERBORN_MANAGED`) |
| Test framework | xunit 2.9.3 on .NET 10, isolated from game DLLs |

## How it builds

```
dotnet build src/PlatformAutofill.csproj
```

Requires Timberborn game assemblies on the build machine. Output is `PlatformAutofill.dll` at the repository root.

## How it tests

```
dotnet test src/tests/PlatformAutofill.Tests/
```

Tests exercise pure logic in `PlatformAutofillRules` and do **not** require the game to be installed.

## Gate

The gate is the test command — it runs without external dependencies and validates the mod's placement-rule logic:

```
dotnet test src/tests/PlatformAutofill.Tests/
```

## project.yml

```yaml
test: dotnet test src/tests/PlatformAutofill.Tests/
tech: csharp, harmony, timberborn, mod
```
