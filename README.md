# clang-format-presets
Presets for clang-format, taken directly from the command line as follows:

```
    > clang-format -style=chromium -dump-config > .chromium.clang-format

    > clang-format -style=gnu -dump-config > .gnu.clang-format

    > clang-format -style=google -dump-config > .google.clang-format

    > clang-format -style=llvm -dump-config > .llvm.clang-format

    > clang-format -style=microsoft -dump-config > .microsoft.clang-format

    > clang-format -style=mozilla -dump-config > .mozilla.clang-format

    > clang-format -style=webkit -dump-config > .webkit.clang-format
```

Useful for feeding into your C/C++ project root folders for formatting/linting.

Integrates with Microsoft CPP Tools VSCode extension via '.vscode/settings.json':

```
    "C_Cpp.clang_format_sortIncludes": null,
    "C_Cpp.clang_format_style": "file",
    "C_Cpp.clang_format_path": "clang-format.exe",
    "C_Cpp.clang_format_fallbackStyle": "{ BasedOnStyle: LLVM, UseTab: Never, IndentWidth: 4, TabWidth: 4, BreakBeforeBraces: Allman, AllowShortIfStatementsOnASingleLine: false, IndentCaseLabels: false, ColumnLimit: 0, AccessModifierOffset: -4, NamespaceIndentation: All, FixNamespaceComments: false }"
```

Licensed under Apache 2.0 with LLVM exceptions.
