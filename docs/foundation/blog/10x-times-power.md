# 10 times power savings, is this possible?
![Logo](img/10x-times-power.jpg?raw=true "Logo")
### How does ThreeFold achieve the efficient power usage in the Zero-OS node?

Today, global Internet and IT infrastructure require enormous amounts of energy far higher than the entire annual electricity consumption of the United Kingdom and it ranks among the most pollutive industries globally (similar to that of airlines).

We believe IT can do a lot better. In fact, we believe we can reduce the Internet’s carbon footprint drastically compared to other industry standard IT capacity producing solutions.

Power consumption is a function of better compute and storage performance requiring more racks and more cooling.

Our solutions achieve roughly 3 times the performance per rack (so we use fewer racks), and the racks require less energy than typical racks in the industry. 


### Less = More


#### Keep it simple 

Over time, integration suites, middleware solutions, enterprise service busses have been invented and implemented to cover integration challenges. This has further complicated IT architectures and has resulted in loss of actual end user workload performance. By eliminating these layers of complexity, the resulting cloud stack presents minimal overhead and therefore requires less hardware which results in lower heat generation and eventually requiring less cooling. By producing less power, the net result is a total energy consumption decreases drastically. 

#### Self-Healing

Keeping things up and running is a business model in modern day IT.  Major vendors earn most of their margin by selling maintenance contracts, performance guarantees, and professional services. Given their business model, there is little to no incentive to make things simple and efficient. Creating a self-healing environment requires minimal manual intervention to replace broken hardware components. Broken hardware components are inevitable, and the Zero-OS distributed node architecture deals with such failures by turning off broken components and provisioning unused capacity. Not having to ship broken parts back and forth together with the corresponding installation knowledge (engineers) means a much smaller carbon emission footprint.

#### “No painkiller” approach

If a specific piece of software or hardware is not delivering the required performance or reliability, we should analyze the core design/algorithm and its usage of soft/hard components to determine root causes of persistent issues and solve for that. Currently, most storage vendors follow the path of least resistance when trying to improve on performance, and their solution for meeting performance targets is to use faster components (CPU, memory, network card, proprietary acceleration) rather than looking at the core algorithms that drive the utilization of those components. Swapping components for faster ones perpetuates a cycle of cutting corners and focuses reliance on innovation from hardware component providers rather than solving the more fundamental and underlying issues.

By using these three principles, a Zero-OS node has a minimal power consumption footprint. Some key examples how this is achieved:

#### Minimise the number of context switches

Virtualization adds a layer of software between the actual end-user workload and physical hardware, but it also allows for multiple workloads to run on the same hardware using excess capacity.  There is definitely merit in building a virtualization solution. Building an effective virtualization solution that does not require abundant context switching is key and is why Zero-OS has been developed.  Zero-OS uses a minimal linux kernel that allows for a number of user spaces to co-exist. In these user spaces, containerised versions of software can be run, taking away the need to have a hypervisor and a virtual OS fueling the virtual machines. This minimises the required overhead for the host OS and takes away the need for a hypervisor and guest operating systems.

#### Minimise the use of network connections

Supercomputing delivered a large number of new technologies. But, not all of the current ones are very usable solutions for everyday workloads. One technology invented to make supercomputers powerful (fast) is the use of Remote Direct Memory Access (RDMA). RDMA allowed physical CPU boards (containing both CPUs and memory) to access other CPU boards in memory stored data over a dedicated channel. This eliminated the need to transport data between CPU nodes over network connections (or other mainstream means to exchange data). The result of this is that a lot less overhead was created to allow for distributed end user workloads to operate over multiple physical cores. The leading brands of server and storage solutions have never considered nor implemented such mechanisms which has increased the need for faster networks - increasing complexity, cost, effort and resources needed to operate the solution.

By using a different, more efficient means to exchange data between physical CPU units, we no longer require forests of switching gear.

#### Minimise the use of number of disks

The storage solution uses slow and big - the bigger the better - HDD disks which drive in rack density and as they spin slower they consume less power and need less cooling. How can you deal with read/write intensive workloads then? The storage algorithm uses a SSD cache to acknowledge I/O coming from the application, fills the erasure coded data blocks in large (up to 64MB) storage containers and writes these big chunks of data to the big and slow HHDs. If you are familiar with HDD disks, you know they like to be streamed on instead of a having a lot of small bits written to in scratchy way.

Continuous innovation in all of these areas have lead to a very efficient technology stack.
