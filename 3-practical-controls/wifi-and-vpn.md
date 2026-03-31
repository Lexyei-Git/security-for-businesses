# Wi‑Fi and VPN

Wi‑Fi and remote access are essential for most small and medium businesses, but they also create common entry points for attackers if not configured securely.

This document explains, in practical terms, how to secure your business Wi‑Fi networks and when and how to use a virtual private network (VPN).

---

## 1. Why Wi‑Fi and VPN security matter

Unsecured or poorly configured Wi‑Fi can allow attackers or unauthorized users to:

- Connect to your internal network from outside your office.  
- Intercept unencrypted traffic and capture sensitive data.  
- Use your network as a launch point for further attacks.

Remote workers connecting from home or public Wi‑Fi are also at higher risk if their connections to your business systems are not properly secured.

A VPN helps create an encrypted tunnel between remote devices and your company network or services, reducing the risk of interception or tampering.

---

## 2. Securing your business Wi‑Fi

### 2.1 Basic configuration expectations

For your main business Wi‑Fi network:

- **Change default settings**
  - Change the default Wi‑Fi network name (SSID) to something that does not reveal your router model or your business identity too clearly.  
  - Change the default administrator username and password for the router or access point.

- **Use strong encryption**
  - Use **WPA2‑Enterprise** or **WPA3‑Enterprise** where possible, especially for larger environments.  
  - For smaller setups that cannot support Enterprise mode, use at least **WPA2‑Personal** or **WPA3‑Personal** with a strong, unique passphrase.

- **Use a strong Wi‑Fi password or passphrase**
  - Avoid short or easy passwords.  
  - Use a long, random or passphrase‑style password that is not reused elsewhere.

- **Update firmware**
  - Keep router and access point firmware up to date to address security vulnerabilities.

### 2.2 Segmentation: business, guest and devices

Do not put everything on a single Wi‑Fi network.

A simple structure:

- **Primary business network**
  - Used by company‑managed devices and staff for business activities.  
  - Protected with strong encryption and a strong password.  
  - Access limited to authorized staff and devices.

- **Guest network**
  - Separate network for visitors, customers and personal devices.  
  - Isolated from the primary business network (guest users should not be able to see internal servers or devices).  
  - Use rate limits and content controls as needed.

- **IoT / smart devices network**
  - Separate network for less‑trusted devices such as cameras, smart TVs, printers and IoT devices.  
  - Isolated from your main business systems as much as possible.

Network segmentation reduces the impact if one device or network is compromised.

---

## 3. Safe use of public and home Wi‑Fi

Business devices used outside the office are exposed to greater risk, especially on public Wi‑Fi.

Guidance for staff:

- **Avoid using untrusted open Wi‑Fi** for sensitive activities.
  - Prefer networks that require a password and are operated by reputable organizations.  

- **Use a VPN on public Wi‑Fi**
  - If staff must use public Wi‑Fi (for example, hotels, airports, cafés), they should connect through a business VPN before accessing business systems or sensitive data.

- **Treat home networks as less secure than office networks**
  - Encourage staff to:
    - Change default router admin passwords at home.  
    - Use WPA2 or WPA3 encryption and a strong Wi‑Fi password.  
    - Place work devices on a separate network if their routers support guest or multiple SSIDs.

---

## 4. What a VPN is and when to use it

A **virtual private network (VPN)** creates an encrypted tunnel between a device (for example, a laptop) and a VPN gateway or service.

VPNs are useful for:

- **Remote access to internal resources**
  - Allowing staff to securely access internal file servers, applications or intranet sites when away from the office.

- **Protecting traffic on untrusted networks**
  - Encrypting data between remote devices and your business environment when using public or home Wi‑Fi.

For small and medium businesses, a VPN is highly recommended when:

- Staff regularly work remotely or from home.  
- Sensitive internal systems are not directly exposed to the internet but must be reachable by remote users.  
- Staff often travel or connect from public Wi‑Fi networks.

---

## 5. Basic VPN best practices

When introducing or reviewing VPN use, consider these points:

- **Strong authentication**
  - Require **MFA** for VPN access (for example, password plus authenticator app or hardware token).  
  - Use strong, unique passwords for VPN accounts.

- **Limit who can use the VPN**
  - Only staff who need remote access should have VPN accounts.  
  - Remove access when people leave or no longer need it.

- **Limit what the VPN can reach**
  - Use firewalls and access control rules so VPN users can only reach the systems and services they need, not your entire internal network.

- **Keep VPN software and devices patched**
  - Regularly update VPN servers, clients and network devices that provide VPN functionality to fix vulnerabilities.

- **Define which devices may connect**
  - Prefer company‑managed devices that meet your security baseline (for example, with up‑to‑date antivirus and patches).  
  - Be cautious about allowing unmanaged personal devices to connect directly to your internal network.

Depending on your setup, the VPN may connect users to:

- Your internal office network.  
- A virtual private network provided by a security or network service provider.  
- Specific cloud resources via a secure tunnel.

---

## 6. Combining Wi‑Fi security and VPN

Wi‑Fi security and VPN are complementary:

- Secure Wi‑Fi (strong encryption, segmentation, strong admin passwords) helps protect your **local network**.  
- A VPN protects **traffic over untrusted networks** and provides secure remote access.

For many small and medium businesses, a sensible combined approach is:

- Internal office:
  - Use secure Wi‑Fi with WPA2/WPA3, segmented networks, and strong passwords.  
  - Use firewalls to separate Wi‑Fi networks from critical servers.

- Remote work and travel:
  - Require VPN use for accessing internal systems over the internet or public Wi‑Fi.  
  - Enforce MFA on VPN and remote access.

This aligns well with baseline guidance for small and medium organizations and common national small‑business security recommendations.

---

## 7. Minimal checklist for Wi‑Fi and VPN

Use this checklist as a quick status check:

- [ ] Our business Wi‑Fi uses WPA2 or WPA3 encryption and a strong, unique password or passphrase.  
- [ ] Default router/admin usernames and passwords have been changed.  
- [ ] We have separated our primary business network from guest and IoT/smart device networks.  
- [ ] Wi‑Fi routers and access points are kept up to date with current firmware.  
- [ ] Staff understand the risks of public Wi‑Fi and when to avoid it.  
- [ ] A business VPN is available for remote work and use on public Wi‑Fi.  
- [ ] VPN access requires MFA and is limited to staff who need it.  
- [ ] VPN and associated network devices are patched and monitored.

Unchecked boxes indicate areas to focus on in your next 30–90 days of security improvements.
