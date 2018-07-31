# DNS module implementation for ns-3 simulator.

## 目的

[janakawest/DNS-for-NS3](https://github.com/janakawest/DNS-for-NS3) をndnSIMで動かす


## 導入方法

```sh
# ndnSIM推奨のシナリオ作成できるところまでやる
cd <your-scenario-dir>

# このリポジトリをextensions以下にサブモジュールとして加える
git submodule add https://github.com/kmdkuk/DNS-for-ndnSIM.git extensions/dns

# ビルド
./waf

# dns-example.ccをscenariosに用意(このリポジトリにはない)
# 大元のdns-exampleがそのまま使える
# https://github.com/awaki75/DNS-for-NS3/blob/master/examples/dns-example.cc

# dns-exampleを実行
./waf --run scratch/dns-example --vis
```

まだ出来てないけど頑張ってできるようにします。
