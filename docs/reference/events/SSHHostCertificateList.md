
|&nbsp;|&nbsp;|&nbsp;|&nbsp;|
|---|---|---|---|
| ssh_host_certificates.id | string | | unique identifier for this SSH Host Certificate |
| ssh_host_certificates.uri | string | | URI of the SSH Host Certificate API resource |
| ssh_host_certificates.created_at | string | | timestamp when the SSH Host Certificate API resource was created, RFC 3339 format |
| ssh_host_certificates.description | string | | human-readable description of this SSH Host Certificate. optional, max 255 bytes. |
| ssh_host_certificates.metadata | string | | arbitrary user-defined machine-readable data of this SSH Host Certificate. optional, max 4096 bytes. |
| ssh_host_certificates.public_key | string | | a public key in OpenSSH Authorized Keys format that this certificate signs |
| ssh_host_certificates.key_type | string | | the key type of the `public_key`, one of `rsa`, `ecdsa` or `ed25519` |
| ssh_host_certificates.ssh_certificate_authority_id | string | | the ssh certificate authority that is used to sign this ssh host certificate |
| ssh_host_certificates.principals | List&lt;string&gt; | | the list of principals included in the ssh host certificate. This is the list of hostnames and/or IP addresses that are authorized to serve SSH traffic with this certificate. Dangerously, if no principals are specified, this certificate is considered valid for all hosts. |
| ssh_host_certificates.valid_after | string | | the time when the ssh host certificate becomes valid, in RFC 3339 format. |
| ssh_host_certificates.valid_until | string | | the time after which the ssh host certificate becomes invalid, in RFC 3339 format. the OpenSSH certificates RFC calls this `valid_before`. |
| ssh_host_certificates.certificate | string | | the signed SSH certificate in OpenSSH Authorized Keys format. this value should be placed in a `-cert.pub` certificate file on disk that should be referenced in your `sshd_config` configuration file with a `HostCertificate` directive |
| uri | string | | URI of the ssh host certificates list API resource |
| next_page_uri | string | | URI of the next page, or null if there is no next page |