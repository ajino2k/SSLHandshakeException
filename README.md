# SSLHandshakeException
Resolving javax.net.ssl.SSLHandshakeException: sun.security.validator.ValidatorException: PKIX path building failed Error?

Resolv SSLshakeException for PMT to connect SDK API monitor transactions (/zserver/jdk1.7.0_11/ )

```echo -n | openssl s_client -connect domain.com:443 | sed -ne '/-BEGIN CERTIFICATE-/,/-END CERTIFICATE-/p' > /tmp/domain.crt```

```keytool -import -v -trustcacerts -alias domain.com -file /tmp/domain.crt -keystore /zserver/jdk1.7.0_11//jre/lib/security/cacerts -keypass changeit -storepass changeit```
