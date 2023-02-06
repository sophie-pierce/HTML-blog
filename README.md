# HTML-Blog

## Azure Enviornment and Cloud Security

### Goal: Create a blog using front end and back end methods

Domain: Azure free domain

Domain Name: PrincessPeach

![sophie pierces cyber blog](https://user-images.githubusercontent.com/109919882/216469099-32b340e1-754c-4dfc-bcae-653d82f4fb64.png)

![blogpost1](https://user-images.githubusercontent.com/109919882/216469235-fb64f156-bba1-41ea-a345-79f928c2a447.png)

![blogpost2](https://user-images.githubusercontent.com/109919882/216469555-7ee10489-8cb8-448b-bdcb-32d3a2e60869.png)

### Networking

IP: 20.48.202.162
IP Location: Toronto, Ontario, Canada

DNS lookup for site:
<pre><code>nslookup</code></pre>

NS record result:

<pre><code>Server:  UnKnown
Address:  192.168.0.1

Non-authoritative answer:
Name:    https://princesspeach.azurewebsites.net/.Home
Addresses:  23.60.91.236
          23.200.237.236
</code></pre>

### Web Development

Runtimestack: 
- PHP 7.4
- Works on front end

On Linux command line, navigate to <pre><code>/var/www/html/assets</code></pre>

<pre><code>cat style.css</code></pre>

File contains back end HTML code for the blog:

<pre><code>* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: Helvetica;
  color: #082D49
}

a{
  text-decoration: none;
  color: #082D49
}


/* apply styles to <header> */
header {
  padding: 35px 35px;
  background-color: Linen;
}

Ect.
</code></pre>

### Cloud

Definitions:

- Cloud Tenant: a person who purchases cloud computing resource
- Access Policy: dictate which user, apllication, or group can alter Key Vault secrets, keys, and certificates
- Access policies protect against malicous attacks by ensuring *only* authorized individuals are    allowed to perform operations
- Keys: represented as JSON Web Key objects, supports many key types and algorithm, enables the use of software-protected and HSM-protected keys
- Secrets: passwords and database connection strings are considered secrets, the key vault accepts the data, encrypts, restores, and returns a secret identifier (ID)
- Certificates: built on top of secrets and keys, add an automated renewal feature. An addressable key and secret are created with the same name as a certificate when a new one is created.

### Cryptography

Self-assigned certificate from Azure 

![azurewebsitescert](https://user-images.githubusercontent.com/109919882/216470553-0c64b897-ade9-422c-b21c-2bd1e6f32134.png)


Validity of certificate: 13 months

Root certificate: DigiCert Trusted Root G4

### Cloud Security

Azure Door enabled

![azurefrontdoor](https://user-images.githubusercontent.com/109919882/216468902-b8d77185-127e-4a37-bce3-272eae1f9f54.png)

![azurefrontdoor2](https://user-images.githubusercontent.com/109919882/216468953-869039ac-220e-4824-ba6f-630d0fb20bf8.png)



Definition:

- SSL Offloading: SSL offloading is the process of removing the SSL based encryption from incoming traffic to relieve the web server from decryption of data. SSL offloading manages the encryption/decryption process on a separate device so it does not affect the web server’s performance.
          
- WAFs are firewalls that operate on Layer 7 and protect applications from common exploits such as SQL injection attacks.

WAF Custom Rule 

![WAF](https://user-images.githubusercontent.com/109919882/217040436-8e5ec3df-5260-44f2-890d-5c02361af7fa.png)

![WAFcustom](https://user-images.githubusercontent.com/109919882/217040005-600d2495-ce9c-4d3d-97c2-e9e105397d64.png)

![WAF2](https://user-images.githubusercontent.com/109919882/217040931-dee1fe8f-7d7f-487e-a550-8a943ecbc1a5.png)
