# Code Schemes

Repository for embedded DRDO code schemes.

## Historical Context and the Evolution of Radar Coding

The development of advanced coding schemes in radar systems was driven by critical physical and operational limitations of simple pulse-echo methods.

### The Problem with High-Power Pulsed Transmission
Initially, radar systems relied on transmitting extremely short, high-power electromagnetic pulses to achieve precise range detection. The range resolution (the ability to distinguish between two close targets) was directly proportional to the shortness of the pulse. However, this approach presented two major challenges:

1.  **Hardware Integrity (Transceiver Overload):** To detect distant targets with a short pulse, the peak power of that pulse had to be immense. This extreme energy often exceeded the physical tolerances of the transceiver components, leading to internal arcing, thermal failure, and "frying" of sensitive electronics.
2.  **Electronic Intelligence (Stealth and LPI):** High-power pulses act as a "lighthouse" in the electromagnetic spectrum. Any enemy equipped with basic ESM (Electronic Support Measures) could easily detect the radar's location from long distances, negating any tactical advantage.

### The Shift to Low-Power, Long-Duration Coding
To overcome these barriers, the concept of **Pulse Compression** and complex coding schemes was introduced. Instead of a single high-power burst, the radar sends a longer, lower-power signal that is "coded."

A primary example is the **Linear Frequency Modulation (LFM)** or **Chirp** signal. In this method:
*   The signal's pitch (frequency) changes continuously (e.g., from low to high) over the duration of the pulse.
*   By using a longer duration, the system can transmit the same total energy as a high-power short pulse but with a much lower peak power, protecting the hardware.
*   Upon receiving the echo, specialized mathematical filters (Matched Filters) "compress" this long coded signal back into a narrow spike. This allows the system to maintain high range resolution and sensitivity while remaining significantly harder for enemies to detect and localize.

This evolution from "brute force" power to "intelligent coding" is the foundation of modern stealthy and high-performance radar systems.
