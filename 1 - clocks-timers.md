# Clocks and Timers

PCs use an RTC (Real-Time Clock) that is typically battery powered. A PC's BIOS (Basic Input/Output System) uses the RTC to set the system clock at boot. But once the PC is connected to the internet, it's able to connect and synchronize its system clock to Network Time Protocol (NTP) servers.

With embedded systems, many times we will not have the luxury of an internet connection, so we rely on alternative timekeeping methods.

### Real-Time Clock (RTC):
   - Embedded systems often use an RTC, similar to PCs, to keep track of the current time and date. This RTC is typically battery-powered to maintain timekeeping even when the system is powered off.
   - The RTC provides a reliable time source for scheduling tasks, logging events, and maintaining accurate timestamps, crucial for applications like data logging, time-stamped transactions, and alarm systems.

### External Oscillator Crystals:
   - Many embedded systems use external oscillator crystals to generate precise clock signals for the microcontroller. These crystals provide a stable frequency reference that ensures accurate timing for system operations.
   - While they don't keep real-time, these crystals are essential for the precise timing required in tasks such as communication protocols (e.g., UART, SPI, I2C), PWM generation, and sensor data sampling.

### Microcontroller Internal Clocks:
   - Microcontrollers often have internal oscillators and clock sources that can be used when high precision is not as critical. These internal clocks are convenient but typically less accurate than external crystals.
   - Some microcontrollers offer calibration features to adjust the internal oscillator frequency based on temperature or other factors.


