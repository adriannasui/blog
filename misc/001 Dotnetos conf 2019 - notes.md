# Dotnetos conf 2019 was a cool learning experience  

![Oops...messed up some refs...a header image should be here](https://github.com/adriannasui/blog/blob/master/misc/resources/001_dotnetos_logo.png?raw=true "Dotnetos logo")  

The speakers were all very good, deeply technical but also had fun presentations. 
We learned a lot about performance profiling, common pitfalls, memory profiling, tips, tricks, and programming in C# for maximum efficiency. I made a short list of concepts, a summary, if you will, and it is listed below

Workshop (Nethermind Ethereum C# Client)
-
Net benchmarking   
Dot memory     
Dot trace   
Merkle trees   
Bloom filters   
Span<T>
MemoryMarshal.Cast<,>
PerfView

Conference - Day 1
-

Virtual stub dispatch     
The book of the runtime   
Dispatch stubs: monomorphic, polymorphic (Compare in benchmarking.net)   
Specialized struct generics rather than interface   
Value type - boxing/unboxing, JIT inlining, unboxing stubs  
Code versioning core CLR  

--- 
Recommended settings for profiling: disable tiered hit, run in release, enable symbols     
Visual studio profiler  
PerfView: flamegraph, other  
Dotnet trace with speedscope for view  

---
Intrisics net 3.0
Quicksort with intrinsics
[https://devblogs.microsoft.com/dotnet/using-net-hardware-intrinsics-api-to-accelerate-machine-learning-scenarios/](https://devblogs.microsoft.com/dotnet/using-net-hardware-intrinsics-api-to-accelerate-machine-learning-scenarios/)

---
EF core
Visitor pattern c#
Explicit compiled queries

---
andrey akinshin
Shift function for comparing performance degradation
Benchmark dotnet can be integrated in tests
Benchmarkdotnet exports R code, you can do plots from that

Day2
----
Async
Daniel Marbach github
CancellationToken, CancellationTokenSource, CancelAfter  
Shortcuts State Machine  
IAsyncDisposable  
ValueTask    
AsyncStreams/AsyncEnumerable/EnumeratorCancellation  
Await Foreach  

---
Matt Ellis - allocation free code  
ValueTuple vs Tuple  
Understanding ValueTask and async/await  
Use references with value types/from c# 7.2  
Ref Return : c# 7.0  
Ref read-only return  
In parameters (value types)  
Span<T> performance - fast implementation  
You can assert on memory allocation of your code  

---
BulkCopy with table lock  
Batchupdate with Temp tables  
BatchMerge  
