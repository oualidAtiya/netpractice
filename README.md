*This project has been created as part of the 42 curriculum by oatiya.*

# NetPractice

## Description

NetPractice is a practical exercise designed to introduce the fundamentals of computer networking. The goal of the project is to fix a series of non-functioning simulated networks by correctly configuring IP addresses, subnet masks, and default gateways so that devices (hosts, switches, and routers) can communicate properly.

The project consists of 10 progressively more complex levels, each presenting a broken network diagram with one or more objectives. The task is to identify and correct the misconfigured, unshaded fields until the network functions as intended, using the training interface's logs and "Check again" feature to validate each configuration.

## Instructions

### Running the training interface

1. Download and extract the project archive into a folder of your choice.
2. From that folder, run the provided script:
   ```bash
   ./run.sh
   ```
   This launches a local web server and opens the training interface in your default browser.
3. If `run.sh` does not work, start the server manually:
   ```bash
   python3 -m http.server 49242
   ```
   Then open `http://localhost:49242` (or whichever port you chose) in your browser.
4. Enter your login in the dedicated field to access your personal configuration, or use the "evaluation" tab to generate a random configuration.

### Solving a level

- Each level displays a network diagram with one or more objectives at the top of the window.
- Modify only the unshaded/editable fields (IP addresses, subnet masks, gateways, etc.) until the network works.
- Use **[Check again]** to verify your configuration.
- Check the logs at the bottom of the page for hints (e.g. missing gateway, invalid IP address) if the configuration is incorrect.
- Once a level is solved, a button appears to move on to the next level.

### Exporting configurations

- Before moving to the next level, click **[Get my config]** to export the current level's configuration file.
- Do this for **all 10 levels** — a configuration file must be exported for each one.

### Submission requirements

- Place all **10 exported configuration files** (one per level) at the **root** of this Git repository.
- Make sure your login was entered in the training interface before exporting, as it is required for evaluation.
- Double-check file names before submitting.
- During the defense, you will need to solve **3 random levels** within a limited time, without using external tools (a simple calculator such as `bc` is tolerated).

## Resources

### Networking concepts studied

- TCP/IP
- subnetting
- gateways
- Routers and switches
- IP classes and CIDR notation
- OSI model layers

### References

- [Networking Lessons](https://networklessons.com/network-fundamentals)
- [Networking Academy](https://www.networkacademy.io/ccna/network-fundamentals)
- [JIT](https://www.youtube.com/playlist?list=PLxbwE86jKRgMpuZuLBivzlM8s2Dk5lXBQ)
- [Practice Subnetting](https://subnetipv4.com/)

### AI usage

AI (Claude) was used to help draft and structure this README.md file, based directly on the project subject's requirements (Description, Instructions, and Resources sections). No AI was used to generate network configurations or solve any of the 10 levels — all level solutions were worked out manually to ensure full understanding of TCP/IP addressing, subnetting, and gateway configuration, and were reviewed with peers before submission.