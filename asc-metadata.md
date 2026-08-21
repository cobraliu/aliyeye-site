# App Store Connect 版本页元数据（可直接复制粘贴）

四个 App 共用：

| 字段 | 值 |
|---|---|
| Privacy Policy URL | `https://docs.aliyeye.site/privacy.html` |
| Support URL | `https://docs.aliyeye.site/support.html` |
| 价格 | 免费（如改付费/内购另行配置） |

> 注意：App 名称、副标题在「App 信息」页填一次全版本通用；描述、关键词、截图在每个版本页填。
> 关键词上限 100 字符（含逗号），中文每字算 1 个。下面的关键词均已控制在上限内。

---

## 1. ColorNest（儿童涂色）

- **Bundle ID**: `site.aliyeye.colornest`
- **App 信息页**
  - 名称：`ColorNest`
  - 副标题（≤30 字符）：`儿童涂色绘本与创作乐园`
  - 分类：主「教育」，副「娱乐」
  - 儿童分类：若走 Kids Category，勾选「5 岁及以下 / 6–8 岁」按实际定位选
- **版本页**
  - 宣传文本（≤170 字符，可随时改不用过审）：
    `数百张精美线稿，自由涂不留白，完成的作品还能生成回放视频分享给家人。`
  - 关键词：`涂色,儿童,画画,绘本,填色,涂鸦,着色,画画本,亲子,美术`
  - 年龄分级：4+
  - 描述：

```
ColorNest 是专为孩子打造的涂色创作乐园。

【海量线稿】数百张精心挑选的线稿，动物、植物、交通工具、节日主题应有尽有，持续更新。
【自由涂色】不限制涂法，手指、画笔随意挥洒，颜色可以涂出线外，孩子怎么开心怎么来。
【作品回放】每一次创作都被完整记录，一键回放绘画过程，孩子的进步看得见。
【语音伴画】内置语音讲解，不认识字的小朋友也能独立使用。
【分享成果】把作品导出成图片，一键分享给爷爷奶奶和小伙伴。
【家长放心】无广告、无内购、无网络、无需注册。家长区内可查看使用时长并进行设置。
所有作品只保存在本机，隐私无忧。

适合年龄：3 岁以上儿童在家长陪伴下使用。
有问题请联系 support@aliyeye.site
```

- **审核备注（Notes for Review）**：

```
This is a fully offline children's coloring app: no network, no IAP, no third-party SDKs.
Parent-facing settings are placed behind a parental gate (long-press puzzle) — see the
"家长" entry on the home screen. All content is stored on-device.
```

---

## 2. Scan2Doc（扫描转 Word/Excel）

- **Bundle ID**: `site.aliyeye.scanpdf2doc`
- **App 信息页**
  - 名称：`Scan2Doc`（若重名备选：`Scan2Doc - 扫描转Word`）
  - 副标题：`扫描文件，一键转 Word Excel`
  - 分类：主「效率」，副「商务」
- **版本页**
  - 宣传文本：`纸质文件拍一拍，自动找边矫正，导出 PDF，还能识别成可编辑的 Word 和 Excel。`
  - 关键词：`扫描,PDF,Word,Excel,文档,OCR,识别,拍照,转格式,办公`
  - 年龄分级：4+
  - 描述（中文为主版本；英、日、韩等语言版本建议同文翻译后分语言填写）：

```
Scan2Doc 把纸变回可编辑的文档——拍摄、整理、导出、识别，全程在你的设备上完成。

【扫描】系统级扫描界面：自动找边、自动抓拍、透视矫正，连拍多页一气呵成。
【整理】页面列表支持拖拽排序、删除、替换，组页顺序你说了算。
【导出 PDF】端上直接生成高清 PDF，随拍随导。
【识别重建】PDF 不只是图片——识别成排版还原的 Word / Excel，表格归表格，段落归段落。
【隐私优先】拍摄与识别全部在本机完成，你的文件不会上传到任何服务器。

无账号、无广告。除匿名下载离线识别语言包外，应用不产生任何网络传输。
支持语言：简体中文、繁体中文、英语、西班牙语、德语、日语、韩语。
有问题请联系 support@aliyeye.site
```

- **审核备注**：

```
The camera is used only for document scanning (VisionKit). All OCR / layout
reconstruction runs on-device; scanned files are never uploaded. The only network
traffic is downloading offline recognition language packs over HTTPS.
```

---

## 3. Lide（iPad 代码编辑器 + SSH）

- **Bundle ID**: `site.aliyeye.lide`
- **App 信息页**
  - 名称：`Lide`
  - 副标题：`Code editor & SSH for iPad`
  - 分类：主「开发者工具」，副「效率」
- **版本页**
  - 界面只有英文，主语言建议英语；中文区可按需附中文描述。
  - 宣传文本：`Native code editing on iPad, with the heavy lifting on your own machine over SSH.`
  - 关键词：`code,editor,SSH,SFTP,terminal,developer,remote,Git,markdown,IDE`
  - 年龄分级：17+（SSH/终端属于不受限网络访问，如实填写）
  - 描述（英文）：

```
Lide is a native code editor built for iPad. Edit locally with full fidelity;
hand the heavy lifting to your own machines over SSH.

ON DEVICE
- A fast, native text view: large files stay responsive, Chinese IME and hardware
  keyboards work properly.
- Syntax highlighting powered by tree-sitter for 20+ languages.
- Built-in Markdown preview, CSV viewing and Git workflows — no plugins required.
- Files live in the Files app: open, edit and save in place.

YOUR MACHINES
- SSH / SFTP client: browse, edit and save files on any remote host you own.
- Interactive terminal with full key support; credentials are stored securely in
  the iOS Keychain.

Everything runs where you choose: iPad handles editing, your machines handle
compiling, debugging and servers. No subscriptions, no accounts, no telemetry.

Requires your own remote machine for SSH features. Questions: support@aliyeye.site
```

- **审核备注（重点，务必填）**：

```
Lide is an editor and SSH client, not an interpreter or app runtime.
No code is downloaded to, stored on, or executed by the iPad itself — iPadOS
sandbox restrictions are fully respected. Language servers, compilers and terminals
run on the USER'S OWN remote machines, reached over standard SSH/SFTP initiated by
the user entering their own host credentials. The iPad acts purely as a thin client,
in the same manner as App Store apps like Termius or Blink Shell.
Demo video: <上传一段 30 秒演示后填链接>
```

---

## 4. EasyNotes（笔记）

- **Bundle ID**: `site.aliyeye.easynotes`
- **App 信息页**
  - 名称：`EasyNotes`（建记录时如撞名，备选：`EasyNotes - 随手记`）
  - 副标题：`随手写，随时翻`
  - 分类：主「效率」，副「教育」
- **版本页**
  - 宣传文本：`一支笔一张无限画布，手写、涂鸦、贴图，随手记下每一个灵感。`
  - 关键词：`笔记,手写,备忘录,日记,涂鸦,手账,便签,记录,画图,iPad`
  - 年龄分级：4+
  - 描述：

```
EasyNotes 让记笔记回到「拿笔就写」的简单。

【无限画布】一张写不完的纸，内容随意摆放，手写、画图、贴图都行。
【顺手好写】Apple Pencil、手指、外接键盘都支持；画出的形状自动规整，随手一画就是整齐的图形。
【好找好翻】笔记库按时间整理，全文搜索，想翻哪页翻哪页。
【iPhone + iPad】手机上快速记，平板上摊开写，两边都好用。
【隐私无忧】没有账号、没有云端、没有广告，你的笔记只存在你自己的设备上。

有问题请联系 support@aliyeye.site
```

- **审核备注**：

```
Fully offline note-taking app: no accounts, no network, no IAP. All notes are
stored in the app sandbox on-device.
```

---

## 提交前检查清单（每个 App 过一遍）

- [ ] 截图已上传（iPhone 6.9"；iPad 13"。Lide 只需 iPad）
- [ ] 描述、关键词、宣传文本已填
- [ ] Privacy Policy URL / Support URL 可打开（HTTPS）
- [ ] 年龄分级问卷已填
- [ ] App Privacy 问卷已填（四个都选"不收集数据"档）
- [ ] 审核备注、审核联系人（姓名+邮箱+电话）已填
- [ ] TestFlight 构建已关联到该版本
- [ ] 发布方式：手动发布 / 自动发布（首次上架建议选「手动发布」，过审后自己挑时间上架）
