## TY51822r3へのファームウェアの書き込み方

この手順は、[TY51822r3ボード](https://www.switch-science.com/catalog/2574/)を購入後、1回だけ行えばOKです。

### 用意するもの

- USB端子のついたPC x 1
- [スイッチサイエンス TY51822r3](https://www.switch-science.com/catalog/2574/) x 1
- USB通信ケーブル (microB端子 <-> 標準A端子) x 1

### 1. ファームウェアのダウンロード

まずPCで[ファームウエア（btGPIO_TY51_20181220.hex）](http://chirimen.org/chirimen-TY51822r3/bc/ble_fw/btGPIO_TY51_20181220.hex)をダウンロードします。

`btGPIO_TY51_20181220.hex`という名前で保存してください。

### 2. PCにTY51822r3ボードを接続

次に、PCにUSBケーブルを使って`TY51822r3`を接続します。
「MBED」というドライブがマウントされます。

> もしドライブがマウントされない場合はケーブルがデータ通信対応であることを確認してください。

### 3. TY51822r3へのファームウエア書き込み

「MBED」ドライブに`btGPIO_TY51_20181220.hex`をコピーします。（ドラッグ＆ドロップでOK）

コピー中は`TY51822r3`ボード上の赤色LEDが点滅します
コピーが終わると再度「MBED」ドライブがマウントされます。

「MBED」ドライブがマウントされたら、一旦「MBED」ドライブを開いてみてください。
FAIL.TXTがあった場合はケーブルを繋ぎ直して再起動してください。

### 4. 再起動

書き込みに成功したら`TY51822r3`ボード上のスイッチを押してボードを再起動してください。

書き込んだファームウエアが起動します。

