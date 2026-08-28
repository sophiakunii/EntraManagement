# EntraManagement
PowerShell scripts and KQL queries for Microsoft Entra ID management.

このリポジトリに保存されているファイルは以下の目的で使用します。

・Create-TAP

CSVファイルに保存されているユーザーの一時アクセスパスをまとめて作成するPowerShellスクリプト
・Remove-MFAMethod
Entraに登録されたユーザーの既存の多要素認証設定を削除するPowerShellスクリプト
・User-who-invite-guest
監査ログをLog Analyticsワークスペースに転送した際、Guestユーザーを作成(招待)したユーザーを特定するためのKQLクエリ

# CSV ファイルの作り方
それぞれのスクリプトで使用するCSVファイルはファイル名を users.csv として、スクリプトファイルと同じフォルダーに保存し、
ファイルは以下のように構成してください。

userprincipalname
a@a.com
b@a.com
c@a.com
