# x86-64 CPU Bring-Up Checklist (Windows 11 Target)

## Stage 0 – Basic Bring-Up
- [ ] Real mode instruction set (16-bit)
- [ ] Switch to protected mode (32-bit)
- [ ] Switch to long mode (64-bit)
- [ ] CPUID basic leaves (vendor, feature bits)
- [ ] Control registers CR0, CR2, CR3, CR4
- [ ] MSR access (RDMSR, WRMSR, EFER, STAR, LSTAR, SFMASK)
- [ ] Basic exceptions (#DE, #UD, #GP, #PF)

## Stage 1 – Paging + DEP/NX
- [ ] IA-32e 4-level paging (PML4, PDPT, PD, PT)
- [ ] 4 KiB pages
- [ ] 2 MiB large pages
- [ ] NX bit support (EFER.NXE + PTE NX)
- [ ] INVLPG instruction
- [ ] TLB

## Stage 2 – Core ISA for Windows
- [ ] Full 64-bit GPRs (RAX–R15)
- [ ] Arithmetic/logic/shift ops
- [ ] CMPXCHG8B
- [ ] CMPXCHG16B
- [ ] XCHG, XADD
- [ ] LOCK prefix semantics
- [ ] SSE2 (XMM registers, mov/add/mul basic ops)
- [ ] FXSAVE/FXRSTOR
- [ ] LAHF/SAHF valid in 64-bit mode

## Stage 3 – Interrupts & APIC
- [ ] IDT setup, IRETQ return
- [ ] Local APIC registers (xAPIC mode)
- [ ] APIC timer interrupt
- [ ] HLT instruction
- [ ] CLI/STI
- [ ] NMI delivery

## Stage 4 – Syscalls & Timing
- [ ] SYSCALL/SYSRET
- [ ] STAR/LSTAR/SFMASK MSRs
- [ ] RDTSC
- [ ] RDMSR/WRMSR (time, APIC, etc.)

## Stage 5 – Firmware & Platform Glue
- [ ] WBINVD, CLFLUSH
- [ ] ACPI MADT, RSDP/XSDT
- [ ] UEFI boot handoff (long mode)
- [ ] Page fault edge cases (NX, US, RW, Present)

## Stage 6 – Nice to Have
- [ ] XSAVE/XRSTOR
- [ ] PREFETCH instructions
- [ ] x2APIC
- [ ] PAT/MTRR
- [ ] RDRAND/RDSEED
