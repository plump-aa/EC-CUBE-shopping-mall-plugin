# ショッピングモールプラグイン

## 概要
[複数ショップの商品を掲載するプラグイン](https://www.ec-cube.net/products/detail.php?product_id=2030)

## フロント画面
### 商品一覧・詳細ページからショップの外部販売サイトへ誘導できる。
- 商品の外部販売サイトが登録されている場合は、販売サイトへリンクする。
- 価格を非表示にできる。

## 管理画面
### ショップを登録することができる。
- 設定>複数ショップ管理画面で、ショップを登録、削除することができる。

    - 登録した際にショップ用の販売種別が登録される。
    - 受注用メールアドレスを登録すると、そのアドレス宛に受注メールが送信される。

### ショップの商品・受注管理用メンバーを登録することができる。
- 設定>システム設定>メンバー管理画面で、ショップの商品・受注管理用メンバーを登録、削除することができる。

### 商品ごとに、外部販売サイト、価格表示、を設定することができる。
- 商品管理で、外部販売サイト、価格表示、を設定することができる。

### ショップごとの受注機能を利用することができる。
- ショップ用の販売種別で登録された商品を受注した際にショップごとの受注となります。

## 利用手順の例
### 管理者で管理画面表示
1. ショップ登録
    - 設定>複数ショップ管理画面でショップを登録する。

2. ショップのメンバー登録
    - 設定>システム設定>メンバー管理画面でショップの商品・受注管理用メンバーを登録する。
    - １で設定したショップを選択、権限「ショップ（ショッピングモールプラグイン用）」を選択し登録する。（権限はショップを選択した際に自動で選択される）

### ショップの商品登録用メンバーで管理画面表示
3. 商品登録
    - 外部販売サイトや価格表示等を設定し、商品を登録する。

4. CSVで商品登録したい場合
    - 商品管理>商品CSV登録画面で商品を登録し、商品管理>ショップ用商品CSV登録画面で商品を更新する。

### フロント画面
5. 商品掲載
    - 外部販売サイトが設定されていれば「カートに入れる」が「販売サイトへ」に変わり、価格表示の設定内容によって、価格が表示・非表示にされる。

## アップデート
- v1.0.1 からのアップデートでショップごとの受注を利用する際は、複数ショップ管理画面でショップ情報を更新してください。受注に利用する販売種別が登録されます。

## 注意
- エラーでログインできない場合は、サーバーの「var/cache/prod/」以下全てを削除すれば解決するかもしれません。
- 複数ショップ管理メニューが表示されない場合は、コンテンツ管理のキャッシュ管理でキャッシュを何回も削除します。
- ショップ用のメンバーでログインすると、設定の店舗設定に基本設定メニューがありますが、配送方法設定へ転送されます。
- 店舗設定の基本設定メニューが非表示になっていないのはURLの /setting/shop 単体でアクセス拒否できないのが理由です。

## ライセンス

MIT
