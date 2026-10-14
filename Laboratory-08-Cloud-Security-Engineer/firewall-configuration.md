# Firewall Configuration

## 1. Allow SSH

Command used:

```bash
sudo ufw allow ssh
```

This rule allows SSH connections through port 22 so remote administration can remain accessible.

## 2. Configure Default Policies

Commands used:

```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
```

The default-deny incoming policy blocks incoming connections unless an existing firewall rule allows them. Outgoing connections are allowed by default.

## 3. Enable the Firewall

Command used:

```bash
sudo ufw enable
```

To verify the firewall configuration, I used:

```bash
sudo ufw status verbose
```

The status showed that UFW was active, incoming traffic was denied by default, and outgoing traffic was allowed.

## 4. Allow the Web Application Port

Command used:

```bash
sudo ufw allow 8080/tcp
```

This rule allows TCP traffic through port 8080 for the web application.

## 5. Firewall Safety

Enabling UFW before allowing SSH can block remote SSH access and may lock an administrator out of the server. Therefore, the SSH rule should be added before enabling the firewall.
