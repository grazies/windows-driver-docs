---
title: Creating an NT Kernel Logger Trace Session
description: Creating an NT Kernel Logger Trace Session
ms.assetid: 606156b9-8ad9-4510-9929-4f0e3b7a3134
keywords: ["trace sessions WDK , NT Kernel Logger", "NT Kernel Logger trace sessions WDK", "Windows Kernel Trace provider WDK"]
---

# Creating an NT Kernel Logger Trace Session


## <span id="ddk_create_a_real_time_nt_kernel_logger_trace_session_tools"></span><span id="DDK_CREATE_A_REAL_TIME_NT_KERNEL_LOGGER_TRACE_SESSION_TOOLS"></span>


You can use TraceView to create an [NT Kernel Logger trace session](nt-kernel-logger-trace-session.md), a trace session built into Windows that records events that are generated by the Windows kernel.

When you create an NT Kernel Logger trace session, you can select a category of system events, such as "Process". TraceView configures the trace session to record all system events in that category; that is, it sets the **EnableFlags** parameter for the trace to, for example, ENABLE\_TRACE\_FLAG\_PROCESS (0x7FFFFFFF). For more information, see the Microsoft Windows SDK documentation.

### <span id="to_create_an_nt_kernel_logger_trace_session"></span><span id="TO_CREATE_AN_NT_KERNEL_LOGGER_TRACE_SESSION"></span>To create an NT Kernel Logger Trace Session

1.  [Start TraceView](starting-and-exiting-traceview.md).

2.  On the **File** menu, click **Create New Log Session**.

3.  Click **Add Provider**.

4.  Click **Kernel Logger**, select one or more of the check boxes that identify NT Kernel Logger session event types, and click **OK**.

5.  In the **Open** dialog box, locate System.tmf, the trace message format (TMF) file for system events. System.tmf is included in the WDK in the tools\\tracing subdirectory.

6.  To add additional providers of any type, click **Add Provider**. This step is optional.

7.  Click **Next**.

8.  [Set basic trace session options](setting-basic-trace-session-options.md), if desired.

9.  [Set advanced trace session options](setting-advanced-trace-session-options.md), if desired.

10. Click **Finish**.

### <span id="comments"></span><span id="COMMENTS"></span>Comments

The NT Kernel Logger trace session appears in the list of the **Named Provider Selection** dialog box as "Windows Kernel Trace." You can use either the **Named Provider Selection** dialog box or the **Kernel Logger** option on the **Provider Control GUID Setup** dialog box to create an NT Kernel Logger trace session. However, only the **Provider Control GUID Setup** dialog box lets you select the kernel components that are traced. For more information about using the **Named Provider Selection** dialog box, see [Creating a trace session for a registered provider](creating-a-trace-session-for-a-registered-provider.md).

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20[devtest\devtest]:%20Creating%20an%20NT%20Kernel%20Logger%20Trace%20Session%20%20RELEASE:%20%2811/17/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")




