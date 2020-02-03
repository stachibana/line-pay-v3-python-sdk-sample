![Screen Shot](https://cl.ly/f91d9e56c17c/pay_sdk_usage_02.png)

# Overview

LINE Pay API v3のPython版SDKの動作を確認出来るWeb Appです。[kintone](https://kintone.cybozu.co.jp/)と連携しているため、過去の取引の一覧を確認したり、返金、オーソリ無効化、自動決済(サブスク)の動作確認も可能です。

[SDK](https://github.com/sumihiro3/line-pay-sdk-python)

# Prepare

## LINE Pay API

* `.env_sample`を`.env`にリネーム
* `.env`記載のID、SECRETをご自身のものに置き換え
  * 加盟店審査が完了している方はご自身のもので
  * まだの方は[Sandbox](https://pay.line.me/jp/developers/techsupport/sandbox/testflow?locale=ja_JP)を作成
* Sandboxを利用しない方は`app.py`の上の方の`LINE_PAY_IS_SANDBOX`を`False`に変更

## kintone

* [開発者ライセンス](https://developer.cybozu.io/hc/ja/articles/360025742471)の申し込み
* `account.yml_sample`を`account.yml`にリネーム
* 以下の画像の通り設定

![kintone description](https://cl.ly/28f3d463696e/kintone_description.png)

## Execute

```bash
$ pip install -r requirements.txt
$ python app.py
```

__Then needs to use ngrok or some tunneling tool to check!__
