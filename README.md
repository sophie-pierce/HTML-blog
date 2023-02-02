# HTML-project-1

## Azure Enviorment and Cloud Security

### Goal: Create a blog using front end and back end methods

Domain: Azure free domain

Domain Name: PrincessPeach

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
- Keys: represented as JSON Web Key objects, supports many key types and algorithm, enables the use of software-protected and HSM-protected keys
- Secrets: passwords and database connection strings are considered secrets, the key vault accepts the data, encrypts, restores, and returns a secret identifier (ID)
- Certificates: built on top of secrets and keys, add an automated renewal feature. An addressable key and secret are created with the same name as a certificate when a new one is created.
