# DDR Timing Supported Formats Notes

## 1. NRZ (Non-Return to Zero)
- **Definition**: NRZ is a data encoding format where the signal level remains high or low throughout the entire bit period without returning to a zero or neutral level.
- **Application in DDR**:
  - Data holds a stable level at designated clock edges.
  - Provides continuous, smooth waveform suitable for simple data transmission.

## 2. DCLK (Data Clock)
- **Definition**: Data clock signal used for data synchronization.
- **Role in DDR**:
  - Data is synchronized and sampled according to the DCLK signal.
  - Works together with DQS (Data Strobe) signals to improve timing control accuracy.

## 3. Edge Strobe
- **Definition**: The data strobe (DQS) pulse emitted at clock edges (rising or falling) for data sampling.
- **Characteristics**:
  - Data is captured on specific clock edges.
  - Enhances accuracy and timing sensitivity of data capture.
  - Reduces timing delay and jitter effects.

## Summary
- DDR timing supports multiple data synchronization formats for flexibility and compatibility.
- NRZ suits basic data encoding, while DCLK and Edge Strobe enable more precise data sampling.

