# BusScope 8085

BusScope is a browser-based learning tool for exploring how supported 8085 assembly instructions translate into machine cycles and bus activity. It pairs instruction execution with a timing diagram, so the relationship between the program and signals on the bus is visible step by step.

## What it shows

- Assemble and run 8085 programs, then inspect the executed-instruction trace.
- Step through machine cycles and T-states with waveforms for CLK, A15–A8, AD7–AD0, ALE, RD, WR, IO/M, S1, and S0.
- Adjust the CPU clock and memory wait states to see their effect on timing.
- Inject logical data-bus faults and inspect how changed read values affect execution.
- Compare two programs by instruction count, machine cycles, T-states, and code size.
- Explore an animated CPU/address-latch/memory view and practice with a waveform quiz.

## Run it

Open `index.html` in a modern browser. No compiler, server, or JavaScript package installation is required. The page is self-contained; Google Fonts are used for typography when online, with system-font fallbacks available offline.

## Scope and assumptions

This is an educational model, not an electrical simulator or a complete hardware emulator. Timing edges are idealized; propagation, setup, and hold delays are not modeled. HOLD/HLDA, hardware interrupts, and INTA are outside the current scope. `RIM` and `SIM` are simplified stubs. The About tab in the application describes the timing model, supported syntax, and additional assumptions.

## Implementation

The application is implemented in a single HTML file with embedded CSS and JavaScript. No external JavaScript libraries are required.
