# 2026年Google AI Studio使用教程：注册登录、模型选择与 API获取
<!-- wp:paragraph -->
<p>随着 Gemini 系列 AI 模型不断更新，Google AI Studio 凭借丰富的模型选择、灵活的参数设置以及 AI 应用开发能力，成为不少开发者、AI 爱好者和内容创作者常用的 AI 工具。</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>想用 Gemini 做一个能接入业务的工具，通常要先验证几件事：提示词能不能稳定输出指定格式，换一个模型后结果有什么差别，最后又该怎么把测试搬到自己的程序里。<strong>Google AI Studio 把这些步骤放在同一个网页工作台里</strong>。你可以先运行提示词、调整参数，验证结果后再获取示例代码或创建 API Key。<a href="https://aistudio.google.com/docs/ai-studio-quickstart?utm_source=chatgpt.com"></a></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>本文从 Google AI Studio 和 Gemini 的区别讲起，再说明如何排查「地区不可用」、登录工作台、选择模型，以及完成第一次测试。</p>
<!-- /wp:paragraph -->

<!-- wp:heading -->
<h2 class="wp-block-heading"><strong>一、Google AI Studio 是什么？与 Gemini 有什么区别？</strong><strong></strong></h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><a href="https://aistudio.google.com/"><u>Google AI Studio</u></a>&nbsp;是 Google 推出的在线 AI 模型体验与应用开发平台。用户无需下载安装软件，即可通过浏览器体验 Gemini 系列模型、调试提示词、调整模型参数、开发 AI 应用及获取 Gemini API Key。<strong></strong></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>日常所说的 <strong>Gemini</strong>&nbsp;可以指 Google 的模型系列，也可以指用户直接使用的 <strong>Gemini App</strong>。下表对比的是 AI Studio 和 Gemini App。</p>
<!-- /wp:paragraph -->

<!-- wp:table -->
<figure class="wp-block-table"><table class="has-fixed-layout"><tbody><tr><td><strong>对比项</strong><strong></strong></td><td><strong>Google AI Studio</strong><strong></strong></td><td><strong>Gemini App</strong><strong></strong></td></tr><tr><td><strong>主要用途</strong></td><td>测试模型、调试提示词、制作应用原型和配置 API</td><td>对话问答、写作、学习和整理资料</td></tr><tr><td><strong>操作方式</strong></td><td>选择模型、调整运行参数、测试输出格式</td><td>通过对话界面直接提交任务</td></tr><tr><td><strong>典型场景</strong></td><td>验证一套商品信息提取规则能否接入业务系统</td><td>总结一份文档，或起草一封邮件</td></tr><tr><td><strong>费用怎么看</strong></td><td>网页测试与程序 API 调用分别看功能、模型和配额</td><td>查看 Gemini App 免费权益或 Google AI 订阅方案</td></tr></tbody></table></figure>
<!-- /wp:table -->

<!-- wp:paragraph -->
<p>如果你只是想让 AI 帮你完成一次任务，可以先用 Gemini App。如果这个任务需要<strong>反复运行、比较模型或接入程序</strong>，用 Google AI Studio 更便于测试。</p>
<!-- /wp:paragraph -->

<!-- wp:image {"lightbox":{"enabled":true},"id":8357,"width":"554px","height":"auto","aspectRatio":"1.840531561461794","sizeSlug":"large","linkDestination":"none","align":"center","style":{"border":{"radius":{"topLeft":"20px","topRight":"20px","bottomLeft":"20px","bottomRight":"20px"}}}} -->
<figure class="wp-block-image aligncenter size-large is-resized has-custom-border"><img src="https://blog-s21n.ipfoxy.com/wp-content/uploads/2026/11/图片2-4-1024x556.png" alt="" class="wp-image-8357" style="border-top-left-radius:20px;border-top-right-radius:20px;border-bottom-left-radius:20px;border-bottom-right-radius:20px;aspect-ratio:1.840531561461794;width:554px;height:auto"/></figure>
<!-- /wp:image -->

<!-- wp:heading -->
<h2 class="wp-block-heading"><strong>二、Google AI Studio 提示“地区不可用”怎么办？</strong><strong></strong></h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>如果打开 Google AI Studio 时提示「所在地区不可用」，或者被跳转到地区说明页，先查看 <a href="https://aistudio.google.com/docs/available-regions"><u>Google AI Studio支持的国家和地区</u></a>。<strong>如果你在支持地区，且平时通过办公代理访问 Google 服务，可以先配置并检测 Chrome 的网络出口，再登录同一个 Google 账号检查关联地区。</strong>&nbsp;</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading"><strong>1. 配置 Chrome代理并检测网络出口</strong><strong></strong></h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>上传文件、生成长回复或在 Build 中预览应用时，网络中断容易表现为上传失败、请求超时或页面一直加载。需要长期使用固定办公出口的团队，可以选择 IPFoxy 静态住ISP 代理。固定 IP 便于复用同一套连接配置，排查问题时也更容易确认浏览器实际走的是哪条线路。</p>
<!-- /wp:paragraph -->

<!-- wp:buttons -->
<div class="wp-block-buttons"><!-- wp:button -->
<div class="wp-block-button"><a class="wp-block-button__link wp-element-button" href="https://app.ipfoxy.com/login?source=Github">注册IPFoxy免费试用</a></div>
<!-- /wp:button --></div>
<!-- /wp:buttons -->

<!-- wp:list -->
<ul class="wp-block-list"><!-- wp:list-item -->
<li><strong>安装 IPFoxy Proxy Manager。</strong> 在日常使用的 Chrome 个人资料中安装扩展，并固定到工具栏。</li>
<!-- /wp:list-item --></ul>
<!-- /wp:list -->

<!-- wp:image {"lightbox":{"enabled":true},"id":8360,"width":"553px","height":"auto","aspectRatio":"1.636094674556213","sizeSlug":"large","linkDestination":"none","align":"center","style":{"border":{"radius":{"topLeft":"20px","topRight":"20px","bottomLeft":"20px","bottomRight":"20px"}}}} -->
<figure class="wp-block-image aligncenter size-large is-resized has-custom-border"><img src="https://blog-s21n.ipfoxy.com/wp-content/uploads/2026/11/图片3-6-1024x624.png" alt="" class="wp-image-8360" style="border-top-left-radius:20px;border-top-right-radius:20px;border-bottom-left-radius:20px;border-bottom-right-radius:20px;aspect-ratio:1.636094674556213;width:553px;height:auto"/></figure>
<!-- /wp:image -->

<!-- wp:list -->
<ul class="wp-block-list"><!-- wp:list-item -->
<li><strong>同步并启用代理。</strong> 从 IPFoxy 控制台获取用户 ID 和 API 密钥，填入扩展设置并保存，再启用团队指定的静态代理。具体界面可参考 <a href="https://www.ipfoxy.net/help/docs/IPFoxyProxyManager"><u>IPFoxy Proxy Manager 配置教程</u></a>。</li>
<!-- /wp:list-item --></ul>
<!-- /wp:list -->

<!-- wp:list -->
<ul class="wp-block-list"><!-- wp:list-item -->
<li><strong>核对 IP 定位、连通性和延迟。</strong> 在同一个 Chrome 窗口查询实际出口 IP，点击插件测试代理按钮，确认是否走了预期线路，再测试代理是否连通、延迟是否稳定。</li>
<!-- /wp:list-item --></ul>
<!-- /wp:list -->

<!-- wp:image {"lightbox":{"enabled":true},"id":8361,"width":"553px","height":"auto","aspectRatio":"1.9335664335664335","sizeSlug":"large","linkDestination":"none","align":"center","style":{"border":{"radius":{"topLeft":"20px","topRight":"20px","bottomLeft":"20px","bottomRight":"20px"}}}} -->
<figure class="wp-block-image aligncenter size-large is-resized has-custom-border"><img src="https://blog-s21n.ipfoxy.com/wp-content/uploads/2026/11/图片4-4-1024x530.png" alt="" class="wp-image-8361" style="border-top-left-radius:20px;border-top-right-radius:20px;border-bottom-left-radius:20px;border-bottom-right-radius:20px;aspect-ratio:1.9335664335664335;width:553px;height:auto"/></figure>
<!-- /wp:image -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading"><strong>2. 查看 Google 账号关联地区，资料有误时申请更正</strong><strong></strong></h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>网络检测正常后，在<strong>同一个 Chrome 个人资料</strong>里打开 <a href="https://policies.google.com/terms"><u>Google服务条款页面</u></a>。先核对右上角邮箱，确认它与登录 AI Studio 的账号一致，再查看页面显示的关联国家或地区。</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>如果你已迁居，而账号仍显示原来的关联地区，可以通过 Google官方地区更正表单按实际情况提交申请，可以参考 <a href="https://www.ipfoxy.net/blog/use-cases/8174"><u>Google 账号关联地区修改教程</u></a>进行申请修改。</p>
<!-- /wp:paragraph -->

<!-- wp:image {"lightbox":{"enabled":true},"id":8362,"width":"552px","height":"auto","aspectRatio":"1.5549295774647887","sizeSlug":"large","linkDestination":"none","align":"center","style":{"border":{"radius":{"topLeft":"20px","topRight":"20px","bottomLeft":"20px","bottomRight":"20px"}}}} -->
<figure class="wp-block-image aligncenter size-large is-resized has-custom-border"><img src="https://blog-s21n.ipfoxy.com/wp-content/uploads/2026/11/图片5-4-1024x658.png" alt="" class="wp-image-8362" style="border-top-left-radius:20px;border-top-right-radius:20px;border-bottom-left-radius:20px;border-bottom-right-radius:20px;aspect-ratio:1.5549295774647887;width:552px;height:auto"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>若关联地区正确、所在地也在支持名单内，但仍无法进入，下一步可以检查 Google 账号是否满足 <strong>18 岁及以上</strong>的要求，以及是否需要完成年龄验证。代理设置只改变浏览器的网络出口，Google 账号关联地区由官方管理，更正后能否使用 AI Studio 仍取决于 Google 的访问要求。</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading"><strong>3. 网页能打开，为什么 Gemini API 还是连不上？</strong><strong></strong></h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Chrome 代理和程序的 API 请求走的是各自的网络。</strong>&nbsp;IPFoxy Proxy Manager 管理 Chrome 流量。本地 Python 脚本、后端服务和云端任务，需要从实际运行环境检查连接。Google 也明确说明，使用 Colab 时，地区限制按 <strong>Colab 实例所在地区</strong>判断。如果网页正常、只有 API 报错，建议先看错误正文，确认是连接超时、项目权限还是配额问题。</p>
<!-- /wp:paragraph -->

<!-- wp:heading -->
<h2 class="wp-block-heading"><strong>三、Google AI Studio 怎么注册和登录？</strong><strong></strong></h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>已有符合条件的 Google 账号，就可以直接登录 Google AI Studio，无需单独创建 AI Studio 账号。</strong>&nbsp;如果还没有 Google 账号，可以先参考 <a href="https://www.ipfoxy.net/blog/use-cases/7895"><u>Gmail 注册教程</u></a>。</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>1、打开 <a href="https://aistudio.google.com/"><u>Google AI Studio官网</u></a>，按页面提示登录 Google 账号。</strong>如果浏览器登录了多个账号，先核对当前显示的邮箱。</p>
<!-- /wp:paragraph -->

<!-- wp:image {"lightbox":{"enabled":true},"id":8363,"width":"554px","height":"auto","aspectRatio":"2.216","sizeSlug":"large","linkDestination":"none","align":"center","style":{"border":{"radius":{"topLeft":"20px","topRight":"20px","bottomLeft":"20px","bottomRight":"20px"}}}} -->
<figure class="wp-block-image aligncenter size-large is-resized has-custom-border"><img src="https://blog-s21n.ipfoxy.com/wp-content/uploads/2026/11/图片6-4-1024x464.png" alt="" class="wp-image-8363" style="border-top-left-radius:20px;border-top-right-radius:20px;border-bottom-left-radius:20px;border-bottom-right-radius:20px;aspect-ratio:2.216;width:554px;height:auto"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p><strong>2、首次使用时，按页面提示阅读并确认相关条款。</strong>如果通过公司或学校账号管理 Cloud 项目，创建密钥和查看用量还可能需要组织授权。</p>
<!-- /wp:paragraph -->

<!-- wp:image {"lightbox":{"enabled":true},"id":8364,"width":"554px","height":"auto","aspectRatio":"2.1811023622047245","sizeSlug":"large","linkDestination":"none","align":"center","style":{"border":{"radius":{"topLeft":"20px","topRight":"20px","bottomLeft":"20px","bottomRight":"20px"}}}} -->
<figure class="wp-block-image aligncenter size-large is-resized has-custom-border"><img src="https://blog-s21n.ipfoxy.com/wp-content/uploads/2026/11/图片7-3-1024x469.png" alt="" class="wp-image-8364" style="border-top-left-radius:20px;border-top-right-radius:20px;border-bottom-left-radius:20px;border-bottom-right-radius:20px;aspect-ratio:2.1811023622047245;width:554px;height:auto"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p><strong>3、进入 Playground，选一个可用模型，输入指令可以开始使用。</strong></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Google AI Studio 的操作界面主要由左侧功能导航栏、中间模型交互区域以及右侧参数设置区域组成。第一次进入工作台，可以先熟悉四个入口：</p>
<!-- /wp:paragraph -->

<!-- wp:list -->
<ul class="wp-block-list"><!-- wp:list-item -->
<li><strong>Playground</strong>：输入提示词，按模型支持情况添加图片或其他文件，然后运行并检查输出。</li>
<!-- /wp:list-item -->

<!-- wp:list-item -->
<li><strong>Run settings</strong>：选择模型、调整参数，并查看该模型支持的功能，例如结构化输出。测试时可以一次只改一项，方便定位结果为什么变化。</li>
<!-- /wp:list-item -->

<!-- wp:list-item -->
<li><strong>Build</strong>：用文字描述应用需求，生成并预览原型，再根据实际结果调整。</li>
<!-- /wp:list-item -->

<!-- wp:list-item -->
<li><strong>Get code</strong>：提示词测试满意后，获取相应语言的调用示例。真正接入程序时，再使用项目的 Gemini API Key。</li>
<!-- /wp:list-item --></ul>
<!-- /wp:list -->

<!-- wp:image {"lightbox":{"enabled":true},"id":8365,"width":"552px","height":"auto","aspectRatio":"2.164705882352941","sizeSlug":"large","linkDestination":"none","align":"center","style":{"border":{"radius":{"topLeft":"20px","topRight":"20px","bottomLeft":"20px","bottomRight":"20px"}}}} -->
<figure class="wp-block-image aligncenter size-large is-resized has-custom-border"><img src="https://blog-s21n.ipfoxy.com/wp-content/uploads/2026/11/图片8-3-1024x473.png" alt="" class="wp-image-8365" style="border-top-left-radius:20px;border-top-right-radius:20px;border-bottom-left-radius:20px;border-bottom-right-radius:20px;aspect-ratio:2.164705882352941;width:552px;height:auto"/></figure>
<!-- /wp:image -->

<!-- wp:heading -->
<h2 class="wp-block-heading"><strong>四、</strong><strong>Google AI Studio 怎么用？核心功能使用教程</strong><strong></strong></h2>
<!-- /wp:heading -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading"><strong>1</strong><strong>. 如何选择 Google AI Studio AI 模型？</strong><strong></strong></h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>先按任务选模型，再用同一组样本比较。以下是 Google 官方模型目录中的代表性选项。工作台实际显示的模型和可用额度，以账号及项目页面为准。</p>
<!-- /wp:paragraph -->

<!-- wp:table -->
<figure class="wp-block-table"><table class="has-fixed-layout"><tbody><tr><td><strong>任务</strong><strong></strong></td><td><strong>可在模型选择器中查看</strong><strong></strong></td><td><strong>测试重点</strong><strong></strong></td></tr><tr><td>摘要、文本分类、日常开发</td><td><strong>Gemini 4 Hydrogen</strong>，也可对比 <strong>Gemini 3.8 Flash</strong></td><td>响应速度、批量样本的输出一致性</td></tr><tr><td>复杂分析、代码调试</td><td><strong>Gemini 4 Neon</strong>&nbsp;或 <strong>Gemini 4 Argon</strong></td><td>是否理解约束、能否处理边界情况</td></tr><tr><td>高难度推理与复杂工程任务</td><td><strong>Gemini 4 Carbon</strong></td><td>正确率是否值得额外的时间或用量</td></tr><tr><td>图片、视频或语音生成</td><td>按任务查看官方目录中的专用模型</td><td>支持的输入、输出格式及计费方式</td></tr></tbody></table></figure>
<!-- /wp:table -->

<!-- wp:paragraph -->
<p>例如，测试商品数据提取时，可以准备一条字段完整的描述、一条缺少价格的描述和一条格式混乱的描述。用相同提示词跑不同模型，检查它们是否能按要求返回字段，以及遇到缺失信息时会不会自行补全。</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading"><strong>2、</strong><strong>Google AI Studio 有哪些热门用法？</strong><strong></strong></h3>
<!-- /wp:heading -->

<!-- wp:list -->
<ul class="wp-block-list"><!-- wp:list-item -->
<li><strong>提示词调试与结构化提取。</strong> 在 Playground 输入几条示例商品资料，要求提取品牌、型号和价格，并把缺失字段返回为 null。如果所选模型支持结构化输出，可以进一步设置字段格式，再对照样本检查结果。</li>
<!-- /wp:list-item -->

<!-- wp:list-item -->
<li><strong>图片或文档理解。</strong> 用支持对应输入的模型上传一张公开的商品截图或一份测试文档，要求提取指定信息。读不清的字段让模型标为「无法确认」，再对照原文件检查。</li>
<!-- /wp:list-item -->

<!-- wp:list-item -->
<li><strong>快速制作应用原型。</strong> 打开 <a href="https://aistudio.google.com/apps"><u>Google AI Studio Build</u></a>，输入「制作一个商品对比页，输入两款产品的名称、价格和参数，生成对比结果」。先测试正常输入和空字段，再逐步加功能。</li>
<!-- /wp:list-item --></ul>
<!-- /wp:list -->

<!-- wp:heading -->
<h2 class="wp-block-heading"><strong>五、Google AI Studio API Key 怎么获取？</strong><strong></strong></h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>直接通过 <a href="https://aistudio.google.com/apikey"><u>Google AI Studio 的 API Keys 页面</u></a>获取即可：</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>1、登录准备用于开发的 Google 账号，进入 <strong>API Keys</strong>。</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>2、选择要用于测试的 <strong>Google Cloud 项目</strong>，点击 <strong>Create API key</strong>。新用户接受条款后，页面可能已显示 Google 自动创建的默认项目和密钥。</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>3、将密钥保存在后端环境变量或密钥管理工具中。调用前核对项目、模型权限和计费状态。发布网页、代码仓库或教程截图时，应避免暴露完整密钥。</p>
<!-- /wp:paragraph -->

<!-- wp:image {"lightbox":{"enabled":true},"id":8366,"width":"553px","height":"auto","aspectRatio":"1.728125","sizeSlug":"large","linkDestination":"none","align":"center","style":{"border":{"radius":{"topLeft":"20px","topRight":"20px","bottomLeft":"20px","bottomRight":"20px"}}}} -->
<figure class="wp-block-image aligncenter size-large is-resized has-custom-border"><img src="https://blog-s21n.ipfoxy.com/wp-content/uploads/2026/11/图片9-3-1024x593.png" alt="" class="wp-image-8366" style="border-top-left-radius:20px;border-top-right-radius:20px;border-bottom-left-radius:20px;border-bottom-right-radius:20px;aspect-ratio:1.728125;width:553px;height:auto"/></figure>
<!-- /wp:image -->

<!-- wp:heading -->
<h2 class="wp-block-heading"><strong>六、Google AI Studio 常见问题</strong><strong></strong></h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>1. Google AI Studio 网页端免费吗？</strong><br>Google AI Studio 网页端提供免费的模型体验及开发功能，符合使用条件的用户可以直接使用 Google 账号登录，无需提前购买 Google AI Pro。免费的网页体验、Gemini API 免费层和付费 API 额度需要分别查看。</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>2. Google AI Studio 无法访问怎么办？</strong><br>如果是页面打不开，先查浏览器连接；如果跳转到地区说明，核对支持地区和账号年龄；如果网页正常、只有 API 报错，查看错误正文。`403` 优先核对权限及报错提示，`429` 优先核对速率限制或配额。</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>3. Google AI Studio 和 Gemini Advanced 有什么区别？</strong><br>大家常说的 <strong>Gemini Advanced</strong>&nbsp;通常指 Gemini App 的高级使用体验，具体权益以当前 <strong>Google AI 订阅方案</strong>为准。<strong>Google AI Studio</strong>&nbsp;则用于测试模型、比较输出、生成调用示例和管理 API Key。如果你购买了 Gemini App 的高级订阅，开发项目的 API 计费和配额仍应在 AI Studio 中单独核对。</p>
<!-- /wp:paragraph -->

<!-- wp:heading -->
<h2 class="wp-block-heading"><strong>七、总结</strong><strong></strong></h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>第一次使用 Google AI Studio，可以先用已有 Google 账号登录，在 Playground 用三条真实样本测试同一个任务。等结果符合预期，再决定在 Build 里制作原型，还是通过 API 接入自己的程序。遇到连接问题时，先判断卡在<strong>浏览器访问、账号资格还是程序调用</strong>。团队有固定浏览器出口需求时，可以用 <strong>IPFoxy Proxy Manager</strong>&nbsp;管理 Chrome 代理，稳定账号网络环境，提高耐用性。</p>
<!-- /wp:paragraph -->
