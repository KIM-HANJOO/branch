# branch
***
                                                       < Input >  

string = '[m] clothes [s] shirts [s] pants [ss] denim [sss] tapered [s] accessories [m] coffee [s] espresso [s] latte [m] Python [s] branch [ss] init_theme'  
              
***

                                  < branch >                                < branch using theme >
                            
                                                                                - Theme_korean -
                                .                                              .                                               
                                ├─clothes                                      ㅏㅡclothes 
                                │  ├─shirts                                    ㅣ  ㅏㅡshirts  
                                │  ├─pants                                     ㅣ  ㅏㅡpants   
                                │  │  └─denim                                  ㅣ  ㅣ  ㄴㅡdenim  
                                │  │     └─tapered                             ㅣ  ㅣ     ㄴㅡtapered   
                                │  └─accessories                               ㅣ  ㄴㅡaccessories   
                                │                                              ㅣ                     
                                ├─coffee                                       ㅏㅡcoffee     
                                │  ├─espresso                                  ㅣ  ㅏㅡespresso    
                                │  └─latte                                     ㅣ  ㄴㅡlatte  
                                │                                              ㅣ          
                                └─Python                                      ㄴㅡPython      
                                   └─branch                                      ㄴㅡbranch       
                                      └─init_theme                                  ㄴㅡinit_theme 

***                                       
                   
                                                         < Code >  
                                                       
    - branch -                                                  - branch using theme -
    
    branched_string = brn.branch(string)                        themed_str = brn.branch_theme('theme_korean()', string)
    
    
    
    
    *you can also make your own theme, and replace 'theme_korean()' to the name of your defined theme function
    
***

                                                     < How to import >  
    import sys
    sys.path.append(*location(dir) of branch.py*)
    import branch as brn

***
