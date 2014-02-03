Layers
---
1 Linux Kernal
===
	* Security
	* Memory & process management
	* Power management
	* Low memory killer
	* Interprocess communiation

2 System libraries
===
	* lots

3 Android Runtime
===
	* Java [write]
	* Dalvik Virtual Machine [execute]

4 Application Framework
===
	* Package manager
	* Window manager
	* View system
	* Resource manager
	* Activity manager
	* ContentProvider[Inter-application data sharing]
	* Location manager
	* Notification manager

Classes
---

Activity
***
[Takes input from user]

Service
***
[Runs in background]

	1 Long running threads with no ui
	2 Data between processes

BroadcastReiever
***
[Listens for and responds to events]

Content Providers
***
[Uses DB style memory]

Steps to creation
---
1 Define Resources
===
[At compilation time, resources generate the R.java class]
	*Layout [.xml] @string/string_name Java: R.layout.layout_name
	*Strings [.xml] @string/string_name Java: R.string.string_name
	*Images
	*Menus
1 Implement Application Classes
===
	*onCreate()
		1 Restore saved state
		1 Set content view
		1 Initialize UI elements
		1 Link UI elements to code actions
1 Package Application
===
AndroidManifest.xml
1 Install & Run
===
