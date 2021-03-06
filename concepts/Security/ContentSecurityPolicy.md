# コンテンツセキュリティポリシー

コンテンツセキュリティポリシー (CSP)はクライアントブラウザにどんな場所からどんな種類のリソース読み込みが許可されているかを伝えるW3Cスペックです。このスペックはターゲットとなるリソースの種類に関するローをの振る舞いを規定するために「ディレクティブ」を利用します。ディレクティブはHTTPレスポンスヘッダーやHTMLメタタグで指定されます。

#### HTTP ヘッダー
| ヘッダー                    | ブラウザ                                                                                |
| ------------------------- | -------------------------------------------------------------------------------------- |
| Content-Security-Policy   | (W3C標準) Chrome バージョン25以降、Firefox バージョン23以降、 Opera バージョン19以降            |
| X-Content-Security-Policy | Firefox バージョン23以前, IE バージョン 10                                                  |
| X-WebKit-CSP              | Chrome バージョン25以前                                                                   |


#### サポートするディレクティブ
| ディレクティブ     | |
|---------------|--------------------------|
| default-src   | 検知されたリソースタイプに関するディレクティブが提示がされいない時（フォールバック） |
| script-src    | 保護対象のリソースがどのスクリプトを実行可能かを定義します。 |
| object-src    | 保護対象のリソースがどこからプラグインを読み込めるかを定義します。 |
| style-src     | 保護対象のリソースがどのCSSを適用できるかを定義します。 |
| img-src       | 保護対象のリソースがどこから画像を読み込めるかを定義します。 |
| media-src     | 保護対象のリソースがどこからビデオとオーディオを読み込めるかを定義します。 |
| frame-src     | 保護対象のリソースがどこから埋め込みフレームを読み込めるかを定義します。 |
| font-src      | 保護対象のリソースがどこからフォントを読み込めるかを定義します。 |
| connect-src   | 保護対象のリソースがスクリプトインタフェースを使ってどのURI読み込めるかを定義します。 |
| form-action   | どのURIがHTMLのフォーム部品の送信先として利用できるかを定義します。  |
| sandbox       | 保護対象のリソースに対して適用されるブラウザのSandboxポリシーを定義します。 |
| script-nonce  | スクリプトエレメントにおいてスクリプト実行に指定された使い捨て乱数を持つことを要求します。 |
| plugin-types  | 保護対象のリソースから呼び出される事のできるプラグインのセットを組み込み可能なリソースの種類を限定することで定義します。 |
| reflected-xss | XSS攻撃をフィルタしたりブロックしたりするためのヒューリスティックを有効化あるいは無効化するようユーザエージェントに指示する、非標準のX-XSS-Protectionヘッダに相当するものです。 |
| report-uri    | ポリシー違反に関してユーザエージェントが通報できるIRLを指定します。 |

> さらなる情報は[W3C CSP Spec](https://w3c.github.io/webappsec/specs/content-security-policy/)をご覧ください。




<docmeta name="uniqueID" value="ContentSecurityPolicy649437">
<docmeta name="displayName" value="Content Security Policy">

