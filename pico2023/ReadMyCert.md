## Details:
### Challenge name: 
ReadMyCert

### Category: 
Cryptography

### Description: 

How about we take you on an adventure on exploring certificate signing requests <br> Take a look at this CSR file [here](https://artifacts.picoctf.net/c/424/readmycert.csr).


## Solve:

Opening the file (I just put it in my web browser), we get this:

`-----BEGIN CERTIFICATE REQUEST-----` <br> 
`MIICpzCCAY8CAQAwPDEmMCQGA1UEAwwdcGljb0NURntyZWFkX215Y2VydF81YWVi
MGQ0Zn0xEjAQBgNVBCkMCWN0ZlBsYXllcjCCASIwDQYJKoZIhvcNAQEBBQADggEP
ADCCAQoCggEBAMCkf11rmV8rgqPvC2ZiPA6W+5RfOTwU6u3WpGvLA+2YFzocBPut
aATTxTPB+uaN2ZN3Z5J2CTFGmPzI4sUQfSqhZGuAqbfMyDDR8pRswmIYVJ6s0Apc
Toi7H8m3IShSbeE0pZUSIJpbK1a7V6lJqgwFMDI1qrgNhGgZaMA/l+d2J0vC3EYd
AijwSs8APcp6woWbFGYwdw5KaBsjn23oVz2G4h3/TmdB5g5e6Oq+kgi38NEpRDS0
ylXo9mUko3FqS4I6y9gOtDEI4uZaCJZuXHDmBpqZ04MfXbIVlHjF9NMOjDvXLonN
650oaANBm4bhBlgid0Fx48Z36tbtAVivZEcCAwEAAaAmMCQGCSqGSIb3DQEJDjEX
MBUwEwYDVR0lBAwwCgYIKwYBBQUHAwIwDQYJKoZIhvcNAQELBQADggEBAHZx6h9r
G/SE7RCoX6ndk5BOJprRiHpxOqPLAWcDyKHfStln0/HcQZzIrRVRsmoHiOmch+md
PBA1b+M5aj+3BWtPR9jOY4vht+ZmHAKa0WfQxwb2dBxsRPKTTDea0wN2u8BHLlSM
PbWPNuz+TKySL41xfwFuM4VN/ywn58GTvdb7HXgwNZCGgo2N1WhRq/dBMiagXMah
yb6gX4erugCu61T5tyD80hgsNBjaqyIdy/whRfC/Pmn3QHmdkqB5ZCPezwb2OLm4
5RDGv3WOB5q0BofoUGhVq757QE8qhL3oTvV2WlLoi3YWaZkJMCeR3vnH92cKC1Ov
FxdQuLOH8GMvl7U=` <br>
`-----END CERTIFICATE REQUEST-----`

A CSR is a certificate signing request, an encrypted block of text sent to apply for a digital identity certificate. 
I found a [CSR decoder](https://www.sslshopper.com/csr-decoder.html) online. Decoding the encrypted text, we see that the common name contains the flag: `picoCTF{read_mycert_5aeb0d4f}`

<img width="548" alt="CSR decoded" src="https://github.com/uuu2q/ctf-writeups/assets/134032122/de4e5aff-a895-446e-bcef-f30266d0e79d">

