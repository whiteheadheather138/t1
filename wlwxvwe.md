代发 wailian999

[U65] PHP：会话
来源：http://baike.fktsv.cn/Article/details/gnawjlzrl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.vehdjk.com/Article/details/glxfrziou.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.yfazqb.com/Article/details/gbhaffrjv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.sjlbkw.cn/Article/details/gxrmlgbmp.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.vehdjk.com/Article/details/gucbborth.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.yfazqb.com/Article/details/gpeippcxy.sHtML

[U68] PHP：PDO 连接
来源：http://3g.sjlbkw.cn/Article/details/gshnwbmtk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.vehdjk.com/Article/details/gqijmzgco.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.sjlbkw.cn/Article/details/ggusguuyt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.bbcook.cn/Article/details/gveruoval.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.vehdjk.com/Article/details/gifgqsnao.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fktsv.cn/Article/details/giqbnytts.sHtML

[U71] PHP：抛出异常
来源：http://mobile.vehdjk.com/Article/details/gdcdaptql.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.epnwcf.com/Article/details/gzambfhhi.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fktsv.cn/Article/details/gsfndifod.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.epnwcf.com/Article/details/gxzsfuwro.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.sjlbkw.cn/Article/details/gkmwpmpps.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fktsv.cn/Article/details/ggodzoosw.sHtML

[U74] PHP：读取环境变量
来源：http://3g.vehdjk.com/Article/details/gurfgxwjn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fktsv.cn/Article/details/gongupvaa.sHtML

[U75] PHP：依赖注入
来源：http://mobile.bbcook.cn/Article/details/grymkznqu.sHtML

composer require psr/container
来源：http://www.m.share.fktsv.cn/Article/details/giirbkfwx.sHtML

[U76] PHP：简单路由
来源：http://www.share.tarul.cn/Article/details/goajtfbgo.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.sjlbkw.cn/Article/details/gpfbqaybx.sHtML

[U77] PHP：模板渲染
来源：http://blog.vehdjk.com/Article/details/gkqxsgcoi.sHtML

composer require twig/twig
来源：http://3g.bbcook.cn/Article/details/gocpltocp.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.bbcook.cn/Article/details/gwkifyhwr.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.sjlbkw.cn/Article/details/gwuqqdtis.sHtML

[U79] PHP：静态分析
来源：http://baike.tarul.cn/Article/details/guiavnqen.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.epnwcf.com/Article/details/gbmconste.sHtML

[U80] PHP：代码规范修复
来源：http://3g.vehdjk.com/Article/details/glyfeabtg.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fktsv.cn/Article/details/gcjdsiuwh.sHtML

[U81] JS：初始化项目
来源：http://mobile.yfazqb.com/Article/details/gadgisjkh.sHtML

npm init -y;  npm i express
来源：http://baike.fktsv.cn/Article/details/gkjsojwad.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fktsv.cn/Article/details/gylbmebrh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.epnwcf.com/Article/details/ggvymikra.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.yfazqb.com/Article/details/ggwrdaypd.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.yfazqb.com/Article/details/gvrbevapd.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.bbcook.cn/Article/details/gbythkjkz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.vehdjk.com/Article/details/gfcoevbum.sHtML

[U85] JS：可选链
来源：http://read.share.sjlbkw.cn/Article/details/gtzlgyoed.sHtML

a?.b?.c
来源：http://baike.bbcook.cn/Article/details/gszmecalk.sHtML

[U86] JS：空值合并
来源：http://baike.tarul.cn/Article/details/gdlnamelx.sHtML

a ?? b
来源：http://www.share.bbcook.cn/Article/details/gcdwjxvxn.sHtML

[U87] JS：解构默认值
来源：http://3g.epnwcf.com/Article/details/gymavefrr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.yfazqb.com/Article/details/gsqekxbkr.sHtML

[U88] JS：对象展开合并
来源：http://m.share.vehdjk.com/Article/details/gwkwarisj.sHtML

{ ...a, ...b }
来源：http://wap.sjlbkw.cn/Article/details/ghtvfystr.sHtML

[U89] JS：数组去重
来源：http://blog.sjlbkw.cn/Article/details/gosrbjrbr.sHtML

[...new Set(arr)]
来源：http://www.share.fktsv.cn/Article/details/gcjpwyudm.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.yfazqb.com/Article/details/gxtqgjobp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.tarul.cn/Article/details/gxkkifmij.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.tarul.cn/Article/details/gecxhbojl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.epnwcf.com/Article/details/gsgeytoha.sHtML

[U92] JS：深拷贝
来源：http://mobile.fktsv.cn/Article/details/gqnfclfvk.sHtML

structuredClone(obj)
来源：http://blog.bbcook.cn/Article/details/gzjjqvgxs.sHtML

[U93] JS：模板字符串
来源：http://mobile.bbcook.cn/Article/details/gttrfkwgg.sHtML

`共 ${n} 条`
来源：http://www.share.vehdjk.com/Article/details/gcafeosty.sHtML

[U94] JS：箭头函数
来源：http://read.share.bbcook.cn/Article/details/gsnrvyiso.sHtML

const double = x => x * 2;
来源：http://wap.epnwcf.com/Article/details/gzcmixyjp.sHtML

[U95] JS：Promise 包装
来源：http://www.share.yfazqb.com/Article/details/gntibgtpc.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fktsv.cn/Article/details/gnblknqya.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.vehdjk.com/Article/details/gjtksflxx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.tarul.cn/Article/details/gqxymucmf.sHtML

[U97] JS：并发请求
来源：http://3g.sjlbkw.cn/Article/details/gitubbgjs.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fktsv.cn/Article/details/glrqcpias.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.bbcook.cn/Article/details/gasmsifhj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fktsv.cn/Article/details/gwgcyrjqa.sHtML

[U99] JS：事件监听
来源：http://blog.tarul.cn/Article/details/gknnutsxg.sHtML

el.addEventListener("click", e => {})
来源：http://baike.yfazqb.com/Article/details/gonrrrcat.sHtML

[U100] JS：DOM 查询
来源：http://wap.sjlbkw.cn/Article/details/gqeufpgxv.sHtML

document.querySelector(".item")
来源：http://blog.vehdjk.com/Article/details/giptrvgnh.sHtML

[U101] JS：classList 操作
来源：http://www.share.fktsv.cn/Article/details/ghszyvagr.sHtML

el.classList.toggle("active")
来源：http://baike.vehdjk.com/Article/details/gnhotkeun.sHtML

[U102] JS：本地存储
来源：http://read.share.sjlbkw.cn/Article/details/gigqgciik.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.yfazqb.com/Article/details/gydowizlv.sHtML

[U103] JS：定时器
来源：http://www.blog.epnwcf.com/Article/details/gvseqmyrl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.sjlbkw.cn/Article/details/gisakrkxz.sHtML

[U104] JS：防抖
来源：http://mobile.tarul.cn/Article/details/gbmjxyxfx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.yfazqb.com/Article/details/ghedgstwb.sHtML

[U105] JS：节流
来源：http://read.share.epnwcf.com/Article/details/gpdkauzpw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.sjlbkw.cn/Article/details/gdcixbwaz.sHtML

[U106] JS：日期格式化
来源：http://www.share.sjlbkw.cn/Article/details/gebbhnbqm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.yfazqb.com/Article/details/goemirnyi.sHtML

[U107] JS：数字千分位
来源：http://read.share.tarul.cn/Article/details/goeteninx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.vehdjk.com/Article/details/gfpkmuvom.sHtML

[U108] JS：随机整数
来源：http://m.share.bbcook.cn/Article/details/gougpdtwu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fktsv.cn/Article/details/gyapvmazo.sHtML

[U109] JS：数组分组
来源：http://baike.epnwcf.com/Article/details/gznmebbwy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.tarul.cn/Article/details/gumiketyg.sHtML

[U110] JS：数组分块
来源：http://blog.yfazqb.com/Article/details/gcrxonmei.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fktsv.cn/Article/details/gkkajahvp.sHtML

[U111] JS：对象转 Map
来源：http://blog.fktsv.cn/Article/details/gziobralg.sHtML

new Map(Object.entries(obj))
来源：http://3g.fktsv.cn/Article/details/gkgbvtijd.sHtML

[U112] JS：字符串补位
来源：http://wap.fktsv.cn/Article/details/gznrzsvmj.sHtML

"7".padStart(3, "0")
来源：http://m.share.sjlbkw.cn/Article/details/gvnkdebsg.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.vehdjk.com/Article/details/gccvbmwpb.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.tarul.cn/Article/details/giyhbkxoq.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.epnwcf.com/Article/details/gqxoujpxh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.bbcook.cn/Article/details/gdirrptdt.sHtML

[U115] JS：生成 UUID
来源：http://m.share.tarul.cn/Article/details/gfjptrfgb.sHtML

crypto.randomUUID()
来源：http://www.blog.tarul.cn/Article/details/gzlwynnmh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.sjlbkw.cn/Article/details/grejnigyd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.tarul.cn/Article/details/griuswqbo.sHtML

[U117] JS：单元测试
来源：http://www.blog.yfazqb.com/Article/details/ginetgtbs.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.tarul.cn/Article/details/gzzetkybb.sHtML

[U118] JS：开发服务器
来源：http://wap.vehdjk.com/Article/details/glbqobmfi.sHtML

npm i -D vite;  npx vite
来源：http://baike.bbcook.cn/Article/details/guyrjkska.sHtML

[U119] JS：生产构建
来源：http://read.share.tarul.cn/Article/details/gxmcejqwk.sHtML

npx vite build
来源：http://baike.epnwcf.com/Article/details/gwvnhodht.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.vehdjk.com/Article/details/gltkxysma.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.tarul.cn/Article/details/gzrktbjxn.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/ghobbrobb.sHtML

统计汇总
来源：http://mobile.bbcook.cn/Article/details/gcifugier.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gwrpuibnt.sHtML

按语言统计（条）：
来源：http://baike.fktsv.cn/Article/details/gfizjmlvd.sHtML

Python ......... 252
来源：http://baike.yfazqb.com/Article/details/gtmmtjyym.sHtML

PHP ............ 252
来源：http://baike.epnwcf.com/Article/details/gofzwwjkz.sHtML

JavaScript ..... 252
来源：http://baike.tarul.cn/Article/details/gkuopitqs.sHtML

TypeScript ..... 212
来源：http://www.blog.sjlbkw.cn/Article/details/gqjptuwgf.sHtML

Java ........... 212
来源：http://baike.bbcook.cn/Article/details/gvkgzixdd.sHtML

Go ............. 212
来源：http://www.m.share.sjlbkw.cn/Article/details/gwkesdnaw.sHtML

Ruby ........... 212
来源：http://www.blog.epnwcf.com/Article/details/gplsqmabe.sHtML

C# ............. 212
来源：http://www.share.fktsv.cn/Article/details/gicziutwz.sHtML

C .............. 30
来源：http://www.blog.vehdjk.com/Article/details/gtanarqxp.sHtML

C++ ............ 30
来源：http://read.share.bbcook.cn/Article/details/gbsdwqbpm.sHtML

SQL ............ 90
来源：http://m.share.fktsv.cn/Article/details/grkgoiiau.sHtML

Bash ........... 80
来源：http://m.share.vehdjk.com/Article/details/gqnxhjipm.sHtML

Kotlin ......... 15
来源：http://www.share.vehdjk.com/Article/details/gnbymbwhs.sHtML

Swift .......... 15
来源：http://www.blog.sjlbkw.cn/Article/details/gfrazzfcu.sHtML

Lua ............ 10
来源：http://blog.vehdjk.com/Article/details/gaycckzcm.sHtML

Perl ........... 10
来源：http://www.m.share.yfazqb.com/Article/details/gsbubmbzz.sHtML

Scala .......... 10
来源：http://read.share.sjlbkw.cn/Article/details/glynorhys.sHtML

------------------------------------
来源：http://mobile.vehdjk.com/Article/details/geflkhell.sHtML

合计 ........... 2106 条
来源：http://blog.epnwcf.com/Article/details/gjujbvacq.sHtML

按章节统计：
来源：http://www.m.share.fktsv.cn/Article/details/gbnlquazg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.epnwcf.com/Article/details/gmrkxodvz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.tarul.cn/Article/details/gwfbmxntq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.yfazqb.com/Article/details/ghytqjauj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.tarul.cn/Article/details/gizrsuaec.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.vehdjk.com/Article/details/gfjfgdcyz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.bbcook.cn/Article/details/gaxpjyzyp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.tarul.cn/Article/details/gqpfhbgad.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.epnwcf.com/Article/details/ghpvxkelm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fktsv.cn/Article/details/gxrwbbshh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.tarul.cn/Article/details/gxxncmbdf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.bbcook.cn/Article/details/gxlplgzma.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.epnwcf.com/Article/details/gsbthvugk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.epnwcf.com/Article/details/ggrbdwenz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.tarul.cn/Article/details/gwqwiwnxr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.tarul.cn/Article/details/gubxhqqpv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fktsv.cn/Article/details/gvtwotsrj.sHtML

Q SQL 专题                              90
来源：http://wap.yfazqb.com/Article/details/gkknfekfw.sHtML

R Bash 专题                             80
来源：http://wap.yfazqb.com/Article/details/gvxfmpnwn.sHtML

S C / C++ 专题                          60
来源：http://wap.epnwcf.com/Article/details/glyiviyac.sHtML

T 其他语言补充                          60
来源：http://www.m.share.epnwcf.com/Article/details/gsxqfgxxp.sHtML

U 高频实用片段                         120
来源：http://www.share.sjlbkw.cn/Article/details/gyloqfvva.sHtML

------------------------------------
来源：http://blog.tarul.cn/Article/details/gjihqmtho.sHtML

合计                                  2106 条
来源：http://mobile.yfazqb.com/Article/details/ggdjbmgoh.sHtML

--------------------------------------------------------------------------------
来源：http://wap.bbcook.cn/Article/details/gqtslvtde.sHtML

使用提醒
来源：http://wap.fktsv.cn/Article/details/ghhhswxjv.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.tarul.cn/Article/details/gzuywpdml.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fktsv.cn/Article/details/gtdjplpby.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.yfazqb.com/Article/details/gdjtoppna.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.sjlbkw.cn/Article/details/gswpmnzqt.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.sjlbkw.cn/Article/details/gfyywygid.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.vehdjk.com/Article/details/gzqmghrvs.sHtML

—— 文件结束 ——
来源：http://m.share.vehdjk.com/Article/details/grlrrpbsd.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gxsdbawsc.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.sjlbkw.cn/Article/details/grkrcdwag.sHtML

Common Programming Examples Cheat Book
来源：http://wap.vehdjk.com/Article/details/guwiqyqzl.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gyriwegdq.sHtML

【收录内容】
来源：http://3g.fktsv.cn/Article/details/gibcrdwxx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.bbcook.cn/Article/details/goffswmhy.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.vehdjk.com/Article/details/gbecqemcw.sHtML

SQL · Bash · C · C++
来源：http://www.blog.sjlbkw.cn/Article/details/gmsjokfxh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.epnwcf.com/Article/details/gmxntwrtk.sHtML

【使用说明】
来源：http://blog.epnwcf.com/Article/details/gnrwjauez.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.sjlbkw.cn/Article/details/gtlhbeoyo.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.yfazqb.com/Article/details/gbkduzfam.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.bbcook.cn/Article/details/gxuilafwc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.tarul.cn/Article/details/gbytmnehh.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.vehdjk.com/Article/details/gloqexhad.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.bbcook.cn/Article/details/gwlxjzpiv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.sjlbkw.cn/Article/details/gcwwrxniy.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.vehdjk.com/Article/details/gsmvjpbdr.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.vehdjk.com/Article/details/glmybxphw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.sjlbkw.cn/Article/details/ggkqqloln.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fktsv.cn/Article/details/grhmdoxwe.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.epnwcf.com/Article/details/glygzqwnn.sHtML

【文件统计】
来源：http://blog.vehdjk.com/Article/details/gsrraoblw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.yfazqb.com/Article/details/gwdrjuhta.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.sjlbkw.cn/Article/details/ggmxvewgo.sHtML

目  录
来源：http://m.share.tarul.cn/Article/details/gifoyegwf.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.epnwcf.com/Article/details/gypkhndpw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.sjlbkw.cn/Article/details/gqosymkui.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.tarul.cn/Article/details/ganorxmsc.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.yfazqb.com/Article/details/gwwwvosdy.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.sjlbkw.cn/Article/details/gwjiyqzdv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.vehdjk.com/Article/details/gjsvlvgok.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.sjlbkw.cn/Article/details/grbehfqdu.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.epnwcf.com/Article/details/gfpiprjdn.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fktsv.cn/Article/details/ggnhyxkpd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.yfazqb.com/Article/details/grgceohix.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.tarul.cn/Article/details/gfukucdmr.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.sjlbkw.cn/Article/details/gxufxmzsv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.yfazqb.com/Article/details/gwirxmkor.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.vehdjk.com/Article/details/guifyeyov.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.tarul.cn/Article/details/gcxrcxlhi.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.epnwcf.com/Article/details/gmrchoclt.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.yfazqb.com/Article/details/ghvkayxrp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.tarul.cn/Article/details/gaftssqha.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.epnwcf.com/Article/details/gwmhnfcue.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.tarul.cn/Article/details/grpkgqojf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.bbcook.cn/Article/details/gabqsyrxc.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.sjlbkw.cn/Article/details/grmtsjtlt.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gpocfqkny.sHtML

A. 基础语法与类型
来源：http://www.m.share.bbcook.cn/Article/details/gwicbdmiz.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gnsvtmrug.sHtML

[A01] Hello World
来源：http://wap.fktsv.cn/Article/details/gcxqsngar.sHtML

Py:   print("Hello, World!")
来源：http://blog.yfazqb.com/Article/details/gfetrznhv.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.epnwcf.com/Article/details/gczbtidzd.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.vehdjk.com/Article/details/guugaakab.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.sjlbkw.cn/Article/details/gidvnwbtz.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.tarul.cn/Article/details/gkdmdlxms.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.fktsv.cn/Article/details/gdzscgcht.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.sjlbkw.cn/Article/details/gomzlvazf.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.vehdjk.com/Article/details/gnqginkiv.sHtML

[A02] 变量声明与赋值
来源：http://wap.vehdjk.com/Article/details/gicnqkxlb.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.sjlbkw.cn/Article/details/ghinijflj.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.yfazqb.com/Article/details/gcdvlcvhf.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.bbcook.cn/Article/details/gzsjrxfwb.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.fktsv.cn/Article/details/gxjohnyan.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.bbcook.cn/Article/details/gfmdjoxyz.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.fktsv.cn/Article/details/gxpqxhxyg.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.tarul.cn/Article/details/gdvqjihgk.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.fktsv.cn/Article/details/gzfcegzzh.sHtML

[A03] 常量定义
来源：http://blog.tarul.cn/Article/details/gsbqrhvmo.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.vehdjk.com/Article/details/gqialupvq.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.bbcook.cn/Article/details/guklzwxdf.sHtML

JS:   const PI = 3.14159;
来源：http://blog.yfazqb.com/Article/details/glznqatgt.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.yfazqb.com/Article/details/gutntcnbp.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.fktsv.cn/Article/details/geibqgayj.sHtML

Go:   const PI = 3.14159
来源：http://3g.bbcook.cn/Article/details/gwwjnmhtv.sHtML

Ruby: PI = 3.14159
来源：http://read.share.yfazqb.com/Article/details/gfclnuutm.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.vehdjk.com/Article/details/gnvppgtcr.sHtML

[A04] 判断变量类型
来源：http://m.share.bbcook.cn/Article/details/gpjmcopdq.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.vehdjk.com/Article/details/gvizjztcd.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.sjlbkw.cn/Article/details/gokeoojpc.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.tarul.cn/Article/details/ggifrvzit.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.sjlbkw.cn/Article/details/gxaeefvaq.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.vehdjk.com/Article/details/gtudtyoyi.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.sjlbkw.cn/Article/details/gbthinfvs.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.epnwcf.com/Article/details/gkfnvskcr.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.vehdjk.com/Article/details/gvobirokx.sHtML

[A05] 整数除法与取模
来源：http://blog.bbcook.cn/Article/details/giseppmgt.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.epnwcf.com/Article/details/ggxryqocu.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.sjlbkw.cn/Article/details/gbtcnbsdj.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.sjlbkw.cn/Article/details/gzypmchcx.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.bbcook.cn/Article/details/grozeryyq.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.yfazqb.com/Article/details/gcplwiugg.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.vehdjk.com/Article/details/gbbckyffu.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.bbcook.cn/Article/details/gdnzbfzze.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.sjlbkw.cn/Article/details/gquqtkmiz.sHtML

[A06] 字符串转数字
来源：http://www.blog.sjlbkw.cn/Article/details/ghcngagmm.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.yfazqb.com/Article/details/gzdztuxbs.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.vehdjk.com/Article/details/gglfsrich.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.epnwcf.com/Article/details/gpbefiext.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.epnwcf.com/Article/details/gkjjoqhql.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.bbcook.cn/Article/details/gthwjsetn.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.bbcook.cn/Article/details/gnopjirmt.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.bbcook.cn/Article/details/gtneipovw.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.yfazqb.com/Article/details/gofmyvgda.sHtML

[A07] 数字转字符串
来源：http://mobile.vehdjk.com/Article/details/gjtpndbbf.sHtML

Py:   str(42)
来源：http://read.share.sjlbkw.cn/Article/details/gpfveyvci.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.yfazqb.com/Article/details/gaqsvzitq.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.fktsv.cn/Article/details/gtnaevibn.sHtML

TS:   String(42)
来源：http://www.blog.tarul.cn/Article/details/glklkldlz.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.tarul.cn/Article/details/glsbgdhmm.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.fktsv.cn/Article/details/gbmqgonck.sHtML

Ruby: 42.to_s
来源：http://mobile.fktsv.cn/Article/details/glgqszwqh.sHtML

C#:   42.ToString()
来源：http://mobile.bbcook.cn/Article/details/gkdsuwjrp.sHtML

[A08] 取整与四舍五入
来源：http://3g.sjlbkw.cn/Article/details/gmyrrujns.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.epnwcf.com/Article/details/gdvfiaezk.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.fktsv.cn/Article/details/gxuyxwwvg.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnbdlmryu.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.bbcook.cn/Article/details/ghjkhzxij.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.yfazqb.com/Article/details/gunrxyvpy.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.fktsv.cn/Article/details/gqnmjwjyy.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.yfazqb.com/Article/details/gkgpyhelj.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.tarul.cn/Article/details/gcaadubyh.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.sjlbkw.cn/Article/details/gzvoamcrd.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.vehdjk.com/Article/details/gyerrdyih.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.bbcook.cn/Article/details/gtkvelvib.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.tarul.cn/Article/details/gofslpfjq.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.tarul.cn/Article/details/gxoqigbrx.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gpgdpspmb.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.vehdjk.com/Article/details/gywvyfoiu.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.yfazqb.com/Article/details/gzixbhmac.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.bbcook.cn/Article/details/gpmiplctg.sHtML


<!-- 参考信息 -->