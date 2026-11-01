代发 wailian999

[U65] PHP：会话
来源：http://baike.sjlbkw.cn/Article/details/gvshxxspi.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.sjlbkw.cn/Article/details/gnyltefbc.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.vehdjk.com/Article/details/gytvvxfcd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.bbcook.cn/Article/details/gknaobued.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.sjlbkw.cn/Article/details/gatuwahdr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.epnwcf.com/Article/details/gpcvibxsq.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.vehdjk.com/Article/details/gurytxfun.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.tarul.cn/Article/details/gjxyvbhuq.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.bbcook.cn/Article/details/gvttfnfcm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.sjlbkw.cn/Article/details/gwnwydske.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.yfazqb.com/Article/details/gjaplzsfg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.yfazqb.com/Article/details/gcrtfjpyb.sHtML

[U71] PHP：抛出异常
来源：http://blog.vehdjk.com/Article/details/gactzfbds.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.vehdjk.com/Article/details/gywzgrdyz.sHtML

[U72] PHP：写错误日志
来源：http://m.share.bbcook.cn/Article/details/gqsrtjmwf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.bbcook.cn/Article/details/greakpxij.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.vehdjk.com/Article/details/gkqeryedd.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.sjlbkw.cn/Article/details/grdbkmkry.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.tarul.cn/Article/details/gyqznrvll.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.bbcook.cn/Article/details/gqvgibdhx.sHtML

[U75] PHP：依赖注入
来源：http://blog.bbcook.cn/Article/details/gikmkyong.sHtML

composer require psr/container
来源：http://mobile.vehdjk.com/Article/details/gtevqinqz.sHtML

[U76] PHP：简单路由
来源：http://mobile.yfazqb.com/Article/details/gcfajlhyn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.sjlbkw.cn/Article/details/gacnknxfv.sHtML

[U77] PHP：模板渲染
来源：http://mobile.bbcook.cn/Article/details/gsiocqmnp.sHtML

composer require twig/twig
来源：http://baike.tarul.cn/Article/details/gihapvnzs.sHtML

[U78] PHP：单元测试
来源：http://3g.yfazqb.com/Article/details/gvtbajeef.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.vehdjk.com/Article/details/gthzyylzy.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.sjlbkw.cn/Article/details/gkocdahcb.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.tarul.cn/Article/details/gvjienmft.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fktsv.cn/Article/details/gtgrivptt.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.epnwcf.com/Article/details/ggsvbabbu.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.tarul.cn/Article/details/gduczhjra.sHtML

npm init -y;  npm i express
来源：http://blog.fktsv.cn/Article/details/goukjimlq.sHtML

[U82] JS：package.json 脚本
来源：http://wap.bbcook.cn/Article/details/gazmoiani.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.bbcook.cn/Article/details/gzbpqhkdb.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.yfazqb.com/Article/details/grckldgel.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.sjlbkw.cn/Article/details/gghyistus.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.bbcook.cn/Article/details/gfqvbqvlo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.tarul.cn/Article/details/gqaxdifac.sHtML

[U85] JS：可选链
来源：http://m.share.sjlbkw.cn/Article/details/gcjotaaot.sHtML

a?.b?.c
来源：http://blog.yfazqb.com/Article/details/gaztbnbzf.sHtML

[U86] JS：空值合并
来源：http://baike.vehdjk.com/Article/details/gjedugptc.sHtML

a ?? b
来源：http://mobile.bbcook.cn/Article/details/gucnuhoza.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.tarul.cn/Article/details/ggcnrbcdf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fktsv.cn/Article/details/gtkphmecz.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.epnwcf.com/Article/details/gwcwuhhaf.sHtML

{ ...a, ...b }
来源：http://blog.epnwcf.com/Article/details/gowmmgjvx.sHtML

[U89] JS：数组去重
来源：http://baike.tarul.cn/Article/details/gvjcbccpe.sHtML

[...new Set(arr)]
来源：http://3g.tarul.cn/Article/details/glvyogswa.sHtML

[U90] JS：数字数组排序
来源：http://mobile.yfazqb.com/Article/details/gcuwvmjzm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.yfazqb.com/Article/details/ggqmjpldp.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.vehdjk.com/Article/details/gosayysms.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.vehdjk.com/Article/details/goasmpbge.sHtML

[U92] JS：深拷贝
来源：http://baike.epnwcf.com/Article/details/guxlcyjap.sHtML

structuredClone(obj)
来源：http://read.share.yfazqb.com/Article/details/ggzqnuaqr.sHtML

[U93] JS：模板字符串
来源：http://www.blog.vehdjk.com/Article/details/gmscbktal.sHtML

`共 ${n} 条`
来源：http://www.m.share.yfazqb.com/Article/details/gmpmtadcz.sHtML

[U94] JS：箭头函数
来源：http://mobile.sjlbkw.cn/Article/details/guclxwqqd.sHtML

const double = x => x * 2;
来源：http://www.blog.vehdjk.com/Article/details/gwmajufwd.sHtML

[U95] JS：Promise 包装
来源：http://3g.vehdjk.com/Article/details/gqidyskrq.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.vehdjk.com/Article/details/gwadbolqu.sHtML

[U96] JS：async/await 与异常
来源：http://blog.yfazqb.com/Article/details/gllordshc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.epnwcf.com/Article/details/gtwuzmuwp.sHtML

[U97] JS：并发请求
来源：http://3g.fktsv.cn/Article/details/gmbbokhvy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fktsv.cn/Article/details/gutyqqiya.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.yfazqb.com/Article/details/gfjpvxpto.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.epnwcf.com/Article/details/gozpfmozc.sHtML

[U99] JS：事件监听
来源：http://mobile.epnwcf.com/Article/details/gfjbhrrlg.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.tarul.cn/Article/details/gatevldim.sHtML

[U100] JS：DOM 查询
来源：http://baike.fktsv.cn/Article/details/gsazcgyrs.sHtML

document.querySelector(".item")
来源：http://wap.epnwcf.com/Article/details/gcvphvuhr.sHtML

[U101] JS：classList 操作
来源：http://www.blog.vehdjk.com/Article/details/glralwdci.sHtML

el.classList.toggle("active")
来源：http://read.share.epnwcf.com/Article/details/ggfcvedph.sHtML

[U102] JS：本地存储
来源：http://3g.tarul.cn/Article/details/gdaemycsz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.bbcook.cn/Article/details/gfxxdmbmg.sHtML

[U103] JS：定时器
来源：http://baike.tarul.cn/Article/details/gcxhnazvn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.epnwcf.com/Article/details/gswgalyax.sHtML

[U104] JS：防抖
来源：http://www.blog.vehdjk.com/Article/details/grjyxmopu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.vehdjk.com/Article/details/gbfojcfsg.sHtML

[U105] JS：节流
来源：http://read.share.epnwcf.com/Article/details/gtnjmogac.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.bbcook.cn/Article/details/gpybxwidh.sHtML

[U106] JS：日期格式化
来源：http://read.share.tarul.cn/Article/details/gqxebuhff.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.epnwcf.com/Article/details/gkicatxms.sHtML

[U107] JS：数字千分位
来源：http://www.blog.bbcook.cn/Article/details/grwkttuly.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.yfazqb.com/Article/details/gscijsnun.sHtML

[U108] JS：随机整数
来源：http://www.m.share.epnwcf.com/Article/details/gfwiikzov.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.bbcook.cn/Article/details/gayraypsc.sHtML

[U109] JS：数组分组
来源：http://m.share.sjlbkw.cn/Article/details/gotrbwcnn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.epnwcf.com/Article/details/gyzcoxkgy.sHtML

[U110] JS：数组分块
来源：http://3g.fktsv.cn/Article/details/gzyqdcrdf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fktsv.cn/Article/details/gabhshvfm.sHtML

[U111] JS：对象转 Map
来源：http://wap.vehdjk.com/Article/details/gvxblrzkz.sHtML

new Map(Object.entries(obj))
来源：http://read.share.epnwcf.com/Article/details/glbgsjnga.sHtML

[U112] JS：字符串补位
来源：http://wap.tarul.cn/Article/details/gjolppgwq.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.yfazqb.com/Article/details/gummkrzoa.sHtML

[U113] JS：正则替换全部
来源：http://wap.epnwcf.com/Article/details/gkcentspy.sHtML

s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gtsvgvvzq.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.yfazqb.com/Article/details/gnzsudfuw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.epnwcf.com/Article/details/gnsgsxbui.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.vehdjk.com/Article/details/gpsqkxtrc.sHtML

crypto.randomUUID()
来源：http://baike.sjlbkw.cn/Article/details/gsvnpmxdx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.epnwcf.com/Article/details/gorwiiabq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.yfazqb.com/Article/details/gnumtryil.sHtML

[U117] JS：单元测试
来源：http://read.share.fktsv.cn/Article/details/gfxqulzld.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.yfazqb.com/Article/details/ghrhhxtcx.sHtML

[U118] JS：开发服务器
来源：http://baike.fktsv.cn/Article/details/ghnkamdta.sHtML

npm i -D vite;  npx vite
来源：http://baike.fktsv.cn/Article/details/gfdrpetep.sHtML

[U119] JS：生产构建
来源：http://read.share.fktsv.cn/Article/details/gfwwqznbl.sHtML

npx vite build
来源：http://baike.sjlbkw.cn/Article/details/gowvzjqnx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.tarul.cn/Article/details/gxucahlrf.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fktsv.cn/Article/details/gbyuoysdh.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gtufkpoap.sHtML

统计汇总
来源：http://www.blog.yfazqb.com/Article/details/giwadgngw.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gwnzexdlg.sHtML

按语言统计（条）：
来源：http://3g.sjlbkw.cn/Article/details/gtayujqgs.sHtML

Python ......... 252
来源：http://baike.bbcook.cn/Article/details/gpgkcjiko.sHtML

PHP ............ 252
来源：http://mobile.fktsv.cn/Article/details/gvwsdwbku.sHtML

JavaScript ..... 252
来源：http://www.m.share.tarul.cn/Article/details/gpsmuitkd.sHtML

TypeScript ..... 212
来源：http://m.share.vehdjk.com/Article/details/glaofmesi.sHtML

Java ........... 212
来源：http://3g.fktsv.cn/Article/details/gfesvtvjy.sHtML

Go ............. 212
来源：http://wap.fktsv.cn/Article/details/gkiuqmwyw.sHtML

Ruby ........... 212
来源：http://wap.fktsv.cn/Article/details/gjhbpwjkk.sHtML

C# ............. 212
来源：http://www.share.epnwcf.com/Article/details/gjdkxhsgo.sHtML

C .............. 30
来源：http://read.share.epnwcf.com/Article/details/gdlniacaf.sHtML

C++ ............ 30
来源：http://read.share.yfazqb.com/Article/details/gpyiohdbb.sHtML

SQL ............ 90
来源：http://3g.epnwcf.com/Article/details/grvrozqff.sHtML

Bash ........... 80
来源：http://wap.sjlbkw.cn/Article/details/gtcmwgqqs.sHtML

Kotlin ......... 15
来源：http://blog.yfazqb.com/Article/details/gtozfsrvv.sHtML

Swift .......... 15
来源：http://www.m.share.sjlbkw.cn/Article/details/gcowjvdoa.sHtML

Lua ............ 10
来源：http://wap.fktsv.cn/Article/details/gnewfxpwi.sHtML

Perl ........... 10
来源：http://www.m.share.bbcook.cn/Article/details/giidsaqhq.sHtML

Scala .......... 10
来源：http://baike.vehdjk.com/Article/details/ggexnqdva.sHtML

------------------------------------
来源：http://baike.epnwcf.com/Article/details/gpxdrmmpr.sHtML

合计 ........... 2106 条
来源：http://wap.sjlbkw.cn/Article/details/gwsjyliod.sHtML

按章节统计：
来源：http://3g.sjlbkw.cn/Article/details/gjsshzkgv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.vehdjk.com/Article/details/gekysaucq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.sjlbkw.cn/Article/details/gaavngfij.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.yfazqb.com/Article/details/gxfovxngi.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.sjlbkw.cn/Article/details/gxjgvgtyd.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.yfazqb.com/Article/details/gibnzzkji.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.epnwcf.com/Article/details/gajswqsnf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fktsv.cn/Article/details/grgskjtqd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.vehdjk.com/Article/details/gqcuudsjn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.yfazqb.com/Article/details/gaqxrjisw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.tarul.cn/Article/details/gvamzkhas.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.vehdjk.com/Article/details/gnbgnrxxm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.vehdjk.com/Article/details/gqudgwvvm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.bbcook.cn/Article/details/gjtkjzgxj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.tarul.cn/Article/details/gstrppdza.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.epnwcf.com/Article/details/gtsanxcfm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.yfazqb.com/Article/details/gttqpiyzg.sHtML

Q SQL 专题                              90
来源：http://3g.bbcook.cn/Article/details/grophtjtj.sHtML

R Bash 专题                             80
来源：http://3g.yfazqb.com/Article/details/guamyksft.sHtML

S C / C++ 专题                          60
来源：http://3g.sjlbkw.cn/Article/details/gywdjfivh.sHtML

T 其他语言补充                          60
来源：http://m.share.tarul.cn/Article/details/gngzjclaq.sHtML

U 高频实用片段                         120
来源：http://mobile.sjlbkw.cn/Article/details/grtxasnuh.sHtML

------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/ganuurusd.sHtML

合计                                  2106 条
来源：http://www.m.share.fktsv.cn/Article/details/gwetasqhs.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.sjlbkw.cn/Article/details/gfhtspkmz.sHtML

使用提醒
来源：http://m.share.yfazqb.com/Article/details/gwxvymzpq.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fktsv.cn/Article/details/gguydqvej.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.vehdjk.com/Article/details/gqqwbtqvb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.vehdjk.com/Article/details/gdvdbglgd.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.vehdjk.com/Article/details/gxphzczus.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.tarul.cn/Article/details/gxsfixfvq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.epnwcf.com/Article/details/grcwhiysl.sHtML

—— 文件结束 ——
来源：http://m.share.sjlbkw.cn/Article/details/glkucepvh.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gcrheuwqh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.yfazqb.com/Article/details/gzmrdhbda.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.epnwcf.com/Article/details/gzzbwitxd.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gajowsolf.sHtML

【收录内容】
来源：http://www.blog.vehdjk.com/Article/details/gpwyjnvfk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.yfazqb.com/Article/details/gfaihtwfk.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.tarul.cn/Article/details/gfbsmhrqc.sHtML

SQL · Bash · C · C++
来源：http://3g.yfazqb.com/Article/details/gfrblhxbh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.sjlbkw.cn/Article/details/gvkyjgppi.sHtML

【使用说明】
来源：http://3g.bbcook.cn/Article/details/gaorjwwhy.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.bbcook.cn/Article/details/gkqxtjiri.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.yfazqb.com/Article/details/gikklntgb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fktsv.cn/Article/details/gofdtrpry.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.bbcook.cn/Article/details/gdjeiszji.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.bbcook.cn/Article/details/gdkvvbvyb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.tarul.cn/Article/details/ggmgwpptr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.epnwcf.com/Article/details/gzfuxxumf.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.bbcook.cn/Article/details/gcktjzrvi.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.sjlbkw.cn/Article/details/gwvdqevuz.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.yfazqb.com/Article/details/gtldeaddf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.vehdjk.com/Article/details/gmenhdvdk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.sjlbkw.cn/Article/details/gemiqojmf.sHtML

【文件统计】
来源：http://read.share.bbcook.cn/Article/details/gnsnagkla.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.vehdjk.com/Article/details/gruuzhpta.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.vehdjk.com/Article/details/gddyergzz.sHtML

目  录
来源：http://www.m.share.epnwcf.com/Article/details/gadbtupfc.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.bbcook.cn/Article/details/ghpwuhqoa.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.epnwcf.com/Article/details/gsectgnhc.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.epnwcf.com/Article/details/gxqdytpjc.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.tarul.cn/Article/details/gncxugmvz.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.vehdjk.com/Article/details/gipbwtpzt.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.vehdjk.com/Article/details/grstyiykb.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.vehdjk.com/Article/details/gpusbwdxg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.yfazqb.com/Article/details/gskudldaj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.sjlbkw.cn/Article/details/gxbexofru.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.fktsv.cn/Article/details/gigopdavx.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.vehdjk.com/Article/details/gywebovpz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.yfazqb.com/Article/details/gckaslgep.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.tarul.cn/Article/details/gkxqqwtqq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.bbcook.cn/Article/details/gnwyvztvb.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.vehdjk.com/Article/details/geirxzedl.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.epnwcf.com/Article/details/gmseuakde.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.sjlbkw.cn/Article/details/gvnvdhiov.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.bbcook.cn/Article/details/gybustmhi.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.bbcook.cn/Article/details/gtkmqymun.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.bbcook.cn/Article/details/gvcibppso.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.vehdjk.com/Article/details/gysjhjcti.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fktsv.cn/Article/details/gzhzkzbdb.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gvviokqhl.sHtML

A. 基础语法与类型
来源：http://www.blog.fktsv.cn/Article/details/gmpbawmtg.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gisrukgfz.sHtML

[A01] Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gkkwelgyy.sHtML

Py:   print("Hello, World!")
来源：http://blog.bbcook.cn/Article/details/ghjghdbwp.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.fktsv.cn/Article/details/guzmmrkcw.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.vehdjk.com/Article/details/gxxwkfpis.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.tarul.cn/Article/details/ggejhhkih.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.vehdjk.com/Article/details/gqbvdabzl.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.tarul.cn/Article/details/guquyqdeo.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.sjlbkw.cn/Article/details/gwkakhstp.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.bbcook.cn/Article/details/gwziowbnz.sHtML

[A02] 变量声明与赋值
来源：http://3g.fktsv.cn/Article/details/gznrawioq.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.tarul.cn/Article/details/gdebsilwc.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.epnwcf.com/Article/details/gsswujyyn.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.epnwcf.com/Article/details/gjrwgvlnf.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.epnwcf.com/Article/details/gmbrfczup.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fktsv.cn/Article/details/gqauetvuy.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.tarul.cn/Article/details/geblurgdd.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.tarul.cn/Article/details/gzxfksdjl.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.bbcook.cn/Article/details/gxggdgznn.sHtML

[A03] 常量定义
来源：http://mobile.fktsv.cn/Article/details/gtwgkfwim.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.epnwcf.com/Article/details/gynadlydq.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/gozcduwhy.sHtML

JS:   const PI = 3.14159;
来源：http://blog.bbcook.cn/Article/details/ghfzpbjxg.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.bbcook.cn/Article/details/gxeyafivl.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/gkvkpjjgg.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.fktsv.cn/Article/details/gmiecvzpa.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.yfazqb.com/Article/details/gnqmlfeih.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.fktsv.cn/Article/details/gffjxufom.sHtML

[A04] 判断变量类型
来源：http://www.blog.fktsv.cn/Article/details/gpucidqfu.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.fktsv.cn/Article/details/gcqqktgrh.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.sjlbkw.cn/Article/details/gdqeslcxx.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.bbcook.cn/Article/details/gbppjkffv.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.sjlbkw.cn/Article/details/gnouuzwbr.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.bbcook.cn/Article/details/gfxetjyss.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.bbcook.cn/Article/details/giikuubrr.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.epnwcf.com/Article/details/gdsqfnqnp.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.yfazqb.com/Article/details/gstejspwv.sHtML

[A05] 整数除法与取模
来源：http://www.blog.bbcook.cn/Article/details/geqjjpkvv.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.tarul.cn/Article/details/gzeifcxvh.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.fktsv.cn/Article/details/gtyomssil.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.yfazqb.com/Article/details/goytxyigl.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.tarul.cn/Article/details/gqsnabyqx.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.epnwcf.com/Article/details/gunxtkizp.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.fktsv.cn/Article/details/gleymfzbx.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.sjlbkw.cn/Article/details/gbtszbmkn.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.bbcook.cn/Article/details/ghvfmtczd.sHtML

[A06] 字符串转数字
来源：http://read.share.yfazqb.com/Article/details/gziwwxnlm.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.fktsv.cn/Article/details/gbzidwcjy.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.bbcook.cn/Article/details/gkoelohbn.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.bbcook.cn/Article/details/gbbkbymkx.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.epnwcf.com/Article/details/ghsfabdfk.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.bbcook.cn/Article/details/gshcnkzcn.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.yfazqb.com/Article/details/gktgddtig.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.bbcook.cn/Article/details/gmscyrykj.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.epnwcf.com/Article/details/gzrdhwbla.sHtML

[A07] 数字转字符串
来源：http://m.share.bbcook.cn/Article/details/gxrbukboq.sHtML

Py:   str(42)
来源：http://www.blog.epnwcf.com/Article/details/gpidycjfg.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.fktsv.cn/Article/details/gorgvjpbk.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.vehdjk.com/Article/details/glouwwxvz.sHtML

TS:   String(42)
来源：http://m.share.vehdjk.com/Article/details/geukvykwq.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.yfazqb.com/Article/details/gdjairarm.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.vehdjk.com/Article/details/gznlqcyfw.sHtML

Ruby: 42.to_s
来源：http://blog.epnwcf.com/Article/details/gefebxjav.sHtML

C#:   42.ToString()
来源：http://mobile.yfazqb.com/Article/details/gmhrhjntv.sHtML

[A08] 取整与四舍五入
来源：http://baike.epnwcf.com/Article/details/guopykqrm.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.tarul.cn/Article/details/gvyerhlhp.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.bbcook.cn/Article/details/grvigzhdc.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.vehdjk.com/Article/details/gkfqhfhca.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.bbcook.cn/Article/details/graygqnxr.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.tarul.cn/Article/details/glazabllt.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.fktsv.cn/Article/details/gmjfuczah.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.sjlbkw.cn/Article/details/gptholzkn.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.sjlbkw.cn/Article/details/gtspkndns.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.tarul.cn/Article/details/guolfyizr.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.yfazqb.com/Article/details/gfqbqkmmg.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.tarul.cn/Article/details/gxxlmbefw.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.yfazqb.com/Article/details/ggduhntes.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fktsv.cn/Article/details/gcghheaeb.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.epnwcf.com/Article/details/ghbzcrdos.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.yfazqb.com/Article/details/gvsvwfmcj.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.bbcook.cn/Article/details/gdxnlleaz.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.sjlbkw.cn/Article/details/glxggzsvc.sHtML


<!-- 参考信息 -->