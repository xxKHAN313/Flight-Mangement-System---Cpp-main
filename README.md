# Flight Route Planner

**C++ flight search and booking simulation**

A C++ flight-planning simulation with linked adjacency lists, route search, airline and transit preferences, and SFML visualization.

C++ · SFML graphics and audio · text-file storage

> Academic prototype. Features below are grounded in the source; validation limits are recorded below.

## What it does

- Flight lookup by origin, destination, and date.
- Route search and filtering by airline or transit city.
- Layover queues and local booking-file output.
- SFML graph visualization and startup audio.

## Getting started

Commands below use Windows PowerShell.

```powershell
git clone https://github.com/xxKHAN313/Flight-Mangement-System---Cpp-main.git
cd Flight-Mangement-System---Cpp-main/Flight-Mangement-System---Cpp-main/DSA
# Example for a compiler-compatible SFML 2 installation at C:/SFML:
g++ -std=c++17 main.cpp graph.cpp flight.cpp layoverqueue.cpp -IC:/SFML/include -LC:/SFML/lib -lsfml-graphics -lsfml-window -lsfml-audio -lsfml-system -o flight-planner.exe
.\flight-planner.exe
```

Install a C++ compiler and a matching SFML 2 distribution; make the SFML runtime DLLs discoverable through PATH. Run from the `DSA` directory so `Flights.txt`, `HotelCharges_perday.txt`, `arial.ttf`, and `output.ogg` resolve correctly.

The repository includes sample routes and media, but their redistribution provenance still needs confirmation. Bookings are local text output. This is a coursework simulation with static schedules, not a live airline booking service.

## Code map

`main.cpp` — console workflow; `graph.cpp` / `graph.h` — routes and visualization; `flight.cpp` / `flight.h` — flight source files; `layoverqueue.cpp` / `layoverqueue.h` — layover queue; `Flights.txt` — sample input.

Browse the [application source](Flight-Mangement-System---Cpp-main/DSA/).

## Validation and limitations

Source and runtime file paths were inspected. The compiler command is untested in this environment; no C++ compiler or SFML installation is available.

## Credits and license

This repository contains academic work. Existing source credits and acknowledgements are retained; individual contributions should be confirmed before attributing the whole project to one person.

No standalone license file was found in the reviewed checkout. Existing notices remain in effect; no new license is asserted here.
