DXVK Benchmark Report: RX 550 & i5-3570 Stability Analysis

This report provides a detailed performance comparison between different DXVK versions (Sarek, GPLAsync, Low-Latency, and Default) using the Tomb Raider benchmark. The goal was to determine which version offers the best balance between raw power and frame pacing on entry-level hardware.
Test Environment

    CPU: Intel Core i5-3570

    GPU: AMD Radeon RX 550 4GB

    OS: Kubuntu 26.04

    Kernel: 7.0.0-15-generic

    Driver: RADV Polaris12

Benchmark Results
DXVK Version	Average FPS	 1% Low FPS	   0.1% Low (Stability)	      Frame Time
Default DXVK	    80.8	    65.5	     	       61.7             12.4 ms
DXVK-Sarek	        82.2	    56.2		           31.9             12.2 ms
DXVK-GPLAsync	    74.8	    57.8	               52.9	            13.4 ms
DXVK-Low-Latency	74.8	    57.1	               45.6	            13.4 ms

Technical Analysis

    The Stability King: Default DXVK proved to be the most consistent version. While others experienced significant drops, this version maintained a 0.1% low of 61.7 FPS, ensuring a stutter-free experience.

    Raw Power vs. Reliability: DXVK-Sarek achieved the highest average frame rate (82.2 FPS). However, its 0.1% low dropped to 31.9 FPS, which can result in noticeable micro-stuttering during intense gameplay.

    Hardware Utilization: Both Default and Sarek versions managed to utilize the GPU at 99-100% load. In contrast, GPLAsync peaked at 93.9%, suggesting it may not be fully optimized for this specific hardware configuration.

    Efficiency: Standard DXVK and Sarek kept CPU utilization lower (~32%) compared to the patched versions (~41%), leaving more overhead for the system.

Final Verdict

For users with an RX 550 and i5-3570, Standard DXVK is the superior choice. While custom versions like Sarek offer slightly higher peak numbers, the standard version provides a significantly smoother and more predictable frame delivery.
