<h2>🌿 Git ブランチ構成（Git-Flow モデル）</h2>

<table>
  <thead>
    <tr>
      <th>ブランチ名</th>
      <th>役割</th>
      <th>分岐元</th>
      <th>マージ先</th>
      <th>備考</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>main</code></td>
      <td>本番リリース履歴</td>
      <td><code>release</code> / <code>hotfix</code></td>
      <td>-</td>
      <td>本番環境にデプロイされた状態を保持</td>
    </tr>
    <tr>
      <td><code>dev</code></td>
      <td>開発統合</td>
      <td><code>main</code></td>
      <td><code>release</code></td>
      <td>ステージング環境と連携</td>
    </tr>
    <tr>
      <td><code>feature/terraform</code></td>
      <td>Terraform構成ドキュメント作成</td>
      <td><code>dev</code></td>
      <td><code>dev</code></td>
      <td>完了後にPRで統合</td>
    </tr>
    <tr>
      <td><code>release/*</code></td>
      <td>リリース準備</td>
      <td><code>dev</code></td>
      <td><code>main</code>, <code>dev</code></td>
      <td>タグ付け・最終調整に使用</td>
    </tr>
    <tr>
      <td><code>hotfix/*</code></td>
      <td>緊急修正</td>
      <td><code>main</code></td>
      <td><code>main</code>, <code>dev</code></td>
      <td>本番障害対応。即時反映</td>
    </tr>
  </tbody>
</table>

<p><strong>📌 運用ルール:</strong></p>
<ul>
  <li><code>main</code> は保護ブランチ。直接コミット禁止</li>
  <li><code>dev</code> はステージング環境と連携し、QA/UATに使用</li>
  <li><code>feature/*</code> は機能ごとに分岐し、完了後 <code>dev</code> にマージ</li>
  <li><code>release/*</code> はタグ付け・承認フロー・最終テストに活用</li>
  <li><code>hotfix/*</code> は障害対応テンプレートと連携</li>
</ul>


<h2>🌿 Git ブランチ構成（Git-Flow モデル）</h2>

<table>
  <thead>
    <tr>
      <th>ブランチ名</th>
      <th>役割</th>
      <th>分岐元</th>
      <th>マージ先</th>
      <th>備考</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>main</code></td>
      <td>本番リリース履歴</td>
      <td><code>release</code> / <code>hotfix</code></td>
      <td>-</td>
      <td>本番環境にデプロイされた状態を保持</td>
    </tr>
    <tr>
      <td><code>dev</code></td>
      <td>開発統合</td>
      <td><code>main</code></td>
      <td><code>release</code></td>
      <td>ステージング環境と連携</td>
    </tr>
    <tr>
      <td><code>feature/terraform</code></td>
      <td>Terraform構成ドキュメント作成</td>
      <td><code>dev</code></td>
      <td><code>dev</code></td>
      <td>完了後にPRで統合</td>
    </tr>
    <tr>
      <td><code>release/*</code></td>
      <td>リリース準備</td>
      <td><code>dev</code></td>
      <td><code>main</code>, <code>dev</code></td>
      <td>タグ付け・最終調整に使用</td>
    </tr>
    <tr>
      <td><code>hotfix/*</code></td>
      <td>緊急修正</td>
      <td><code>main</code></td>
      <td><code>main</code>, <code>dev</code></td>
      <td>本番障害対応。即時反映</td>
    </tr>
  </tbody>
</table>

<p><strong>📌 運用ルール:</strong></p>
<ul>
  <li><code>main</code> は保護ブランチ。直接コミット禁止</li>
  <li><code>dev</code> はステージング環境と連携し、QA/UATに使用</li>
  <li><code>feature/*</code> は機能ごとに分岐し、完了後 <code>dev</code> にマージ</li>
  <li><code>release/*</code> はタグ付け・承認フロー・最終テストに活用</li>
  <li><code>hotfix/*</code> は障害対応テンプレートと連携</li>
</ul>