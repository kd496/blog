### Event loops

// 15.08.2023
Programs run sequentially from 'top to bottom', instruction after instruction, until no more instructions are there to execute. To be able to implement various programming concepts that by their nature require an indefinitely long running program (e.g. ~~asynchronous programming~~), ~~an infinite loop can be used that performs a desired action on each iteration. But this is a native approach that has it's downsides, hence the general notion of event loop exists.~~

Instead asynchronous programming I could simply say 'listening to events'.

Infinite loop is not quite simply a native approach. There's a more fundamental difference. An event-loop uses interrupt-driven I/O instead of polling. While, Until, For, etc. loops are polling loops.

Most event loops will suspend if there are no events ready, which means the operating system will not give the task any execution time until an event happens.

Every GUI application requires an event loop.
