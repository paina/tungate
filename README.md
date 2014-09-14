tungate
=======

L2TP/DHCPv6 access concentrator and client

For the present README is in Japanese. Feel free to mail me in English. I can use English a little. :)

tungate は、IPv6 を L2TP 経由でばらまくためのシステムです。サーバ側も、クライアント側も開発しています。

要求ソフトウェア
---------------

tungate は、L2TP, DHCPv6 それぞれのサーバ・クライアントを連携させるための仲介ソフトウェアです。
そのため、各種のソフトウェアを必要とします。
対応 OS がサーバとクライアントで FreeBSD と Linux なんてひどすぎるんじゃないのというツッコミはアリです。

|                     |対応OS      |L2TP Server/Client |DHCPv6 Server/Client |
|---------------------|------------|-------------------|---------------------|
|ac (server)          |FreeBSD     |mpd5               |Kea DHCP Server      |
|名前募集中 (client)  |Linux       |xl2tpd             |ISC-DHCP (client)    |


ToDo
----

* DHCPv6-PD 対応！
* mpd.secret generator
* connectivity checker
* etc. etc.

バージョン履歴
--------------

* Ver.1
    * wide-dhcp-{server,client} + xl2tpd ベースの実装
    * いまのところ非公開ですが、それなりに動いていました
    * DHCPv6 PD 非対応
* Ver.2
    * これ
    * まだぜんぜんできてない

Copyright
---------

Copyright © SATO Taisuke <<paina@paina.jp>> 2014
