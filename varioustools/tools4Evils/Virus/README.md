Virus
===========

A simple virus via Autorum(Windows Autorun.inf 4 some kinds of drives)
4 the virus 
1. add new section
2. fill out the section
3. fix the PE
4. sets the new Entry Point


A payload trik
1. use some tech to run the codes
2. code reloc // #define RECODE(A) { _asm call A _asm A: _asm pop ebx _asm lea eas,A _asm sub ebx,eax}
3. get the kernel32
4. search API Addr(here loadlibrary)
4. use loadlibrary to load shell32.dll
5. now we could run ShellExecute (via GetProcAddress)


Self Del
1. get Process names
2. construction a cmd (del FileName > nul)
3. set Priority for self
4. CreateProcess (a Remote Thread)
5. set Priority Remote Thread