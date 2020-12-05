# code smells 101    
## the goals of refactoring is apply more changes with less effort       


### 1.bloaters (kill big)   
<table  border="1">
  <tr>
    <td>#</td>
    <td>name </td>
    <td>when </td>
    <td>how? </td>
  </tr>
  <tr>
    <td> 1 </td>
    <td> long method   </td>
    <td>  loc > 10 </td>
    <td> extract method      </td>
  </tr>
   <tr>
    <td> 2 </td>
    <td> large class </td>
    <td>  class methods length >10  </td> 
    <td> extract class       </td> 
  </tr>
   <tr>
    <td> 3 </td>
    <td> primitive obsession  </td>
    <td> Using primitives types instead of small objects. </td> 
    <td> extract to class/object        </td> 
  </tr>
  <tr>
    <td> 4 </td>
    <td> long parameter list  </td>
    <td> paramether length > 4  </td> 
    <td> extract to class/object         </td>
  </tr>
  <tr>
    <td> 5 </td>
    <td> data clumps  </td>
    <td>  different parts of the code contain identical groups of variables   </td> 
    <td> extract to class/object        </td>
  </tr>
</table>
    
> extract larges to container (object/class/function)

### 2.OOP abuser (kill big)   
<table  border="1">
  <tr>
    <td>#</td>
    <td>name </td>
    <td>when </td>
    <td>how? </td>
  </tr>
  <tr>
    <td> 1 </td>
    <td> alternative classes with different interfaces      </td>
    <td> classes have same behavior (interface)</td>
    <td> extract interface(class)      </td>
  </tr>
   <tr>
    <td> 2 </td>
    <td> refused bequest  </td>
    <td> The unneeded methods may simply go unused or be redefined and give off exceptions.   </td> 
    <td> delegation / extract super class       </td> 
  </tr>
   <tr>
    <td> 3 </td>
    <td> switch statements </td>
    <td> swtich statement with type checking inside for/if/... </td> 
    <td> extract to class/object  (state/strategy/iterator)      </td> 
  </tr>

  <tr>
    <td> 4 </td>
    <td> temporary field  </td>
    <td> some fields unused almost </td> 
    <td> extract to class/object         </td>
  </tr>

</table>

> use delegation of extract to class

### 3.change preventers    
    
    
     
<table  border="1">
  <tr>
    <td>#</td>
    <td>name </td>
    <td>when </td>
    <td>how? </td>
  </tr>
  <tr>
    <td> 1 </td>
    <td> divergent change      </td>
    <td> You find yourself having to change many unrelated methods when you make changes to a class.  </td>
    <td> extract class      </td>
  </tr>
   <tr>
    <td> 2 </td>
    <td> parallel inheritance hierarchies  </td>
    <td> make instance referer to hard composition   </td> 
    <td> use delegation for instance with composition       </td> 
  </tr>
   <tr>
    <td> 3 </td>
    <td> shotgun surgery</td>
    <td> swtich statement with type checking inside for/if/... </td> 
    <td> extract (super|sub) class     </td> 
  </tr>
</table>

 > extract or delegate   

### 4.dispensables    

<table  border="1">
  <tr>
    <td>#</td>
    <td>name </td>
    <td>when </td>
    <td>how? </td>
  </tr>
  <tr>
    <td> 1 </td>
    <td> comments     </td>
    <td> many unneeded comments  </td>
    <td> remove them      </td>
  </tr>
   <tr>
    <td> 2 </td>
    <td> duplicate code   </td>
    <td> duplicate code     </td> 
    <td> remove duplicate please        </td> 
  </tr>
   <tr>
    <td> 3 </td>
    <td> data class</td>
    <td> class in data container without any logic inside</td> 
    <td>    </td> 
  </tr>
   <tr>
    <td> 4 </td>
    <td> dead code  </td>
    <td> code without using some where</td> 
    <td> remove it :|     </td> 
  </tr>
  <tr>
    <td> 5 </td>
    <td> lazy class  </td>
    <td> code with little using </td> 
    <td> fire them     </td> 
  </tr>
    <tr>
    <td> 6</td>
    <td> speculative Generality  </td>
    <td> we will need it in future , so let it be </td> 
    <td> no need premature optimization , remove it    </td> 
  </tr>
    
</table> 

> remove extra unused/duplicate entities

### 5.couplers 

<table  border="1">
  <tr>
    <td>#</td>
    <td>name </td>
    <td>when </td>
    <td>how? </td>
  </tr>
  <tr>
    <td> 1 </td>
    <td> feature envy     </td>
    <td> method accesses the data of another object more than its own data. </td>
    <td> extract method | move method      </td>
  </tr>
   <tr>
    <td> 2 </td>
    <td> inappropriate intimacy  </td>
    <td> Keep a close eye on classes that spend too much time together. Good classes should know as little about each other as possible.      </td> 
    <td> move method | move field   </td> 
  </tr>
   <tr>
    <td> 3 </td>
    <td>incomplete library class</td>
    <td> Sooner or later, libraries stop meeting user needs. The only solution to the problem—changing the library—is often impossible since the library is read-only.</td> 
    <td> foriegn method | local extension   </td> 
  </tr>
   <tr>
    <td> 4 </td>
    <td> message chains  </td>
    <td> $a->b()->c()->d()</td> 
    <td> hide delegate | extract method     </td> 
  </tr>
   <tr>
    <td> 5 </td>
    <td> middle man  </td>
    <td> If a class performs only one action, delegating work to another class, why does it exist at all?</td> 
    <td> hide delegate | extract method     </td> 
  </tr>
</table>     

> extract reponsibilty or item    

# solution


**order of refactoring** 

                                    /-----container |delegate 
      variable -> method -> class -<-----interface | abstract
                                    \------inherience 

remove extra unused/duplicate entities 
- unused or duplicate

compose | extract | delegate   
- your x is large
- oop abuser(wrong interface request to others)
- change preventers(too many change applied behavior or same class)
- request for others( responsibity) 
- if request(access) is more than 50% of time, extract class otherwise delegate

