# moipodapp
MOI pod client app is used to start a moi pod binary and fetch statistics
Please refer to qavalidator.moinet.io website for more details : 



MAC-OS :

clone this repo :  git clone https://gitlab.com/sarvalabs/moinet/moipod-binary.git
-- cd moipod-binary
switch branch to mac-os : git checkout mac-os
execute "npm i @nuid/zk@0.0.12 -g"
execute "./moipod.mac-os --type setup -nodedir ."
execute "./moipod.mac-os --type run --nodedir . --pass Test@123"
--pass flag is the local keystore password provided during the setup stage.

LINUX :

clone this repo : git clone https://gitlab.com/sarvalabs/moinet/moipod-binary.git

switch branch to linux-os : git checkout linux-os
execute "npm i @nuid/zk@0.0.12 -g"
execute "./moipod.linux-os --type setup -nodedir ."
execute "./moipod.linux-os --type run --nodedir . --pass Test@123"
--pass flag is the local keystore password provided during the setup stage.

WINDOWS :

clone this repo
switch branch to windows-os.
execute "npm i @nuid/zk@0.0.12 -g"
execute "./moipod.windows-os --type setup -nodedir ."
execute "./moipod.windows-os --type run --nodedir . --pass Test@123"
--pass flag is the local keystore password provided during the setup stage.

TO SEE YOUR INCENTIVE : PASS YOUR KRAMAID TO BELOW COMMAND :
curl --location --request POST 'https://qapnapi.moinet.io/moi/readtokeninfo' 
--header 'Content-Type: application/json' 
--data-raw '{
"krama_id":"UhJNSsPZ8TdvqELKefQhspevrKpqJ1LBVW5Ks7cmWtsxdRNRsFmRAGJeii4nMxEjjd1Y3NMkZhhEyep8mxCLCpjByd24mRLXZXFjRzX8FfnGAeBhA9tXST6vaxHXg8McrTz7fhJXcRF7t8FqaCnm4PCyJYMbEaiBGVBnvkmAgZU1PEZGrvmpa4t.16Uiu2HAmLoNu7Hy6MD4pSBuWBF7YJdz6U6TeJ4iJzjSVSUPBC3j7",
"epoch_id": "1",
"start_timestamp": 0,
"end_timestamp" : 9999999999
}
'
