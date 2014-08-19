==========================
LabVIEW TSVN_LvPlugin
==========================

# 概要
  LabVIEW開発環境のツールメニューにTortoiseSVNの Log/Add/Commit/Export の項目
を追加するためのプラグインVIです。
  LabVIEW用のTortoiseSVNツールキットといえば、ViewpointSystemsの
TSVN Toolkitが有名ですが、そこまでしなくても、とりあえず編集中のVIのログが
見れて、add/commitの操作ができれば、という軽めの用途向け。
  TortoiseSVNのコマンドラインTortoiseProc.exeを呼び出しますので、
TortoiseSVNがインストールされている必要があります。
  また、すでにSVN管理されているソース・ファイルが対象になります。
SVNへの登録等の操作は、TortoiseSVNを使って行ってください。

ちなみにTSVN Toolkitはこちら
  http://www.viewpointusa.com/product/ni-labview-toolkits/tsvn-toolkit/

# インストール

## 対応する環境
  LabVIEW 2009 で作成しています。Windows用です。

## インストール方法
  TSVN_Add_LvPlugin.vi、TSVN_Commit_LvPlugin.vi、TSVN_Log_LvPlugin.vi、TSVN_Export_LvPlugin.viの
４つのファイルを LabVIEW インストールフォルダの所定の場所にコピーするだけです。

## インストールする場所
LabVIEW 32bit版の場合、以下の場所にファイルをコピーします。


    Windows 32bit:
      C:\Program Files\National Instruments\LabVIEW 20xx\project

    Windows 64bit:
      C:\Program Files(x86)\National Instruments\LabVIEW 20xx\project

  "20xx" の部分には使用しているLabVIEW のバージョン(2009,2010,2011,2012,...)
が入ります。複数バージョンがインストールされている場合は、それぞれの
バージョンのprojectフォルダにコピーしてください。

  ファイルをコピーした後、LabVIEWを再起動すると、ツールメニューに
"TSVN Add","TSVN Commit","TSVN Log", "TSVN Export" が表示されます。

## 使い方
  すでにSVN管理されているソースファイルを、LabVIEWで開いて、開いた状態で
ツールメニューから"TSVN ..."を選択すると、TortoiseSVNのログやコミット画面が
表示されます。

