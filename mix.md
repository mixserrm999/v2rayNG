`keytool -genkeypair -v -keystore my-release-key.jks -keyalg RSA -keysize 2048 -validity 10000 -alias my-key-alias`
`[Convert]::ToBase64String((Get-Content -Path my-release-key.jks -Encoding Byte)) | Set-Content keystore.b64`
