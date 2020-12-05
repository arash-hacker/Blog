# design-pattern-all-in-one-blog
1. generate object (creation)   
2. get object property with structure (structural)   
3. get behavior against other (behavioral)  
____________
## creational 
### generate with partial generator   
1.prototype(clone)  
2.singleton      
3.builder(direcotr with builder)   
4.factory  
5.abstract factory   
_____________________
## structural  
### f[h . i . j . k ....]*g () == f.g() | f.h.i.j.g() | f.h.i...g()  
### get inner structure (input types) 


input types (x, f(), class, monad, 3rdParty)    
output types  [x,x,x,..] | x | Nullify(x)  

1.adaptor (transform input one step, so change input structure from base)    
2.decorator (map reduce filter with input serilized (more than one step), doesn't change input structur)     
3.facade (decorate middleware for new release)    
4.proxy (middleware for access function) **HOC**     
5.fly weight (extract common structure for optimize memory)     
  |     
  |--extract common     
  |     
6.bridge ( split a large class or a set of closely related )        
7.composite (access with hierarchies)       
8.**nullify** possible with null checking    
9.**arraify** possible with map functor  

## behavior  
#### how act a server with other (client(s)|server(s))   
1.chain of responsiblity (with manually set order of operation)       
2.template (with hardcoded order of operation)  



3.iterator (just getnext() and hasMore() implimented. sort of childs can be BFS,DFS,SJF,...)          
4.mediator(one server , many clients . **all** must be connected to server, unidirection with server, child to child communicate is not possible)      
5.observer(one server, many client, **some** of them can subscribe to server, bidirection with server, child can connect together)      
6.memnto(cache)     
7.state     
8.strategy   
9.command   
10.visitor(logic handler is parent, child can't override)      
11.composite like(login handler is child)    
12.**pre-do-post** categorize actions in just 3 part(validate,process,serialize)   


# distributed
** comming soon ??? **   

___________________
# summary   
## behavior request action types  
> one server **with** many clients(server contains them,(clients are server's child))     
> many clients outside **to** one server(server is not container of clients|child)    
> one to one   

## behavior many types connected together     
> graph(each client can connect directly with other clients)       
> tree(server connect like tree to childs(clients) ,so no way each client to other client directly)         


<table  border="1">
  <tr>
    <td>**`#`**</td>
    <td>**request types** </td>
    <td>**many types **</td>
    <td>**which to use?** </td>
  </tr>
  <tr>
    <td> 1 </td>
    <td> one to many </td>
    <td> tree      </td>
    <td>visitor - logic owner is parent </td>
  </tr>
   <tr>
    <td> 2 </td>
    <td> one to many  </td> 
    <td> tree       </td> 
    <td>    compisite -logic owner is child  </td>
  </tr>
   <tr>
    <td> 3 </td>
    <td> one to many  </td> 
    <td> tree       </td> 
    <td>   iterator-like above,but diff in getNext,hasNext method strategy  </td>
  </tr>
  <tr>
    <td> 4 </td>
    <td> one to many  </td> 
    <td> star       </td>
    <td>   mediator - one direction communicate with server </td>
  </tr>
   <tr>
    <td> 5 </td>
    <td> one to many </td> 
    <td> graph       </td> 
    <td>  observer - childs communicate with childs maybe directly  </td>
  </tr>
</table>
________________________
<table border="1">
  
  <tr>
    <td>**`#`**</td>
    <td>**request types **</td>
    <td>** server has state?**  </td>
    <td>**which to use?** </td>
  </tr>
  <tr>
    <td> 1 </td>
    <td> many to one </td>
    <td> true      </td>
    <td>cache(memento) </td>
  </tr>
   <tr>
    <td> 2 </td>
    <td> many to one  </td> 
    <td> true       </td> 
    <td>   strategy </td>
  </tr>
  <tr>
    <td> 3 </td>
    <td> many to one  </td> 
    <td> true      </td> 
    <td>   state </td>
  </tr>
   <tr>
    <td> 4 </td>
    <td> many to one </td> 
    <td> false       </td> 
    <td>  command(just pure functions) </td>
  </tr>
</table>

_________

<table border="1">
  
  <tr>
    <td>**`#`**</td>
    <td>**request types **</td>
    <td>**server has order? ** </td>
    <td>**which to use?** </td>
  </tr>
  <tr>
    <td> 1 </td>
    <td> one to one </td>
    <td> true      </td>
    <td> chain of responsibility -just define chain functor and connect to next chain </td>
  </tr>
   <tr>
    <td> 2 </td>
    <td> one to one  </td> 
    <td> false       </td> 
    <td>   template - every part can be done random (just replace virtual method)  </td>
  </tr>
  <tr>
    <td> 3 </td>
    <td> one to one  </td> 
    <td> true maybe false     </td> 
    <td>   **pre-process-post** </td>
  </tr>
   <tr>
    <td> 4 </td>
    <td> one to one </td> 
    <td> false       </td> 
    <td>  **dynamic pipeline (plugins)** add dynamic config like micro-kernel plugins </td>
  </tr>
</table>
     
chain of resposible -> 3 -> 1 -> `2`->    
template ->1 :heavy_check_mark: ->`2` :heavy_multiplication_x: ->3 :heavy_check_mark:->     
can user **nullify** or **arraify** within step `2`    
dynamic pipeline ->4,5,6 || 3,2,1 || 7,1,8,9,5,3,3,1     











