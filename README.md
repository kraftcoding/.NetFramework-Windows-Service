# .NetFramework-Windows-Service
A sample Windows Service (.NET 4.7.2 Framework) C# 

## Introduction

This a .Net 4.7.2 project to figure out how to create and configure a custom Windows Service in C# using Visual Studio. For those who don't know much about Windows Services, it could be wise to quickly summarize what they actually are and how they differ from a standard console program or desktop application.

## Windows Services

In Windows-based operating systems, the term **Windows Service** refers to a computer program without a user-interface that completely operates in the background. If you know Unix-based environments, you could think of it as a Windows version of a typical Unix daemon. A Windows service must conform to the interface rules and protocols of the **Service Control Manager**, the kernel component responsible for managing Windows services.

Once installed, the Windows Service can be configured using the _Service Control Manager_ (**services.exe**) to start when the operating system is started and run in the background as long as Windows is running; alternatively, they can be started manually or by an event. It's also possible to manually pause, stop and restart the service.

Each service can also be configured to run within a context of a specific user or system account: for example, most Windows services that come shipped with the OS are pre-configured to run within the context of three system accounts: _System_, _Network Service_ and _Local Service_. Such behaviours allow them to operate even when the machine is unmanaged and/or a standard user is not logged on.

To get a glimpse of all services running on a Windows machine you can either:

-   Open **Control Panel**, then navigate to the **Administrative Tools** and click on the **Services** icon.
-   Press **Window + R** to open the **Run** window, then type **services.msc** and press ENTER.
