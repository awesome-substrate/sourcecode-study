# initial phase code study

1. main fun node/scr/main.js

2. construct_service_factory!
  this macro is the key to start all required service, to find all service, search executor.spawn. 
  all them run tokio runtime
  
    **start_aura** core/consensus/aura/lib.rs
  
    this mehtod is called in AuthoritySetup of the macro
    * consensus entry point
    
    * proposal 
      core/service/src/consensus.rs
    
    **start_thread** network
    
    this is called a part of new newwork service. it is inited in the FullService of the macro
  
3. main loop fn run_until_exit node/cli/lib.rs
