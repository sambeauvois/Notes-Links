##Windows 10 apps

Projet *Centenial* : MSI --> APPX

Projet *Astoria* : Android -> APPX

Projet *ISLANDWOOD* : IOS --> APPX

Projet *Westminster* : Website --> APPX

On peut avoir un store "private" pour entreprises

===> Summer 2015


##C# 6

https://github.com/dotnet/roslyn

"a bunch of little new featutes that we hadn't had time to add in previous versions"

https://github.com/dotnet/roslyn/wiki/Languages-features-in-C%23-6-and-VB-14

- nameof
- using static
- string interpolation : $"{propname}"
- null propagation
- element init : Dictionaries
- exception filters : try catch *when* (changed from "if")
- Automatic properties : readonly, default structures. immutable data structure
- override ToString()=>$"{}"; 
- await in finally block


FXCop/StyleCop -> peuvent être remplacés par Roslyn

Tip : Visual studio: File, open solution : select an "exe"

See discussions for c#7 : https://github.com/dotnet/roslyn/labels/Language-C%23
=> include team's meeting minutes

------

##Ecmascript 6

Keywords and features:
- 'let' : like 'var' but in a scope
- const
- default arguments for 'undefined' (not 'null')
- Template litterals : ", ', and now ` : `hello ${name}`
- let somevalues=[1,2,3]   ...somevalues
- let numbers=[1,2]; let [x,y] = numbers;
- 

Classes

let Dev = function()

becomes ==> 

class Dev{
 constructor (param){
 }
 
 DoWork(){
 }
 
 getName(){
  }
setName(name){
}

}

class xxx extends Dev

 
 module  = namespace ==> Scope
 
 
 -- import {class1, class2} from "module.js"
-- import * as m from "module.js"

any.foreach(dev=> {});

for(let x of xx){ ==> == foreach
}


yield

promises

for now :
ecmascript 6 -> transpile 

google traceyr
babel
typescript

Ecmascript 6 is now Ecmascript 2015 (future versions : 2017, 2020, ...)


##EF7

Complete rewrite

1st release will be a preview (to be shipped with asp.net 5)

new : 

- Context.Add
- Context.AddRange
- Batch CUD (default batch size : 100 items -> configurable)
- Unique constraints
- Functions in queries
- TypeConversions
- Default Database values
- Shadow states (additional propertines that context pocos)
- Disconected graphes
- 


##Typescript

- module-> namespace
- class
- interface
- enum
- type (gives a real intellisense)
- lambdas (x=> {})
- generics
- for
- arrays
- 


VS2013 transpile
VS2015 needs gulp task


##DDD

Books : 
- Domain Driven Design by Eric Evans : reference
- Implementing Domain Driven Design by Vaughn Vernon

Twitter : @DDDBE


'Guard.Against<ex>(condition)'

##MS BAND

##DDD for DB driven mind

Check 'front desk solution' on github : https://github.com/julielerman/TEE14Demo ?


##Chrome developer tools

https://developer.chrome.com/devtools/docs/tips-and-tricks#console-table

- Search : css selector
- Find in styles
- Shift+Click on color selector --> Color picker on the html page
- JS sources : ctrl + P -> open a search box
- ctrl + shift + p -> open a search box for method search
- break point on function  -> link on source
- modify code, then save to test the code
- right-click -> local modification : chrome session actions 
 

Console :

````
console.groupColapsed("xxx");
console.log("...");
/// ... more console
console.groupEnd("xxx");

````

```
console.time("xxx");
// dowork
console.timeEnd("xxx");
```

console.log("xx",object);

console.table(array);
console.table(array,["col1", "col2"]);

console.log("%C txt","color:blue");

console.count("xxx");


Editor:
document.body.contenteditable : true|false; --> edit in page --> test for translations or text adaptations

callstack
-> filtrable : right click, blackbox script

settings

console : show timestamps

if dev tools are open : right click on the refresh button

Device emulation :
-> network connection : offline, gprs, 3G, ....)

network tab 
-> blue line : document is ready
orange : image + frames are loaded

time :

black : load time
gray : network latency

size : gzipped or not

right click on network grid

filter (funnel icon)

right click : save as "har with context" -->  chrome har viewer

Timeline :
Record
Do action a few times (at least 3)
click on "collect garbage" (a few times)
stop record
Nodes -> if like stairs -> memory leak !


//// More
http://peterkellner.net/2015/05/25/magic-in-chrome-javascript-debugger/

## metaprograming .NET


yield break; -> to check 


switch snippet ;-)

Enumerable.Repeat

Check reactive extentions on github.






