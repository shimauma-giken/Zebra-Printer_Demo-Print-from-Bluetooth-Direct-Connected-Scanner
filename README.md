## ADF2.0を用いてBluetooth経由でスキャナから直接ラベル印刷をする方法

本ガイドはDS8178をベースに説明をする。
他スキャナを利用の際は設定が一部異なる可能性があることをご了承頂きたい。

</br>

1. プリンタとスキャンを工場出荷状態に戻す。

1. 下記scncfgファイルを用いて、123ScanでADF2.0の設定をする。

    > 参考設定  
    > "Config File_DS8178_Untitled1_2023.11.18.scncfg"

1. 123Scanを終了。

1. Notepadを開く。バーコードをスキャンした結果として、下記のようなZPLがアウトプットされれば正常に設定されている。

        ＾XA^FO50,50^BCN,100,Y,N^FD4904910024940^FS^XZ

1. プリンタとスキャナをBluetooth接続する。

    > Zebra BlutoothスキャナとZebra プリンタと直接接続する方法  
    > https://github.com/shimauma-giken/Zebra-Scanner-How-to-direct-connect-bluetooth-scanner-to-printer

1. JANコードなどのバーコードをスキャンする。スキャンした内容に応じたバーコードがプリンタから出力されれば設定は完了。

