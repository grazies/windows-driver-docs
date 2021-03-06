---
title: Tracking Per-Stream Context in a Legacy File System Filter Driver
author: windows-driver-content
description: Tracking Per-Stream Context in a Legacy File System Filter Driver
ms.assetid: d908ee30-a433-460c-8c14-883702b4f810
keywords: ["context tracking WDK file system"]
---

# Tracking Per-Stream Context in a Legacy File System Filter Driver


## <span id="ddk_tracking_per_stream_context_in_a_file_system_filter_driver_if"></span><span id="DDK_TRACKING_PER_STREAM_CONTEXT_IN_A_FILE_SYSTEM_FILTER_DRIVER_IF"></span>


<div class="alert">
<strong>Note</strong>   For optimal reliability and performance, we recommend using [file system minifilter drivers](filter-manager-and-minifilter-driver-architecture.md) instead of legacy file system filter drivers. Also, legacy file system filter drivers can’t attach to direct access (DAX) volumes. For more about file system minifilter drivers, see [Advantages of the Filter Manager Model](advantages-of-the-filter-manager-model.md). To port your legacy driver to a minifilter driver, see [Guidelines for Porting Legacy Filter Drivers](guidelines-for-porting-legacy-filter-drivers.md).
</div>
 

This section covers per-stream context tracking in Microsoft Windows XP and later OS versions. The following topics are discussed:

[File Streams, Stream Contexts, and Per-Stream Contexts](file-streams--stream-contexts--and-per-stream-contexts.md)

[Creating and Using Per-Stream Context Structures](creating-and-using-per-stream-context-structures.md)

 

 


--------------------


