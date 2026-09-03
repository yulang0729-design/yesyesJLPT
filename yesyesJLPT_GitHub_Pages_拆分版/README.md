# yesyesJLPT — 2023年12月 JLPT N3 在线真题工作台

## 文件结构

- `index.html`：主工作台（已保留现有 Supabase 连接与答题逻辑）
- `assets/audio/n3-listening.mp3`：N3 听力原声音频
- `assets/images/listening/`：听力原卷第 36～47 页图片

## GitHub Pages

将整个文件夹内容上传到仓库根目录，并在 GitHub 的 Settings → Pages 中选择 `main` 分支、`/(root)`。

## Supabase

当前 `index.html` 已保留原工作台中的 Supabase URL / Publishable key，以及提交成绩时写入 `jlpt_n3_submissions` 的逻辑。

注意：如果 Supabase 数据表/RLS 尚未配置，需要在 Supabase 控制台执行你已有的 schema SQL；不要把 service_role key 放进前端。
