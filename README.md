# Infinite Memory Glitch Array - Probably useless

## What
A very large array, that only grows/shrinks based on the values inserted. Can store terabytes of data with fast insertion and access. This could have real applications such as:
- Paired with an intelligent entity-indexing strategy, technically this could be used to setup a very silly ECS with direct-index lookup of entity data.
- idk. fun probably

## How
Reserves all the memory you would ever need, but only commits as you insert data. 

## Features
Indexes just like a normal array, allowing very fast iteration and indexing. Allows you to fake the storage of terabytes of memory.

## Is this useful or even new?
Not really. Just kind of funny.
This is how memory is handled behind the scenes, this just adds the guarantee that allocated memory is contiguous.

## Resources

https://learn.microsoft.com/en-us/windows/win32/memory/memory-limits-for-windows-releases
- Talks about the limits of virtual memory and regular memory

https://learn.microsoft.com/en-us/windows-hardware/drivers/gettingstarted/virtual-address-spaces
- How it virtual memory works
