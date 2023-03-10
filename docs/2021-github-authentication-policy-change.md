# GitHub 认证政策将于 2021 年 5 月变更

> 原文：<https://www.gitkraken.com/blog/2021-github-authentication-policy-change>

如果您已经通过 GitKraken 中的 OAuth 连接了您的 GitHub 集成，您就可以开始了！

GitHub 正在改变它的安全策略，不再允许只有用户名/密码的访问。这一变化将于 2021 年 8 月 13 日生效，并影响所有提供 [GitHub 集成](/integrations/github)的桌面 Git 应用，包括 GitKraken。

已经使用 OAuth 向 GitHub 认证的用户不会受到影响。OAuth 是 GitKraken 配置文件设置中的默认连接方法。

但是，如果您一直依赖用户名和密码来连接 GitHub 和 GitKraken，现在是时候过渡到 OAuth、SSH 或使用 PAT 了。

### 使用 OAuth 将 GitKraken 连接到 GitHub

通过 OAuth 连接到 GitHub，或者仔细检查您已经完成的工作:

1.  打开 gitkraken
2.  打开`Preferences`菜单(使用右上角的齿轮⚙️图标)，点击左侧菜单中的`Integrations`
3.  点击`GitHub`显示您的连接状态。如果您之前已经连接过，您的状态将显示为“已连接”,无需进一步操作。如果您尚未连接，它将如下所示:

4.  点击“连接到 GitHub”
5.  在打开的新网页浏览器窗口中，点击“继续授权”
6.  按照 GitHub 登录页面上的流程登录您的 GitHub 帐户

如果成功，下一个屏幕应该会显示:“GitHub 和 GitKraken 准备就绪！”🎉

提醒:GitKraken 允许多个配置文件，每个文件都有自己的设置和偏好。确保检查每个配置文件的连接，以避免 GitHub 强制执行这一更改时出现意外。

关于 GitKraken 的 [GitHub 集成](/integrations/github)的更多信息和进一步的细节，请参见我们的支持文档。

现在，如果您只是需要建立或验证您的 GitHub 连接，您在这里的工作已经完成。但是如果你想更深入地了解这一变化，我们邀请你继续阅读…

GitHub 认证初级读本

### GitHub 是最受软件开发人员欢迎的在线协作平台之一，用于跟踪和共享代码。它受欢迎的原因之一是本地开发工具、CI/CD 管道和各种各样的应用程序可以很容易地与平台集成。GitHub 让用户可以非常容易地连接各种集成，允许开发人员选择他们喜欢的认证路径。

在即将到来的 GitHub 认证变更之前，用户有多种连接路径可供选择:

用户名和密码

1.  SSH 密钥
2.  个人访问令牌
3.  OAuth 令牌
4.  GitHub 应用令牌
5.  个人访问令牌和 OAuth 令牌看起来非常相似，用途相同。两者都与请求令牌的用户相关联，这意味着他们将拥有与用户相同的权限。这种差异实际上可以归结为概念，以及手动管理帐户凭证的个人偏好。

个人访问令牌需要从一个服务内部生成，比如 GitHub，并且需要手动管理和共享。

使用 OAuth，您可以授权应用程序代表您与服务对话。这是通过远程服务器和本地机器之间的握手来完成的；授权人可能永远看不到实际生成的凭证。

个人访问令牌和 OAuth 授权过程都非常安全，通常都一次性授予整个帐户的权限，包括用户或其组织所有者可以访问的任何存储库。

另一方面，GitHub 应用程序令牌用于授予应用程序或集成特定的权限，而不提供更广泛的访问。由于这些是特定于应用程序的，它们向组织授予权限，但限制授权服务可以访问哪些回购。如果安装 GitHub 应用程序的人离开了组织或失去了访问权限，这些应用程序也会保持安装状态。

个人访问令牌和 OAuth 授权过程都非常安全，通常都一次性授予整个帐户的权限，包括用户或其组织所有者可以访问的任何存储库。

对 GitHub 认证过程的更改

截至 2021 年 8 月，该列表上的第一个选项——用户名和密码——将被取消，以推动世界走向更安全的互联网。

### 对 GitHub 认证过程的更改

从 2021 年 8 月 13 日开始，我们在 GitHub.com 上认证 Git 操作时将不再接受账户密码。受影响的工作流:命令行 Git 使用 Git 访问桌面应用程序任何直接使用您的密码访问 GitHub.com 上 Git 库的应用程序/服务

你可以在 GitHub 博客上阅读更多关于这个的详细信息。

> 从 2021 年 8 月 13 日开始，我们在 GitHub.com 上认证 Git 操作时将不再接受账户密码。受影响的工作流:命令行 Git 使用 Git 访问桌面应用程序任何直接使用您的密码访问 GitHub.com 上 Git 库的应用程序/服务

计划在 6 月 30 日和 7 月 28 日进行 GitHub 限电

在 8 月 13 日之前，GitHub 还将在 6 月 30 日和 7 月 28 日安排用户名/密码认证的“限电”,以便测试这一变化，并在正式变化之前“鼓励受影响的客户更新他们的认证方法”。

### 至于他们为什么做出这种改变，我们可以再次引用他们的博客帖子:

在 8 月 13 日之前，GitHub 还将在 6 月 30 日和 7 月 28 日安排用户名/密码认证的“限电”,以便测试这一变化，并在正式变化之前“鼓励受影响的客户更新他们的认证方法”。

*与基于密码的身份验证相比，令牌提供了许多安全优势:*

*1。unique——令牌特定于 GitHub，可以在每次使用或每台设备上生成。*

> *2。可撤销—可以随时单独撤销令牌，而无需更新不受影响的凭据。*
> 
> *3。受限—可以缩小令牌的范围，仅允许用例所需的访问。*
> 
> *4。随机-令牌不像您需要记住或定期输入的简单密码那样受到字典或暴力攻击的影响。*
> 
> *3。受限—可以缩小令牌的范围，仅允许用例所需的访问。*
> 
> GitKraken 是更好、更安全的工作流程的关键

如果你读了这篇文章并且还没有下载 GitKraken，现在是你的机会了。将 GitKraken 与 Github 集成在一起，我们可以做到这一切，甚至更多:

### 在 GitHub 帐户上创建存储库，包括。git 忽略和许可

自动生成一个 SSH 密钥对并将其添加到 GitHub 中

*   GitKraken 的 Fork 存储库
*   将验证保存到配置文件中
*   从 GitHub repo 列表克隆
*   创建和管理拉式请求
*   从 GitHub repo 列表克隆
*   享受 GitKraken 提供的所有令人难以置信的功能 [并立即下载](https://www.gitkraken.com/download)。

享受 GitKraken 提供的所有令人难以置信的功能 [并立即下载](https://www.gitkraken.com/download)。