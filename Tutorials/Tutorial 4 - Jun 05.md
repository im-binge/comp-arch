## Virtual Memory
- Essentially, virtual memory refers to when traditional storage, like HDDs or SSDs are partly allocated to be used as memory.

- Physical addresses (PA) are the actual addresses used by the hardware to request reads/writes from/to RAM
- Virtual addresses (VA) are the addresses used by programmers/compilers to reference memory locations
- Translation between PAs and VAs is done by the memory management unit (MMU)

---
##### VM-related Terminology
- page:  A unit of memory (equivalent to a cache’s block)
- page hit:  When a program tries to access a virtual address within a page that is currently located in memory
- page fault:  When a program tries to access a virtual address within a page that is not currently located in memory
- swapped out:  When a page in memory is moved to disk
- swapped in:  When a page on disk is moved to memory
- fragmentation: refers to when files are stored non-continuously on a drive, harming performance. This is solved with virtual memory.

---

`no. of pages = process size/page size`
`page table size = no. of pages * page table entry size`

---

Consider a single level paging scheme. The virtual address space in 4 MB and page size is 4 KB. What is the maximum page table entry size possible such that the entire page table fits well in one page?

---

`no. of pages = process size / page size`
`= 4 MB/4 KB = 4 × 2^20 / 4 × 2^10 = 2^10 pages`

`table size = no. of pages * table entry size`
`4KB <= 2^10 * table entry size`
`4KB / 2^10 = table entre size`
`4 <= table entry size`

---

Two processes, A and B, share a common library loaded into physical memory, which occupies 10 pages. Given a system with 1 GB of physical memory and a page size of 8 KB, calculate the percentage of physical memory saved by sharing a library between the two processes instead of loading it separately into each process's address space.

`page size = 8 KB`
`library size = 10 * 8 KB = 80 KB`

`shared = 160 KB / 1 GB`
`not shared = 80 KB / 1 GB`

`not shared = 0.00016`
`shared = 0.00008`
`saved = 0.00008`

`percentage = 0.008%`

---

Consider a single‐level paging scheme where the virtual address space is **8 MB** and the page size is **4 KB**. What is the maximum page‐table‐entry (PTE) size (in bytes) such that the entire page table occupies exactly one page in physical memory?

`no. of pages = process size / page size`
`= 8 MB / 4 KB`
`8 * 2^20 / 4 × 2^10`
`2048 pages`

`table size = no. of pages * pte
`4 KB >= 2048 * pte`
`4 KB / 2048 <= pte`
`2 bytes <= pte`

---

Two processes, C and D, share a common library that occupies **20 pages** in physical memory. The system has **512 MB** of physical RAM, and the page size is **16 KB**. Calculate the percentage of physical memory saved by sharing this library between the two processes instead of loading it separately into each process’s address space.

`page size = 16 KB`
`library size = 20 pages * 16 KB = 320 KB`

`shared = 320 KB / 512 MB`
`not shared = 640 KB / 512 MB`

`saved = 640 KB / 512 MB = 0.00125`

`percentage saved = 0.125%`

---

It's a depiction of how Linux handles virtual memory.
The stack area handles functions and local variables.
The heap is used for dynamic allocation, and 'grows' towards the stack to reduce wasted space. Similarly, the stack grows towards the heap.
The offsets of the stack and heap are randomized to ward against malicious attacks on known data.