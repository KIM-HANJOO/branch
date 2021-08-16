# BRANCH
**BRANCH is a user module** for expressing vertical / horizontal relationship between objects  
inspired by directory branches, **no additional libraries needed (acts only with lists)**
  
***   
<p align="center">
  <img src="https://github.com/suhyuuk/branch/blob/main/example_gif.gif"  img width="800px"/>
<p/>

***   

#### different themes and theme customization are also available !  

<p align="center">
  <img src="https://github.com/suhyuuk/branch/blob/main/theme_example.gif"  img width="800px"/>
<p/>

***
  
<div align="center">
< How to use >
</div>

                                                     
                                                     
1. branch making is only based on the bracketed sign and the sequence you write.
    
2. [m] is for the top level titles, in this example, are 'clothes', 'coffee', 'Python'.
    
3. [s] is sub-level of [m], [ss] is sub-level of [s], 
       continously, [sss] is sub-level of [ss]..
       
4. the shape of the branch will be automatically made
   
    
***   
~~~                     

                                                       < Input >  
                                                       
    string = '[m] clothes [s] shirts [s] pants [ss] denim [sss] tapered [s] accessories [m] coffee [s] espresso [s] latte [m] Python [s] branch [ss] init_theme'   
              
~~~
                                                 
                                      < Result >  
                                      
                                      - Default -                      
                                                                                           
                                     .                                    
                                     ├─clothes                            
                                     │  ├─shirts                              
                                     │  ├─pants                       
                                     │  │  └─denim                            
                                     │  │     └─tapered                          
                                     │  └─accessories                     
                                     │                                     
                                     ├─coffee                              
                                     │  ├─espresso                        
                                     │  └─latte                           
                                     │                                    
                                     └─Python                                
                                        └─branch                             
                                           └─init_theme         
                           
                      
***                   
 
                                      < Themes >  
                           
                           
                           
             - Larva race theme -                        - Korean -                      
                                                                                
                Larva race! 
                                                           .                               
                ...෴                                    ㅏㅡclothes                      
                   ...෴                                 ㅣ  ㅏㅡshirts                   
                   ...෴                                 ㅣ  ㅏㅡpants                    
                      ...෴                              ㅣ  ㅣ  ㄴㅡdenim                
                         ...෴                           ㅣ  ㅣ     ㄴㅡtapered           
                   ...෴                                 ㅣ  ㄴㅡaccessories              
                                                          ㅣ                               
                ...෴                                    ㅏㅡcoffee                       
                   ...෴                                 ㅣ  ㅏㅡespresso                 
                   ...෴                                 ㅣ  ㄴㅡlatte                    
                                                          ㅣ                               
                ...෴                                    ㄴㅡPython                       
                   ...෴                                    ㄴㅡbranch                    
                      ...෴                                    ㄴㅡinit_theme             
                          

***                                         
<div align="center">
< How to import > 
</div>
  
~~~                                                       
    import sys
    sys.path.append(*location(dir) of branch.py*)
    import branch as brn
~~~

<div align="center">
< How to re-import >  
</div>  
  
~~~                                                      
    from imp import reload 
    reload(brn) 
~~~
  
<div align="center">
< Code >  
</div>  
  
~~~                                                  
  import sys
  sys.path.append(%%your branch location%%)
  import branch as brn

  string = '[m] clothes [s] shirts [s] pants [ss] denim [sss] tapered [s] accessories \
            [m] coffee [s] espresso [s] latte \
            [m] Python [s] branch [ss] init_theme'

  default = brn.branch(string)
  theme_larva = brn.branch_theme('larva', string)
  theme_korean = brn.branch_theme('theme_korean', string)     
~~~
* you can also make your own theme, and replace 'theme_korean()' to the name of your defined theme function

                                                    


