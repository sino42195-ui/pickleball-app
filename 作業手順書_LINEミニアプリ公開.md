# LINEミニアプリ公開 作業手順書
## P-Crew中野 ピックルボールスケジュール管理アプリ

---

## 全体の流れ

```
① GitHubアカウント作成
　　↓
② GitHubリポジトリ作成
　　↓
③ index.htmlをアップロード
　　↓
④ GitHub Pagesを有効化
　　↓
⑤ LINE DevelopersのEndpoint URLを更新
　　↓
⑥ LINEミニアプリとして公開（審査申請）
```

---

## STEP 1｜GitHubアカウント作成

1. https://github.com にアクセス
2. 「Sign up」をクリック
3. メールアドレス・パスワード・ユーザー名を入力して登録

> ✅ すでにアカウントがある場合はスキップ

---

## STEP 2｜GitHubリポジトリ作成

1. GitHubにログインし、右上の「**+**」→「**New repository**」をクリック
2. 以下の通り入力：
   - **Repository name**：`pickleball-app`（任意）
   - **公開設定**：**Public**（必須）
3. 「**Create repository**」をクリック

---

## STEP 3｜index.htmlをアップロード

1. 作成したリポジトリのページを開く
   - URL例：`https://github.com/ユーザー名/pickleball-app`
2. 「**Add file**」→「**Upload files**」をクリック
3. `index.html` をドラッグ＆ドロップ
4. 「**Commit changes**」をクリック

> ⚠️ ファイルはフォルダに入れず、リポジトリ直下に置くこと

---

## STEP 4｜GitHub Pagesを有効化

1. リポジトリの「**Settings**」タブをクリック
2. 左メニューの「**Pages**」をクリック
3. 以下の通り設定：
   - **Source**：`Deploy from a branch`
   - **Branch**：`main` / `/ (root)`
4. 「**Save**」をクリック
5. 数分後にページをリロードすると以下のURLが発行される：

```
https://ユーザー名.github.io/pickleball-app/
```

> ✅ P-Crew中野の場合：`https://sino42195-ui.github.io/pickleball-app/`

---

## STEP 5｜LINE DevelopersのEndpoint URLを更新

1. https://developers.line.biz にログイン
2. 該当のチャネルを選択
3. 「**LIFF**」タブをクリック
4. 該当のLIFFアプリをクリック
5. **Endpoint URL** を以下に変更：
   ```
   https://sino42195-ui.github.io/pickleball-app/
   ```
6. 「**Update**」をクリックして保存

---

## STEP 6｜動作確認

1. スマホのLINEからLIFF URLを開く
2. カレンダー・予定一覧が正しく表示されるか確認
3. 出欠登録が正常に動作するか確認

---

## STEP 7｜index.htmlを更新する場合（今後の手順）

機能追加・修正後にファイルを更新する手順：

1. https://github.com/sino42195-ui/pickleball-app を開く
2. 「**Add file**」→「**Upload files**」をクリック
3. 新しい `index.html` をドラッグ＆ドロップ
4. 「**Commit changes**」をクリック
5. 数分後に自動反映される

> ✅ **LINE DevelopersのEndpoint URLの変更は不要**

---

## STEP 8｜LINEミニアプリ審査申請（一般公開する場合）

### 審査前の確認事項

- [ ] アイコン・デザインガイドラインへの準拠
- [ ] プライバシーポリシーの設定
- [ ] チャネル説明に正しいサービス内容を記載
- [ ] [LINEミニアプリポリシー](https://terms2.line.me/LINE_MINI_App?lang=ja)の遵守

### 審査申請手順

1. LINE Developersコンソールにログイン
2. 該当チャネルの「**審査申請**」タブを開く
3. 必要事項を入力して「**審査を申請する**」をクリック
4. 審査結果はコンソールと登録メールに通知される

### 審査期間

- 通常：**1〜2週間**
- 却下・再申請の場合：さらに数日追加
- バッファ込みで **1ヶ月前後**を見込むこと

---

## 関連URL一覧

| 項目 | URL |
|------|-----|
| GitHubリポジトリ | https://github.com/sino42195-ui/pickleball-app |
| 公開URL（Endpoint URL） | https://sino42195-ui.github.io/pickleball-app/ |
| LINE Developers | https://developers.line.biz |
| GAS API | https://script.google.com/macros/s/AKfycbzANBsvAux2oFUL9X3pS3vetDwX7jK-ku2qZoliWca5veqgi95o0kcTN6_Tg12jvkpYdw/exec |
| LINEミニアプリポリシー | https://terms2.line.me/LINE_MINI_App?lang=ja |

---

*作成日：2026年5月*
