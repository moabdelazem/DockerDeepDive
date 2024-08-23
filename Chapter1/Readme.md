# Chapter 1 - Container History

Applications are the powerhouse of every modern business. When applications break,
businesses break.
Most applications run on servers, and in the past, we were limited to running one
application per server. As a result, the story went something like this:
Every time a business needed a new application, it had to buy a new server. Unfortunately, we weren’t very good at modeling the performance requirements of new
applications, and the IT departments had to guess
This often resulted in businesses buying very expensive servers with a lot more performance capability than the apps needed.

As soon as VMware came along, the world became much better. We finally had a
technology that allowed us to safely run multiple business applications on a single
server. But, and there’s always a but! As great as VMs are, they’re far from perfect.

A feature of the VM model is every VM needing its own dedicated operating system
(OS). Unfortunately, this has several drawbacks, including:

- Every OS consumes CPU, RAM, and other resources we’d rather use on applications
- Every VM and OS needs patching
- Every VM and OS needs monitoring

VMs are also slow to boot and not very portable.

A feature of the container model is that every container shares the OS of the host it’s
running on. This means a single host can run more containers than VMs. For example,
a host that can run 10 VMs might be able to run 50 containers, making containers far
more efficient than VMs.

Docker was the magic that made Linux containers easy and brought them to the masses.
We’ll talk a lot more about Docker in the next chapter.

Windows containers run Windows apps and require a host system with a Windows kernel.
Windows 10, Windows 11, and all modern versions of Windows Server natively support
Windows containers.

Windows systems can also run Linux containers via the WSL 3 (Windows Subsystem for
Linux) subsystem.

However, despite all the work developing Windows containers, almost all containers are
Linux containers. This is because Linux containers are smaller and faster, and more
tooling exists for Linux.

## Chapter Summary

We used to live in a world where every time the business needed a new application,
we had to buy a brand-new server. VMware came along and allowed us to drive more
value out of new and existing servers. However, following the success of VMware and
hypervisors came a newer, more efficient, and portable virtualization technology called
containers. However, containers were complex and hard to implement until Docker came
along and made them easy. WebAssembly is powering a third wave of cloud computing,
but Docker and the container ecosystem are evolving to work with WebAssembly, and
the book has an entire chapter dedicated to Docker and WebAssembly.
