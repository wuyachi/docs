# DevNet

This is zion side chain network setup configuration file ONLY in <strong>DEVNET</strong> mode, it's used to build and attach zion nodes.


## Genesis file
```dat
{
    "config": {
        "chainId": 108, 
        "homesteadBlock": 0,
        "eip150Block": 0,
        "eip155Block": 0,
        "eip158Block": 0,
        "byzantiumBlock": 0,
        "constantinopleBlock": 0,
        "petersburgBlock": 0,
        "hotstuff": {
            "protocol": "basic"
        }
    },
    "alloc": {
        "0x09f4E484D43B3D6b20957F7E1760beE3C6F62186": {"publicKey": "0x030187435897ad02f6340915f18a5b5c3879a78968044605e18499d9bef48ba4a8", "balance": ""},
        "0x294b8211E7010f457d85942aC874d076D739E32a": {"publicKey": "0x03df2a729a896e41e80475525ac93524b041bafe06a22e61d59d9233df6279f4fc", "balance": ""},
        "0x9deAD91D8632DCEEC701710bAF7922324DD45F58": {"publicKey": "0x03ff211d429616c46ce57b7ff15527b9b1df7e08d1221ea2298eeb530bd0673902", "balance": ""},
        "0xc5e2344b875e236b3475e9e4E70448525cA5210F": {"publicKey": "0x02139a07905f7cfa2740437d728bf5c60f4c7c4a263edafd4f1437f6f6f712b361", "balance": ""}
    },
    "coinbase": "0x0000000000000000000000000000000000000000",
    "difficulty": "0x1",
    "extraData": "0x0000000000000000000000000000000000000000000000000000000000000000f89bf8549409f4e484d43b3d6b20957f7e1760bee3c6f6218694294b8211e7010f457d85942ac874d076d739e32a949dead91d8632dceec701710baf7922324dd45f5894c5e2344b875e236b3475e9e4e70448525ca5210fb8410000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000c080",
    "gasLimit": "0xffffffff",
    "nonce": "0x4510809143055965",
    "mixhash": "0x0000000000000000000000000000000000000000000000000000000000000000",
    "parentHash": "0x0000000000000000000000000000000000000000000000000000000000000000",
    "timestamp": "0x00"
}
```

## Validators

Address | Public Key
---|---
0x09f4E484D43B3D6b20957F7E1760beE3C6F62186|0x030187435897ad02f6340915f18a5b5c3879a78968044605e18499d9bef48ba4a8
0x294b8211E7010f457d85942aC874d076D739E32a|0x03df2a729a896e41e80475525ac93524b041bafe06a22e61d59d9233df6279f4fc
0x9deAD91D8632DCEEC701710bAF7922324DD45F58|0x03ff211d429616c46ce57b7ff15527b9b1df7e08d1221ea2298eeb530bd0673902
0xc5e2344b875e236b3475e9e4E70448525cA5210F|0x02139a07905f7cfa2740437d728bf5c60f4c7c4a263edafd4f1437f6f6f712b361

## Machine
IP | SSH Port 
---|---
101.32.98.88|22
124.156.208.166|22

## Nodes
Node Index | IP | Rpc Port | Mode
---|---|---|---
0|101.32.98.88|22000|Miner
1|124.156.208.166|22000|Miner
2|101.32.98.88|22001|Miner
3|124.156.208.166|22001|Miner

## Main chain Contracts
ChainID | CrossChainID | Contract Name | Contract address
---|---|---|---
10897 | 1 | native lock proxy | 0x7d79D936DA7833c7fe056eB450064f34A327DcA8
10897 | 1 | native token wrapper | 0x5D315b2f0C63890eFbfB37c26E0ae0807e72bCc9

## Side chain Contracts
ChainID | CrossChainID | Contract Name | Contract address
---|---|---|---
108 | 77 | eccd | 0x34d4a23A1FC0C694f0D74DDAf9D8d564cfE2D430
108 | 77 | eccm | 0xc6195336878Fc34B1b5A13895015a97c1aD9cc25
108 | 77 | native lock proxy | 0x7d79D936DA7833c7fe056eB450064f34A327DcA8
108 | 77 | native token wrapper | 0x3b2749D4Ca77837730e8ff8318DC9cc688595E95