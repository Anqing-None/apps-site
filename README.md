# 记一页 · 轻点记账官方网站

这是 `apps.xieanqing.top` 的 GitHub Pages 源码，为“记一页”和“轻点记账”提供官方隐私政策与用户支持页面。

## 正式地址

- 首页：`https://apps.xieanqing.top/`
- 记一页隐私政策：`https://apps.xieanqing.top/jiyiye/privacy/`
- 记一页用户支持：`https://apps.xieanqing.top/jiyiye/support/`
- 轻点记账隐私政策：`https://apps.xieanqing.top/qingdian/privacy/`
- 轻点记账用户支持：`https://apps.xieanqing.top/qingdian/support/`

## 发布到 GitHub Pages

1. 在 GitHub 新建公开仓库，建议名称 `app-pages`。
2. 将本目录全部文件提交并推送到仓库的 `main` 分支。
3. 打开仓库 **Settings → Pages**。
4. 在 **Build and deployment** 选择 **GitHub Actions**；本项目内的工作流会自动发布。
5. 发布成功后，在 **Custom domain** 确认填写 `apps.xieanqing.top`。
6. 在阿里云 DNS 为 `xieanqing.top` 增加记录：
   - 记录类型：`CNAME`
   - 主机记录：`apps`
   - 记录值：`Anqing-None.github.io`
7. DNS 生效且 GitHub 检查通过后，勾选 **Enforce HTTPS**。

不要把根域名或 `www` 的现有记录改掉；只新增 `apps` 子域名即可。

## 本地预览

在本目录运行任意静态文件服务器，例如：

```sh
python3 -m http.server 8080
```

然后访问 `http://localhost:8080/`。

## 网站隐私

网站没有 JavaScript、Cookie、广告、第三方字体或访问分析。页面托管于 GitHub Pages，访问日志等必要技术信息仍可能由 GitHub 按其政策处理。

## 更新隐私政策

- 修改政策正文时，同时更新页面顶部的版本与日期。
- 轻点记账的数据流如有变化，应同步核对 App 内隐私说明和 App Store Connect 的隐私标签。
- 不要把轻点记账描述为“完全离线”：它包含私人 iCloud 同步和用户主动开启的云端截图识别。
