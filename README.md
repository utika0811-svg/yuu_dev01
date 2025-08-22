<h2>🌿 ローカルブランチ vs リモートブランチ</h2>

<table>
  <thead>
    <tr>
      <th>項目</th>
      <th>ローカルブランチ</th>
      <th>リモートブランチ</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>📍存在場所</td>
      <td>自分のPC（ローカル環境）</td>
      <td>GitHubなどのリモートリポジトリ</td>
    </tr>
    <tr>
      <td>👤操作できる人</td>
      <td>自分だけ</td>
      <td>チーム全員（push/pull権限による）</td>
    </tr>
    <tr>
      <td>🔄更新方法</td>
      <td><code>git commit</code> で更新</td>
      <td><code>git push</code> / <code>git fetch</code> で同期</td>
    </tr>
    <tr>
      <td>🔍確認コマンド</td>
      <td><code>git branch</code></td>
      <td><code>git branch -r</code></td>
    </tr>
    <tr>
      <td>🔗追跡関係</td>
      <td><code>origin/xxx</code> を追跡することが多い</td>
      <td>ローカルブランチが追跡対象になる</td>
    </tr>
    <tr>
      <td>🛠️作成方法</td>
      <td><code>git checkout -b ブランチ名</code></td>
      <td><code>git push</code> でリモートに作成される</td>
    </tr>
    <tr>
      <td>🧹削除方法</td>
      <td><code>git branch -d ブランチ名</code></td>
      <td><code>git push origin --delete ブランチ名</code></td>
    </tr>
  </tbody>
</table>

<p><strong>補足:</strong> ローカルブランチは自分の作業用。リモートブランチはチーム共有用。作業完了後は <code>git push</code> でリモートに公開し、他のメンバーが <code>git fetch</code> や <code>git checkout</code> で参加できるようにします。</p>