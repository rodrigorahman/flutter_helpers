# Gerando chave Android
keytool -genkey -v -keystore ./key.jks -keyalg RSA -keysize 2048 -validity 10000 -alias key

# Vendo Chave
keytool -exportcert -list -v -alias key -keystore ./key.jks
