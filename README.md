# Cryptography

Below is an example from a friend of an AES encrypted message. I will decrypt it.

F4mEn+ap7qEBdu35sCWXyFcsCY3FhbgAROFIuiHW56vI1tJpJ2TgLLj4MZoEmSRNh2awn3mKpShslpOpolozpmR1lmKSDxiMODVOOypwrxM6qwI2HX1Fo+HxlKB+wOvWiHfJURdoeOs0eJsojj61J7KoNLWh+0+uMCi/0RxrQGgHVIT9qlWYIyh4uV+pvY9jKcq3aRu8zrfSoKG9H26Vm7UYgBSigMJI8tgo5/C1wY/UmLBNtiK2zIRpZSmQwTiNdwGj3fBJSoBwlyJWsXdNHgmK3/Br/O9Vy5f3nnhR/MtL2+0By1dmJaMs0P0Cmv1OWYu+7o9dot5oA/rTSLW9p4ejS20SOVps/GhUm9l4vTUQGzX056qfP2Om863YhAnKHHRh22jx4wl3kfcsj62soQKcui2mTbAeF56O53f+04GwfSB3BHgGsVuLnbjqQSjW7YlwRUA/stq374TsnmgoQYhW3fes1RdZNu08TWrM2bOG1SYs6KaVn54htqwy7Q0uCCIGZKWEIt+py75OwFtoa+gampHTuXi+oPEjIDi8Za5936NRzz5NZsnNua4ODV3AH7mJDShqxMvbcRPA0CA+arkhy6W6lcTf6HB4ztX97vY/FlUnSLKN6DDyhweumD0iQtK366yZkBsPELty+ikxUlz13Rk+5QvJvLBeW4qxGhJeb2n9o6Ue+Y8lARhLTHMWCunaaVqN6L9p69WjC6XqjR5h82bXCo3GEEwiaQz7KwGYo+vckPpnaubOu3hKJCZbk3yD8P3lhfmak8asbsZmAzYRgkQxvas6RGfQK9YAkdvgN+PlNpR26dzaMMUcowXYYJZuAKGfsiIjGHceXx+RZ199g++ABtRTV0xp8MdSXerq1/fX8SHlPKoooThaloKVZWKtVOszf+E/OEk0vv6V6A==

Key: F1D0F7E7B7D2B4F053FBA9332CA2F2CABB822A82316186D9EA5293C900B20330

IV:  6E7CDE9F6287EC339E23938E817F3F8E

Command to decrypt 

openssl enc -pbkdf2 -nosalt -aes-256-cbc -d -in meetingplace_update.txt.enc -base64 -K [partner key] -iv [partner IV]


Decrpyted message 

![image](https://user-images.githubusercontent.com/80080368/123197161-21e94880-d479-11eb-81db-92de54764a7a.png)


Generate your own key pair

![image](https://user-images.githubusercontent.com/80080368/123198721-98874580-d47b-11eb-9de3-439f0f9cd7f2.png)



command to encrypt 

openssl enc -pbkdf2 -nosalt -aes-256-cbc -in meetingplace_update.txt -out meetingplace_update.txt.enc -base64 -K <your_key> -iv <your_iv>

![image](https://user-images.githubusercontent.com/80080368/123199033-206d4f80-d47c-11eb-968b-41c74a546616.png)


