# VPN Test Lab Report

## Scope
Implement and test a VPN in a virtual environment.

## Prerequisite Technologies
- A virtual machine on the Azure Cloud.
- A personal computer with an internet connection.
- A VPN solution like **Proton VPN**.

---

## Steps

### 1. Observe IP Address from Local and Virtual Machines
1. Browse to [https://whatismyipaddress.com](https://whatismyipaddress.com) from your personal computer and take note of the IP address.
2. Create a resource group and associated **Windows 10 VM** in the Azure cloud.
3. From the VM, visit [https://whatismyipaddress.com](https://whatismyipaddress.com) and take note of the IP address.

### 2. Sign Up and Connect to VPN
1. Sign up for the free version of **Proton VPN** on your local PC.
2. Inside the VM, download and install the **Proton VPN client**.
3. Log in at [https://account.protonvpn.com/login](https://account.protonvpn.com/login).
4. Choose a VPN server in another country and connect.
5. Visit [https://whatismyipaddress.com](https://whatismyipaddress.com) again and note the new IP address.
6. Try browsing to sites like **Google**, **Disney**, or **Amazon** to observe any regional differences such as language or localized content.

---

## Findings
1. From my **local PC**, I found my original IP address using [whatismyipaddress.com](https://whatismyipaddress.com).
2. From the **Azure VM**, the IP address was `71.237.117.117`, located in **Quincy, Washington**.
3. After connecting to **Proton VPN**, the new IP address was `169.150.218.4`, located in **Amsterdam, Noord-Holland, Netherlands**.
4. Visiting **YouTube Trending** while connected to the VPN showed a lot of local content from the Netherlands.
5. After switching to another Proton VPN server, I received IP `185.177.126.133`, located in **Naaldwijk, Zuid-Holland, Netherlands**.

---

## Conclusion
- The VPN successfully masked my real IP address and changed my perceived geographic location.
- Websites adapted their content based on the detected region.
- This experiment demonstrated how VPNs enhance privacy and allow users to bypass geographic restrictions.
