# LabVIEW TSVN_LvPlugin

## 概要
  LabVIEW開発環境のツールメニューにTortoiseSVNの Log/Add/Commit/Export の項目
を追加するためのプラグインVIです。
  LabVIEW用のTortoiseSVNツールキットといえば、ViewpointSystemsの
TSVN Toolkitなどが有名ですが、そこまでしなくても、とりあえず編集中のVIのログが
見られて、add/commitの操作ができれば、という軽めの用途向けに作成しました。
自分で使ってます。
  TortoiseSVNのコマンドラインTortoiseProc.exeを呼び出しますので、
TortoiseSVNがインストールされている必要があります。
  また、すでにSVN管理されているソース・ファイルが対象になります。
SVNへの登録等の操作は、TortoiseSVNを使って行ってください。

### 対応する環境
  LabVIEW 2009 で作成しており、LabVIEW 2009以上であれば動きます。
  Windows用です。

## インストール

### インストール方法
  TSVN_Add_LvPlugin.vi、TSVN_Commit_LvPlugin.vi、TSVN_Log_LvPlugin.vi、TSVN_Export_LvPlugin.viの
４つのファイルを LabVIEW インストールフォルダの所定の場所にコピーするだけです。

### インストールする場所
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

### 使い方
  すでにSVN管理されているソースファイルを、LabVIEWで開き、該当VIファイルがアクティブの
状態で、ツールメニューから"TSVN ..."のいずれかのメニューを選択すると、TortoiseSVNのログや
コミット画面が表示されます。追加(add)は、裏で追加されるだけですので、エクスプローラで
確認してください。
