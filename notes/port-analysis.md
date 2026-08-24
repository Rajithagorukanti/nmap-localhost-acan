# Port Analysis (Nmap Localhost Scan)

## 135/tcp – msrpc (Microsoft Windows RPC)
- Windows RPC service used for internal communication.
- Normal on Windows systems.
- Medium risk externally, but safe on localhost behind a firewall.

## 445/tcp – microsoft-ds (SMB)
- SMB file sharing service.
- Normal on Windows.
- Historically exploited (e.g., WannaCry), but home systems are protected by firewalls.

## 902/tcp – ssl/vmware-auth
- VMware Authentication Daemon.
- Appears when VMware is installed.
- Used for VM remote control and management.

## 912/tcp – vmware-auth
- VMware Authentication Daemon.
- Normal for VMware environments.
- Internal service, low risk on localhost.
