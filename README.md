# epchian-adapter

本项目适配了openwallet.AssetsAdapter接口，给应用提供了底层的区块链协议支持。

## 如何测试

openwtester包下的测试用例已经集成了openwallet钱包体系，创建conf文件，新建EP.ini文件，编辑如下内容：

```ini

# transaction type
txType = "cosmos-sdk/StdTx"
# message type
msgSend = "cosmos-sdk/MsgSend"
msgVote = "cosmos-sdk/MsgVote"
msgDelegate = "cosmos-sdk/MsgDelegate"
# message choose 1-send  2-vote  3-delegate
msgType = 1


# mainnet rest api url
mainnetRestAPI = "http://47.57.26.144:20036"
# mainnet node api url
mainnetNodeAPI = ""
# chain id
mainnetChainID = "epc-v1"
# mainnet denom
mainnetDenom = "uepc"

# testnet rest api url
testnetRestAPI = ""
# testnet node api url
testnetNodeAPI = ""
# chain id
testnetChainID = ""
# testnet denom
testnetDenom = ""

# Is network test?
isTestNet = false

# scan mempool or not
isScanMemPool = false

# pay fee or not
payFee = true
# minimum fee to pay in muon/uatom(1 mon = 1000000muon , 1 atom = 1000000uatom)
minFee = 500000
# standed gas
stdGas = 200000

# Cache data file directory, default = "", current directory: ./data
dataDir = ""
```
