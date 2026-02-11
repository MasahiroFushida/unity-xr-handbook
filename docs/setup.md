---
title: 環境構築
permalink: /setup/
---

# 環境構築
unity 6000.3.3f1 以降をインストールしてください。
- [Unity Hub](https://unity.com/download) をインストール
- Unity Hub から Unity 6000.3.3f1 以降をインストール

プロジェクトを作成
- Unity Hub を開く
- 「新規作成」をクリック
- テンプレートは「Universal 3D」を選択
- プロジェクト名を入力
- 「作成」をクリック

Asset Store or Package Manager から以下のパッケージをインストールしてください。
- Meta XR Core SDK (必要あれば、sampleもインストールしてください)
- Meta Interaction SDK（必要あれば、sampleもインストールしてください）
- OpenXR Plugin（Unity Registryからインストールしてください）

(File)-(Build Profiles)を開き、Androidを選択して、<Switch Platform>をクリックしてください。

(Edit)-(Project Settings)を開き、<XR Plug-in Management>を選択し、Androidタブでoculusにチェックを入れてください。DesktopタブではOculusにチェックを入れてください。

Target DeviceをQuest3に設定してください。

OpenXRのMeta XRの設定
- Android
![alt text](/docs/handson/asset/setup/image.png)

- Desktop
![alt text](/docs/handson/asset/setup/image-1.png)

- Project Setup Tool でFix All
![alt text](/docs/handson/asset/setup/image-2.png)


(Edit)-(Project Settings)-(Player)を開き、Player タブで以下の設定を行ってください。


![alt text](/docs/handson/asset/setup/image-4.png)


Override Default Package Nameのチェックを外す
![alt text](/docs/handson/asset/setup/image-5.png)