# GZ302 Linux Setup

**Professional-grade Linux setup script specifically designed for the ASUS ROG Flow Z13 (GZ302) laptop.** Transform your GZ302 into a perfectly optimized Linux powerhouse with automated hardware fixes, intelligent power management, and optional software stacks for gaming, AI development, and virtualization.

> **🔥 Version 4.1.1 - Python Implementation Fix!** Complete Python version of the setup script with enhanced error handling, maintainability, and cross-platform compatibility. Fixed AUR package installation issues. Choose between Bash and Python implementations.

## ✨ Key Features

### 🔧 **Comprehensive Hardware Support**
- **Automated MediaTek MT7925e Wi-Fi fixes** - Eliminates disconnection issues
- **Complete ASUS touchpad integration** - Full gesture and precision support  
- **Optimized AMD Ryzen AI 395+ performance** - Unlocks full processor potential
- **Advanced thermal management** - Sustained performance without throttling

### ⚡ **Intelligent Power Management** 
- **7-tier TDP control system** - From 10W emergency to 65W maximum performance
- **Automatic AC/battery switching** - Smart profile changes based on power source
- **Real-time monitoring** - Live power status, battery level, and performance metrics
- **Optimized for GZ302 hardware** - Profiles tuned specifically for AMD Ryzen AI 395+

### 🎮 **Complete Gaming Stack**
- **Steam + compatibility layers** - Proton, Wine, and Windows game support
- **Performance monitoring** - MangoHUD overlay with FPS, temps, and utilization
- **Automatic optimizations** - GameMode system tuning during gameplay
- **Multiple game stores** - Lutris for GOG, Epic, and other platforms

### 🤖 **Local AI Development**
- **Ollama integration** - Run Llama, Mistral, CodeLlama models locally
- **ROCm acceleration** - AMD GPU computing for AI workloads
- **Optimized for Ryzen AI** - Takes advantage of GZ302's AI acceleration features
- **Complete Python ML stack** - PyTorch, Transformers, and modern frameworks

### 📸 **Enterprise Snapshots**
- **Multi-filesystem support** - ZFS, Btrfs, ext4 (LVM), and XFS compatibility
- **Automated daily backups** - Set-and-forget system protection
- **Instant recovery** - Restore to any previous system state
- **Smart space management** - Automatic cleanup of old snapshots

## 🚀 Installation

**Now available in both Bash and Python versions!** Both provide identical functionality - choose your preferred implementation:

### Python Version (Recommended)
**Modern Python implementation with improved error handling and maintainability:**

```bash
curl -L https://raw.githubusercontent.com/th3cavalry/GZ302-Linux-Setup/main/gz302_setup.py -o gz302_setup.py
chmod +x gz302_setup.py
sudo ./gz302_setup.py
```

### Bash Version (Original)
**Battle-tested original implementation:**

```bash
curl -L https://raw.githubusercontent.com/th3cavalry/GZ302-Linux-Setup/main/gz302_setup.sh -o gz302_setup.sh
chmod +x gz302_setup.sh
sudo ./gz302_setup.sh
```

**Both versions automatically detect your Linux distribution and provide identical functionality.**

**Supported Linux Distributions:**
- **Arch-based**: Arch Linux, EndeavourOS, Manjaro
- **Debian-based**: Ubuntu, Pop!_OS, Linux Mint  
- **RPM-based**: Fedora, Nobara
- **OpenSUSE**: Tumbleweed and Leap

## What Gets Fixed

### Hardware Problems (Applied Automatically)
- **Wi-Fi Issues** - Fixes MediaTek MT7925e disconnections and stability problems
- **Touchpad Problems** - Enables proper ASUS touchpad detection and functionality
- **Audio Issues** - Configures ASUS-specific audio hardware and drivers
- **Camera Issues** - Sets up camera drivers and hardware detection
- **GPU Problems** - Optimizes AMD GPU performance and thermal management
- **Power Management** - Advanced TDP control and battery optimization
- **Thermal Control** - Intelligent thermal management for sustained performance

### Advanced Power Management (Always Installed)
Our script installs comprehensive **TDP (Thermal Design Power) management** that gives you full control over your laptop's performance and battery life:

#### 🔋 Seven Power Profiles Available:
- **`max_performance`** - 65W absolute maximum (AC power only, short bursts)
- **`gaming`** - 54W gaming optimized (AC power recommended) 
- **`performance`** - 45W high performance (AC power recommended)
- **`balanced`** - 35W balanced performance/efficiency (default)
- **`efficient`** - 25W better efficiency with good performance
- **`power_saver`** - 15W maximum battery life
- **`ultra_low`** - 10W emergency battery extension

#### 🤖 Automatic Power Switching:
- **Smart AC/Battery Detection** - Automatically switches profiles when you plug/unplug power
- **Configurable Preferences** - Set different profiles for AC and battery power
- **Real-time Monitoring** - Shows current power source, battery level, and active profile

### What Can Be Installed (Your Choice)

#### 🎮 Gaming Software Suite
- **Game Stores**: Steam, Lutris, ProtonUp-Qt for easy game management
- **Performance Tools**: MangoHUD (performance overlay), GameMode (system optimization)
- **Compatibility**: Wine, Proton, and Windows game compatibility layers
- **Optimizations**: Automatic gaming performance tweaks and kernel optimizations

#### 🤖 AI/LLM Software Stack  
- **Ollama** - Local LLM server for running AI models (Llama, Mistral, etc.)
- **ROCm** - AMD GPU acceleration for AI workloads
- **Python Libraries** - PyTorch, Transformers, and ML frameworks
- **Hardware Acceleration** - Optimized for GZ302's AMD Ryzen AI 395+ processor

#### 💻 Hypervisor Platforms (Choose One)
1. **KVM/QEMU with virt-manager** - Open source, excellent performance
2. **VirtualBox** - Oracle's user-friendly virtualization platform
3. **VMware Workstation Pro** - Commercial, feature-rich solution
4. **Xen Hypervisor** - Enterprise-grade Type-1 hypervisor  
5. **Proxmox VE** - Complete virtualization management platform
6. **Hyper-V** - Microsoft's virtualization technology (where supported)

#### 📸 System Snapshots & Recovery
- **Multi-Filesystem Support** - Works with ZFS, Btrfs, ext4 (LVM), and XFS
- **Automatic Daily Snapshots** - Background system state preservation
- **Manual Snapshot Control** - Create snapshots before major changes
- **Easy Recovery** - Restore system to any previous snapshot
- **Space Management** - Automatic cleanup of old snapshots

#### 🔒 Secure Boot Configuration
- **Enhanced Security** - Boot integrity and kernel signature verification
- **Multi-Bootloader Support** - Works with GRUB, systemd-boot, and rEFInd
- **Automatic Signing** - Kernel modules automatically signed on updates
- **UEFI Integration** - Seamless integration with ASUS UEFI firmware

## How To Use

**Important:** Always restart your computer after running either script!

The setup script automatically detects your Linux distribution and applies the appropriate configuration. **Choose either the Python or Bash version** - both provide identical functionality:

### Python Version (Recommended)
```bash
curl -L https://raw.githubusercontent.com/th3cavalry/GZ302-Linux-Setup/main/gz302_setup.py -o gz302_setup.py
chmod +x gz302_setup.py
sudo ./gz302_setup.py
```

### Bash Version (Original)
```bash
curl -L https://raw.githubusercontent.com/th3cavalry/GZ302-Linux-Setup/main/gz302_setup.sh -o gz302_setup.sh
chmod +x gz302_setup.sh
sudo ./gz302_setup.sh
```

**The script works on all supported distributions** - Arch Linux, Ubuntu, Fedora, and OpenSUSE (including their derivatives like EndeavourOS, Manjaro, Pop!_OS, Linux Mint, and Nobara).

### Step 2: What The Script Will Ask You

The script will ask if you want to install optional software. **All hardware fixes and TDP management are installed automatically** - these questions are only for additional software:

#### 🎮 Gaming Software Bundle
**Includes:** Steam, Lutris, ProtonUp-Qt, MangoHUD, GameMode, Wine
- **Steam** - Primary game store and launcher
- **Lutris** - Open-source game manager for GOG, Epic, etc.
- **ProtonUp-Qt** - Easy Proton/Wine version management
- **MangoHUD** - In-game performance overlay (FPS, temps, usage)
- **GameMode** - Automatic system optimizations during gaming
- **Wine** - Windows application compatibility layer

#### 🤖 AI/LLM Software Stack
**Includes:** Ollama, ROCm, Python AI libraries
- **Ollama** - Local AI server (run Llama, Mistral, CodeLlama models)
- **ROCm** - AMD GPU acceleration for AI workloads
- **PyTorch & Transformers** - Modern machine learning frameworks
- **Optimized for GZ302's AMD Ryzen AI 395+ processor**

#### 💻 Hypervisor Platform (Choose One)
1. **KVM/QEMU + virt-manager** - Best performance, open source
2. **VirtualBox** - Easiest to use, good for beginners  
3. **VMware Workstation Pro** - Professional features, commercial
4. **Xen Hypervisor** - Enterprise-grade, Type-1 hypervisor
5. **Proxmox VE** - Complete virtualization management
6. **Skip** - Don't install any virtualization software

#### 📸 System Snapshots
**Automatic filesystem backups supporting:**
- **ZFS** - Advanced snapshots with compression
- **Btrfs** - Built-in snapshot capabilities  
- **ext4** - LVM-based snapshots
- **XFS** - Limited snapshot support
- **Daily automatic snapshots** + manual control via `gz302-snapshot`

#### 🔒 Secure Boot Setup  
**Enhanced boot security featuring:**
- **Kernel signature verification** - Ensures kernel integrity
- **Automatic signing** - New kernels signed automatically  
- **Multi-bootloader support** - GRUB, systemd-boot, rEFInd
- **UEFI integration** - Works with ASUS firmware

**Just answer `y` (yes) or `n` (no) for each option!** For hypervisors, choose the numbered option (1-6) that you prefer.

> 💡 **Tip:** You can always run the script again later to install additional software you initially skipped.

## Useful Commands (After Setup)

### 🔋 Advanced Power Management

#### Basic TDP Profile Control:
```bash
# Set performance profiles
gz302-tdp max_performance  # 65W maximum (AC only)
gz302-tdp gaming           # 54W gaming optimized
gz302-tdp performance      # 45W high performance  
gz302-tdp balanced         # 35W balanced (default)
gz302-tdp efficient        # 25W efficient performance
gz302-tdp power_saver      # 15W maximum battery life
gz302-tdp ultra_low        # 10W emergency extension
```

#### System Monitoring & Status:
```bash
gz302-tdp status           # Show current profile, power source, battery %
gz302-tdp list             # List all available profiles with wattage
```

#### 🤖 Automatic Profile Switching:
```bash
gz302-tdp config           # Configure automatic AC/battery switching
gz302-tdp auto             # Enable/disable automatic switching
```

**Example automatic setup:**
- **AC Power**: Automatically switches to `gaming` or `performance` profile
- **Battery Power**: Automatically switches to `efficient` or `power_saver` profile
- **Smart Detection**: Only switches when power source actually changes

### 📸 System Snapshots & Recovery

#### Snapshot Management:
```bash
gz302-snapshot create      # Create a new system backup
gz302-snapshot list        # View all available snapshots  
gz302-snapshot cleanup     # Remove old snapshots (keeps last 5)
gz302-snapshot restore     # Interactive snapshot restoration
```

**Supported Filesystems:** ZFS, Btrfs, ext4 (with LVM), XFS
**Automatic Schedule:** Daily snapshots created automatically

### 🎮 Gaming Performance Tools

#### Performance Monitoring:
```bash
gamemoded -s               # Check GameMode status
mangohud your_game         # Launch game with performance overlay
systemctl status gamemode  # Verify GameMode service
```

#### Steam Integration:
```bash
# Add to Steam launch options for any game:
mangohud %command%         # Enable performance overlay
gamemoderun %command%      # Enable gaming optimizations
```

### 🔧 Hardware Control & Diagnostics

#### ASUS Hardware Controls:
```bash
systemctl status supergfxd asusctl  # Check ASUS services
sudo systemctl restart supergfxd    # Restart GPU switching
asusctl profile -l                  # List available power profiles
supergfxctl -g                      # Check current GPU mode
```

#### Wi-Fi Troubleshooting:
```bash
systemctl status NetworkManager     # Check network service
sudo modprobe -r hid_asus && sudo modprobe hid_asus  # Reset ASUS drivers
```

### 🤖 AI/LLM Management (If Installed)

#### Ollama Local AI Server:
```bash
systemctl status ollama             # Check Ollama service
ollama list                         # List installed models
ollama pull llama2                  # Download a model
ollama run llama2                   # Start interactive chat
```

#### ROCm GPU Acceleration:
```bash
rocm-smi                           # AMD GPU status and monitoring
clinfo                             # OpenCL device information
```

## Problems? Here's How To Fix Them

### 🔋 Power & Performance Issues

#### TDP Profile Not Working
- **Check current status**: `gz302-tdp status`
- **Verify installation**: `which gz302-tdp` (should show `/usr/local/bin/gz302-tdp`)
- **Manual profile test**: `sudo gz302-tdp balanced`
- **Check logs**: `journalctl -u gz302-tdp-auto.service -f`

#### Battery Draining Too Fast
- **Switch to power-saving profile**: `gz302-tdp power_saver` or `gz302-tdp ultra_low`
- **Enable automatic switching**: `gz302-tdp config` (set battery profile to `efficient`)
- **Check current profile**: `gz302-tdp status`

#### Performance Lower Than Expected
- **Use high-performance profile**: `gz302-tdp gaming` or `gz302-tdp max_performance` (AC power only)
- **Verify AC power**: `gz302-tdp status` should show "Power Source: AC"
- **Check thermal throttling**: Monitor temperatures during use

### 📶 Wi-Fi Issues

#### Wi-Fi Not Working or Disconnecting
- **First step**: Restart your computer (fixes most MediaTek MT7925e issues)
- **Check NetworkManager**: `systemctl status NetworkManager`
- **Reset drivers**: `sudo modprobe -r hid_asus && sudo modprobe hid_asus`
- **Check Wi-Fi power management**: `iwconfig` (look for Power Management settings)

### 🖱️ Touchpad Problems

#### Touchpad Not Responding  
- **First step**: Restart your computer
- **Reset ASUS drivers**: `sudo modprobe -r hid_asus && sudo modprobe hid_asus`
- **Check touchpad detection**: `xinput list` (look for ASUS touchpad)

### 🎮 Gaming Performance Issues

#### Games Running Slowly
- **Use gaming TDP profile**: `gz302-tdp gaming`
- **Verify correct kernel**: Make sure you selected the right kernel at boot
- **Check GameMode**: `gamemoded -s` (should show "gamemode is active")
- **Monitor performance**: `mangohud your_game` to see real-time stats
- **GPU switching**: `supergfxctl -g` to check current GPU mode

#### Steam Games Not Starting
- **Check Proton**: Update to latest Proton version in Steam
- **GameMode integration**: Add `gamemoderun %command%` to launch options
- **Performance overlay**: Add `mangohud %command%` to launch options

### 🔧 ASUS Hardware Controls

#### ASUS Controls Not Working
- **Check services**: `systemctl status supergfxd asusctl`
- **Restart services**: `sudo systemctl restart supergfxd asusctl`
- **ROG Control Center**: Launch with `rog-control-center`
- **Check logs**: `journalctl -b | grep -i asus`

#### SuperGFXD "Could not find dGPU" Errors
If you see repeated error messages like `[ERROR supergfxctl::zbus_iface] get_runtime_status: Could not find dGPU`:

- **Normal for integrated-only systems**: This is expected on GZ302 models with only integrated AMD graphics
- **Stop the service**: `sudo systemctl stop supergfxd && sudo systemctl disable supergfxd`
- **Check GPU hardware**: `lspci | grep -i "vga\|3d\|display"` to verify if you have discrete GPU
- **Re-run setup script**: The latest version automatically detects GPU configuration and only enables supergfxd when needed

### 📸 Snapshot Issues

#### Snapshots Failing to Create
- **Check filesystem**: `gz302-snapshot list` will show supported filesystem
- **Disk space**: Ensure sufficient free space (at least 20% recommended)
- **Permissions**: Run as root: `sudo gz302-snapshot create`

### 🤖 AI/LLM Issues (If Installed)

#### Ollama Not Responding
- **Check service**: `systemctl status ollama`
- **Restart service**: `sudo systemctl restart ollama`
- **Check port**: `curl http://localhost:11434` (should respond)

#### ROCm GPU Not Detected
- **Check ROCm installation**: `rocm-smi`
- **Verify GPU support**: `clinfo` (should show AMD GPU)
- **Reboot required**: ROCm often requires reboot after installation

## 📝 Changelog

### Version 4.1.1 (Latest)
**Python Implementation Fix - AUR Package Installation Error Resolution**

#### 🐛 Issues Fixed:
- **Fixed AUR package installation failure**: Resolved "Running makepkg as root is not allowed" error in Python script by implementing proper user context for `yay` and `paru` operations
- **Enhanced AUR helper support**: Python script now correctly uses `sudo -u real_user` pattern for all AUR package installations, matching the bash script behavior
- **Improved error handling**: Better handling of missing AUR helpers with automatic yay installation as the real user
- **Fixed ryzenadj installation**: Specifically resolved the ryzenadj AUR package installation that was failing due to root execution

#### 🔧 Technical Details:
- Modified `install_ryzenadj_arch()` method to use proper user context with `sudo -u real_user` 
- Fixed all AUR installations in Python script including ProtonUp-Qt, VMware Workstation, and Xen packages
- Ensured consistency between bash and Python implementations for AUR operations
- Added automatic yay installation process that respects user privileges

#### 📋 Implementation Details:
- **Both versions available**: Users can choose between the original Bash script (`gz302_setup.sh`) and the new Python version (`gz302_setup.py`)
- **Identical functionality**: All hardware fixes, TDP management, and optional software installations preserved
- **Fixed compatibility**: Python version now works correctly on Arch-based systems without root makepkg errors

### Version 4.1
**Hardware Fixes Update - Critical Hardware Compatibility Improvements**

#### 🔧 Issues Fixed:
- **Fixed systemd service errors**: Removed invalid `ConditionKernelModule=hid_asus` directive that was causing systemd warnings
- **Updated camera drivers**: Replaced deprecated `uvcvideo nodrop=1` parameter with modern `quirks=128` configuration  
- **Enhanced ASUS hardware support**: Added dedicated ASUS WMI and HID module optimizations to reduce error messages
- **Improved touchpad functionality**: Added comprehensive libinput X11 configuration to prevent touch jump detection issues
- **Better service reliability**: Added `RemainAfterExit=yes` and proper module checking to systemd services
- **Resolved ACPI BIOS errors**: Added kernel parameters to handle duplicate ACPI object warnings on boot
- **Enhanced Wi-Fi stability**: Removed invalid mt7925e module parameters that caused kernel warnings
- **Improved audio support**: Added ACP70 platform fixes for newer AMD audio hardware
- **Optimized storage I/O**: Added proper NVMe scheduler configuration to prevent attribute write failures

#### 🛠️ Technical Details:
- Fixed kernel log errors related to ASUS HID device probe failures (error -12) with memory buffer optimization
- Eliminated deprecated kernel parameter warnings for UVC camera module
- Addressed touch jump detection warnings in libinput for better touchpad experience
- Reduced ASUS WMI fan curve error messages (error -19)
- Added ACPI kernel parameters (`acpi_osi=! acpi_osi="Windows 2020" acpi_enforce_resources=lax`) to resolve boot warnings
- Cleaned up Wi-Fi module parameters to only include valid options supported by mt7925e driver
- Enhanced audio configuration with ACP70 ASoC machine driver support for proper AMD audio platform detection
- Implemented intelligent I/O scheduler selection for NVMe, SSD, and HDD devices
- Applied fixes consistently across all supported distributions (Arch, Debian, Fedora, OpenSUSE)

### Version 4.0
**Major Update - Streamlined Single-Script Architecture**

- Consolidated all distribution-specific scripts into one intelligent setup script
- Added automatic Linux distribution detection
- Comprehensive feature documentation and user guidance
- Enhanced TDP management with 7-tier power profiles
- Improved hardware support and compatibility fixes

## Need Help?

If something goes wrong:

1. Check error messages: `journalctl -b`
2. Create an issue on GitHub with:
   - What went wrong
   - Error messages you saw
   - Your laptop model (make sure it's GZ302)

## Thanks To

This project builds on great work from:
- [asus-linux.org](https://asus-linux.org) community
- Shahzebqazi's Asus-Z13-Flow-2025-PCMR repository  
- Level1Techs Forum Community
- Arch Linux community

## License

This project is open source under the MIT License.
