# job-quest-readme

JobQuest - 勤怠・人材マネジメントWebアプリ
JobQuest は、飲食店などの現場でアルバイトの勤怠、時給、レベル、スキル、代理出勤などをRPG的に統合管理できるWebアプリです。スマホ・PC・タブレットなどブラウザが使える端末からアクセス可能です。
---

🌐 特徴
✅ 勤怠管理（出勤・退勤）
✅ 欠勤・代理募集フォーム
✅ シフトレベル調整＆編成
✅ アルバイトのスキル・レベルの可視化
✅ 業務履歴の蓄積＆昇給ロジック
✅ マネージャー・店長向け管理画面
✅ 自社従業員の社内登用支援（SaaS営業職など）

---

📱 対応端末
スマートフォン（PWA対応）
タブレット
PC（Google Chrome 推奨）

---

🔐 ログイン方式
メールアドレスとパスワードによるログイン
Firebase Authentication（匿名ログインなども対応可能）

---

🏗️ 使用技術スタック
| 項目            | 内容                            |
|-----------------|---------------------------------|
| フロントエンド  | Next.js 14（App Router）        |
| UI              | Tailwind CSS + Headless UI      |
| バックエンドAPI | Next.js API Routes              |
| データベース    | Firebase Firestore               |
| 認証管理        | Firebase Authentication          |
| デプロイ先      | Vercel                          |
| 通知機能        | Slack Webhook or LINE代替SNS     |

---

📊 主な機能
✅ アルバイト用マイページ
出勤／退勤ボタン（現在時刻と端末情報を記録）
勤務履歴と経験値の確認
欠勤連絡と代理募集フォーム（送信後、通知が飛ぶ）

✅ マネージャー／店長用画面
全バイトの勤怠一覧表示
代理出勤者の確定操作
シフトのパーティー構成（平均レベル等）表示
ゲームバランス・昇給設定調整

✅ スマホ忘れ対策
店舗共用タブレット／PCからログイン打刻
マネージャーによる代理打刻機能
紙バックアップ用打刻表のダウンロード

---

🚀 PWA（プログレッシブWebアプリ）対応
ホーム画面にアイコン追加可能
ロック画面にプッシュ通知（将来的に実装）

---

⚙️ 開発環境セットアップ
``bash
git clone https://github.com/your-org/jobquest.git
cd jobquest
npm install
cp .env.local.example .env.local  # Firebase設定を記述
npm run dev



⸻

📁 ディレクトリ構成（例）

/app
  /dashboard         # 店長管理画面
  /mypage            # アルバイト用マイページ
  /admin             # ゲームバランス設定
/api
  /clockin           # 出勤・退勤API
  /absence           # 欠勤・代理募集API
/firebase            # Firebase設定
/public
/styles



⸻

📅 今後の展望
    •    ネイティブアプリ化（React Native Expo）
    •    AIによる人材推薦や評価の自動提案
