# [Error Handling](error-handling.md)
## [About Error Handling](about-error-handling.md)
### [Error Mode](error-mode.md)
### [Last-Error Code](last-error-code.md)
### [Notifying the User](notifying-the-user.md)
### [Message Tables](message-tables.md)
### [Fatal Application Exit](fatal-application-exit.md)
### [Error Message Guidelines](error-message-guidelines.md)
## [Using Error Handling](using-error-handling.md)
### [Retrieving the Last-Error Code](retrieving-the-last-error-code.md)
## [Error Handling Reference](error-handling-reference.md)
### [Error Handling Functions](error-handling-functions.md)
#### [Beep](/windows/win32/WinBase/?branch=master)
#### [CaptureStackBackTrace](capturestackbacktrace.md)
#### [FatalAppExit](/windows/win32/WinBase/?branch=master)
#### [FlashWindow](/windows/win32/Winuser/nf-winuser-flashwindow?branch=master)
#### [FlashWindowEx](/windows/win32/Winuser/nf-winuser-flashwindowex?branch=master)
#### [FormatMessage](/windows/win32/WinBase/nf-winbase-formatmessage?branch=master)
#### [GetErrorMode](/windows/win32/WinBase/?branch=master)
#### [GetLastError](/windows/win32/WinBase/?branch=master)
#### [GetThreadErrorMode](/windows/win32/WinBase/?branch=master)
#### [MessageBeep](/windows/win32/WinUser/nf-winuser-messagebeep?branch=master)
#### [RtlLookupFunctionEntry](/windows/win32/WinNT/nf-winnt-rtllookupfunctionentry?branch=master)
#### [RtlNtStatusToDosError](/windows/win32/Winternl/nf-winternl-rtlntstatustodoserror?branch=master)
#### [RtlNtStatusToDosErrorNoTeb](/windows/win32/Winternl/?branch=master)
#### [RtlPcToFileHeader](/windows/win32/WinNT/nf-winnt-rtlpctofileheader?branch=master)
#### [RtlUnwind](/windows/win32/WinNT/nf-winnt-rtlunwind?branch=master)
#### [RtlUnwind2](/windows/win32/WinNT/nf-winnt-rtlunwind2?branch=master)
#### [RtlUnwindEx](/windows/win32/WinNT/nf-winnt-rtlunwindex?branch=master)
#### [RtlVirtualUnwind](/windows/win32/WinNT/nf-winnt-rtlvirtualunwind?branch=master)
#### [SetErrorMode](/windows/win32/WinBase/?branch=master)
#### [SetLastError](/windows/win32/WinBase/?branch=master)
#### [SetLastErrorEx](/windows/win32/Winuser/nf-winuser-setlasterrorex?branch=master)
#### [SetThreadErrorMode](/windows/win32/WinBase/?branch=master)
### [Error Handling Macros](error-handling-macro.md)
#### [C_ASSERT](/windows/win32/WinNT/nf-winnt-c_assert?branch=master)
### [Error Handling Structures](error-handling-structures.md)
#### [FLASHWINFO](/windows/win32/Winuser/ns-winuser-flashwinfo?branch=master)
### [System Error Codes](system-error-codes.md)
#### [System Error Codes (0-499)](system-error-codes--0-499-.md)
#### [System Error Codes (500-999)](system-error-codes--500-999-.md)
#### [System Error Codes (1000-1299)](system-error-codes--1000-1299-.md)
#### [System Error Codes (1300-1699)](system-error-codes--1300-1699-.md)
#### [System Error Codes (1700-3999)](system-error-codes--1700-3999-.md)
#### [System Error Codes (4000-5999)](system-error-codes--4000-5999-.md)
#### [System Error Codes (6000-8199)](system-error-codes--6000-8199-.md)
#### [System Error Codes (8200-8999)](system-error-codes--8200-8999-.md)
#### [System Error Codes (9000-11999)](system-error-codes--9000-11999-.md)
#### [System Error Codes (12000-15999)](system-error-codes--12000-15999-.md)
# [Basic Debugging](basic-debugging.md)
## [About Basic Debugging](about-basic-debugging.md)
### [Debugging Terminology](debugging-terminology.md)
### [Debug Support from Process, Thread, and Exception Functions](debug-support-from-process-thread-and-exception-functions.md)
#### [Process Functions for Debugging](process-functions-for-debugging.md)
#### [Thread Functions for Debugging](thread-functions-for-debugging.md)
#### [Exception Functions for Debugging](exception-handling-functions-for-debugging.md)
## [Using Basic Debugging](using-basic-debugging.md)
### [Configuring Automatic Debugging](configuring-automatic-debugging.md)
### [Creating a Basic Debugger](creating-a-basic-debugger.md)
#### [Debugging a Running Process](debugging-a-running-process.md)
#### [Writing the Debugger's Main Loop](writing-the-debugger-s-main-loop.md)
#### [Communicating with the Debugger](communicating-with-the-debugger.md)
## [Debugging Reference](debugging-reference.md)
### [Debugging Events](debugging-events.md)
### [Debugging Functions](debugging-functions.md)
#### [CheckRemoteDebuggerPresent](/windows/win32/WinBase/?branch=master)
#### [ContinueDebugEvent](/windows/win32/WinBase/?branch=master)
#### [DebugActiveProcess](/windows/win32/WinBase/?branch=master)
#### [DebugActiveProcessStop](/windows/win32/WinBase/?branch=master)
#### [DebugBreak](/windows/win32/WinBase/?branch=master)
#### [DebugBreakProcess](/windows/win32/WinBase/nf-winbase-debugbreakprocess?branch=master)
#### [DebugSetProcessKillOnExit](/windows/win32/WinBase/nf-winbase-debugsetprocesskillonexit?branch=master)
#### [FatalExit](/windows/win32/WinBase/nf-winbase-fatalexit?branch=master)
#### [FlushInstructionCache](flushinstructioncache.md)
#### [GetThreadContext](/windows/win32/WinBase/nf-dbgeng-idebugadvanced4-getthreadcontext?branch=master)
#### [GetThreadSelectorEntry](/windows/win32/WinBase/nf-winbase-getthreadselectorentry?branch=master)
#### [IsDebuggerPresent](/windows/win32/WinBase/?branch=master)
#### [OutputDebugString](/windows/win32/WinBase/?branch=master)
#### [ReadProcessMemory](readprocessmemory.md)
#### [SetThreadContext](/windows/win32/WinBase/nf-dbgeng-idebugadvanced4-setthreadcontext?branch=master)
#### [WaitForDebugEvent](/windows/win32/WinBase/?branch=master)
#### [WaitForDebugEventEx](/windows/win32/WinBase/?branch=master)
#### [Wow64GetThreadContext](/windows/win32/WinBase/nf-winbase-wow64getthreadcontext?branch=master)
#### [Wow64GetThreadSelectorEntry](/windows/win32/WinBase/nf-winbase-wow64getthreadselectorentry?branch=master)
#### [Wow64SetThreadContext](/windows/win32/WinBase/nf-winbase-wow64setthreadcontext?branch=master)
#### [WriteProcessMemory](writeprocessmemory.md)
### [Debugging Structures](debugging-structures.md)
#### [CONTEXT](/windows/win32/WinNT/ns-winnt-_arm64_nt_context?branch=master)
#### [CREATE_PROCESS_DEBUG_INFO](create-process-debug-info-str.md)
#### [CREATE_THREAD_DEBUG_INFO](create-thread-debug-info-str.md)
#### [DEBUG_EVENT](debug-event-str.md)
#### [EXCEPTION_DEBUG_INFO](exception-debug-info-str.md)
#### [EXIT_PROCESS_DEBUG_INFO](exit-process-debug-info-str.md)
#### [EXIT_THREAD_DEBUG_INFO](exit-thread-debug-info-str.md)
#### [LDT_ENTRY](/windows/win32/WinNT/ns-winnt-_ldt_entry?branch=master)
#### [LOAD_DLL_DEBUG_INFO](load-dll-debug-info-str.md)
#### [OUTPUT_DEBUG_STRING_INFO](output-debug-string-info-str.md)
#### [RIP_INFO](rip-info-str.md)
#### [Thread Environment Block (Debugging Notes)](thread-environment-block--debugging-notes-.md)
#### [UNLOAD_DLL_DEBUG_INFO](unload-dll-debug-info-str.md)
#### [WOW64_CONTEXT](/windows/win32/WinNT/ns-winnt-_wow64_context?branch=master)
#### [WOW64_FLOATING_SAVE_AREA](/windows/win32/WinNT/ns-winnt-_wow64_floating_save_area?branch=master)
#### [WOW64_LDT_ENTRY](/windows/win32/WinNT/ns-winnt-_wow64_ldt_entry?branch=master)
# [Debug Help Library](debug-help-library.md)
## [About DbgHelp](about-dbghelp.md)
### [DbgHelp Versions](dbghelp-versions.md)
### [Symbol Files](symbol-files.md)
### [Symbol Handling](symbol-handling.md)
#### [Symbol Handler Initialization](symbol-handler-initialization.md)
#### [Symbol Paths](symbol-paths.md)
#### [Symbol Loading](symbol-loading.md)
#### [Deferred Symbol Loading](deferred-symbol-loading.md)
#### [Decorated Symbol Names](decorated-symbol-names.md)
#### [Finding Symbols](finding-symbols.md)
#### [Public, Global, and Local Symbols](public--global--and-local-symbols.md)
#### [Symbol Handler Cleanup](symbol-handler-cleanup.md)
### [Symbol Server and Symbol Stores](symbol-servers-and-symbol-stores.md)
#### [Using SymSrv](using-symsrv.md)
#### [Using SymStore](using-symstore.md)
#### [Using Other Symbol Stores](using-other-symbol-stores.md)
#### [SymStore Command-Line Options](symstore-command-line-options.md)
#### [Symbol Server and Internet Firewalls](symbol-servers-and-internet-firewalls.md)
### [Minidump Files](minidump-files.md)
### [Source Server](source-server-and-source-indexing.md)
### [Updated Platform Support](updated-platform-support.md)
## [Using DbgHelp](using-dbghelp.md)
### [Calling the DbgHelp Library](calling-the-dbghelp-library.md)
### [Initializing the Symbol Handler](initializing-the-symbol-handler.md)
### [Loading a Symbol Module](loading-a-symbol-module.md)
### [Getting Notifications](getting-notifications.md)
### [Enumerating Symbol Modules](enumerating-symbol-modules.md)
### [Enumerating Symbols](enumerating-symbols.md)
### [Retrieving Symbol Information by Name](retrieving-symbol-information-by-name.md)
### [Retrieving Symbol Information by Address](retrieving-symbol-information-by-address.md)
### [Retrieving Undecorated Symbol Names](retrieving-undecorated-symbol-names.md)
### [Unloading a Symbol Module](unloading-a-symbol-module.md)
### [Terminating the Symbol Handler](terminating-the-symbol-handler.md)
## [DbgHelp Reference](dbghelp-reference.md)
### [DbgHelp Enumerations](dbghelp-enumerations.md)
#### [IMAGEHLP_EXTENDED_OPTIONS](/windows/win32/DbgHelp/ne-dbghelp-imagehlp_extended_options?branch=master)
#### [IMAGEHLP_SYMBOL_TYPE_INFO](/windows/win32/DbgHelp/ne-dbghelp-_imagehlp_symbol_type_info?branch=master)
#### [MINIDUMP_CALLBACK_TYPE](/windows/win32/minidumpapiset/ne-minidumpapiset-_minidump_callback_type?branch=master)
#### [MINIDUMP_HANDLE_OBJECT_INFORMATION_TYPE](/windows/win32/minidumpapiset/ne-minidumpapiset-_minidump_handle_object_information_type?branch=master)
#### [MINIDUMP_SECONDARY_FLAGS](/windows/win32/minidumpapiset/ne-minidumpapiset-_minidump_secondary_flags?branch=master)
#### [MINIDUMP_STREAM_TYPE](/windows/win32/minidumpapiset/ne-minidumpapiset-_minidump_stream_type?branch=master)
#### [MINIDUMP_TYPE](/windows/win32/minidumpapiset/ne-minidumpapiset-_minidump_type?branch=master)
#### [MODULE_WRITE_FLAGS](/windows/win32/minidumpapiset/ne-minidumpapiset-_module_write_flags?branch=master)
#### [THREAD_WRITE_FLAGS](/windows/win32/minidumpapiset/ne-minidumpapiset-_thread_write_flags?branch=master)
### [DbgHelp Functions](dbghelp-functions.md)
#### [EnumDirTree](/windows/win32/Dbghelp/nf-dbghelp-enumdirtree?branch=master)
#### [EnumDirTreeProc](/windows/win32/DbgHelp/nc-dbghelp-penumdirtree_callback?branch=master)
#### [EnumerateLoadedModules64](/windows/win32/Dbghelp/nf-dbghelp-enumerateloadedmodules?branch=master)
#### [EnumerateLoadedModulesEx](/windows/win32/Dbghelp/nf-dbghelp-enumerateloadedmodulesex?branch=master)
#### [EnumerateLoadedModulesProc64](/windows/win32/DbgHelp/nc-dbghelp-penumloaded_modules_callback?branch=master)
#### [FindDebugInfoFile](/windows/win32/Dbghelp/nf-dbghelp-finddebuginfofile?branch=master)
#### [FindDebugInfoFileEx](/windows/win32/Dbghelp/nf-dbghelp-finddebuginfofileex?branch=master)
#### [FindDebugInfoFileProc](/windows/win32/DbgHelp/nc-dbghelp-pfind_debug_file_callback?branch=master)
#### [FindExecutableImage](/windows/win32/Dbghelp/nf-dbghelp-findexecutableimage?branch=master)
#### [FindExecutableImageEx](/windows/win32/Dbghelp/nf-dbghelp-findexecutableimageex?branch=master)
#### [FindExecutableImageProc](/windows/win32/DbgHelp/nc-dbghelp-pfind_exe_file_callback?branch=master)
#### [FunctionTableAccessProc64](/windows/win32/DbgHelp/nc-dbghelp-pfunction_table_access_routine?branch=master)
#### [GetModuleBaseProc64](/windows/win32/DbgHelp/nc-dbghelp-pget_module_base_routine?branch=master)
#### [GetSymLoadError](/windows/win32/DbgHelp/nf-dbghelp-getsymloaderror?branch=master)
#### [GetTimestampForLoadedLibrary](/windows/win32/Dbghelp/nf-dbghelp-gettimestampforloadedlibrary?branch=master)
#### [ImageDirectoryEntryToData](/windows/win32/Dbghelp/nf-dbghelp-imagedirectoryentrytodata?branch=master)
#### [ImageDirectoryEntryToDataEx](/windows/win32/Dbghelp/nf-dbghelp-imagedirectoryentrytodataex?branch=master)
#### [ImagehlpApiVersion](/windows/win32/Dbghelp/nf-dbghelp-imagehlpapiversion?branch=master)
#### [ImagehlpApiVersionEx](/windows/win32/Dbghelp/nf-dbghelp-imagehlpapiversionex?branch=master)
#### [ImageNtHeader](/windows/win32/Dbghelp/nf-dbghelp-imagentheader?branch=master)
#### [ImageRvaToSection](/windows/win32/Dbghelp/nf-dbghelp-imagervatosection?branch=master)
#### [ImageRvaToVa](/windows/win32/Dbghelp/nf-dbghelp-imagervatova?branch=master)
#### [MakeSureDirectoryPathExists](/windows/win32/Dbghelp/nf-dbghelp-makesuredirectorypathexists?branch=master)
#### [MapDebugInformation](/windows/win32/Dbghelp/nf-dbghelp-mapdebuginformation?branch=master)
#### [MiniDumpCallback](/windows/win32/minidumpapiset/nc-minidumpapiset-minidump_callback_routine?branch=master)
#### [MiniDumpReadDumpStream](/windows/win32/minidumpapiset/nf-minidumpapiset-minidumpreaddumpstream?branch=master)
#### [MiniDumpWriteDump](/windows/win32/minidumpapiset/nf-minidumpapiset-minidumpwritedump?branch=master)
#### [ReadProcessMemoryProc64](/windows/win32/DbgHelp/nc-dbghelp-pread_process_memory_routine?branch=master)
#### [SearchTreeForFile](/windows/win32/Dbghelp/nf-dbghelp-searchtreeforfile?branch=master)
#### [SetSymLoadError](/windows/win32/DbgHelp/nf-dbghelp-setsymloaderror?branch=master)
#### [StackWalk64](/windows/win32/DbgHelp/nf-dbghelp-stackwalk?branch=master)
#### [StackWalkEx](/windows/win32/DbgHelp/nf-dbghelp-stackwalkex?branch=master)
#### [SymAddrIncludeInlineTrace](/windows/win32/DbgHelp/nf-dbghelp-symaddrincludeinlinetrace?branch=master)
#### [SymAddSourceStream](/windows/win32/Dbghelp/nf-dbghelp-symaddsourcestream?branch=master)
#### [SymAddSymbol](/windows/win32/Dbghelp/nf-dbghelp-symaddsymbol?branch=master)
#### [SymCleanup](/windows/win32/Dbghelp/nf-dbghelp-symcleanup?branch=master)
#### [SymCompareInlineTrace](/windows/win32/DbgHelp/nf-dbghelp-symcompareinlinetrace?branch=master)
#### [SymDeleteSymbol](/windows/win32/Dbghelp/nf-dbghelp-symdeletesymbol?branch=master)
#### [SymEnumerateModules64](/windows/win32/Dbghelp/nf-dbghelp-symenumeratemodules?branch=master)
#### [SymEnumerateModulesProc64](/windows/win32/DbgHelp/nc-dbghelp-psym_enummodules_callback?branch=master)
#### [SymEnumerateSymbols64](/windows/win32/Dbghelp/nf-dbghelp-symenumeratesymbols?branch=master)
#### [SymEnumerateSymbolsProc64](/windows/win32/DbgHelp/nc-dbghelp-psym_enumsymbols_callback?branch=master)
#### [SymEnumLines](/windows/win32/Dbghelp/nf-dbghelp-symenumlines?branch=master)
#### [SymEnumLinesProc](/windows/win32/DbgHelp/nc-dbghelp-psym_enumlines_callback?branch=master)
#### [SymEnumProcesses](/windows/win32/DbgHelp/nf-dbghelp-symenumprocesses?branch=master)
#### [SymEnumProcessesProc](/windows/win32/DbgHelp/nc-dbghelp-psym_enumprocesses_callback?branch=master)
#### [SymEnumSourceFiles](/windows/win32/DbgHelp/nf-dbghelp-symenumsourcefiles?branch=master)
#### [SymEnumSourceFilesProc](/windows/win32/DbgHelp/nc-dbghelp-psym_enumsourcefiles_callback?branch=master)
#### [SymEnumSourceFileTokens](/windows/win32/Dbghelp/nf-dbghelp-symenumsourcefiletokens?branch=master)
#### [PENUMSOURCEFILETOKENSCALLBACK](/windows/win32/Dbghelp/nc-dbghelp-penumsourcefiletokenscallback?branch=master)
#### [SymEnumSourceLines](/windows/win32/DbgHelp/nf-dbghelp-symenumsourcelines?branch=master)
#### [SymEnumSymbols](/windows/win32/Dbghelp/nf-dbghelp-symenumsymbols?branch=master)
#### [SymEnumSymbolsEx](/windows/win32/DbgHelp/nf-dbghelp-symenumsymbolsex?branch=master)
#### [SymEnumSymbolsForAddr](/windows/win32/Dbghelp/nf-dbghelp-symenumsymbolsforaddr?branch=master)
#### [SymEnumSymbolsProc](/windows/win32/DbgHelp/nc-dbghelp-psym_enumeratesymbols_callback?branch=master)
#### [SymEnumTypes](/windows/win32/Dbghelp/nf-dbghelp-symenumtypes?branch=master)
#### [SymEnumTypesByName](/windows/win32/Dbghelp/nf-dbghelp-symenumtypesbyname?branch=master)
#### [SymFindDebugInfoFile](/windows/win32/Dbghelp/nf-dbghelp-symfinddebuginfofile?branch=master)
#### [SymFindExecutableImage](/windows/win32/Dbghelp/nf-dbghelp-symfindexecutableimage?branch=master)
#### [SymFindFileInPath](/windows/win32/DbgHelp/nf-dbghelp-symfindfileinpath?branch=master)
#### [SymFindFileInPathProc](/windows/win32/DbgHelp/nc-dbghelp-pfindfileinpathcallback?branch=master)
#### [SymFromAddr](/windows/win32/Dbghelp/nf-dbghelp-symfromaddr?branch=master)
#### [SymFromIndex](/windows/win32/Dbghelp/nf-dbghelp-symfromindex?branch=master)
#### [SymFromInlineContext](/windows/win32/DbgHelp/nf-dbghelp-symfrominlinecontext?branch=master)
#### [SymFromName](/windows/win32/Dbghelp/nf-dbghelp-symfromname?branch=master)
#### [SymFromToken](/windows/win32/Dbghelp/nf-dbghelp-symfromtoken?branch=master)
#### [SymFunctionTableAccess64](/windows/win32/Dbghelp/nf-dbghelp-symfunctiontableaccess?branch=master)
#### [SymFunctionTableAccess64AccessRoutines](/windows/win32/DbgHelp/nf-dbghelp-symfunctiontableaccess64accessroutines?branch=master)
#### [SymGetExtendedOption](/windows/win32/DbgHelp/nf-dbghelp-symgetextendedoption?branch=master)
#### [SymGetFileLineOffsets64](/windows/win32/Dbghelp/nf-dbghelp-symgetfilelineoffsets64?branch=master)
#### [SymGetHomeDirectory](/windows/win32/Dbghelp/nf-dbghelp-symgethomedirectory?branch=master)
#### [SymGetLineFromAddr64](/windows/win32/Dbghelp/nf-dbghelp-symgetlinefromaddr?branch=master)
#### [SymGetLineFromInlineContext](/windows/win32/DbgHelp/nf-dbghelp-symgetlinefrominlinecontext?branch=master)
#### [SymGetLineFromName64](/windows/win32/Dbghelp/nf-dbghelp-symgetlinefromname?branch=master)
#### [SymGetLineNext64](/windows/win32/Dbghelp/nf-dbghelp-symgetlinenext?branch=master)
#### [SymGetLinePrev64](/windows/win32/Dbghelp/nf-dbghelp-symgetlineprev?branch=master)
#### [SymGetModuleBase64](/windows/win32/Dbghelp/nf-dbghelp-symgetmodulebase?branch=master)
#### [SymGetModuleInfo64](/windows/win32/Dbghelp/nf-dbghelp-symgetmoduleinfo?branch=master)
#### [SymGetOmaps](/windows/win32/Dbghelp/nf-dbghelp-symgetomaps?branch=master)
#### [SymGetOptions](/windows/win32/Dbghelp/nf-dbghelp-symgetoptions?branch=master)
#### [SymGetScope](/windows/win32/Dbghelp/nf-dbghelp-symgetscope?branch=master)
#### [SymGetSearchPath](/windows/win32/Dbghelp/nf-dbghelp-symgetsearchpath?branch=master)
#### [SymGetSourceFile](/windows/win32/Dbghelp/nf-dbghelp-symgetsourcefile?branch=master)
#### [SymGetSourceFileChecksum](/windows/win32/Dbghelp/nf-dbghelp-symgetsourcefilechecksum?branch=master)
#### [SymGetSourceFileFromToken](/windows/win32/Dbghelp/nf-dbghelp-symgetsourcefilefromtoken?branch=master)
#### [SymGetSourceFileToken](/windows/win32/Dbghelp/nf-dbghelp-symgetsourcefiletoken?branch=master)
#### [SymGetSourceVarFromToken](/windows/win32/Dbghelp/nf-dbghelp-symgetsourcevarfromtoken?branch=master)
#### [SymGetSymbolFile](/windows/win32/Dbghelp/nf-dbghelp-symgetsymbolfile?branch=master)
#### [SymGetSymFromAddr64](/windows/win32/Dbghelp/nf-dbghelp-symgetsymfromaddr?branch=master)
#### [SymGetSymFromName64](/windows/win32/Dbghelp/nf-dbghelp-symgetsymfromname?branch=master)
#### [SymGetSymNext64](/windows/win32/Dbghelp/nf-dbghelp-symgetsymnext?branch=master)
#### [SymGetSymPrev64](/windows/win32/Dbghelp/nf-dbghelp-symgetsymprev?branch=master)
#### [SymGetTypeFromName](/windows/win32/Dbghelp/nf-dbghelp-symgettypefromname?branch=master)
#### [SymGetTypeInfo](/windows/win32/Dbghelp/nf-dbghelp-symgettypeinfo?branch=master)
#### [SymGetTypeInfoEx](/windows/win32/Dbghelp/nf-dbghelp-symgettypeinfoex?branch=master)
#### [SymInitialize](/windows/win32/Dbghelp/nf-dbghelp-syminitialize?branch=master)
#### [SymLoadModule64](/windows/win32/Dbghelp/nf-dbghelp-symloadmodule?branch=master)
#### [SymLoadModuleEx](/windows/win32/Dbghelp/nf-dbghelp-symloadmoduleex?branch=master)
#### [SymMatchFileName](/windows/win32/Dbghelp/nf-dbghelp-symmatchfilename?branch=master)
#### [SymMatchString](/windows/win32/DbgHelp/nf-dbghelp-symmatchstring?branch=master)
#### [SymNext](/windows/win32/DbgHelp/nf-dbghelp-symnext?branch=master)
#### [SymPrev](/windows/win32/DbgHelp/nf-dbghelp-symprev?branch=master)
#### [SymQueryInlineTrace](/windows/win32/DbgHelp/nf-dbghelp-symqueryinlinetrace?branch=master)
#### [SymRefreshModuleList](/windows/win32/Dbghelp/nf-dbghelp-symrefreshmodulelist?branch=master)
#### [SymRegisterCallback64](/windows/win32/Dbghelp/nf-dbghelp-symregistercallback?branch=master)
#### [SymRegisterCallbackProc64](/windows/win32/DbgHelp/nc-dbghelp-psymbol_registered_callback?branch=master)
#### [SymRegisterFunctionEntryCallback64](/windows/win32/Dbghelp/nf-dbghelp-symregisterfunctionentrycallback?branch=master)
#### [SymRegisterFunctionEntryCallbackProc64](/windows/win32/DbgHelp/nc-dbghelp-psymbol_funcentry_callback?branch=master)
#### [SymSearch](/windows/win32/Dbghelp/nf-dbghelp-symsearch?branch=master)
#### [SymSetContext](/windows/win32/Dbghelp/nf-dbghelp-symsetcontext?branch=master)
#### [SymSetExtendedOption](/windows/win32/DbgHelp/nf-dbghelp-symsetextendedoption?branch=master)
#### [SymSetHomeDirectory](/windows/win32/Dbghelp/nf-dbghelp-symsethomedirectory?branch=master)
#### [SymSetOptions](/windows/win32/Dbghelp/nf-dbghelp-symsetoptions?branch=master)
#### [SymSetParentWindow](/windows/win32/Dbghelp/nf-dbghelp-symsetparentwindow?branch=master)
#### [SymSetScopeFromAddr](/windows/win32/Dbghelp/nf-dbghelp-symsetscopefromaddr?branch=master)
#### [SymSetScopeFromIndex](/windows/win32/Dbghelp/nf-dbghelp-symsetscopefromindex?branch=master)
#### [SymSetScopeFromInlineContext](/windows/win32/DbgHelp/nf-dbghelp-symsetscopefrominlinecontext?branch=master)
#### [SymSetSearchPath](/windows/win32/Dbghelp/nf-dbghelp-symsetsearchpath?branch=master)
#### [SymSrvDeltaName](/windows/win32/DbgHelp/nf-dbghelp-symsrvdeltaname?branch=master)
#### [SymSrvGetFileIndexes](/windows/win32/DbgHelp/nf-dbghelp-symsrvgetfileindexes?branch=master)
#### [SymSrvGetFileIndexInfo](/windows/win32/Dbghelp/nf-dbghelp-symsrvgetfileindexinfo?branch=master)
#### [SymSrvGetFileIndexString](/windows/win32/DbgHelp/nf-dbghelp-symsrvgetfileindexstring?branch=master)
#### [SymSrvGetSupplement](/windows/win32/DbgHelp/nf-dbghelp-symsrvgetsupplement?branch=master)
#### [SymSrvIsStore](/windows/win32/DbgHelp/nf-dbghelp-symsrvisstore?branch=master)
#### [SymSrvStoreFile](/windows/win32/DbgHelp/nf-dbghelp-symsrvstorefile?branch=master)
#### [SymSrvStoreSupplement](/windows/win32/DbgHelp/nf-dbghelp-symsrvstoresupplement?branch=master)
#### [SymUnDName64](/windows/win32/Dbghelp/nf-dbghelp-symundname?branch=master)
#### [SymUnloadModule64](/windows/win32/Dbghelp/nf-dbghelp-symunloadmodule?branch=master)
#### [TranslateAddressProc64](/windows/win32/DbgHelp/nc-dbghelp-ptranslate_address_routine?branch=master)
#### [UnDecorateSymbolName](/windows/win32/Dbghelp/nf-dbghelp-undecoratesymbolname?branch=master)
#### [UnmapDebugInformation](/windows/win32/Dbghelp/nf-dbghelp-unmapdebuginformation?branch=master)
### [DbgHelp Structures](dbghelp-structures.md)
#### [_IMAGE_RUNTIME_FUNCTION_ENTRY](/windows/win32/WinNT/ns-winnt-_image_runtime_function_entry?branch=master)
#### [ADDRESS64](/windows/win32/DbgHelp/ns-dbghelp-_tagaddress?branch=master)
#### [API_VERSION](/windows/win32/DbgHelp/ns-dbghelp-api_version?branch=master)
#### [FPO_DATA](/windows/win32/WinNT/ns-winnt-_fpo_data?branch=master)
#### [IMAGE_DEBUG_INFORMATION](/windows/win32/DbgHelp/ns-dbghelp-_image_debug_information?branch=master)
#### [IMAGEHLP_CBA_EVENT](/windows/win32/DbgHelp/ns-dbghelp-_imagehlp_cba_event?branch=master)
#### [IMAGEHLP_CBA_READ_MEMORY](/windows/win32/DbgHelp/ns-dbghelp-_imagehlp_cba_read_memory?branch=master)
#### [IMAGEHLP_DEFERRED_SYMBOL_LOAD64](/windows/win32/DbgHelp/ns-dbghelp-_imagehlp_deferred_symbol_load?branch=master)
#### [IMAGEHLP_DUPLICATE_SYMBOL64](/windows/win32/DbgHelp/ns-dbghelp-_imagehlp_duplicate_symbol?branch=master)
#### [IMAGEHLP_GET_TYPE_INFO_PARAMS](/windows/win32/DbgHelp/ns-dbghelp-_imagehlp_get_type_info_params?branch=master)
#### [IMAGEHLP_LINE64](/windows/win32/DbgHelp/ns-dbghelp-_imagehlp_line?branch=master)
#### [IMAGEHLP_MODULE64](/windows/win32/DbgHelp/ns-dbghelp-_imagehlp_module?branch=master)
#### [IMAGEHLP_STACK_FRAME](/windows/win32/DbgHelp/ns-dbghelp-_imagehlp_stack_frame?branch=master)
#### [IMAGEHLP_SYMBOL64](/windows/win32/DbgHelp/ns-dbghelp-_imagehlp_symbol?branch=master)
#### [KDHELP64](/windows/win32/DbgHelp/ns-dbghelp-_kdhelp?branch=master)
#### [LOADED_IMAGE](/windows/win32/DbgHelp/ns-dbghelp-_loaded_image?branch=master)
#### [MINIDUMP_CALLBACK_INFORMATION](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_callback_information?branch=master)
#### [MINIDUMP_CALLBACK_INPUT](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_callback_input?branch=master)
#### [MINIDUMP_CALLBACK_OUTPUT](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_callback_output?branch=master)
#### [MINIDUMP_DIRECTORY](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_directory?branch=master)
#### [MINIDUMP_EXCEPTION](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_exception?branch=master)
#### [MINIDUMP_EXCEPTION_INFORMATION](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_exception_information?branch=master)
#### [MINIDUMP_EXCEPTION_STREAM](/windows/win32/minidumpapiset/ns-minidumpapiset-minidump_exception_stream?branch=master)
#### [MINIDUMP_FUNCTION_TABLE_DESCRIPTOR](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_function_table_descriptor?branch=master)
#### [MINIDUMP_FUNCTION_TABLE_STREAM](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_function_table_stream?branch=master)
#### [MINIDUMP_HANDLE_DATA_STREAM](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_handle_data_stream?branch=master)
#### [MINIDUMP_HANDLE_DESCRIPTOR](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_handle_descriptor?branch=master)
#### [MINIDUMP_HANDLE_DESCRIPTOR_2](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_handle_descriptor_2?branch=master)
#### [MINIDUMP_HANDLE_OBJECT_INFORMATION](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_handle_object_information?branch=master)
#### [MINIDUMP_HANDLE_OPERATION_LIST](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_handle_operation_list?branch=master)
#### [MINIDUMP_HEADER](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_header?branch=master)
#### [MINIDUMP_INCLUDE_MODULE_CALLBACK](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_include_module_callback?branch=master)
#### [MINIDUMP_INCLUDE_THREAD_CALLBACK](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_include_thread_callback?branch=master)
#### [MINIDUMP_IO_CALLBACK](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_io_callback?branch=master)
#### [MINIDUMP_LOCATION_DESCRIPTOR](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_location_descriptor?branch=master)
#### [MINIDUMP_MEMORY_DESCRIPTOR](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_memory_descriptor?branch=master)
#### [MINIDUMP_MEMORY_INFO](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_memory_info?branch=master)
#### [MINIDUMP_MEMORY_INFO_LIST](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_memory_info_list?branch=master)
#### [MINIDUMP_MEMORY_LIST](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_memory64_list?branch=master)
#### [MINIDUMP_MISC_INFO](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_misc_info?branch=master)
#### [MINIDUMP_MISC_INFO_2](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_misc_info_2?branch=master)
#### [MINIDUMP_MODULE](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_module?branch=master)
#### [MINIDUMP_MODULE_CALLBACK](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_module_callback?branch=master)
#### [MINIDUMP_MODULE_LIST](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_module_list?branch=master)
#### [MINIDUMP_READ_MEMORY_FAILURE_CALLBACK](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_read_memory_failure_callback?branch=master)
#### [MINIDUMP_STRING](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_string?branch=master)
#### [MINIDUMP_SYSTEM_INFO](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_system_info?branch=master)
#### [MINIDUMP_THREAD](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_thread?branch=master)
#### [MINIDUMP_THREAD_CALLBACK](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_thread_callback?branch=master)
#### [MINIDUMP_THREAD_EX](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_thread_ex?branch=master)
#### [MINIDUMP_THREAD_EX_CALLBACK](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_thread_ex_callback?branch=master)
#### [MINIDUMP_THREAD_EX_LIST](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_thread_ex_list?branch=master)
#### [MINIDUMP_THREAD_INFO](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_thread_info?branch=master)
#### [MINIDUMP_THREAD_INFO_LIST](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_thread_info_list?branch=master)
#### [MINIDUMP_THREAD_LIST](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_thread_list?branch=master)
#### [MINIDUMP_UNLOADED_MODULE](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_unloaded_module?branch=master)
#### [MINIDUMP_UNLOADED_MODULE_LIST](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_unloaded_module_list?branch=master)
#### [MINIDUMP_USER_STREAM](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_user_stream?branch=master)
#### [MINIDUMP_USER_STREAM_INFORMATION](/windows/win32/minidumpapiset/ns-minidumpapiset-_minidump_user_stream_information?branch=master)
#### [MODLOAD_CVMISC](/windows/win32/DbgHelp/ns-dbghelp-_modload_cvmisc?branch=master)
#### [MODLOAD_DATA](/windows/win32/DbgHelp/ns-dbghelp-_modload_data?branch=master)
#### [OMAP](/windows/win32/Dbghelp/ns-dbghelp-_omap?branch=master)
#### [SOURCEFILE](/windows/win32/DbgHelp/ns-dbghelp-_sourcefile?branch=master)
#### [SRCCODEINFO](/windows/win32/DbgHelp/ns-dbghelp-_srccodeinfo?branch=master)
#### [STACKFRAME64](/windows/win32/DbgHelp/ns-dbghelp-_tagstackframe?branch=master)
#### [STACKFRAME_EX](/windows/win32/DbgHelp/ns-dbghelp-_tagstackframe_ex?branch=master)
#### [SYMBOL_INFO](/windows/win32/DbgHelp/ns-dbghelp-_symbol_info?branch=master)
#### [SYMSRV_INDEX_INFO](/windows/win32/Dbghelp/ns-dbghelp-symsrv_index_info?branch=master)
#### [TI_FINDCHILDREN_PARAMS](/windows/win32/DbgHelp/ns-dbghelp-_ti_findchildren_params?branch=master)
### [Image Help Library](image-help-library.md)
#### [About ImageHlp](about-imagehlp.md)
##### [PE Format](pe-format.md)
##### [Image Access Functions](image-access-functions.md)
##### [ImageHlp Image Integrity Functions](image-integrity-functions.md)
##### [ImageHlp Image Modification Functions](image-modification-functions.md)
#### [ImageHlp Reference](imagehlp-reference.md)
##### [ImageHlp Functions](imagehlp-functions.md)
###### [BindImage](/windows/win32/Imagehlp/nf-imagehlp-bindimage?branch=master)
###### [BindImageEx](/windows/win32/Imagehlp/nf-imagehlp-bindimageex?branch=master)
###### [CheckSumMappedFile](/windows/win32/Imagehlp/nf-imagehlp-checksummappedfile?branch=master)
###### [DigestFunction](/windows/win32/Imagehlp/nc-imagehlp-digest_function?branch=master)
###### [GetImageConfigInformation](/windows/win32/Imagehlp/nf-imagehlp-getimageconfiginformation?branch=master)
###### [GetImageUnusedHeaderBytes](/windows/win32/Imagehlp/nf-imagehlp-getimageunusedheaderbytes?branch=master)
###### [ImageAddCertificate](/windows/win32/Imagehlp/nf-imagehlp-imageaddcertificate?branch=master)
###### [ImageEnumerateCertificates](/windows/win32/Imagehlp/nf-imagehlp-imageenumeratecertificates?branch=master)
###### [ImageGetCertificateData](/windows/win32/Imagehlp/nf-imagehlp-imagegetcertificatedata?branch=master)
###### [ImageGetCertificateHeader](/windows/win32/Imagehlp/nf-imagehlp-imagegetcertificateheader?branch=master)
###### [ImageGetDigestStream](/windows/win32/Imagehlp/nf-imagehlp-imagegetdigeststream?branch=master)
###### [ImageLoad](/windows/win32/Imagehlp/nf-imagehlp-imageload?branch=master)
###### [ImageRemoveCertificate](/windows/win32/Imagehlp/nf-imagehlp-imageremovecertificate?branch=master)
###### [ImageUnload](/windows/win32/Imagehlp/nf-imagehlp-imageunload?branch=master)
###### [MapAndLoad](/windows/win32/Imagehlp/nf-imagehlp-mapandload?branch=master)
###### [MapFileAndCheckSum](/windows/win32/Imagehlp/nf-imagehlp-mapfileandchecksuma?branch=master)
###### [ReBaseImage](/windows/win32/Imagehlp/nf-imagehlp-rebaseimage?branch=master)
###### [ReBaseImage64](/windows/win32/Imagehlp/nf-imagehlp-rebaseimage64?branch=master)
###### [SetImageConfigInformation](/windows/win32/Imagehlp/nf-imagehlp-setimageconfiginformation?branch=master)
###### [SplitSymbols](/windows/win32/Imagehlp/nf-imagehlp-splitsymbols?branch=master)
###### [StatusRoutine](/windows/win32/Imagehlp/nc-imagehlp-pimagehlp_status_routine?branch=master)
###### [TouchFileTimes](/windows/win32/Imagehlp/nf-imagehlp-touchfiletimes?branch=master)
###### [UnMapAndLoad](/windows/win32/Imagehlp/nf-imagehlp-unmapandload?branch=master)
###### [UpdateDebugInfoFile](/windows/win32/Imagehlp/nf-imagehlp-updatedebuginfofile?branch=master)
###### [UpdateDebugInfoFileEx](/windows/win32/Imagehlp/nf-imagehlp-updatedebuginfofileex?branch=master)
##### [ImageHlp Structures](imagehlp-structures.md)
###### [IMAGE_COFF_SYMBOLS_HEADER](/windows/win32/WinNT/ns-winnt-_image_coff_symbols_header?branch=master)
###### [IMAGE_DATA_DIRECTORY](/windows/win32/WinNT/ns-winnt-_image_data_directory?branch=master)
###### [IMAGE_DEBUG_DIRECTORY](/windows/win32/WinNT/ns-winnt-_image_debug_directory?branch=master)
###### [IMAGE_FILE_HEADER](/windows/win32/WinNT/ns-winnt-_image_file_header?branch=master)
###### [IMAGE_FUNCTION_ENTRY](/windows/win32/WinNT/ns-winnt-_image_function_entry?branch=master)
###### [IMAGE_LOAD_CONFIG_DIRECTORY64](/windows/win32/WinNT/ns-winnt-_image_load_config_directory32?branch=master)
###### [IMAGE_NT_HEADERS](/windows/win32/WinNT/ns-winnt-_image_nt_headers?branch=master)
###### [IMAGE_OPTIONAL_HEADER](/windows/win32/WinNT/ns-winnt-_image_optional_header?branch=master)
###### [IMAGE_SECTION_HEADER](/windows/win32/WinNT/ns-winnt-_image_section_header?branch=master)
# [Structured Exception Handling](structured-exception-handling.md)
## [About Structured Exception Handling](about-structured-exception-handling.md)
### [Exception Handling](exception-handling.md)
#### [Exception Dispatching](exception-dispatching.md)
#### [Debugger Exception Handling](debugger-exception-handling.md)
#### [Floating-Point Exceptions](floating-point-exceptions.md)
### [Frame-based Exception Handling](frame-based-exception-handling.md)
### [Vectored Exception Handling](vectored-exception-handling.md)
### [Termination Handling](termination-handling.md)
### [Handler Syntax](handler-syntax.md)
#### [Exception-Handler Syntax](exception-handler-syntax.md)
#### [Termination-Handler Syntax](termination-handler-syntax.md)
## [Using Structured Exception Handling](using-structured-exception-handling.md)
### [Using an Exception Handler](using-an-exception-handler.md)
### [Using a Termination Handler](using-a-termination-handler.md)
### [Using a Vectored Exception Handler](using-a-vectored-exception-handler.md)
## [Structured Exception Handling Reference](structured-exception-handling-reference.md)
### [Structured Exception Handling Functions](structured-exception-handling-functions.md)
#### [AbnormalTermination](abnormaltermination.md)
#### [AddVectoredContinueHandler](/windows/win32/WinBase/?branch=master)
#### [AddVectoredExceptionHandler](/windows/win32/WinBase/?branch=master)
#### [GetExceptionCode](getexceptioncode.md)
#### [GetExceptionInformation](getexceptioninformation.md)
#### [RaiseException](/windows/win32/WinBase/?branch=master)
#### [RaiseFailFastException](/windows/win32/WinBase/?branch=master)
#### [RemoveVectoredContinueHandler](/windows/win32/WinBase/?branch=master)
#### [RemoveVectoredExceptionHandler](/windows/win32/WinBase/?branch=master)
#### [RtlAddFunctionTable](/windows/win32/WinNT/nf-winnt-rtladdfunctiontable?branch=master)
#### [RtlAddGrowableFunctionTable](/windows/win32/WinNT/nf-winnt-rtladdgrowablefunctiontable?branch=master)
#### [RtlCaptureContext](/windows/win32/WinNT/nf-winnt-rtlcapturecontext?branch=master)
#### [RtlDeleteFunctionTable](/windows/win32/WinNT/nf-winnt-rtldeletefunctiontable?branch=master)
#### [RtlDeleteGrowableFunctionTable](/windows/win32/WinNT/nf-winnt-rtldeletegrowablefunctiontable?branch=master)
#### [RtlGrowFunctionTable](/windows/win32/WinNT/nf-winnt-rtlgrowfunctiontable?branch=master)
#### [RtlInstallFunctionTableCallback](/windows/win32/WinNT/nf-winnt-rtlinstallfunctiontablecallback?branch=master)
#### [RtlRestoreContext](/windows/win32/WinNT/nf-winnt-rtlrestorecontext?branch=master)
#### [SetUnhandledExceptionFilter](/windows/win32/WinBase/?branch=master)
#### [UnhandledExceptionFilter](/windows/win32/WinBase/?branch=master)
#### [VectoredHandler](/windows/win32/WinNT/nc-winnt-pvectored_exception_handler?branch=master)
### [Structured Exception Handling Structures](structured-exception-handling-structures.md)
#### [EXCEPTION_POINTERS](/windows/win32/WinNT/ns-winnt-_exception_pointers?branch=master)
#### [EXCEPTION_RECORD](/windows/win32/WinNT/ns-winnt-_exception_record?branch=master)
# [Wait Chain Traversal](wait-chain-traversal.md)
## [Using WCT](using-wct.md)
## [WCT Reference](wct-reference.md)
### [CloseThreadWaitChainSession](/windows/win32/Wct/nf-wct-closethreadwaitchainsession?branch=master)
### [GetThreadWaitChain](/windows/win32/Wct/nf-wct-getthreadwaitchain?branch=master)
### [OpenThreadWaitChainSession](/windows/win32/Wct/nf-wct-openthreadwaitchainsession?branch=master)
### [RegisterWaitChainCOMCallback](/windows/win32/Wct/nf-wct-registerwaitchaincomcallback?branch=master)
### [WAITCHAIN_NODE_INFO](/windows/win32/Wct/ns-wct-_waitchain_node_info?branch=master)
### [PWAITCHAINCALLBACK](/windows/win32/Wct/nc-wct-pwaitchaincallback?branch=master)
# [Intel AVX](avx-support-portal.md)
## [Working with XState Context](working-with-xstate-context.md)
## [AVX Functions](avx-functions.md)
### [CopyContext](/windows/win32/WinBase/nf-winbase-copycontext?branch=master)
### [GetEnabledXStateFeatures](/windows/win32/WinBase/nf-winbase-getenabledxstatefeatures?branch=master)
### [GetXStateFeaturesMask](/windows/win32/WinBase/nf-winbase-getxstatefeaturesmask?branch=master)
### [InitializeContext](/windows/win32/WinBase/nf-winbase-initializecontext?branch=master)
### [LocateXStateFeature](/windows/win32/WinBase/nf-winbase-locatexstatefeature?branch=master)
### [SetXStateFeaturesMask](/windows/win32/WinBase/nf-winbase-setxstatefeaturesmask?branch=master)
