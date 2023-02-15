# Design Patterns: 

• Design Patterns 
• Proxy
• Facade
• Null Object 
• Template
• Iterator
• What is an anti-pattern? 


## Proxy (addition behaviour) 
- 1. Put someone but restrict using proxy.. concerts/stadium (control access) (security, caching)  
- 2. 3 ways/types
- i) Remote => different namespace, server, (out of application)
- ii) Virtual => Virtual control access to a resource that expensive to create (caching) (lazy evaluation) (it’s costly so proxy takes care)
- iii) Protection => Access management -> only users allowed to access resources -> (roles, isAuthorized)
 
## Facade (Complexity) (Higher level interface)
- Client will interact with one class -> It will take care of other interacts and return the value. (Single responsibility principle)
- Talk only to your friends not your friends of friends (coupling)  
- A -> B -> C not friends but B can be interface.
- Exterior of the building (outside of the building) but still you need everything (plumbing, wiring, electric, walls, heater) 
- Unified Interface to set of interfaces 

## Null object 
- tony hoare - inventor of null -> million dollar mistake -> cause its binary 
- Null iterator, Null Command => implementation 
- Iterator should return something, If the leaf node has none. Then use Null iterator.
- Ok Cancel Dialog (command pattern) -> OkCommand & CancelCommand -> if can remove CancelCommand & cancel btn. And have NoCancel.
￼

## Template (Skeleton) (Not really a method but a template method)
- Template (some parts missing -> subclasses can add those)
- Poster Example 
- Filling PDF info => they care about the info and PDF (should not be created/ redesigned by each one)
- Poster template -> 3 clients -> remove duplicate code => template design 

## Iterator (Collections or enumeration)
* Without caring about the collections (just iterate through it)
* HasNext() getItem()

## Anti patterns: 
1. Job security cause no one knows that what you wrote.
2. Revenge (just watch the world burn) (legal code review passing coding)
3. Functions -> tiny functions  => spaghetti code => Code review (unit testable)
4. !! Usage in if condition 
5. Recursive -> iterator & iterator -> recursive 
6. Comments (Please don’t touch it)

## Mushrooms Management: 
- “Keep your developers in the dark and feed them fertilizer" 
- Silicon valley product demo to end users
- 30% of development cost. 
- Prototyping and user feedback (answers)

## Cut and paste Programming:
- “Hey, I thought you fixed that bug already, so why is it doing this again?" "Man, you guys work fast. Over 400,000 lines of code in three weeks is outstanding progress!"
- Refactor - subclasses, remove cut paste code.

## Walking through a Minefield
- Bug free (software testing)

## Input Kludge: 
- Failed behavioral test. (Stupid tester/PO)
- nondemonstration software, use production-quality algorithms. 

## Spaghetti:
- “Ugh! What a mess!" "You do realize that the language supports more than one function, right?" "It's easier to rewrite this code than to attempt to modify it."
- Code clean up

## Dead End: 
- No longer maintained and supported by the supplier.
- Customization & throw away code.

## Golden Hammer: 
- Explore New technology
- PoC or usage in on going project 

## Boat Anchor: 
- No purpose 

## Poltergeists: 
- Anecdotal Evidence: "I'm not exactly sure what this class does, but it sure is important!"
- Encapsulate and classes.

## Lava Flow: 
- “Oh that! Well Ray and Emil (they're no longer with the company) wrote that routine back when Jim (who left last month) was trying a workaround for Irene's input processing code (she's in another department now, too). I don't think it's used anywhere now, but I'm not really sure. Irene didn't really document it very clearly, so we figured we would just leave well enough alone for now. After all, the bloomin' thing works doesn't it?!"
* Frequent unjustifiable variables and code fragments in the system.
* Undocumented complex, important-looking functions, classes, or segments that don't clearly relate to the system architecture.
* Very loose, "evolving" system architecture.
* Whole blocks of commented-out code with no explanation or documentation.
* Lots of "in flux" or "to be replaced" code areas.
* Unused (dead) code, just left in.
* Unused, inexplicable, or obsolete interfaces located in header file
- An important principle is to avoid architecture changes during active development.
- it is important to establish system-level software interfaces that are stable, well-defined, and clearly documented

## The Blob: 
- “This is the class that is really the heart of our architecture."
- Single class with a large number of attributes
- Identify or categorize related attributes and operations
￼
￼ 
￼
