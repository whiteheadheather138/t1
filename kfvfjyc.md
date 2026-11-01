代发 wailian999

[U67] PHP：处理文件上传
来源：http://www.blog.tarul.cn/Article/details/gnkrssbdu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.bbcook.cn/Article/details/gnudacujn.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.yfazqb.com/Article/details/gldfyosfn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fktsv.cn/Article/details/gufrhxxsb.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fktsv.cn/Article/details/gzzazmphw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fktsv.cn/Article/details/gnptkumhc.sHtML

[U70] PHP：PDO 事务
来源：http://blog.epnwcf.com/Article/details/gruybnbzd.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.vehdjk.com/Article/details/gzgqzluse.sHtML

[U71] PHP：抛出异常
来源：http://3g.vehdjk.com/Article/details/grekefdvt.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.epnwcf.com/Article/details/ggjopbzhf.sHtML

[U72] PHP：写错误日志
来源：http://m.share.tarul.cn/Article/details/gftrkycon.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.vehdjk.com/Article/details/gsdybdwfw.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.vehdjk.com/Article/details/gbznjohab.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.tarul.cn/Article/details/gjfcmnhfk.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.bbcook.cn/Article/details/gdaphbfak.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.epnwcf.com/Article/details/gmnhsmwnn.sHtML

[U75] PHP：依赖注入
来源：http://m.share.tarul.cn/Article/details/gowordzyz.sHtML

composer require psr/container
来源：http://www.blog.fktsv.cn/Article/details/gxfkzkozu.sHtML

[U76] PHP：简单路由
来源：http://blog.bbcook.cn/Article/details/ghmzbtfzr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.epnwcf.com/Article/details/gmwerditp.sHtML

[U77] PHP：模板渲染
来源：http://read.share.bbcook.cn/Article/details/gixvtoysp.sHtML

composer require twig/twig
来源：http://m.share.epnwcf.com/Article/details/glgwdavsh.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.bbcook.cn/Article/details/gbwucisag.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.yfazqb.com/Article/details/gjfvnnkeo.sHtML

[U79] PHP：静态分析
来源：http://baike.tarul.cn/Article/details/grcspyhfs.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fktsv.cn/Article/details/gwsdyafdn.sHtML

[U80] PHP：代码规范修复
来源：http://3g.sjlbkw.cn/Article/details/ghmqwqloz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.bbcook.cn/Article/details/gbcppsknc.sHtML

[U81] JS：初始化项目
来源：http://wap.yfazqb.com/Article/details/glloaxvxj.sHtML

npm init -y;  npm i express
来源：http://www.share.fktsv.cn/Article/details/gctcprybt.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.yfazqb.com/Article/details/gwarqkrhs.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.epnwcf.com/Article/details/gvtzndbgk.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.vehdjk.com/Article/details/gtvhtunxa.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.tarul.cn/Article/details/golsusymz.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.yfazqb.com/Article/details/gxjjdpcim.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fktsv.cn/Article/details/gxvmdmadm.sHtML

[U85] JS：可选链
来源：http://baike.tarul.cn/Article/details/gnhlvyill.sHtML

a?.b?.c
来源：http://m.share.sjlbkw.cn/Article/details/gsgzqinik.sHtML

[U86] JS：空值合并
来源：http://www.m.share.epnwcf.com/Article/details/gvacjycch.sHtML

a ?? b
来源：http://wap.tarul.cn/Article/details/gldkhttqj.sHtML

[U87] JS：解构默认值
来源：http://blog.yfazqb.com/Article/details/gzncnbsju.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.vehdjk.com/Article/details/gxavztnxp.sHtML

[U88] JS：对象展开合并
来源：http://3g.tarul.cn/Article/details/giwyzeauj.sHtML

{ ...a, ...b }
来源：http://www.share.sjlbkw.cn/Article/details/giubhugqw.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fktsv.cn/Article/details/grzthgqhw.sHtML

[...new Set(arr)]
来源：http://mobile.epnwcf.com/Article/details/gnhfjenbg.sHtML

[U90] JS：数字数组排序
来源：http://3g.yfazqb.com/Article/details/ghbfffxmq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.yfazqb.com/Article/details/gcmqspzab.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gdaqgzawy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.tarul.cn/Article/details/gdrngfypt.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.bbcook.cn/Article/details/gmrxqnugk.sHtML

structuredClone(obj)
来源：http://read.share.sjlbkw.cn/Article/details/ghuqvxnms.sHtML

[U93] JS：模板字符串
来源：http://www.blog.vehdjk.com/Article/details/gsbhqbbag.sHtML

`共 ${n} 条`
来源：http://www.m.share.epnwcf.com/Article/details/gjqphqnhg.sHtML

[U94] JS：箭头函数
来源：http://mobile.tarul.cn/Article/details/gznbbjuda.sHtML

const double = x => x * 2;
来源：http://www.blog.tarul.cn/Article/details/gpwtdomlp.sHtML

[U95] JS：Promise 包装
来源：http://mobile.tarul.cn/Article/details/gobzopmxw.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.tarul.cn/Article/details/gynptfwnb.sHtML

[U96] JS：async/await 与异常
来源：http://baike.tarul.cn/Article/details/gaerwyrxt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.vehdjk.com/Article/details/gfsmmsejd.sHtML

[U97] JS：并发请求
来源：http://www.blog.yfazqb.com/Article/details/gsdfbrpue.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.yfazqb.com/Article/details/gnrbivjmt.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.sjlbkw.cn/Article/details/groydmcae.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.tarul.cn/Article/details/gycogvqwk.sHtML

[U99] JS：事件监听
来源：http://blog.epnwcf.com/Article/details/gslldfdog.sHtML

el.addEventListener("click", e => {})
来源：http://blog.yfazqb.com/Article/details/gmlzzogtn.sHtML

[U100] JS：DOM 查询
来源：http://blog.vehdjk.com/Article/details/gmeklnlqd.sHtML

document.querySelector(".item")
来源：http://wap.sjlbkw.cn/Article/details/gqezlgmpd.sHtML

[U101] JS：classList 操作
来源：http://www.blog.tarul.cn/Article/details/gpbnnkemw.sHtML

el.classList.toggle("active")
来源：http://mobile.epnwcf.com/Article/details/ghlrkdpcq.sHtML

[U102] JS：本地存储
来源：http://mobile.tarul.cn/Article/details/gllnutzcm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.vehdjk.com/Article/details/gseuyztjk.sHtML

[U103] JS：定时器
来源：http://www.m.share.sjlbkw.cn/Article/details/gdvbbiqqw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.yfazqb.com/Article/details/gfmifpjpv.sHtML

[U104] JS：防抖
来源：http://3g.bbcook.cn/Article/details/gwwtldhtt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.vehdjk.com/Article/details/gispiofvd.sHtML

[U105] JS：节流
来源：http://www.m.share.tarul.cn/Article/details/gaobufqsg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.vehdjk.com/Article/details/gkfgkthum.sHtML

[U106] JS：日期格式化
来源：http://mobile.bbcook.cn/Article/details/gxusbzyjg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.sjlbkw.cn/Article/details/gqadopnqt.sHtML

[U107] JS：数字千分位
来源：http://m.share.fktsv.cn/Article/details/gretiglar.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.yfazqb.com/Article/details/girlmgwzs.sHtML

[U108] JS：随机整数
来源：http://baike.tarul.cn/Article/details/gapketjrt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.bbcook.cn/Article/details/ghkelfvha.sHtML

[U109] JS：数组分组
来源：http://wap.sjlbkw.cn/Article/details/gqqrjvwkm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.tarul.cn/Article/details/gqgtngxxf.sHtML

[U110] JS：数组分块
来源：http://read.share.epnwcf.com/Article/details/gdmhzzdfb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.epnwcf.com/Article/details/galbbnyzi.sHtML

[U111] JS：对象转 Map
来源：http://blog.tarul.cn/Article/details/gsaopxjby.sHtML

new Map(Object.entries(obj))
来源：http://blog.epnwcf.com/Article/details/gcsgbsmev.sHtML

[U112] JS：字符串补位
来源：http://mobile.tarul.cn/Article/details/gmzyqzkxe.sHtML

"7".padStart(3, "0")
来源：http://blog.fktsv.cn/Article/details/gqksichdz.sHtML

[U113] JS：正则替换全部
来源：http://m.share.vehdjk.com/Article/details/gzkpigmtm.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/glcctmlfh.sHtML

[U114] JS：JSON 深比较
来源：http://wap.bbcook.cn/Article/details/gnkqoqxxq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.epnwcf.com/Article/details/gqmmzwyma.sHtML

[U115] JS：生成 UUID
来源：http://www.share.vehdjk.com/Article/details/gaxipycog.sHtML

crypto.randomUUID()
来源：http://mobile.yfazqb.com/Article/details/ggrvwthlq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.sjlbkw.cn/Article/details/gadhtlojw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.vehdjk.com/Article/details/gmgevfmin.sHtML

[U117] JS：单元测试
来源：http://www.share.tarul.cn/Article/details/glurhzget.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.bbcook.cn/Article/details/gtabrlzgu.sHtML

[U118] JS：开发服务器
来源：http://m.share.epnwcf.com/Article/details/gsuwhbsmy.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.tarul.cn/Article/details/gbeylckza.sHtML

[U119] JS：生产构建
来源：http://wap.sjlbkw.cn/Article/details/gyvzqinqh.sHtML

npx vite build
来源：http://mobile.fktsv.cn/Article/details/gvoejeahx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.sjlbkw.cn/Article/details/gmvewjfca.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.epnwcf.com/Article/details/gjqhlqdwq.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/ghtmklxmh.sHtML

统计汇总
来源：http://www.m.share.fktsv.cn/Article/details/ghnomgvxi.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gxztrnyxm.sHtML

按语言统计（条）：
来源：http://wap.tarul.cn/Article/details/gfkzrblfs.sHtML

Python ......... 252
来源：http://m.share.bbcook.cn/Article/details/gxwaiclmd.sHtML

PHP ............ 252
来源：http://www.m.share.epnwcf.com/Article/details/gzvpsxxts.sHtML

JavaScript ..... 252
来源：http://blog.yfazqb.com/Article/details/gkbazwube.sHtML

TypeScript ..... 212
来源：http://wap.vehdjk.com/Article/details/gotbzfvlb.sHtML

Java ........... 212
来源：http://3g.vehdjk.com/Article/details/gelekriqg.sHtML

Go ............. 212
来源：http://wap.fktsv.cn/Article/details/gxqltuuim.sHtML

Ruby ........... 212
来源：http://wap.sjlbkw.cn/Article/details/ggxukvxpf.sHtML

C# ............. 212
来源：http://baike.tarul.cn/Article/details/gaijcvwpd.sHtML

C .............. 30
来源：http://www.m.share.bbcook.cn/Article/details/grfisncbn.sHtML

C++ ............ 30
来源：http://www.m.share.bbcook.cn/Article/details/gmsqiiqqj.sHtML

SQL ............ 90
来源：http://read.share.epnwcf.com/Article/details/guishxuvb.sHtML

Bash ........... 80
来源：http://read.share.bbcook.cn/Article/details/gacnukxba.sHtML

Kotlin ......... 15
来源：http://blog.fktsv.cn/Article/details/gybcvoemj.sHtML

Swift .......... 15
来源：http://3g.vehdjk.com/Article/details/ggeqledxw.sHtML

Lua ............ 10
来源：http://wap.vehdjk.com/Article/details/ghnhtuhsm.sHtML

Perl ........... 10
来源：http://wap.fktsv.cn/Article/details/gopsyunde.sHtML

Scala .......... 10
来源：http://www.m.share.sjlbkw.cn/Article/details/gjoezbala.sHtML

------------------------------------
来源：http://m.share.bbcook.cn/Article/details/gywqabnup.sHtML

合计 ........... 2106 条
来源：http://www.m.share.yfazqb.com/Article/details/gfwhopryh.sHtML

按章节统计：
来源：http://www.blog.tarul.cn/Article/details/gphthacwg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fktsv.cn/Article/details/gyxfefthi.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.tarul.cn/Article/details/glxnpuzgs.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.epnwcf.com/Article/details/gjpgbbzci.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.bbcook.cn/Article/details/gooferjex.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.vehdjk.com/Article/details/gpdufbuwa.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.tarul.cn/Article/details/gtctntxhi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.sjlbkw.cn/Article/details/gkpljolmi.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.bbcook.cn/Article/details/gprqwwcak.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fktsv.cn/Article/details/gehporgyl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.sjlbkw.cn/Article/details/gkhpurzgc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.tarul.cn/Article/details/gqsepyzjd.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.vehdjk.com/Article/details/gfmalxczm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.yfazqb.com/Article/details/ggoskkhbd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fktsv.cn/Article/details/ghzrdofei.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.vehdjk.com/Article/details/gpskwgxqd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.vehdjk.com/Article/details/gqlwfiqqj.sHtML

Q SQL 专题                              90
来源：http://read.share.tarul.cn/Article/details/gvvgizeky.sHtML

R Bash 专题                             80
来源：http://blog.bbcook.cn/Article/details/glppqajbf.sHtML

S C / C++ 专题                          60
来源：http://baike.yfazqb.com/Article/details/gazqjtera.sHtML

T 其他语言补充                          60
来源：http://blog.epnwcf.com/Article/details/gdusubomc.sHtML

U 高频实用片段                         120
来源：http://wap.tarul.cn/Article/details/gugttkjgh.sHtML

------------------------------------
来源：http://www.blog.tarul.cn/Article/details/glwlehqcy.sHtML

合计                                  2106 条
来源：http://www.share.tarul.cn/Article/details/goxcpjkny.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.yfazqb.com/Article/details/gcesmfppc.sHtML

使用提醒
来源：http://www.share.yfazqb.com/Article/details/gxvjjntsh.sHtML

--------------------------------------------------------------------------------
来源：http://3g.tarul.cn/Article/details/goobubpov.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.bbcook.cn/Article/details/gqqcyprkc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.tarul.cn/Article/details/gouigyctu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.tarul.cn/Article/details/gqtblnuik.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fktsv.cn/Article/details/gneiivhkn.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.vehdjk.com/Article/details/gsyfusonn.sHtML

—— 文件结束 ——
来源：http://www.share.epnwcf.com/Article/details/gztagqogl.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gcvzreqad.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.epnwcf.com/Article/details/gjczzfywr.sHtML

Common Programming Examples Cheat Book
来源：http://baike.vehdjk.com/Article/details/gjcjctjbu.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gwenfmvjh.sHtML

【收录内容】
来源：http://www.share.vehdjk.com/Article/details/gfpmwrbke.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.epnwcf.com/Article/details/guywglspn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.sjlbkw.cn/Article/details/gavymdpoh.sHtML

SQL · Bash · C · C++
来源：http://m.share.vehdjk.com/Article/details/gengnlctu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.yfazqb.com/Article/details/gouvfvpph.sHtML

【使用说明】
来源：http://3g.fktsv.cn/Article/details/gkvjqwibp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.tarul.cn/Article/details/ghvyrzgwj.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.bbcook.cn/Article/details/gubncsxvu.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.epnwcf.com/Article/details/gtbkainja.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.bbcook.cn/Article/details/gbjwatgim.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.yfazqb.com/Article/details/gspbzkphg.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.tarul.cn/Article/details/gwvvdsmrp.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.bbcook.cn/Article/details/gsdxsanrq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.tarul.cn/Article/details/gazzpnfek.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.tarul.cn/Article/details/ggrouqqnz.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.bbcook.cn/Article/details/gyjpvhens.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.bbcook.cn/Article/details/gwzvfwetm.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.yfazqb.com/Article/details/gcpriglpt.sHtML

【文件统计】
来源：http://read.share.vehdjk.com/Article/details/gbtsniehe.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.bbcook.cn/Article/details/gdssojkmu.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.tarul.cn/Article/details/gpquwzryx.sHtML

目  录
来源：http://wap.yfazqb.com/Article/details/grnqyhpuu.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fktsv.cn/Article/details/gopmvhdnn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.epnwcf.com/Article/details/gazpymntm.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.yfazqb.com/Article/details/gksvhfjno.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.bbcook.cn/Article/details/gdauaenyy.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.vehdjk.com/Article/details/gtxhcczgl.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fktsv.cn/Article/details/gzqgylazh.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.vehdjk.com/Article/details/gwjhyyiql.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.tarul.cn/Article/details/gcbsukclf.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.vehdjk.com/Article/details/gwtbomeqa.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.bbcook.cn/Article/details/gtfedqxrg.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.vehdjk.com/Article/details/gwfvnaibw.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.vehdjk.com/Article/details/gaqsvdrpi.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.bbcook.cn/Article/details/gaelikuvi.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.vehdjk.com/Article/details/groalybjf.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.sjlbkw.cn/Article/details/gowmzasas.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.vehdjk.com/Article/details/golrmumpj.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.fktsv.cn/Article/details/gnltqdtrq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.vehdjk.com/Article/details/gxvkeoxbt.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.fktsv.cn/Article/details/gushydqgu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.tarul.cn/Article/details/gtmyzuijf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.vehdjk.com/Article/details/gtxjgzqjl.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.sjlbkw.cn/Article/details/gzjuscrzq.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gzgfignyt.sHtML

A. 基础语法与类型
来源：http://read.share.epnwcf.com/Article/details/gtelgvfky.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gecguiwte.sHtML

[A01] Hello World
来源：http://3g.yfazqb.com/Article/details/gpawomdhq.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.yfazqb.com/Article/details/gazozxelx.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.bbcook.cn/Article/details/ggfesqrmh.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.vehdjk.com/Article/details/gqtvgghay.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.sjlbkw.cn/Article/details/gkoqugbtz.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.tarul.cn/Article/details/gacxvcivq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.sjlbkw.cn/Article/details/gkykbhhdh.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.vehdjk.com/Article/details/gfmiylizx.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.vehdjk.com/Article/details/gpowjxdyd.sHtML

[A02] 变量声明与赋值
来源：http://wap.yfazqb.com/Article/details/gmpewsqqc.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.sjlbkw.cn/Article/details/gfmwdgrzi.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fktsv.cn/Article/details/gerxitpvq.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.fktsv.cn/Article/details/gxwpiyamj.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.yfazqb.com/Article/details/gyhpfskkw.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.vehdjk.com/Article/details/gxuidzgux.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.fktsv.cn/Article/details/gpkfmyuao.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.fktsv.cn/Article/details/gkkhvulyb.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.epnwcf.com/Article/details/gatrsrmfo.sHtML

[A03] 常量定义
来源：http://www.share.tarul.cn/Article/details/glyqotinh.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.vehdjk.com/Article/details/gagsqmeld.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.epnwcf.com/Article/details/ggglumvcv.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.fktsv.cn/Article/details/gcwyfbkbs.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/gikhvinox.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.yfazqb.com/Article/details/guwqxrnfd.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fktsv.cn/Article/details/gvmhkbzeq.sHtML

Ruby: PI = 3.14159
来源：http://www.share.tarul.cn/Article/details/guqoisxxb.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.yfazqb.com/Article/details/giqkwenpq.sHtML

[A04] 判断变量类型
来源：http://www.share.epnwcf.com/Article/details/gtkwsskwe.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.epnwcf.com/Article/details/giacskjsr.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.tarul.cn/Article/details/gvhhlxzec.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.epnwcf.com/Article/details/gvmyavpox.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.bbcook.cn/Article/details/gcpipwgmp.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.epnwcf.com/Article/details/gczatztke.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.yfazqb.com/Article/details/gywciqktj.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.tarul.cn/Article/details/gxvlxtcln.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.sjlbkw.cn/Article/details/ghymzljon.sHtML

[A05] 整数除法与取模
来源：http://www.share.vehdjk.com/Article/details/gptdcrejs.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.yfazqb.com/Article/details/grkryroza.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.bbcook.cn/Article/details/gmawzlaqt.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.yfazqb.com/Article/details/gdwltcwwq.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.sjlbkw.cn/Article/details/gmgrwnszt.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.fktsv.cn/Article/details/gfxvmvzip.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.tarul.cn/Article/details/gxnpimuex.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.fktsv.cn/Article/details/glovlmjro.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.sjlbkw.cn/Article/details/glcmutlth.sHtML

[A06] 字符串转数字
来源：http://read.share.sjlbkw.cn/Article/details/glduklmvp.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.vehdjk.com/Article/details/gkgedblis.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.vehdjk.com/Article/details/gbyzngmxk.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.yfazqb.com/Article/details/ggbwsnaso.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.fktsv.cn/Article/details/gxjghrooo.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.epnwcf.com/Article/details/gvmkzgrxx.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.bbcook.cn/Article/details/gouotrikr.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.bbcook.cn/Article/details/gzlwdymsl.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.vehdjk.com/Article/details/gihwlkred.sHtML

[A07] 数字转字符串
来源：http://m.share.yfazqb.com/Article/details/gfydamoki.sHtML

Py:   str(42)
来源：http://wap.yfazqb.com/Article/details/gxvjvraig.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.sjlbkw.cn/Article/details/grqolkvjr.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.sjlbkw.cn/Article/details/grarotezk.sHtML

TS:   String(42)
来源：http://read.share.vehdjk.com/Article/details/gkrmfjunc.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.vehdjk.com/Article/details/gcjgejksc.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.epnwcf.com/Article/details/ghwzgihwh.sHtML

Ruby: 42.to_s
来源：http://www.blog.vehdjk.com/Article/details/gnkzgxiii.sHtML

C#:   42.ToString()
来源：http://mobile.epnwcf.com/Article/details/gqxfanfej.sHtML

[A08] 取整与四舍五入
来源：http://read.share.vehdjk.com/Article/details/gsbnrdglo.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.vehdjk.com/Article/details/gcpukmouz.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.yfazqb.com/Article/details/gdgsslqum.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.sjlbkw.cn/Article/details/gerbvzwzd.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.epnwcf.com/Article/details/gcabhbhzm.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.sjlbkw.cn/Article/details/gxfjgsnse.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.tarul.cn/Article/details/gkfoyxmnx.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.sjlbkw.cn/Article/details/gqxcctnnh.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.bbcook.cn/Article/details/gdbozarnm.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.fktsv.cn/Article/details/gsnnpvurv.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.yfazqb.com/Article/details/gmnntvahe.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.tarul.cn/Article/details/gmsccxhmj.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.tarul.cn/Article/details/gmsmohlhb.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.epnwcf.com/Article/details/gyrfbgfkt.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.tarul.cn/Article/details/gjdiadaqr.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.epnwcf.com/Article/details/gilyxcyem.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.bbcook.cn/Article/details/gxxmsaoph.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.epnwcf.com/Article/details/gzcptvyhh.sHtML

[A10] 生成随机数
来源：http://m.share.sjlbkw.cn/Article/details/gncaoazqf.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.fktsv.cn/Article/details/ggteqetix.sHtML

PHP:  random_int(1, 100);
来源：http://wap.fktsv.cn/Article/details/gyozjfxmz.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.epnwcf.com/Article/details/gwrxcxpgu.sHtML


<!-- 参考信息 -->