# タビカケ プライバシーポリシー / Privacy Policy

最終更新日: 2026年8月12日

## 日本語

タビカケ（以下「本アプリ」)は、ユーザーのプライバシーを尊重します。本ポリシーでは、本アプリにおける情報の取り扱いを説明します。

### 1. データの保存場所
本アプリで記録されたデータ（支出金額、写真、場所、メモ、カテゴリ、イベント、アルバム）は、原則として**お使いの端末内にのみ保存**されます。共有機能（第3項）を利用する場合に限り、共有対象のデータがサーバーに保存されます。

### 2. アカウント
本アプリの利用にアカウント登録は不要です。氏名・メールアドレス・電話番号等の連絡先情報は一切取得しません。共有機能を利用する場合のみ、任意の表示名（ニックネーム可）と、アプリが自動生成する匿名IDが作成されます。

### 3. 共有機能（共有ブック・サークル。いずれも任意の機能）
共有ブック（共有家計簿）またはサークル（スポット共有）を利用する場合に限り、以下の情報が当方のサーバーに保存されます:
- 任意の表示名と匿名のユーザーID（Vercel / Neon、シンガポールリージョン）
- 共有ブックに追加した記録、およびサークルへ共有をONにした記録（金額・店名/場所・カテゴリ名・メモ・日時・位置座標・割り勘の設定）
- **共有をONにした記録に添付された写真（縮小版）**。写真は非公開ストレージ（Cloudflare R2）に保存され、有効期限付きの署名URLを通じて、同じブック・サークルのメンバーのみが閲覧できます

記録の共有・写真の共有はいずれも**記録ごとに手動でONにしたときだけ**行われます（初期設定はOFF）。これらの情報は、メンバー間での表示・集計のみに使用され、第三者への提供・広告目的の利用は一切ありません。共有した記録・写真は作成者がいつでも共有解除・削除でき、ブックやサークルから脱退・削除した場合も対応するデータはサーバーから削除されます。データの完全削除をご希望の場合は、下記の連絡先までお問い合わせください。共有機能を使わない限り、すべてのデータは従来どおり端末内にのみ保存されます。

### 4. プッシュ通知（任意）
サークルで新しいスポットが共有されたことをお知らせするため、通知を許可した場合に限り、端末の通知用トークン（Expo Push Token。氏名等を含まない、通知配信のためだけの識別子）がサーバーに保存されます。通知はOSの設定からいつでもオフにでき、オフにしてもアプリの他の機能に影響はありません。

### 5. 位置情報
本アプリは、支出した場所の店名を提案するために位置情報を使用します。この際、現在地の座標が地図データサービス（Google Places API、OpenStreetMap Nominatim / Overpass API）に送信されますが、これは店名・地名の検索のみを目的とした一時的な通信であり、ユーザーを識別する情報は含まれません。開発者がこの通信を収集・保存することはありません。位置情報の利用は端末の設定からいつでも無効にできます。

### 6. 写真
写真ライブラリおよびカメラへのアクセスは、支出の記録に写真を添付する目的でのみ使用されます。写真は原則として端末内にのみ保存され、あなたが記録の共有をONにした場合に限り、縮小版が第3項のとおりサーバーに保存されます。

### 7. 解析・広告
本アプリは、アクセス解析ツール・広告SDK・トラッキング技術を一切使用していません。

### 8. データの削除
記録の削除は本アプリ内からいつでも行えます。アプリを削除すると、端末内のすべてのデータが削除されます（共有機能を利用していた場合、サーバー上の共有データの削除は第3項をご覧ください）。

### 9. お問い合わせ
本ポリシーに関するお問い合わせ: tomjoepatience@gmail.com

## English

Tabikake ("the App") respects your privacy.

- **Local-first storage**: Data recorded in the App (amounts, photos, places, memos, categories, events, albums) is stored on your device. Only if you use the optional sharing features, the shared data is stored on our server.
- **No contact information**: The App never collects your name, email address, or phone number. If you use a sharing feature, an optional display name (nickname) and an anonymous, app-generated user ID are created.
- **Sharing features (Shared Books & Circles — both optional)**: When you use Shared Books or Circles, the following is stored on our server: your display name and anonymous user ID (Vercel / Neon, Singapore region); the records you add to shared books or explicitly share to circles (amount, place name, category name, memo, date, coordinates, and split settings); and **downsized copies of photos attached to records you chose to share**. Photos are kept in private storage (Cloudflare R2) and are viewable only by members of the same book/circle via expiring signed URLs. Sharing is **opt-in per record** (off by default). This data is used solely to display and aggregate records among members, and is never shared with third parties or used for advertising. You can stop sharing or delete your shared records and photos at any time; leaving or deleting a book/circle also removes the corresponding data from the server. Contact us for complete data deletion. If you never use the sharing features, all data stays on your device.
- **Push notifications (optional)**: If you allow notifications, a push token (Expo Push Token — an identifier used only to deliver notifications, containing no personal details) is stored on our server to notify you when a new spot is shared in your circles. You can turn notifications off in your OS settings at any time.
- **Location**: Your coordinates are sent to map data services (Google Places API, OpenStreetMap Nominatim / Overpass API) solely to suggest nearby place names. These requests contain no user identifiers, and the developer does not collect or retain this data.
- **Photos**: Photo library and camera access are used only to attach photos to your records. Photos stay on your device unless you explicitly share a record, in which case a downsized copy is stored as described above.
- **No analytics or ads**: The App contains no analytics tools, ad SDKs, or trackers.
- **Deletion**: Deleting the App removes all data from your device. For server-side shared data, see the sharing section above.
- **Contact**: tomjoepatience@gmail.com
