---
description: "Learn more about: ICorProfilerInfo12::EventPipeCreateProvider Method"
title: "ICorProfilerInfo12::EventPipeCreateProvider Method"
ms.date: "03/19/2021"
api_name:
  - "ICorProfilerInfo12.EventPipeCreateProvider"
api_location:
  - "coreclr.dll"
  - "corprof.idl"
api_type:
  - "COM"
---
# ICorProfilerInfo12::EventPipeCreateProvider method

Creates an EventPipe provider that the profiler can use to write events for other EventPipe listeners to receive.

## Syntax

```cpp
    HRESULT EventPipeCreateProvider(
                [in, string] const WCHAR    *providerName,
                [out] EVENTPIPE_PROVIDER    *pProvider);
```

## Parameters

`providerName`\
[in] The name of the provider to create.

`pProvider`\
[out] A caller provided pointer that will be filled with the ID of the provider when the function returns.

## Requirements

**Platforms:** See [.NET supported operating systems](https://github.com/dotnet/core/blob/main/os-lifecycle-policy.md).

**Header:** CorProf.idl, CorProf.h

**.NET Versions:** Available since .NET 5.0

## See also

- [EventPipe Overview](../../../core/diagnostics/eventpipe.md)
- [Well Known EventProviders](../../../core/diagnostics/well-known-event-providers.md)
- [ICorProfilerCallback10 Interface](icorprofilercallback10-interface.md)
- [ICorProfilerInfo12 Interface](icorprofilerinfo12-interface.md)
