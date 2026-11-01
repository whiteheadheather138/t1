代发 wailian999

[U71] PHP：抛出异常
来源：http://wap.bbcook.cn/Article/details/gboofzhpd.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.sjlbkw.cn/Article/details/gkcnrdvjo.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.sjlbkw.cn/Article/details/gvupmaxil.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.sjlbkw.cn/Article/details/gmqcxvgdw.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.sjlbkw.cn/Article/details/gfvltyltc.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.vehdjk.com/Article/details/gtshufpax.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fktsv.cn/Article/details/gwsevcewg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.bbcook.cn/Article/details/gdxokgisc.sHtML

[U75] PHP：依赖注入
来源：http://baike.vehdjk.com/Article/details/gayugklgi.sHtML

composer require psr/container
来源：http://wap.epnwcf.com/Article/details/gtojixdth.sHtML

[U76] PHP：简单路由
来源：http://mobile.fktsv.cn/Article/details/gtuaghpfj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.epnwcf.com/Article/details/gotvbbhbw.sHtML

[U77] PHP：模板渲染
来源：http://3g.tarul.cn/Article/details/ghteiqbqt.sHtML

composer require twig/twig
来源：http://www.m.share.bbcook.cn/Article/details/gumfpwhev.sHtML

[U78] PHP：单元测试
来源：http://blog.tarul.cn/Article/details/gxsoptwcq.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.bbcook.cn/Article/details/ghgrdaeag.sHtML

[U79] PHP：静态分析
来源：http://www.blog.sjlbkw.cn/Article/details/gxekshjng.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.tarul.cn/Article/details/gbuvgwego.sHtML

[U80] PHP：代码规范修复
来源：http://blog.sjlbkw.cn/Article/details/gylckykcl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.bbcook.cn/Article/details/gfmwzvqpf.sHtML

[U81] JS：初始化项目
来源：http://read.share.epnwcf.com/Article/details/gpoeadvkj.sHtML

npm init -y;  npm i express
来源：http://read.share.sjlbkw.cn/Article/details/ggcgqrsmr.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.bbcook.cn/Article/details/gbztzfbrh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.epnwcf.com/Article/details/gghbrxfua.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.sjlbkw.cn/Article/details/goftfrrju.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.sjlbkw.cn/Article/details/gtkbrohqf.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.yfazqb.com/Article/details/gsfjxrecp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.bbcook.cn/Article/details/gdsimmogz.sHtML

[U85] JS：可选链
来源：http://m.share.tarul.cn/Article/details/gybgsfgkp.sHtML

a?.b?.c
来源：http://blog.vehdjk.com/Article/details/gluppulgt.sHtML

[U86] JS：空值合并
来源：http://www.share.fktsv.cn/Article/details/gnueapabv.sHtML

a ?? b
来源：http://www.m.share.yfazqb.com/Article/details/ggmnbvvpd.sHtML

[U87] JS：解构默认值
来源：http://3g.epnwcf.com/Article/details/gebnttzcw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fktsv.cn/Article/details/gpdkxmnzi.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.epnwcf.com/Article/details/gvarpsbep.sHtML

{ ...a, ...b }
来源：http://www.m.share.epnwcf.com/Article/details/gmpjsnjdr.sHtML

[U89] JS：数组去重
来源：http://wap.fktsv.cn/Article/details/ggrtqtpou.sHtML

[...new Set(arr)]
来源：http://mobile.vehdjk.com/Article/details/gjlxxsklx.sHtML

[U90] JS：数字数组排序
来源：http://mobile.yfazqb.com/Article/details/gjqqubevz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fktsv.cn/Article/details/gsafxqddd.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.vehdjk.com/Article/details/gocdbrtbr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.vehdjk.com/Article/details/gmzqvvdxe.sHtML

[U92] JS：深拷贝
来源：http://mobile.sjlbkw.cn/Article/details/givynmqtj.sHtML

structuredClone(obj)
来源：http://read.share.vehdjk.com/Article/details/gbyguoykj.sHtML

[U93] JS：模板字符串
来源：http://baike.fktsv.cn/Article/details/gargbawqu.sHtML

`共 ${n} 条`
来源：http://mobile.epnwcf.com/Article/details/gmjnwthij.sHtML

[U94] JS：箭头函数
来源：http://3g.vehdjk.com/Article/details/godxmahih.sHtML

const double = x => x * 2;
来源：http://www.blog.yfazqb.com/Article/details/gcyifzokc.sHtML

[U95] JS：Promise 包装
来源：http://blog.bbcook.cn/Article/details/gqntrdcpe.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.epnwcf.com/Article/details/greodxalm.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.sjlbkw.cn/Article/details/glixfvyel.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fktsv.cn/Article/details/gdiaqdpkh.sHtML

[U97] JS：并发请求
来源：http://baike.sjlbkw.cn/Article/details/gsakjfzvy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.yfazqb.com/Article/details/grszmupar.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.vehdjk.com/Article/details/gikhpeftj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.epnwcf.com/Article/details/gvyemckzv.sHtML

[U99] JS：事件监听
来源：http://www.share.sjlbkw.cn/Article/details/gbkeanpoj.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.vehdjk.com/Article/details/gtyuujivw.sHtML

[U100] JS：DOM 查询
来源：http://blog.fktsv.cn/Article/details/gxxsujsep.sHtML

document.querySelector(".item")
来源：http://www.blog.fktsv.cn/Article/details/gbygflunw.sHtML

[U101] JS：classList 操作
来源：http://baike.yfazqb.com/Article/details/gevpladhd.sHtML

el.classList.toggle("active")
来源：http://www.m.share.sjlbkw.cn/Article/details/guuxbkdyk.sHtML

[U102] JS：本地存储
来源：http://blog.tarul.cn/Article/details/gxmetcojl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.tarul.cn/Article/details/gkdvipzsc.sHtML

[U103] JS：定时器
来源：http://www.m.share.fktsv.cn/Article/details/gtdqymkqd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.epnwcf.com/Article/details/givaxxihn.sHtML

[U104] JS：防抖
来源：http://wap.fktsv.cn/Article/details/ghyvuhwxb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.yfazqb.com/Article/details/gwdfwsjrz.sHtML

[U105] JS：节流
来源：http://3g.sjlbkw.cn/Article/details/gplmixwsh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.bbcook.cn/Article/details/glzhfytzl.sHtML

[U106] JS：日期格式化
来源：http://3g.sjlbkw.cn/Article/details/gwctqogrm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.vehdjk.com/Article/details/gawcagtim.sHtML

[U107] JS：数字千分位
来源：http://blog.bbcook.cn/Article/details/gyevojdpg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.tarul.cn/Article/details/gwxkdmncn.sHtML

[U108] JS：随机整数
来源：http://www.share.sjlbkw.cn/Article/details/gfcpylfwo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.vehdjk.com/Article/details/gsrtljrut.sHtML

[U109] JS：数组分组
来源：http://read.share.fktsv.cn/Article/details/girzabhmz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.vehdjk.com/Article/details/gqmctevpt.sHtML

[U110] JS：数组分块
来源：http://blog.bbcook.cn/Article/details/gzgogilkf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.epnwcf.com/Article/details/glocfnppf.sHtML

[U111] JS：对象转 Map
来源：http://m.share.epnwcf.com/Article/details/gwcetcroq.sHtML

new Map(Object.entries(obj))
来源：http://m.share.epnwcf.com/Article/details/grrltsysx.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fktsv.cn/Article/details/gepmrudfr.sHtML

"7".padStart(3, "0")
来源：http://m.share.bbcook.cn/Article/details/gesfdlyid.sHtML

[U113] JS：正则替换全部
来源：http://read.share.vehdjk.com/Article/details/gkgogzfpi.sHtML

s.replaceAll("a", "b")
来源：http://blog.epnwcf.com/Article/details/ghqplyarg.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.bbcook.cn/Article/details/gaynudhhp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fktsv.cn/Article/details/gatanjrnj.sHtML

[U115] JS：生成 UUID
来源：http://m.share.bbcook.cn/Article/details/gliptxfqq.sHtML

crypto.randomUUID()
来源：http://mobile.fktsv.cn/Article/details/gvkqvrmpy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.sjlbkw.cn/Article/details/gnzefxerd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.tarul.cn/Article/details/gqqygmtaw.sHtML

[U117] JS：单元测试
来源：http://mobile.vehdjk.com/Article/details/ghmimddzz.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.sjlbkw.cn/Article/details/gpexqmwha.sHtML

[U118] JS：开发服务器
来源：http://read.share.fktsv.cn/Article/details/gnwzfcjdg.sHtML

npm i -D vite;  npx vite
来源：http://wap.yfazqb.com/Article/details/gomecxnpf.sHtML

[U119] JS：生产构建
来源：http://baike.yfazqb.com/Article/details/gbdbfhhaj.sHtML

npx vite build
来源：http://mobile.fktsv.cn/Article/details/ghamycajw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.sjlbkw.cn/Article/details/gcpgrkowx.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.bbcook.cn/Article/details/gipltjfrl.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/giryjahft.sHtML

统计汇总
来源：http://read.share.bbcook.cn/Article/details/gkqmgfllv.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gtpdbupxc.sHtML

按语言统计（条）：
来源：http://mobile.epnwcf.com/Article/details/gsyyiwsfq.sHtML

Python ......... 252
来源：http://3g.tarul.cn/Article/details/gkktqvtvm.sHtML

PHP ............ 252
来源：http://www.m.share.epnwcf.com/Article/details/ghgnnessw.sHtML

JavaScript ..... 252
来源：http://wap.vehdjk.com/Article/details/gdcnjgvgo.sHtML

TypeScript ..... 212
来源：http://mobile.tarul.cn/Article/details/glovoudkp.sHtML

Java ........... 212
来源：http://read.share.sjlbkw.cn/Article/details/ggokqvdke.sHtML

Go ............. 212
来源：http://read.share.epnwcf.com/Article/details/gozpdcbuy.sHtML

Ruby ........... 212
来源：http://mobile.yfazqb.com/Article/details/gdeyovmyr.sHtML

C# ............. 212
来源：http://blog.yfazqb.com/Article/details/govbtyvuk.sHtML

C .............. 30
来源：http://m.share.fktsv.cn/Article/details/gdgsdsqtp.sHtML

C++ ............ 30
来源：http://read.share.fktsv.cn/Article/details/gnwfhpmxh.sHtML

SQL ............ 90
来源：http://blog.yfazqb.com/Article/details/grythpitg.sHtML

Bash ........... 80
来源：http://www.blog.fktsv.cn/Article/details/gjizhjoaa.sHtML

Kotlin ......... 15
来源：http://3g.tarul.cn/Article/details/gecjootdm.sHtML

Swift .......... 15
来源：http://wap.vehdjk.com/Article/details/gpehhkhhv.sHtML

Lua ............ 10
来源：http://mobile.vehdjk.com/Article/details/gxiuaddis.sHtML

Perl ........... 10
来源：http://www.share.bbcook.cn/Article/details/gqvwiyiux.sHtML

Scala .......... 10
来源：http://www.share.epnwcf.com/Article/details/gslfbegyb.sHtML

------------------------------------
来源：http://www.blog.bbcook.cn/Article/details/geeyidpex.sHtML

合计 ........... 2106 条
来源：http://blog.tarul.cn/Article/details/gsadhxjlg.sHtML

按章节统计：
来源：http://3g.sjlbkw.cn/Article/details/gmwdfenax.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.yfazqb.com/Article/details/gruyuqgnv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.epnwcf.com/Article/details/guekrsniv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.epnwcf.com/Article/details/ggswblnfk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fktsv.cn/Article/details/gfntfciyq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.epnwcf.com/Article/details/gtliydkpo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.yfazqb.com/Article/details/gxdwjkoro.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.yfazqb.com/Article/details/gkwrxxggl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.tarul.cn/Article/details/gnzbwjowo.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.tarul.cn/Article/details/gyzavinht.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fktsv.cn/Article/details/goswpuzgn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.yfazqb.com/Article/details/gfnmtsmdk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.sjlbkw.cn/Article/details/gkanfydst.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.yfazqb.com/Article/details/ghhsrwfyb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.vehdjk.com/Article/details/gwtfvyxtn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fktsv.cn/Article/details/gvfeasrja.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.yfazqb.com/Article/details/gxrdkwosc.sHtML

Q SQL 专题                              90
来源：http://3g.tarul.cn/Article/details/gwrxtbefl.sHtML

R Bash 专题                             80
来源：http://wap.sjlbkw.cn/Article/details/gazgjqhna.sHtML

S C / C++ 专题                          60
来源：http://mobile.epnwcf.com/Article/details/guncrbqdn.sHtML

T 其他语言补充                          60
来源：http://3g.yfazqb.com/Article/details/gitwvoqly.sHtML

U 高频实用片段                         120
来源：http://blog.vehdjk.com/Article/details/gjnketwkh.sHtML

------------------------------------
来源：http://baike.yfazqb.com/Article/details/glvcsnfsr.sHtML

合计                                  2106 条
来源：http://baike.tarul.cn/Article/details/gzdwbepzy.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.bbcook.cn/Article/details/gbgczeixn.sHtML

使用提醒
来源：http://mobile.sjlbkw.cn/Article/details/ghnvrpaik.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.bbcook.cn/Article/details/gvxlqjlvn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.epnwcf.com/Article/details/giythlcrb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.yfazqb.com/Article/details/gahzbkajn.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.yfazqb.com/Article/details/gytcmkorf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.vehdjk.com/Article/details/gdstahtcg.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.yfazqb.com/Article/details/gjayhrjgg.sHtML

—— 文件结束 ——
来源：http://mobile.fktsv.cn/Article/details/gheinkfpe.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gaifnqfnw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.bbcook.cn/Article/details/gynpidmbb.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.yfazqb.com/Article/details/gpafozoqx.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gudkydmhi.sHtML

【收录内容】
来源：http://www.share.bbcook.cn/Article/details/golrmzehn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.epnwcf.com/Article/details/ghoigrlib.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.tarul.cn/Article/details/gmmwhrwyp.sHtML

SQL · Bash · C · C++
来源：http://m.share.epnwcf.com/Article/details/gtkpnlcrp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.tarul.cn/Article/details/gggeykesg.sHtML

【使用说明】
来源：http://mobile.epnwcf.com/Article/details/gatceqdqh.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.epnwcf.com/Article/details/gbhpyxmet.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.tarul.cn/Article/details/ggghzazam.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.vehdjk.com/Article/details/gnwwwtuef.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fktsv.cn/Article/details/gendeqxnx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.tarul.cn/Article/details/gceiyskpg.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.sjlbkw.cn/Article/details/gigcibgob.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fktsv.cn/Article/details/gljeloyjs.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.tarul.cn/Article/details/gdyhkkhrx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.tarul.cn/Article/details/gjmswbkaz.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.epnwcf.com/Article/details/gpfynhkop.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fktsv.cn/Article/details/gahflflyo.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.yfazqb.com/Article/details/gvtcohgce.sHtML

【文件统计】
来源：http://www.blog.fktsv.cn/Article/details/gfbzcucbu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.vehdjk.com/Article/details/gvxgfmdkz.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fktsv.cn/Article/details/gmfioeyic.sHtML

目  录
来源：http://blog.fktsv.cn/Article/details/gmyhgjfkl.sHtML

--------------------------------------------------------------------------------
来源：http://blog.sjlbkw.cn/Article/details/gmsvstxdz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.sjlbkw.cn/Article/details/geouhoeka.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.yfazqb.com/Article/details/gporhfdio.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.bbcook.cn/Article/details/gcewjlnjs.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.yfazqb.com/Article/details/gjwqtduls.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.tarul.cn/Article/details/gskavzxwf.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.bbcook.cn/Article/details/gaknefawm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.epnwcf.com/Article/details/gtatetyfr.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.yfazqb.com/Article/details/gxwdwzvzc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.tarul.cn/Article/details/glthntjfu.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.bbcook.cn/Article/details/gmyboqrfo.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.yfazqb.com/Article/details/gbdlzztwj.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gihrnpkba.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.epnwcf.com/Article/details/gbflacqgu.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.yfazqb.com/Article/details/gyvpvblhs.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.sjlbkw.cn/Article/details/gpqhmrrnz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.sjlbkw.cn/Article/details/glqztewuc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.sjlbkw.cn/Article/details/gppudanbh.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.epnwcf.com/Article/details/gmhkmegfj.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.tarul.cn/Article/details/gcdexnifc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.sjlbkw.cn/Article/details/gvvtcvkkh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.tarul.cn/Article/details/gqszpecgz.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/geliumlpi.sHtML

A. 基础语法与类型
来源：http://m.share.epnwcf.com/Article/details/gqjdodkun.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gvbxchpev.sHtML

[A01] Hello World
来源：http://www.share.fktsv.cn/Article/details/gccpetkah.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.bbcook.cn/Article/details/grksrjrmu.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.bbcook.cn/Article/details/gkegozmmz.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.sjlbkw.cn/Article/details/gacntlwlz.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.epnwcf.com/Article/details/gpkbthvpy.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.fktsv.cn/Article/details/gzplbeqtw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.vehdjk.com/Article/details/gfnqmytwz.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.bbcook.cn/Article/details/gdlfkdcmp.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.tarul.cn/Article/details/ggflvopbp.sHtML

[A02] 变量声明与赋值
来源：http://wap.vehdjk.com/Article/details/gvmhmnvbc.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.fktsv.cn/Article/details/guqqmdedw.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.bbcook.cn/Article/details/gndponztl.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.epnwcf.com/Article/details/gnikdaxfz.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.epnwcf.com/Article/details/gifrlovrz.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.vehdjk.com/Article/details/glnuranod.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.yfazqb.com/Article/details/gvblgibbr.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.sjlbkw.cn/Article/details/guafjogou.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.sjlbkw.cn/Article/details/gtrgknqht.sHtML

[A03] 常量定义
来源：http://m.share.bbcook.cn/Article/details/grewoaxqu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.tarul.cn/Article/details/gwchbinib.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.fktsv.cn/Article/details/gcfjxxshx.sHtML

JS:   const PI = 3.14159;
来源：http://baike.bbcook.cn/Article/details/grtgwhtfn.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.tarul.cn/Article/details/gtoqexcgx.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.bbcook.cn/Article/details/ghmrkczjj.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.fktsv.cn/Article/details/geadkbsgh.sHtML

Ruby: PI = 3.14159
来源：http://www.share.sjlbkw.cn/Article/details/gtldtiwyk.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/gbqjwhlxf.sHtML

[A04] 判断变量类型
来源：http://www.blog.sjlbkw.cn/Article/details/gmpjiayml.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.vehdjk.com/Article/details/gywluakps.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.epnwcf.com/Article/details/geeewoqtz.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.bbcook.cn/Article/details/gbypbzssj.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.vehdjk.com/Article/details/gcxcthyii.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.tarul.cn/Article/details/gzyjsfmru.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.tarul.cn/Article/details/gqpxkczsl.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.tarul.cn/Article/details/gauphmgwj.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.sjlbkw.cn/Article/details/gmghhzgsw.sHtML

[A05] 整数除法与取模
来源：http://www.share.yfazqb.com/Article/details/genwfkgul.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.epnwcf.com/Article/details/gsqlzetuw.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.sjlbkw.cn/Article/details/gqyrmgclr.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.bbcook.cn/Article/details/gbkklreqw.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.tarul.cn/Article/details/gvjcnbdbk.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.yfazqb.com/Article/details/gvegkjubt.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.tarul.cn/Article/details/ggfeyuqdq.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.tarul.cn/Article/details/gannjpczv.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.sjlbkw.cn/Article/details/ggkfnpagk.sHtML

[A06] 字符串转数字
来源：http://www.blog.vehdjk.com/Article/details/gqeigmyia.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.tarul.cn/Article/details/gavleiken.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.bbcook.cn/Article/details/gkvimhrhh.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.bbcook.cn/Article/details/guephpjzb.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.vehdjk.com/Article/details/gqehkwnls.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.tarul.cn/Article/details/gsdqerewz.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.bbcook.cn/Article/details/gazecysfa.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.tarul.cn/Article/details/gxdjbxmgh.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.tarul.cn/Article/details/gcoibtzom.sHtML

[A07] 数字转字符串
来源：http://www.blog.yfazqb.com/Article/details/gllzbgtvy.sHtML

Py:   str(42)
来源：http://read.share.yfazqb.com/Article/details/gvupbwxfn.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.vehdjk.com/Article/details/gunkbcvga.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.yfazqb.com/Article/details/gtqghnbgp.sHtML

TS:   String(42)
来源：http://www.share.sjlbkw.cn/Article/details/gwpzcmtsb.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.fktsv.cn/Article/details/gndcblxlb.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.sjlbkw.cn/Article/details/ghmpckblw.sHtML

Ruby: 42.to_s
来源：http://baike.yfazqb.com/Article/details/grlgzsplx.sHtML

C#:   42.ToString()
来源：http://www.m.share.vehdjk.com/Article/details/gcyvbxfoj.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.yfazqb.com/Article/details/gjmhbvavk.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.sjlbkw.cn/Article/details/gzrjwqain.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.bbcook.cn/Article/details/gzsmaamtb.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.sjlbkw.cn/Article/details/gbhdphxka.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.epnwcf.com/Article/details/guypctbco.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.bbcook.cn/Article/details/gbklyklcu.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.vehdjk.com/Article/details/gkshohzpv.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.yfazqb.com/Article/details/gxfcnrtmp.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.sjlbkw.cn/Article/details/glupbeuuf.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.bbcook.cn/Article/details/gwjxqsadb.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fktsv.cn/Article/details/gudyoajno.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.bbcook.cn/Article/details/gjxpiiwzj.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.tarul.cn/Article/details/grarglmej.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gxbpyinkw.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.sjlbkw.cn/Article/details/gleyurtvs.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.yfazqb.com/Article/details/gsjwhhnti.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.sjlbkw.cn/Article/details/glutxvemt.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.fktsv.cn/Article/details/gqbkvudzk.sHtML

[A10] 生成随机数
来源：http://blog.bbcook.cn/Article/details/gzyzkdzcc.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.tarul.cn/Article/details/gfjyayyzp.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.epnwcf.com/Article/details/gsfgsimbb.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.vehdjk.com/Article/details/godwozwni.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.bbcook.cn/Article/details/gpdqbzuqn.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.sjlbkw.cn/Article/details/gikedkelu.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.bbcook.cn/Article/details/gdnrslrbf.sHtML

Ruby: rand(1..100)
来源：http://baike.epnwcf.com/Article/details/gwtbszczu.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.yfazqb.com/Article/details/gktaftopk.sHtML

[A11] 条件表达式（三元）
来源：http://wap.fktsv.cn/Article/details/gshoxmajc.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.yfazqb.com/Article/details/gtowhuvtv.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.sjlbkw.cn/Article/details/garqtlgbi.sHtML


<!-- 参考信息 -->