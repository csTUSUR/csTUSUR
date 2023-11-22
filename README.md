How to use git repository.
Folders structure:
  /LDPC_core
    /scripts                   -- You can store matalb, tcl, bash, etc. scripts in this folder
    /sim                       -- In this directory store sim sources and scripts
      /src                     -- Sources for simulation
      /include                 -- *.svh, *.vh, *_pkg.sv files. Folder to store headers and packages 
      /scripts                 -- Scripts for simulation
    /rtl                       -- This folder must contain all synthesys modules
      /example_core_v0         -- Folder of rtl instance. 
        /src                   -- Sources for example_core_v0 iplementation
        /sim                   -- Folder must contain simulations sources and scripts for this instance
        /include
        /scriptrs
        /docs                  -- Manuals for core
      /...
    /docs

    Rules:
    1. You can't commit or push in main branch
    2. For each new instance developer must create new branch 
    3. Name of this branch and task in Yougile must be same
    4. After full creating and debug new instance developer must create merge request
    5. Rewiever on berge request is csTUSUR.
