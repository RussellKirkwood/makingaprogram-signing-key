# makingaprogram-signing-key

helpful reference.
https://bernhardelbl.wordpress.com/2012/03/20/create-a-non-expiring-test-certificate-pfx-for-clickonce-applications/

to make the cert
makecert -sv XXX.pvk -n CN=XXX XXX.cer -b 05/01/2020 -e 12/31/2030 -r

to make private key
pvk2pfx -pvk "XXX.pvk" -spc "XXX.cer" -pfx "XXX.pfx"
