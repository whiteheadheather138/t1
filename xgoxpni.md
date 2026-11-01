代发 wailian999

[U69] PHP：PDO 预处理
来源：http://read.share.epnwcf.com/Article/details/gsvgurobk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.epnwcf.com/Article/details/giiwcbmxd.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.epnwcf.com/Article/details/gsmialqjh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.sjlbkw.cn/Article/details/glytdqdfh.sHtML

[U71] PHP：抛出异常
来源：http://read.share.epnwcf.com/Article/details/gtbbsviuc.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.bbcook.cn/Article/details/gibtxdnlt.sHtML

[U72] PHP：写错误日志
来源：http://3g.fktsv.cn/Article/details/gxdebzuab.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.bbcook.cn/Article/details/gcvdutdhc.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.yfazqb.com/Article/details/gkcqngyob.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.tarul.cn/Article/details/gzjfwipyc.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fktsv.cn/Article/details/gqkskltmn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.bbcook.cn/Article/details/goiirrkqj.sHtML

[U75] PHP：依赖注入
来源：http://mobile.tarul.cn/Article/details/gxnybucik.sHtML

composer require psr/container
来源：http://www.m.share.fktsv.cn/Article/details/gjcmcmbau.sHtML

[U76] PHP：简单路由
来源：http://read.share.fktsv.cn/Article/details/gfkphzfxr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.yfazqb.com/Article/details/gtmixrjon.sHtML

[U77] PHP：模板渲染
来源：http://3g.tarul.cn/Article/details/gqechkool.sHtML

composer require twig/twig
来源：http://blog.yfazqb.com/Article/details/gnlqqwodp.sHtML

[U78] PHP：单元测试
来源：http://wap.sjlbkw.cn/Article/details/gmjsqkxpg.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.bbcook.cn/Article/details/gbhltkilx.sHtML

[U79] PHP：静态分析
来源：http://wap.epnwcf.com/Article/details/gwnmpsajj.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.yfazqb.com/Article/details/gowdjqnri.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.bbcook.cn/Article/details/gbscsmxnb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.vehdjk.com/Article/details/gtkvrjpyz.sHtML

[U81] JS：初始化项目
来源：http://baike.bbcook.cn/Article/details/glhdzywfs.sHtML

npm init -y;  npm i express
来源：http://baike.yfazqb.com/Article/details/gygrodnty.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.bbcook.cn/Article/details/govuapmmh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.yfazqb.com/Article/details/gqunlsxoh.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fktsv.cn/Article/details/gdyeunect.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.tarul.cn/Article/details/gupdxjkkq.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.yfazqb.com/Article/details/gbmmbqske.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.vehdjk.com/Article/details/gkuxvykha.sHtML

[U85] JS：可选链
来源：http://wap.vehdjk.com/Article/details/gyuywgypf.sHtML

a?.b?.c
来源：http://baike.yfazqb.com/Article/details/gxlntlzlv.sHtML

[U86] JS：空值合并
来源：http://mobile.tarul.cn/Article/details/gxlybtzvt.sHtML

a ?? b
来源：http://read.share.bbcook.cn/Article/details/gjqgtefjr.sHtML

[U87] JS：解构默认值
来源：http://www.blog.bbcook.cn/Article/details/gdzjoxetp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.yfazqb.com/Article/details/ggludczsy.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fktsv.cn/Article/details/gakfimuxq.sHtML

{ ...a, ...b }
来源：http://m.share.yfazqb.com/Article/details/gaggnmqpf.sHtML

[U89] JS：数组去重
来源：http://m.share.bbcook.cn/Article/details/gecbpjhpx.sHtML

[...new Set(arr)]
来源：http://mobile.sjlbkw.cn/Article/details/gbgmbsuee.sHtML

[U90] JS：数字数组排序
来源：http://www.share.vehdjk.com/Article/details/gtffuamup.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.vehdjk.com/Article/details/gjzuffedi.sHtML

[U91] JS：对象键值遍历
来源：http://wap.tarul.cn/Article/details/gitwehucy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fktsv.cn/Article/details/grumjxmgt.sHtML

[U92] JS：深拷贝
来源：http://baike.bbcook.cn/Article/details/gdjwqupsn.sHtML

structuredClone(obj)
来源：http://www.share.yfazqb.com/Article/details/gmjfyfaqt.sHtML

[U93] JS：模板字符串
来源：http://read.share.fktsv.cn/Article/details/gdcjurdwu.sHtML

`共 ${n} 条`
来源：http://baike.sjlbkw.cn/Article/details/gpdhycbkm.sHtML

[U94] JS：箭头函数
来源：http://www.share.sjlbkw.cn/Article/details/gpjdtaepm.sHtML

const double = x => x * 2;
来源：http://read.share.fktsv.cn/Article/details/gseobwsgp.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.vehdjk.com/Article/details/gcjvzgqja.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fktsv.cn/Article/details/geinitqyj.sHtML

[U96] JS：async/await 与异常
来源：http://blog.vehdjk.com/Article/details/gablnpadn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.vehdjk.com/Article/details/gfanfxqkb.sHtML

[U97] JS：并发请求
来源：http://www.share.fktsv.cn/Article/details/gpgdqsyxl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.tarul.cn/Article/details/ghpmlugdi.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.yfazqb.com/Article/details/ggoermskm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.yfazqb.com/Article/details/gsepbgxer.sHtML

[U99] JS：事件监听
来源：http://wap.tarul.cn/Article/details/gocreosnx.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.sjlbkw.cn/Article/details/gsynwpndf.sHtML

[U100] JS：DOM 查询
来源：http://www.share.tarul.cn/Article/details/geseerjst.sHtML

document.querySelector(".item")
来源：http://www.blog.bbcook.cn/Article/details/gclwmetfh.sHtML

[U101] JS：classList 操作
来源：http://m.share.tarul.cn/Article/details/gsttunsbs.sHtML

el.classList.toggle("active")
来源：http://baike.epnwcf.com/Article/details/gxipnxazh.sHtML

[U102] JS：本地存储
来源：http://wap.yfazqb.com/Article/details/glgvdrtul.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.vehdjk.com/Article/details/gkgmbuiry.sHtML

[U103] JS：定时器
来源：http://www.m.share.yfazqb.com/Article/details/gzoifcnsk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.vehdjk.com/Article/details/gktnevnpc.sHtML

[U104] JS：防抖
来源：http://www.blog.epnwcf.com/Article/details/gdwuyraqb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.vehdjk.com/Article/details/guharuezk.sHtML

[U105] JS：节流
来源：http://m.share.vehdjk.com/Article/details/gqvsatctn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.bbcook.cn/Article/details/gcowjzsmh.sHtML

[U106] JS：日期格式化
来源：http://blog.sjlbkw.cn/Article/details/gwydnbfkv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fktsv.cn/Article/details/gxqyaxotv.sHtML

[U107] JS：数字千分位
来源：http://www.share.bbcook.cn/Article/details/guqdacsfy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.yfazqb.com/Article/details/gekodoopi.sHtML

[U108] JS：随机整数
来源：http://www.share.tarul.cn/Article/details/gwdwoyswq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.vehdjk.com/Article/details/gglvmrzwa.sHtML

[U109] JS：数组分组
来源：http://read.share.vehdjk.com/Article/details/gchhxghrk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.epnwcf.com/Article/details/ghppqvnai.sHtML

[U110] JS：数组分块
来源：http://m.share.yfazqb.com/Article/details/gbgpcddga.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.epnwcf.com/Article/details/gostxuelu.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.yfazqb.com/Article/details/gqjxntxos.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.tarul.cn/Article/details/gijexgynb.sHtML

[U112] JS：字符串补位
来源：http://3g.sjlbkw.cn/Article/details/guqtkhioy.sHtML

"7".padStart(3, "0")
来源：http://read.share.yfazqb.com/Article/details/gmadkebfn.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.bbcook.cn/Article/details/gbarxhzcq.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fktsv.cn/Article/details/gtimtsiaw.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqeeuckh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.vehdjk.com/Article/details/girftrwkr.sHtML

[U115] JS：生成 UUID
来源：http://www.share.tarul.cn/Article/details/gcoppqwbc.sHtML

crypto.randomUUID()
来源：http://www.blog.yfazqb.com/Article/details/gljxcpdnz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.tarul.cn/Article/details/givvyrhct.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fktsv.cn/Article/details/gmdhdauoa.sHtML

[U117] JS：单元测试
来源：http://wap.sjlbkw.cn/Article/details/gcpkvrzao.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.epnwcf.com/Article/details/gicczhopm.sHtML

[U118] JS：开发服务器
来源：http://blog.bbcook.cn/Article/details/gmgtxrpfp.sHtML

npm i -D vite;  npx vite
来源：http://www.share.bbcook.cn/Article/details/gzyljzylv.sHtML

[U119] JS：生产构建
来源：http://baike.fktsv.cn/Article/details/gsodparuc.sHtML

npx vite build
来源：http://www.blog.yfazqb.com/Article/details/gblhqiiyd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.bbcook.cn/Article/details/gkcjtgmns.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fktsv.cn/Article/details/grwdkmrql.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/goucwfkzw.sHtML

统计汇总
来源：http://blog.epnwcf.com/Article/details/gnxrpaoaq.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gqabhybqj.sHtML

按语言统计（条）：
来源：http://baike.sjlbkw.cn/Article/details/ggwtqpore.sHtML

Python ......... 252
来源：http://www.share.fktsv.cn/Article/details/gqdvezope.sHtML

PHP ............ 252
来源：http://wap.epnwcf.com/Article/details/gnuwrulxl.sHtML

JavaScript ..... 252
来源：http://wap.bbcook.cn/Article/details/guyltpgzh.sHtML

TypeScript ..... 212
来源：http://baike.epnwcf.com/Article/details/gxufsadtf.sHtML

Java ........... 212
来源：http://read.share.tarul.cn/Article/details/gdlbtpahh.sHtML

Go ............. 212
来源：http://baike.tarul.cn/Article/details/gghensvjl.sHtML

Ruby ........... 212
来源：http://baike.sjlbkw.cn/Article/details/grnirrifx.sHtML

C# ............. 212
来源：http://baike.sjlbkw.cn/Article/details/gosznizrd.sHtML

C .............. 30
来源：http://wap.yfazqb.com/Article/details/gnzpokpyh.sHtML

C++ ............ 30
来源：http://3g.vehdjk.com/Article/details/gqggmnjpn.sHtML

SQL ............ 90
来源：http://read.share.tarul.cn/Article/details/gylzrmypk.sHtML

Bash ........... 80
来源：http://m.share.tarul.cn/Article/details/gemduzlbk.sHtML

Kotlin ......... 15
来源：http://www.blog.sjlbkw.cn/Article/details/gxidlrzpo.sHtML

Swift .......... 15
来源：http://baike.epnwcf.com/Article/details/ggnazoteu.sHtML

Lua ............ 10
来源：http://baike.sjlbkw.cn/Article/details/ggsimcbic.sHtML

Perl ........... 10
来源：http://m.share.sjlbkw.cn/Article/details/gyfsfpvgh.sHtML

Scala .......... 10
来源：http://www.share.fktsv.cn/Article/details/gopwzicsp.sHtML

------------------------------------
来源：http://m.share.vehdjk.com/Article/details/gegbvqtrx.sHtML

合计 ........... 2106 条
来源：http://m.share.epnwcf.com/Article/details/gkhahprjz.sHtML

按章节统计：
来源：http://read.share.yfazqb.com/Article/details/gnpmyksdl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fktsv.cn/Article/details/gmdxyzuzb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.bbcook.cn/Article/details/gqqorctvj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.yfazqb.com/Article/details/gysrleoxl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.epnwcf.com/Article/details/gwkzcgphr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.tarul.cn/Article/details/gewkegxjd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.bbcook.cn/Article/details/gvrmwiqqe.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.yfazqb.com/Article/details/gdfqgtata.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fktsv.cn/Article/details/gqegpyerz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.yfazqb.com/Article/details/gmzjgbdkm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.bbcook.cn/Article/details/glydkehzi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fktsv.cn/Article/details/gpxcavjwo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.epnwcf.com/Article/details/gscmnmplr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.sjlbkw.cn/Article/details/gylnbjdqo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.sjlbkw.cn/Article/details/godwqoweq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.epnwcf.com/Article/details/gaqwyhral.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.bbcook.cn/Article/details/gnqkihnqb.sHtML

Q SQL 专题                              90
来源：http://wap.epnwcf.com/Article/details/gbucljvhg.sHtML

R Bash 专题                             80
来源：http://blog.fktsv.cn/Article/details/gflqstinj.sHtML

S C / C++ 专题                          60
来源：http://baike.sjlbkw.cn/Article/details/gzpswupje.sHtML

T 其他语言补充                          60
来源：http://www.share.tarul.cn/Article/details/gbngntopi.sHtML

U 高频实用片段                         120
来源：http://www.share.fktsv.cn/Article/details/gxfooioxg.sHtML

------------------------------------
来源：http://m.share.vehdjk.com/Article/details/globgxyvd.sHtML

合计                                  2106 条
来源：http://www.m.share.vehdjk.com/Article/details/gddrxtqfj.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.tarul.cn/Article/details/gehdaqhar.sHtML

使用提醒
来源：http://3g.yfazqb.com/Article/details/gwazglxen.sHtML

--------------------------------------------------------------------------------
来源：http://3g.yfazqb.com/Article/details/glehixmpc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fktsv.cn/Article/details/gsfjbxzsk.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.vehdjk.com/Article/details/gzmrpioez.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.yfazqb.com/Article/details/grnuzkaad.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.tarul.cn/Article/details/gieklwayy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.sjlbkw.cn/Article/details/gualhnggz.sHtML

—— 文件结束 ——
来源：http://blog.epnwcf.com/Article/details/gqymphygg.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/garmstwkz.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.vehdjk.com/Article/details/gyizvrrvc.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.sjlbkw.cn/Article/details/gdziebnif.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gourzrgzd.sHtML

【收录内容】
来源：http://read.share.bbcook.cn/Article/details/goqnkoizp.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fktsv.cn/Article/details/gfbslvnwg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.sjlbkw.cn/Article/details/gtzvzpqet.sHtML

SQL · Bash · C · C++
来源：http://blog.tarul.cn/Article/details/geqnvbzpf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.fktsv.cn/Article/details/gehowuavo.sHtML

【使用说明】
来源：http://baike.sjlbkw.cn/Article/details/gmkhrjyph.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fktsv.cn/Article/details/gyfkgqkzm.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.vehdjk.com/Article/details/gxgvplizz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.bbcook.cn/Article/details/gvpjbubhn.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fktsv.cn/Article/details/gaehshuej.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.tarul.cn/Article/details/gwzqkxjaz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.epnwcf.com/Article/details/gvdeqhexh.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.bbcook.cn/Article/details/gyoqhrwfb.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.bbcook.cn/Article/details/gwzogrqhu.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.bbcook.cn/Article/details/grrcwwpiu.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.vehdjk.com/Article/details/gpsduvlki.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.sjlbkw.cn/Article/details/gkoibxrtz.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.vehdjk.com/Article/details/gjchkomlu.sHtML

【文件统计】
来源：http://3g.yfazqb.com/Article/details/gnrgiurxr.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fktsv.cn/Article/details/gltfjftkq.sHtML

--------------------------------------------------------------------------------
来源：http://baike.epnwcf.com/Article/details/gmmppmqjh.sHtML

目  录
来源：http://blog.epnwcf.com/Article/details/gprghniqa.sHtML

--------------------------------------------------------------------------------
来源：http://3g.sjlbkw.cn/Article/details/gpqlgywmd.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.tarul.cn/Article/details/gquerqnpx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.vehdjk.com/Article/details/gaipqtmxn.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.tarul.cn/Article/details/gzmhsdqxt.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.sjlbkw.cn/Article/details/ganlkhmha.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.sjlbkw.cn/Article/details/gqbktjldv.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.tarul.cn/Article/details/geaskuwmf.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.yfazqb.com/Article/details/gwzqpxxhq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.vehdjk.com/Article/details/gttyqxnxh.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.tarul.cn/Article/details/gkillqobv.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.tarul.cn/Article/details/gvtnpeher.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.yfazqb.com/Article/details/geccrtdbt.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fktsv.cn/Article/details/gsccnychc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.vehdjk.com/Article/details/gloabgnfv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.tarul.cn/Article/details/goyfaumhx.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.epnwcf.com/Article/details/gmxslqbab.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.bbcook.cn/Article/details/gzrhluidq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.bbcook.cn/Article/details/gwrjbkabl.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.fktsv.cn/Article/details/gplggkpwt.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.epnwcf.com/Article/details/glmxnxtwt.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fktsv.cn/Article/details/glldgaykr.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.epnwcf.com/Article/details/gsgbrkhym.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gulmznbsb.sHtML

A. 基础语法与类型
来源：http://blog.sjlbkw.cn/Article/details/gnatebzou.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gqtqgkmry.sHtML

[A01] Hello World
来源：http://baike.fktsv.cn/Article/details/gyqzszpye.sHtML

Py:   print("Hello, World!")
来源：http://wap.bbcook.cn/Article/details/gvanxtjvy.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.tarul.cn/Article/details/gdrosuadc.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.yfazqb.com/Article/details/guanfenuw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.yfazqb.com/Article/details/gkrizkjjf.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.yfazqb.com/Article/details/glczbweeu.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.bbcook.cn/Article/details/gsnmphouk.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fktsv.cn/Article/details/gnqnaxucz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.bbcook.cn/Article/details/gslcpkjjc.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.vehdjk.com/Article/details/giuhrsona.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.bbcook.cn/Article/details/gwkufdcjt.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.tarul.cn/Article/details/gtazhavyg.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.epnwcf.com/Article/details/gewnghynn.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.vehdjk.com/Article/details/gmkwfsbmg.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.epnwcf.com/Article/details/glyycszjl.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.yfazqb.com/Article/details/gdykphptn.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.yfazqb.com/Article/details/gkpucexrz.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.sjlbkw.cn/Article/details/grtnmditw.sHtML

[A03] 常量定义
来源：http://3g.bbcook.cn/Article/details/gqchcvokl.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.bbcook.cn/Article/details/gknwtnqcl.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gurhsxoxr.sHtML

JS:   const PI = 3.14159;
来源：http://baike.tarul.cn/Article/details/gggxvbovt.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.vehdjk.com/Article/details/gbhjqtwbo.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.bbcook.cn/Article/details/gnufnstfl.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwompvqn.sHtML

Ruby: PI = 3.14159
来源：http://3g.tarul.cn/Article/details/gexrviicv.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.vehdjk.com/Article/details/gfuvzkutv.sHtML

[A04] 判断变量类型
来源：http://baike.tarul.cn/Article/details/guxtdtaae.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.yfazqb.com/Article/details/gkahyhray.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.vehdjk.com/Article/details/gsdtucnre.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.bbcook.cn/Article/details/gvkohgfzn.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.sjlbkw.cn/Article/details/gecnycbbl.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.vehdjk.com/Article/details/gpdjtnmhh.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.vehdjk.com/Article/details/gzwfsexzn.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.sjlbkw.cn/Article/details/gdqedfmms.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fktsv.cn/Article/details/gdbnvxflm.sHtML

[A05] 整数除法与取模
来源：http://read.share.tarul.cn/Article/details/gajpoohtv.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.bbcook.cn/Article/details/gyokfjyfk.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.bbcook.cn/Article/details/gtkwapsby.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.yfazqb.com/Article/details/gtyjsnmmz.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.bbcook.cn/Article/details/gmiawacqw.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.yfazqb.com/Article/details/glvtonccq.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.yfazqb.com/Article/details/gfhzxcdne.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.sjlbkw.cn/Article/details/gtpiuajwl.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.vehdjk.com/Article/details/gqrploxeo.sHtML

[A06] 字符串转数字
来源：http://read.share.fktsv.cn/Article/details/galplmmtm.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.epnwcf.com/Article/details/gqvwkwzoq.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.fktsv.cn/Article/details/gfbfewnrq.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.yfazqb.com/Article/details/geekeemje.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.vehdjk.com/Article/details/geuvekoug.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.epnwcf.com/Article/details/gkumvynax.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.vehdjk.com/Article/details/gcrlbqrgy.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.yfazqb.com/Article/details/gclkvgnzm.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.bbcook.cn/Article/details/gcywzzqte.sHtML

[A07] 数字转字符串
来源：http://read.share.fktsv.cn/Article/details/grrcjfsrb.sHtML

Py:   str(42)
来源：http://3g.yfazqb.com/Article/details/gnkytmeed.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.sjlbkw.cn/Article/details/ggbzqxiyp.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.bbcook.cn/Article/details/gwwkclumq.sHtML

TS:   String(42)
来源：http://read.share.tarul.cn/Article/details/gwwzkcbqr.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.vehdjk.com/Article/details/gdezymezv.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.epnwcf.com/Article/details/gvuwwcrhr.sHtML

Ruby: 42.to_s
来源：http://www.blog.epnwcf.com/Article/details/gdwhhuqwy.sHtML

C#:   42.ToString()
来源：http://mobile.tarul.cn/Article/details/gfzeotjfz.sHtML

[A08] 取整与四舍五入
来源：http://baike.epnwcf.com/Article/details/gelsggcfg.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.fktsv.cn/Article/details/gystswnje.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.vehdjk.com/Article/details/gmtkjcwaz.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.sjlbkw.cn/Article/details/gxqpkzjww.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.sjlbkw.cn/Article/details/gaqstsaul.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.yfazqb.com/Article/details/gzvmqxszr.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.sjlbkw.cn/Article/details/gbnqbmgel.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.yfazqb.com/Article/details/gjscchhwl.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.epnwcf.com/Article/details/gammkliqv.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.yfazqb.com/Article/details/gppsdptzo.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fktsv.cn/Article/details/gysvxzklv.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gebkdooto.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.epnwcf.com/Article/details/gncdxebou.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.epnwcf.com/Article/details/grpgueexn.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.epnwcf.com/Article/details/gyyjektih.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.yfazqb.com/Article/details/grvwebyxw.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.tarul.cn/Article/details/goskelvnh.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnyorvgfb.sHtML

[A10] 生成随机数
来源：http://baike.vehdjk.com/Article/details/gjtmoubyi.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.fktsv.cn/Article/details/gasmcvjfp.sHtML

PHP:  random_int(1, 100);
来源：http://www.share.bbcook.cn/Article/details/gxrblytzv.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.yfazqb.com/Article/details/guodpxcag.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.tarul.cn/Article/details/gpdkkpzxz.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.fktsv.cn/Article/details/glpsdyifj.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.bbcook.cn/Article/details/grmogergw.sHtML

Ruby: rand(1..100)
来源：http://3g.epnwcf.com/Article/details/goentnodh.sHtML


<!-- 参考信息 -->