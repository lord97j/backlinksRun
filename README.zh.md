🌍 *[English](README.md) ∙ [简体中文](README.zh.md)*

# BacklinksRun

[BacklinksRun](https://BacklinksRun.net/) 是一个开源的无数据库架构的开发者工具导航网站

<!-- ## Star 历史

[![Star 历史图表](https://api.star-history.com/svg?repos=iamcorey/BacklinksRun&type=Date)](https://star-history.com/#iamcorey/BacklinksRun&Date)


## 预览

![BacklinksRun](https://img.magicbox.tools/screenshot_img/BacklinksRun_zh.png?version=081702) -->

## 特性

- **无数据库架构**：利用 GitHub 进行内容存储和管理。
- **动态内容**：使用 Next.js 服务器端渲染动态渲染内容。
- **Markdown 支持**：使用 Markdown 格式编写内容，便于编辑和版本控制。
- **管理界面**：内置管理面板用于内容管理。
- **响应式设计**：使用 Tailwind CSS 实现完全响应式设计。
- **SEO 友好**：通过动态元数据优化搜索引擎。
- **易于部署**：简单的 Vercel 部署流程。
- **内置分析支持**：集成分析支持脚本，兼容 Google Analytics 和 Plausible Analytics。
- **国际化**：支持多语言，可轻松扩展以支持更多语言。
- **深色模式**：支持深色模式，可轻松扩展以支持更多主题。
- **广告支持**：支持 Google Adsense 和可以轻松扩展以支持更多广告。


### 技术栈
- Next.js - 框架
- Tailwind CSS - CSS 框架
- Shadcn/UI - 组件库
- Vercel - 部署
- Next-Intl - 国际化
- Analytics - Google Analytics & Plausible Analytics & ...
- Ads - Google Adsense & ...

---


## 向 BacklinksRun 添加新的开发者工具

想要将您的网站添加到 BacklinksRun 吗？

### 提交您网站的两种方式
1. 通过 [GitHub Issues](https://github.com/iamcorey/BacklinksRun/issues) 提交您的网站，获得免费的 dofollow 链接。

2. 或者您也可以通过更改 `data/json/[locale]` 文件夹中的 jsonc 文件并创建拉取请求来提交您的网站。
（请阅读我们的[投稿指南](/data/md/add-new-developer-tools.md)了解详情）

### 提交格式

请遵循以下格式：
- [ ] **name**：提供描述您添加的工具或数据的简短标题。
- [ ] **description**：清楚地说明添加了什么工具或数据以及属于哪个类别。
- [ ] **url**：提供工具的 url。
- [ ] **category**：提供工具的类别。
- [ ] **tags**：提供工具的几个标签。（最多 3 个标签）
- [ ] **icon_url**：提供工具图标的 url。（可选）如果未提供，图标将自动生成。


### 附加说明
- **仅限开发者工具**：请不要提交与开发无关的工具。
- **不允许联盟链接**：不要包含联盟链接。
- **禁止垃圾信息**：不要包含垃圾信息。
- **可访问的 URL**：确保 url 可访问。



## 部署您自己的 BacklinksRun

### 在 Vercel 上部署

[![使用 Vercel 部署](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2FiAmCorey%2FBacklinksRun&project-name=BacklinksRun&repository-name=BacklinksRun&external-id=https%3A%2F%2Fgithub.com%2FiAmCoreye%2FBacklinksRun%2Ftree%2Fmain)



## 先决条件

- Node.js（14 版本或更高）
- npm/pnpm/yarn（随 Node.js 一起提供）
- Git
- GitHub 账户
- Vercel 账户（用于部署）

## 安装

1. 克隆仓库：
   ```
   git clone https://github.com/iAmCorey/BacklinksRun
   cd BacklinksRun
   ```

2. 安装依赖：
   ```
   npm install
   pnpm install
   yarn
   ```

3. 在根目录创建一个 `.env.local` 文件并添加以下内容：
   ```
   GITHUB_TOKEN=你的github个人访问令牌（可选）
   GITHUB_OWNER=你的github用户名（可选）
   GITHUB_REPO=你的仓库名（可选）
   ACCESS_PASSWORD=你的安全访问密码（可选）
   JWT_SECRET=你的密钥（可选）
   NEXT_PUBLIC_GOOGLE_ANALYTICS_ID=你的google分析ID(G-xxx)（可选）
   NEXT_PUBLIC_PLAUSIBLE_URL=你的plausible数据域（可选）
   NEXT_PUBLIC_GOOGLE_ADSENSE_ID=你的google广告ID(ca-pub-xxx)（可选）
   ```

4. 设置你的 GitHub 仓库：
   - 在 GitHub 上创建一个新仓库
   - 在仓库中创建两个文件夹：`data/json/[locale]` 和 `data/md`
   - 在 `data/json/[locale]` 中，创建相关的 jsonc 文件，内容为空数组：`[]`

5. 运行开发服务器：
   ```
   npm run dev
   pnpm dev
   yarn run dev
   ```

访问 `http://localhost:3000` 查看您的 BacklinksRun 实例在本地运行。

## 部署

1. 将您的代码推送到 GitHub。
2. 登录 Vercel 并从您的 GitHub 仓库创建一个新项目。
3. 在 Vercel 中配置环境变量：
   - `GITHUB_TOKEN`（可选）
   - `GITHUB_OWNER`（可选）
   - `GITHUB_REPO`（可选）
   - `ACCESS_PASSWORD`（可选）
   - `JWT_SECRET`（可选）
   - `NEXT_PUBLIC_GOOGLE_ANALYTICS_ID`（可选）
   - `NEXT_PUBLIC_PLAUSIBLE_URL`（可选）
   - `NEXT_PUBLIC_GOOGLE_ADSENSE_ID`（可选）
4. 部署项目。

有关详细的部署指南，请参阅我们的[安装和部署指南](/data/md/deploy-own-BacklinksRun.md)。

## 使用
### 手动
- 工具：更改 `data/json/[locale]` 文件夹中的 jsonc 文件。
- 文章：更改 `data/md` 文件夹中的 markdown 文件。

### 通过管理面板
（需要配置 GITHUB 相关的环境变量。）
- 通过导航到 `/admin` 并使用您的 `ACCESS_PASSWORD` 访问管理面板。
- 通过管理界面创建和编辑文章。
- 在管理面板中管理资源。
- 所有更改都会自动与您的 GitHub 仓库同步。


---


## 更新日志
查看 [CHANGELOG.md](./CHANGELOG.md) 获取详细的更改列表。

## 贡献

我们欢迎对 BacklinksRun 的贡献！请阅读我们的[投稿指南](/data/md/add-new-developer-tools.md)，了解我们的行为准则和提交拉取请求的流程。

## 许可证

BacklinksRun 是根据 [MIT 许可证](./LICENSE) 授权的开源软件。


## 致谢

BacklinksRun 使用以下工具和库构建：
- [GitBase](https://gitbase.app/) 
- [DevToolset](https://devtoolset.net/) 
- [Favicon.im](https://favicon.im/) 
- [Next.js](https://nextjs.org/)
- [Tailwind CSS](https://tailwindcss.com/)
- [Shadcn/UI](https://ui.shadcn.com/)

我们感谢这些项目的维护者和贡献者。

