# Edgar Lecuyer

**C/C++ engineer — PKI, VPN and network security.**
I work on the certificate and VPN stacks of [Stormshield](https://www.stormshield.com/) firewalls
(Airbus Defence and Space Cyber Programmes).

Most of my day job is C on a FreeBSD-based appliance: certificate enrollment over TLS, IPsec, and
the plumbing underneath. The constraints are the interesting part. A daemon that runs for months
without restarting turns a few bytes leaked per request into an outage six weeks later, and anything
reachable from the network is an attack surface before it is a feature. So I spend a lot of time on
things that never show up in a demo — cleaning up OpenSSL objects properly, running Valgrind while I
write rather than at the end, and working out the smallest set of privileges a process can survive
on.

That code is proprietary, so it is not here. What is here is the other half: engines, compilers and
renderers I built from scratch, mostly to find out how they actually work.

---

## Projects

**[R-Type](https://github.com/EdgarLec/Epitech-R-Type)** · C++, UDP, CMake
A 2D game engine written from scratch on a custom ECS, with online multiplayer over a binary UDP
protocol and an authoritative server that arbitrates state. Cross-platform builds, CI, Docker.

**[RayTracer](https://github.com/EdgarLec/RayTracer)** · C++, TCP, multithreading
A ray tracer that spreads a render across a cluster. Nodes report their thread count so work is
split by what each machine can take, and the network renderer implements the same interface as the
local one — the caller cannot tell where its pixels came from.

**[Corewar](https://github.com/EdgarLec/Corewar)** · C
An assembler and the virtual machine that runs its bytecode. Lexing, parsing, instruction encoding
and label resolution on one side; a shared memory arena, per-process cycle costs and a scheduler on
the other.

**[Arcade](https://github.com/EdgarLec/Arcade)** · C++, dlopen
A game platform where neither the games nor the graphics backends are linked in. The core knows two
abstract interfaces; everything else is a shared object loaded at runtime and swappable without
leaving the program.

**[Gomoku](https://github.com/EdgarLec/Gomoku)** · C++
A minimax engine for five-in-a-row. The search is only tractable because move generation stays near
existing stones and the evaluator recognises the shapes that decide the game.

---

## Tools

`C (C99)` · `C++` · `OpenSSL` · `FreeBSD` · `Linux` · `Valgrind` · `LLDB` · `Make` · `CMake` · `Git`

Also comfortable in Python, OpenGL, Unity.

---

📍 Lille, France (CET) · 🌍 English C1, after a year on exchange in South Korea
📫 [LinkedIn](https://www.linkedin.com/in/edgar-lecuyer-240419232/) · lecuyer.edgar@gmail.com
