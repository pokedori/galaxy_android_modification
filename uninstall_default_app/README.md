# 概要
アンインストールができないものをアンインストールする方法<br>

## 事前準備(Windows)
Windowsで、以下をinstallする<br>
<br>
・Android USB Driver for Windowsのインストール<br>
https://developer.samsung.com/mobile/android-usb-driver.html
<br>
・ツールをダウンロード<br>
　https://developer.android.com/studio/releases/platform-tools<br>
　リンク切れならこちら：https://drive.google.com/file/d/1Qjgae7S5nH03jHc0TLVQyvOwGMNvlmBk/view?usp=drive_link<br>
<br>

## 手順
<br>
コマンドラインでアンインストールした場所へ移動<br>
<br>
３．adb.exe shellで接続<br>
　　→必要に応じて：Diagモード（\*#0808# > MTP )にする。<br>
  　→USBデバッグモードにする。<br>
４．docomoのパッケージを調べる<br>
　　→pm list packages | grep docomo<br>
５．削除<br>
　　→pm uninstall --user 0 <パッケージ名><br>
６．削除できないアプリ<br>
　　→android上でデバイス管理アプリとして設定されているので、解除してから消す必要がある。<br>
　　com.nttdocomo.android.wipe<br>
　　com.nttdocomo.android.remotelock<br>
７．Galaxyのカレンダー<br>
　　pm uninstall --user 0 com.samsung.android.calendar<br>
８．ドコモのユーザー管理<br>
　　pm uninstall --user 0 com.android.contacts<br>

・参考URL<br>
https://note.com/nekofuton/n/nae2421530dc1
<br>
<br>

・Galaxy s22 ultraを削除する際のコマンド例<br>
pm uninstall --user 0 com.nttdocomo.android.wipe<br>
pm uninstall --user 0 com.nttdocomo.android.devicehelp<br>
pm uninstall --user 0 com.nttdocomo.android.anshinsecurity<br>
pm uninstall --user 0 com.nttdocomo.android.apnsw<br>
pm uninstall --user 0 jp.co.nttdocomo.carriermail<br>
pm uninstall --user 0 com.nttdocomo.android.remotelock<br>
pm uninstall --user 0 com.nttdocomo.android.msg<br>
pm uninstall --user 0 jp.co.nttdocomo.anshinmode<br>
pm uninstall --user 0 com.nttdocomo.android.schedulememo<br>
pm uninstall --user 0 com.nttdocomo.android.mascot<br>
pm uninstall --user 0 com.nttdocomo.android.homezozo<br>
pm uninstall --user 0 jp.co.nttdocomo.lcsapp<br>
pm uninstall --user 0 com.nttdocomo.android.mymagazine<br>
pm uninstall --user 0 com.nttdocomo.android.databackup<br>
pm uninstall --user 0 com.nttdocomo.android.idmanager<br>
pm uninstall --user 0 com.nttdocomo.android.dmenu2<br>
pm uninstall --user 0 com.nttdocomo.android.anmane2<br>
pm uninstall --user 0 jp.co.nttdocomo.saigaiban<br>
pm uninstall --user 0 com.nttdocomo.android.felicaremotelock<br>
pm uninstall --user 0 com.nttdocomo.android.docomoset<br>
pm uninstall --user 0 com.nttdocomo.android.pf.dcmippushaggregator<br>
pm uninstall --user 0 com.nttdocomo.android.initialization<br>
pm uninstall --user 0 com.nttdocomo.android.applicationmanager<br>
pm uninstall --user 0 com.nttdocomo.android.store<br>
pm uninstall --user 0 com.nttdocomo.android.applicationmanagersub<br>
<br>
pm uninstall --user 0 com.android.contacts<br>
pm uninstall --user 0 com.samsung.android.app.spage<br>
pm uninstall --user 0 com.microsoft.skydrive<br>
pm uninstall --user 0 com.google.android.apps.tachyon<br>
pm uninstall --user 0 com.samsung.android.calendar<br>

<br>
pm uninstall --user 0 com.samsung.android.honeyboard<br>
