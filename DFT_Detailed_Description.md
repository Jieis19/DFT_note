# Detailed Description of DFT Techniques

## Scan Chains
- **Definition**: Connect flip-flops inside the circuit in a serial manner to form a “scan chain.”  
- **Purpose**: Allows external test equipment to directly control and observe internal register states for detecting logic errors and manufacturing defects.  
- **How It Works**:  
  - Test vectors are shifted into the scan chain to set circuit states bit by bit.  
  - After the test, results are shifted out and compared to expected values.  
- **Advantages**:  
  - Increases test coverage.  
  - Simplifies test vector generation and control.  
  - Detects internal faults hard to catch in normal functional tests.

## Built-In Self-Test (BIST)
- **Definition**: Embeds dedicated testing logic within the chip to automatically run test procedures, generate test vectors, and analyze results.  
- **Types**:  
  - Logic BIST: Self-tests logic circuits.  
  - Memory BIST: Tests memory cells.  
- **How It Works**:  
  - When activated, BIST logic internally generates and applies test vectors.  
  - Results are automatically checked and faults reported.  
- **Advantages**:  
  - Reduces reliance on external test equipment.  
  - High testing speed and efficiency.  
  - Suitable for on-site self-diagnostics and system health monitoring.

## Boundary Scan (JTAG)
- **Definition**: A test technology based on IEEE 1149.1 standard, adding scan chains around chip I/O pins for direct testing of pin and PCB connections.  
- **How It Works**:  
  - Devices implement Boundary Scan Registers controlling and monitoring signals at the I/O pins.  
  - Accessed via the JTAG interface (Test Access Port Controller) for point-to-point test and debugging.  
- **Uses**:  
  - Testing PCB solder joints quality.  
  - System-level functional tests.  
  - Debugging and firmware programming.  
- **Advantages**:  
  - Tests complex pin and interconnects without physical probes.  
  - Supports chained multi-chip testing.  
  - Greatly improves test feasibility and efficiency.

## Test Point Insertion
- **Definition**: Inserting additional test points on critical signals or nodes during design to increase observability and controllability during manufacturing tests.  
- **Purpose**:  
  - Improve access to internal signals.  
  - Enhance test coverage and accuracy.  
- **Implementation**:  
  - Configured in design tools by adding multiplexers or switches at key nodes.  
- **Benefits**:  
  - Eases internal signal probing.  
  - Allows precise stimulation of internal states.  
  - Reduces fault diagnosis time.

