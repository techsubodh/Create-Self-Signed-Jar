# Create-Self-Signed-Jar
How to Create a (Self-)Signed Jar

Folloow Below Steps to self sign the Jar 

Steps,

1.	Open cmd (default location will be – ‘C:\Users\subodh’)
2.	Create Keystore- keytool -genkey -keyalg RSA -alias myJarKey -keystore myKeystore -validity 360
3.	it will create ‘myKeystore’ certificate in ‘C:\Users\subodh’
4.	signhed with jarsigner tool - Go to jar derectory where jar ’myjar.jar’  is lactated ‘C:\jarfile’ and copy ‘keystore’ from ‘C:\Users\subodh’ to ‘C:\jarfile’
5.	Execute ‘jarsigner.exe -keystore myKeystore -verbose myjar.jar myJarKey’ 

