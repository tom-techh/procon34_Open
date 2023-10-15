# procon34_Open
第34回高専プロコン(procon34)競技部門で優勝したチーム蟹高専のexeを公開します。
アルゴリズムは以下を参照してください。
https://twitter.com/Kujira_Box/status/1713500920926101728

# 使用方法
## player.json
チームの情報、サーバへの接続関係を書き込みます。exeと同じディレクトリに配置してください。  
parallel 並行試合の時、0or1で2試合どちらに繋ぐか決めます。本番は使いませんでした。  
token テストサーバーの試合規定に使用したtokenを利用してください。  
url 試合のサーバのURLに/matchesを付けてください。  
search_msec 探索+POSTのために用意する時間です。サーバの調子に合わせて変更できるようにしましたが300で大丈夫です。  
search_depth ビームサーチやDFSによるソルバーを模索していた時に使っていた名残です。消さずに残してください(コード直すのがめんどくさい...)  

## procon34.exe
機能を列挙します。  
1.マウスを左クリックで建築目標の追加 右クリックで破壊目標の追加 マウスホイールクリックで「1ターンで敵壁を味方壁にする」目標を追加(職人2人が近くにいない場合は、破壊後建築目標に切り替わる)  
2. Spaceを押しながら1で目標を削除  
3.Tab,Shiftで味方,敵のみの盤面情報を表示 Cで職人のみ表示  
4.Gで破壊することで点数の上がる味方壁を破壊目標に追加  
5.数字キー1~職人数 キーを押しながらマスを左クリックするとそのマスにその職人が強制的に移動する キーを押しながらbackspaceで強制移動を解除  
6.deleteで全目標を削除  
7.GUI右の城マーク,+4,+2 x4,x2 白い方が建築目標の追加で黒い方が破壊目標の追加です 4,2という数字は格子の周期性に関係しています  

![スクリーンショット (250)](https://github.com/tom-techh/procon34_Open/assets/102672343/75402da7-192c-4d29-bb2f-9bce7cde965d)

## おまけ  
jsonfolderに試合規定のjsonを入れておきます  
BOM付UTF8のものがたまに混ざっているのでUTF8にvscodeでエンコード+保存してください  
