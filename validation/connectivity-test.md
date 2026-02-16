


# Connectivity Test

## Public Subnet EC2
- **Ping test:** `ping -c 3 8.8.8.8` → successful
- **Curl test:** `curl ifconfig.me` → shows public IP (e.g., 3.238.139.2)

## Private Subnet EC2
- **Ping test:** `ping -c 3 8.8.8.8` → failed (no internet)
- **Curl test:** `curl ifconfig.me` → failed (no internet)

**Note:** Private subnets are intentionally isolated from the internet. This behavior is expected. All connectivity tests confirm that public and private subnets are configured correctly.
