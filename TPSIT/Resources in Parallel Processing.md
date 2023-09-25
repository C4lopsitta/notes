# Resources
A resource is any hardware needed by a process to do what it's meant to do. It can be anything from RAM to CPU but also external devices such as Printers, Webcams or other devices.
Resources are divided in **classes** and resources in the same class are equivalent to eachother. An example can be a memory pool, printers of the same type, etc. A process cannot request a specific device or item from a class, it'll get one that is deemed good by the Operating System. Instances in these classes have a multiplicity that says how many processes can work on that resource instance simultaneously. To get a resource, unsurprisingly, the process has to request them.
There are issues with resources that can happen like **deadlock** or **starvation**.
Resources can be **static** or **dynamic**. Static resources are kept by the process from the start all the way to the end while dynamic ones are given and removed from a process continuously depending on if the process needs them at the moment or not.

| Resource organization planning | Resource control |
| ------------------------------ | -----------------| 
| Allocation                     | Optimization     |
| Availability                   | Authentication   |
| Cost | Checking of correct operation and exception |

## Resource - Process diagram
```mermaid
flowchart LR
A((Process))
B[Resource]

A <-.-> B
```
## Request classification
A request can be classified by the following methods:.
### Number
- Single
  A single request is the simple definition of a request for a single resource from one class that happens one at a time
- Multiple
CHECK ON BOOK PAGE 14

## Assignation classification
- Static
  The resource is kept by the process happens when the process is created and it's returned by it when it ends.
- Dynamic
  The process requests it when it needs it and returns it when it's not needed anymore.
## Resource classification
- Serial resource
  A serial resource cannot be given to multiple processes and each process that needs it gets queued to access it and gets it one at a time. This is called **mutually exclusive**. An example are printers.
- Non serial resources
  These can be used at the same time by multiple processes, such as read-only files.
- Preemptive resources
  Preemptive resources can be given back by the process before it ends execution because it doesn't need it for now, but it must be given back to the process that initially requested it. The process that takes it temporarily cannot modify it or edit anything about it.

## Common memory area cooperation
This ancient method of inter process communication works by declaring a memory area that can be used by multiple processes so that both can read or write on that memory area.
This is not a good idea.

