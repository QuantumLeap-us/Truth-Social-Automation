# TruthWave - Truth Social Automation Suite

TruthWave is a comprehensive automation solution for Truth Social platform management, designed for users who need to operate multiple accounts with consistent fingerprinting and engagement capabilities.

## Key Features

1. **Advanced Account Creation** - Bulk generation of authentic Truth Social accounts with realistic profiles
2. **Fingerprint Consistency** - Maintains identical device characteristics between account creation and usage
3. **Human Behavior Simulation** - Intelligent browsing patterns, randomized delays, and selective engagement
4. **Proxy Management System** - Smart allocation and rotation of proxy servers to prevent detection
5. **Automated Engagement** - Automatic liking of specified posts across multiple accounts

## Technical Highlights

- **Device Fingerprinting**: Generates and maintains consistent browser fingerprints
- **Proxy Integration**: Supports various proxy formats with automatic health checking
- **Adaptive Timing**: Simulates human operation intervals to avoid bot detection
- **Failure Recovery**: Automatically handles account failures and proxy cooldowns
- **Browsing Algorithms**: Replicates authentic user browsing habits before engagement

## System Requirements

1. **Python Environment**: Python 3.7+
2. **Required Dependencies**:
   ```bash
   pip install botasaurus faker curl-cffi
   ```
3. **Node.js**: Required for certain advanced features
4. **Network**: Working internet connection with HTTP/HTTPS request capabilities

## Implementation Guide

### Step 1: Account Creation

Execute the following command to create new accounts:
```bash
python bot.py
```
Enter the desired number of accounts when prompted. The system will automatically handle registration and save account information.

### Step 2: Post Engagement

Run the following command to begin automatic engagement:
```bash
python driver.py
```

The system will utilize previously created accounts, maintaining the same fingerprints and proxies used during account creation.

### Advanced Options

```bash
# Test a specific proxy
python driver.py --test-proxy 45.39.115.187:5598:username:password

# Reset all failed accounts and cooldown timers
python driver.py --reset-failed
```

## Configuration Details

Primary configurations are stored in:
- `config.json`: Core configuration settings
- `proxies.txt`: List of proxy servers
- `settings.txt`: Thread count, max likes, and proxy settings
- `links.txt`: Post URLs to engage with
- `post.txt`: Content template for automated posting

## Security Features

1. Automatic preservation and reuse of consistent device fingerprints
2. Intelligent proxy rotation and cooldown system
3. Automatic detection of account suspension status
4. Adaptive delay system to prevent detection

## Performance Optimization

The TruthWave system has been optimized to minimize operation times while maintaining realistic behavior patterns:
- Reduced browsing times between actions
- Optimized waiting periods for API calls
- Intelligent proxy selection to reduce failures
- Automatic retry mechanisms for temporary issues

---

TruthWave delivers enhanced account management and engagement on the Truth Social platform through sophisticated fingerprinting technology and human behavior simulation, helping users achieve consistent, reliable automation without triggering platform defenses. 