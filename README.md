# Gerobug  
**The first open-source self-managed bug bounty platform.**

Are you a company planning to run your own bug bounty program on a minimal budget?  
**WE GOT YOU!**

We understand that some organizations have struggled to establish their own bug bounty program. Using a third-party managed platform usually comes with a hefty price tag and potential security risks. On the other hand, building your own self-managed platform can be time-consuming and requires ongoing effort to maintain.

## Why Gerobug?

- **EASY**: Get your bug bounty program running with just a single line of command.
- **SECURE**: Gerobug uses email parsing and network segregation to minimize security risks.
- **OPEN SOURCE**: It's FREE.

## (Minimum) Recommended Specifications
- Ubuntu 24.04
- vCPU: 2 Cores
- RAM: 2 GB
- HDD: 16 GB

## Requirements
- Gmail or Outlook Email with App password implemented
- VPN Server (Recommended for Production Server)
- Domain for HTTPS (Recommended for Production Server)
- Ports: 80, 443, 6320
- Python 3.x
- Docker
- Docker Compose v2
- *(No need to install anything manually; we'll handle it for you!)*

## Deployment and Usage

To deploy Gerobug:

1. Clone this repository:
   ```bash
   git clone https://github.com/gerobug/gerobug
   ```

2. Navigate to the `gerobug` directory:
   ```bash
   cd gerobug
   ```

3. Run the Setup Script:
   ```bash
   ./gerobug.sh
 

4. Follow the setup instructions (Refer to the documentation for details).

By default, the **Gerobug Dashboard** will listen on port **6320**.  
Access the login page at:  
`http://[Domain/IP]:6320/login`

## Credentials
- **Username**: geromin
- **Password**: Randomly generated at `gerobug/gerobug_dashboard/secrets/gerobug_secret.env`


## Main Features

- **Network Segregation**  
  All services are running in separate containers. Public users can only access the static page (Rules and Guidelines).

- **Easy and Quick Installation**  
  Use our run script to install Gerobug quickly and easily!

- **HTTPS Implementation**  
  Automated HTTPS configuration using **NGINX** and **Let's Encrypt**.

- **Homepage**  
  The public-facing page that contains the **Rules** and **Guidelines** for your bug bounty program.

- **Email Parser**  
  Bug hunters submit their findings via email, which Gerobug will parse, filter, and display on the dashboard.

- **Auto Reply and Notifications for Bug Hunters**  
  Bug hunters will receive automatic replies and notifications if there are any updates on their reports.

- **Notification Channel**  
  The company will also be notified via **Slack** or **Telegram** if a new report is submitted.

- **User Management**  
  Gerobug has a role-based user management system.

- **Report Management**  
  Easily manage reports with a **kanban model dashboard**.

- **Report Filtering and Flagging**  
  Reports are filtered and flagged if duplicate issues are found.

- **CVSS / OWASP Risk Calculator**  
  Gerobug integrates the **CVSS** and **OWASP Risk Calculator** to assist in the bug review process.

- **Email Blacklisting**  
  Temporarily block and release emails that have been flagged for spam activity.

- **Auto Generate Certificate**  
  Gerobug can automatically generate certificates of appreciation for bug hunters, saving you time.

- **Personalization**  
  Customize Gerobug's appearance to match your brand colors.

- **Logging and Log Rotation**  
  Gerobug has internal audit logs with log rotation enabled.

- **Hall of Fame / Wall of Fame / Leaderboard**  
  Yes, we even have a **Hall of Fame** to recognize top contributors!

