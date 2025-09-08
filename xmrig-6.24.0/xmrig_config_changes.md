# XMRig Configuration Changes

## Pool Configuration

```json
"pools": [
    {
        "algo": "rx/0",           // Set to RandomX algorithm
        "coin": "XMR",           // Set to Monero
        "url": "pool.supportxmr.com:443",  // Changed from donate pool
        "user": "478woeDJZDh48qAiznzMR7X22NQeHMvZP3guvcBbV2qD74RtTiM2bbPLSJkxWFG88rR2XTfhCPPDtZSkAPAsKXsKR6rsBAL",  // Your Monero address
        "tls": true              // Enabled TLS encryption
    }
]
```

## CPU Thread Configuration

```json
"cpu": {
    "rx": [0, 1, 2, 3]          // Limited to 4 threads (was 14)
}
```

## Why These Changes Were Made

1. **Pool URL:** Changed from donation pool to actual Monero mining pool
2. **User address:** Added your Monero wallet address to receive payments
3. **Algorithm:** Specified RandomX (rx/0) for Monero mining
4. **Thread limit:** Reduced from 14 to 4 threads to protect your hardware and reduce heat/power consumption
5. **TLS enabled:** Secure connection to mining pool