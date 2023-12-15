# SSH (Secure Shell) Cheatsheet

## 1. Connect to a Remote Server
```bash
ssh username@remote_host
```
**Example:**
```bash
ssh john@example.com
```

## 2. Connect with a Specific Port
```bash
ssh -p port_number username@remote_host
```
**Example:**
```bash
ssh -p 2222 john@example.com
```

## 3. Specify Identity File (Private Key)
```bash
ssh -i /path/to/private_key username@remote_host
```
**Example:**
```bash
ssh -i ~/.ssh/id_rsa john@example.com
```

## 4. SCP (Secure Copy)

### Copy Local File to Remote Server
```bash
scp /path/to/local/file username@remote_host:/path/on/remote/server
```

### Copy Remote File to Local Machine
```bash
scp username@remote_host:/path/to/remote/file /path/on/local/machine
```
**Example:**
```bash
scp /path/to/local/file john@example.com:/home/john/documents
```

## 5. Forward Local Port to Remote Server
```bash
ssh -L local_port:localhost:remote_port username@remote_host
```
**Example:**
```bash
ssh -L 8080:localhost:80 john@example.com
```

## 6. Generate SSH Key Pair
```bash
ssh-keygen -t rsa -b 2048
```
**Example:**
```bash
ssh-keygen -t rsa -b 4096
```

## 7. Copy SSH Public Key to Remote Server
```bash
ssh-copy-id username@remote_host
```
**Example:**
```bash
ssh-copy-id john@example.com
```

## 8. Close SSH Connection
Type `exit` and press Enter.

## 9. SSH Config File
The SSH config file is located at `~/.ssh/config` and can be used to configure various SSH settings.
```bash
Host example
    HostName example.com
    User john
    Port 2222
    IdentityFile ~/.ssh/id_rsa_example
```
