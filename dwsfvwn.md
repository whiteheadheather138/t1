代发 wailian999

[U65] PHP：会话
来源：http://www.share.vehdjk.com/Article/details/gpxyvldxx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/gkztulvox.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.bbcook.cn/Article/details/gqhbonpkn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fktsv.cn/Article/details/gbpldtwwj.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.vehdjk.com/Article/details/gzblcgqzt.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.sjlbkw.cn/Article/details/grxqtxrcv.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.bbcook.cn/Article/details/gdmjrjxyv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fktsv.cn/Article/details/gwevqqayq.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.yfazqb.com/Article/details/geobnygcz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.tarul.cn/Article/details/gggqmcehj.sHtML

[U70] PHP：PDO 事务
来源：http://baike.epnwcf.com/Article/details/gaaxudiss.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fktsv.cn/Article/details/gkmketcim.sHtML

[U71] PHP：抛出异常
来源：http://baike.sjlbkw.cn/Article/details/gcoblbexo.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.yfazqb.com/Article/details/gkyxniyod.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.sjlbkw.cn/Article/details/gxfsdmpck.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.bbcook.cn/Article/details/glldwduwp.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.vehdjk.com/Article/details/gxmshpkxp.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.bbcook.cn/Article/details/gmonswsls.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.sjlbkw.cn/Article/details/gafaazvpp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.yfazqb.com/Article/details/gjnvulixi.sHtML

[U75] PHP：依赖注入
来源：http://m.share.yfazqb.com/Article/details/gtllxhasw.sHtML

composer require psr/container
来源：http://www.m.share.tarul.cn/Article/details/gegkojipg.sHtML

[U76] PHP：简单路由
来源：http://read.share.vehdjk.com/Article/details/gpfbzprdf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.bbcook.cn/Article/details/ghronkqno.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.bbcook.cn/Article/details/goabyyafy.sHtML

composer require twig/twig
来源：http://blog.sjlbkw.cn/Article/details/ggfkqvmsz.sHtML

[U78] PHP：单元测试
来源：http://blog.sjlbkw.cn/Article/details/glhhsvrul.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.bbcook.cn/Article/details/guyddxsyu.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.tarul.cn/Article/details/gmjnnualo.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.tarul.cn/Article/details/goqycehsb.sHtML

[U80] PHP：代码规范修复
来源：http://3g.epnwcf.com/Article/details/gnksmsyza.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.tarul.cn/Article/details/gwekvplbl.sHtML

[U81] JS：初始化项目
来源：http://www.share.yfazqb.com/Article/details/gmocamoju.sHtML

npm init -y;  npm i express
来源：http://wap.bbcook.cn/Article/details/gihathegj.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.sjlbkw.cn/Article/details/gmduvxnvc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.vehdjk.com/Article/details/gptbjukqx.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.tarul.cn/Article/details/gwgajiahi.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.epnwcf.com/Article/details/gqpovjzid.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.vehdjk.com/Article/details/gptcjgbhp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.tarul.cn/Article/details/givxwnpsl.sHtML

[U85] JS：可选链
来源：http://baike.bbcook.cn/Article/details/ghtwofrim.sHtML

a?.b?.c
来源：http://wap.epnwcf.com/Article/details/gtbazesfc.sHtML

[U86] JS：空值合并
来源：http://www.share.fktsv.cn/Article/details/gofebgrbf.sHtML

a ?? b
来源：http://mobile.sjlbkw.cn/Article/details/golvdrgjk.sHtML

[U87] JS：解构默认值
来源：http://baike.sjlbkw.cn/Article/details/geldfjdsx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fktsv.cn/Article/details/gjxsnaing.sHtML

[U88] JS：对象展开合并
来源：http://www.share.vehdjk.com/Article/details/ggmhvlbov.sHtML

{ ...a, ...b }
来源：http://mobile.tarul.cn/Article/details/gbhmvtqip.sHtML

[U89] JS：数组去重
来源：http://www.m.share.tarul.cn/Article/details/gqhipqonk.sHtML

[...new Set(arr)]
来源：http://blog.epnwcf.com/Article/details/gasepibke.sHtML

[U90] JS：数字数组排序
来源：http://baike.tarul.cn/Article/details/gypbfzzyl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.tarul.cn/Article/details/ghweadtei.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fktsv.cn/Article/details/gdpztftiq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.bbcook.cn/Article/details/gmlelqwyv.sHtML

[U92] JS：深拷贝
来源：http://www.share.fktsv.cn/Article/details/gcrtqlsgt.sHtML

structuredClone(obj)
来源：http://m.share.epnwcf.com/Article/details/grdvftusz.sHtML

[U93] JS：模板字符串
来源：http://m.share.sjlbkw.cn/Article/details/gilcphvwg.sHtML

`共 ${n} 条`
来源：http://baike.vehdjk.com/Article/details/grgkxcwik.sHtML

[U94] JS：箭头函数
来源：http://3g.epnwcf.com/Article/details/glpcwmvcr.sHtML

const double = x => x * 2;
来源：http://baike.vehdjk.com/Article/details/ghwgmpbio.sHtML

[U95] JS：Promise 包装
来源：http://m.share.vehdjk.com/Article/details/gwywrxwxb.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fktsv.cn/Article/details/gjfxndutx.sHtML

[U96] JS：async/await 与异常
来源：http://blog.yfazqb.com/Article/details/gusfmnxfd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.vehdjk.com/Article/details/gjjtlfbzd.sHtML

[U97] JS：并发请求
来源：http://www.share.sjlbkw.cn/Article/details/gcpqhahpz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gltdhgivv.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.sjlbkw.cn/Article/details/girmuouub.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.sjlbkw.cn/Article/details/gvcgxvekh.sHtML

[U99] JS：事件监听
来源：http://read.share.bbcook.cn/Article/details/gbshostnt.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.sjlbkw.cn/Article/details/gzhixmkrj.sHtML

[U100] JS：DOM 查询
来源：http://mobile.sjlbkw.cn/Article/details/gbkhytkdl.sHtML

document.querySelector(".item")
来源：http://www.blog.bbcook.cn/Article/details/gbrgqqesy.sHtML

[U101] JS：classList 操作
来源：http://www.blog.epnwcf.com/Article/details/ggwfnkerj.sHtML

el.classList.toggle("active")
来源：http://www.share.yfazqb.com/Article/details/geittfopq.sHtML

[U102] JS：本地存储
来源：http://3g.vehdjk.com/Article/details/gujlykpxt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.tarul.cn/Article/details/grdyemfge.sHtML

[U103] JS：定时器
来源：http://m.share.sjlbkw.cn/Article/details/gonznwtnh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.yfazqb.com/Article/details/gulwygshu.sHtML

[U104] JS：防抖
来源：http://wap.epnwcf.com/Article/details/gemnhtbeb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.epnwcf.com/Article/details/gcjxzwahu.sHtML

[U105] JS：节流
来源：http://mobile.fktsv.cn/Article/details/gmkwacoan.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fktsv.cn/Article/details/gmvnmqman.sHtML

[U106] JS：日期格式化
来源：http://wap.fktsv.cn/Article/details/guyofivrm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.bbcook.cn/Article/details/gmpexbrsw.sHtML

[U107] JS：数字千分位
来源：http://mobile.sjlbkw.cn/Article/details/gadjeqjgg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.sjlbkw.cn/Article/details/gyoqfmrim.sHtML

[U108] JS：随机整数
来源：http://www.blog.yfazqb.com/Article/details/gicvlbnxy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.sjlbkw.cn/Article/details/gdtyvmcdp.sHtML

[U109] JS：数组分组
来源：http://wap.fktsv.cn/Article/details/gifxejsig.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.bbcook.cn/Article/details/glxtvcokb.sHtML

[U110] JS：数组分块
来源：http://wap.vehdjk.com/Article/details/gcaqjusif.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.yfazqb.com/Article/details/gprtykkev.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.yfazqb.com/Article/details/gomyqocae.sHtML

new Map(Object.entries(obj))
来源：http://blog.epnwcf.com/Article/details/gcrnyayzh.sHtML

[U112] JS：字符串补位
来源：http://www.blog.tarul.cn/Article/details/gbiukisww.sHtML

"7".padStart(3, "0")
来源：http://www.blog.vehdjk.com/Article/details/gicartzfb.sHtML

[U113] JS：正则替换全部
来源：http://blog.vehdjk.com/Article/details/gqujuzgfj.sHtML

s.replaceAll("a", "b")
来源：http://wap.tarul.cn/Article/details/gwlrgeydr.sHtML

[U114] JS：JSON 深比较
来源：http://baike.yfazqb.com/Article/details/gakqllaem.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fktsv.cn/Article/details/ggvhznhtj.sHtML

[U115] JS：生成 UUID
来源：http://3g.yfazqb.com/Article/details/grssgooep.sHtML

crypto.randomUUID()
来源：http://www.m.share.sjlbkw.cn/Article/details/gantjdqmm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fktsv.cn/Article/details/gedszyzgj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.bbcook.cn/Article/details/goczguyrj.sHtML

[U117] JS：单元测试
来源：http://wap.vehdjk.com/Article/details/gkjevutnl.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fktsv.cn/Article/details/gkobdobwh.sHtML

[U118] JS：开发服务器
来源：http://mobile.bbcook.cn/Article/details/ghycixyzs.sHtML

npm i -D vite;  npx vite
来源：http://wap.tarul.cn/Article/details/gnbqeptam.sHtML

[U119] JS：生产构建
来源：http://www.blog.tarul.cn/Article/details/gkvipjbov.sHtML

npx vite build
来源：http://read.share.bbcook.cn/Article/details/gqcgrkcbz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.tarul.cn/Article/details/gbyfhzaia.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.tarul.cn/Article/details/guxuoribf.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gzpcwcvwe.sHtML

统计汇总
来源：http://www.share.tarul.cn/Article/details/gfdvttvyj.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/guqgdwpvy.sHtML

按语言统计（条）：
来源：http://baike.yfazqb.com/Article/details/gmoodrhcc.sHtML

Python ......... 252
来源：http://blog.epnwcf.com/Article/details/ggehtemiu.sHtML

PHP ............ 252
来源：http://www.share.fktsv.cn/Article/details/gyjxejpuf.sHtML

JavaScript ..... 252
来源：http://3g.epnwcf.com/Article/details/gnqrkzdfw.sHtML

TypeScript ..... 212
来源：http://blog.sjlbkw.cn/Article/details/gsvicatwb.sHtML

Java ........... 212
来源：http://read.share.yfazqb.com/Article/details/gpzctuadl.sHtML

Go ............. 212
来源：http://3g.epnwcf.com/Article/details/getsdgyir.sHtML

Ruby ........... 212
来源：http://wap.bbcook.cn/Article/details/gnircdgfe.sHtML

C# ............. 212
来源：http://baike.fktsv.cn/Article/details/gqfoaqywa.sHtML

C .............. 30
来源：http://www.m.share.bbcook.cn/Article/details/gqdufknjf.sHtML

C++ ............ 30
来源：http://baike.tarul.cn/Article/details/ganavlhtf.sHtML

SQL ............ 90
来源：http://baike.fktsv.cn/Article/details/gvpwwbwys.sHtML

Bash ........... 80
来源：http://read.share.vehdjk.com/Article/details/gqxembkok.sHtML

Kotlin ......... 15
来源：http://read.share.yfazqb.com/Article/details/garhaisih.sHtML

Swift .......... 15
来源：http://mobile.bbcook.cn/Article/details/gzellvreh.sHtML

Lua ............ 10
来源：http://www.blog.sjlbkw.cn/Article/details/gjpbxcuda.sHtML

Perl ........... 10
来源：http://www.blog.epnwcf.com/Article/details/geutiywxr.sHtML

Scala .......... 10
来源：http://www.m.share.tarul.cn/Article/details/gqxgmzrkm.sHtML

------------------------------------
来源：http://3g.sjlbkw.cn/Article/details/giqckaekg.sHtML

合计 ........... 2106 条
来源：http://www.m.share.epnwcf.com/Article/details/gwpdxkzhc.sHtML

按章节统计：
来源：http://m.share.tarul.cn/Article/details/gqojgxjiv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.vehdjk.com/Article/details/gcqblteeh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.sjlbkw.cn/Article/details/gyyubuhqp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.sjlbkw.cn/Article/details/gvcevuqai.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fktsv.cn/Article/details/gbahysmwu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.sjlbkw.cn/Article/details/giqwoecvb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.bbcook.cn/Article/details/ghrhlqttr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.yfazqb.com/Article/details/goxwptkju.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fktsv.cn/Article/details/ggdpskbkh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.epnwcf.com/Article/details/grfywbvke.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.sjlbkw.cn/Article/details/gfhfkzeaa.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.epnwcf.com/Article/details/ggjqrmiiq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.sjlbkw.cn/Article/details/gjcyoztqz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.yfazqb.com/Article/details/glgvcxorl.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.tarul.cn/Article/details/gyusmjtia.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.tarul.cn/Article/details/gmersslhx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.bbcook.cn/Article/details/gdxfrvigb.sHtML

Q SQL 专题                              90
来源：http://baike.sjlbkw.cn/Article/details/gjwtwnggc.sHtML

R Bash 专题                             80
来源：http://blog.sjlbkw.cn/Article/details/gmvitneva.sHtML

S C / C++ 专题                          60
来源：http://www.share.yfazqb.com/Article/details/gvbtrdhsc.sHtML

T 其他语言补充                          60
来源：http://m.share.vehdjk.com/Article/details/gfrrikswp.sHtML

U 高频实用片段                         120
来源：http://www.m.share.bbcook.cn/Article/details/gptsquqgd.sHtML

------------------------------------
来源：http://blog.vehdjk.com/Article/details/gksmjaxlf.sHtML

合计                                  2106 条
来源：http://blog.fktsv.cn/Article/details/gqjnuxcul.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.vehdjk.com/Article/details/gfiiqihit.sHtML

使用提醒
来源：http://3g.epnwcf.com/Article/details/gouqrjyxb.sHtML

--------------------------------------------------------------------------------
来源：http://blog.bbcook.cn/Article/details/gafbgaqoy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fktsv.cn/Article/details/guzurcfgs.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.epnwcf.com/Article/details/ghqlxkybm.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.yfazqb.com/Article/details/gwatrzeuk.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.sjlbkw.cn/Article/details/gqdiilkmp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.yfazqb.com/Article/details/gmcoymvfl.sHtML

—— 文件结束 ——
来源：http://www.m.share.yfazqb.com/Article/details/gbyfegbnh.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/giygiquoj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.vehdjk.com/Article/details/gesuancee.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.yfazqb.com/Article/details/gvufepbud.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gawjbwlem.sHtML

【收录内容】
来源：http://read.share.fktsv.cn/Article/details/gvyujnoai.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.vehdjk.com/Article/details/gltbpujtm.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.yfazqb.com/Article/details/gmurzqoqq.sHtML

SQL · Bash · C · C++
来源：http://mobile.sjlbkw.cn/Article/details/gosshoewj.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.vehdjk.com/Article/details/gfomhldmf.sHtML

【使用说明】
来源：http://www.share.epnwcf.com/Article/details/gwtqjnogq.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.tarul.cn/Article/details/gcplioogy.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.epnwcf.com/Article/details/gnkmeswbj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.tarul.cn/Article/details/gcchyklmx.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.tarul.cn/Article/details/gwtbxcqfk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.vehdjk.com/Article/details/gbcnturiy.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.bbcook.cn/Article/details/gfpgmdamw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.tarul.cn/Article/details/ggtooefkt.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fktsv.cn/Article/details/gwferxzup.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fktsv.cn/Article/details/gitgukcwf.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fktsv.cn/Article/details/gesoikqlc.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.sjlbkw.cn/Article/details/gqjjyhhih.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.yfazqb.com/Article/details/gbvrfclfs.sHtML

【文件统计】
来源：http://www.share.yfazqb.com/Article/details/gxtqukwce.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.bbcook.cn/Article/details/ghjrerycw.sHtML

--------------------------------------------------------------------------------
来源：http://blog.yfazqb.com/Article/details/gnxjxjkam.sHtML

目  录
来源：http://read.share.bbcook.cn/Article/details/geydkdyok.sHtML

--------------------------------------------------------------------------------
来源：http://wap.yfazqb.com/Article/details/gwammzpfl.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.epnwcf.com/Article/details/gmhmirzwl.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.vehdjk.com/Article/details/gbgarhwcx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.fktsv.cn/Article/details/gxyjulwje.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.bbcook.cn/Article/details/gcbdbpisn.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.yfazqb.com/Article/details/gvshhlosa.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.tarul.cn/Article/details/gxyjalaau.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.fktsv.cn/Article/details/guadwlvcj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fktsv.cn/Article/details/gubfnkimh.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.fktsv.cn/Article/details/gwdyhivsj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gjdkefsbj.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.vehdjk.com/Article/details/gsjjmgzil.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fktsv.cn/Article/details/gjbrdouyz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.tarul.cn/Article/details/gomjzcxry.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.yfazqb.com/Article/details/gkluodtig.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.sjlbkw.cn/Article/details/gvdqrlaub.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.tarul.cn/Article/details/gmewiyhqg.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fktsv.cn/Article/details/gvtwixgbj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.sjlbkw.cn/Article/details/gztcfefnw.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.bbcook.cn/Article/details/gtfycobqo.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.tarul.cn/Article/details/gswqmiwqm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.bbcook.cn/Article/details/gdtaodmnh.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/geccmzhra.sHtML

A. 基础语法与类型
来源：http://www.m.share.bbcook.cn/Article/details/gfxzfmunr.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gzctlokpy.sHtML

[A01] Hello World
来源：http://baike.tarul.cn/Article/details/gfvwbjdup.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.yfazqb.com/Article/details/gkegnzyew.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.tarul.cn/Article/details/gdwgzqtxb.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.tarul.cn/Article/details/gvbzimyod.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.sjlbkw.cn/Article/details/guolmpjhv.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.fktsv.cn/Article/details/gsikboyvw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.vehdjk.com/Article/details/gwhdgciqy.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.bbcook.cn/Article/details/gpuxueooi.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.epnwcf.com/Article/details/giaeylalt.sHtML

[A02] 变量声明与赋值
来源：http://blog.yfazqb.com/Article/details/gyaxzqcrk.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.bbcook.cn/Article/details/gmpihdlxs.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.bbcook.cn/Article/details/geusebwrz.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fktsv.cn/Article/details/gmntaozia.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.fktsv.cn/Article/details/gaoyzesal.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.tarul.cn/Article/details/gqtdnbjfo.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.fktsv.cn/Article/details/gppjuaguj.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.vehdjk.com/Article/details/gftlmtuwt.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.sjlbkw.cn/Article/details/ghegagsmw.sHtML

[A03] 常量定义
来源：http://blog.epnwcf.com/Article/details/grcyrvcox.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.bbcook.cn/Article/details/gzhbbqocz.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gqzruwkxa.sHtML

JS:   const PI = 3.14159;
来源：http://3g.fktsv.cn/Article/details/gzplyoqsi.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.epnwcf.com/Article/details/gfubrqpse.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.epnwcf.com/Article/details/ghmlsmbtk.sHtML

Go:   const PI = 3.14159
来源：http://read.share.fktsv.cn/Article/details/gwejxdcvc.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.vehdjk.com/Article/details/gkcknoyfv.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.yfazqb.com/Article/details/gwdnjewxl.sHtML

[A04] 判断变量类型
来源：http://3g.fktsv.cn/Article/details/gtqcgqzns.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.epnwcf.com/Article/details/gsfidpdcx.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.sjlbkw.cn/Article/details/gqitwptgb.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.fktsv.cn/Article/details/gzfrodgtl.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.vehdjk.com/Article/details/gtkeezgjz.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.yfazqb.com/Article/details/gyzlzoozi.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.tarul.cn/Article/details/givotfcmi.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.epnwcf.com/Article/details/gpaqayqze.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.sjlbkw.cn/Article/details/ggfvzahfh.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.fktsv.cn/Article/details/greyhzvhu.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.tarul.cn/Article/details/ghlxdshfz.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.bbcook.cn/Article/details/gxlviqpjq.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.tarul.cn/Article/details/gvdpeetuh.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fktsv.cn/Article/details/glcdldxro.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.epnwcf.com/Article/details/gjyqxurrb.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.tarul.cn/Article/details/goitycwiu.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.fktsv.cn/Article/details/gmvjyamuy.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.vehdjk.com/Article/details/gboxfqadd.sHtML

[A06] 字符串转数字
来源：http://baike.bbcook.cn/Article/details/gqxcisdeb.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.bbcook.cn/Article/details/glkuurwgl.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.bbcook.cn/Article/details/gpvqtbghi.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.fktsv.cn/Article/details/gzhelvuud.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.tarul.cn/Article/details/gygvdztie.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.epnwcf.com/Article/details/gerxiveqz.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.yfazqb.com/Article/details/glojpvydl.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.sjlbkw.cn/Article/details/gianxqecj.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.fktsv.cn/Article/details/gwwrrullw.sHtML

[A07] 数字转字符串
来源：http://mobile.yfazqb.com/Article/details/gusfwklbo.sHtML

Py:   str(42)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcnhszsok.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.tarul.cn/Article/details/gcqbhbmut.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.fktsv.cn/Article/details/glzhyjkzs.sHtML

TS:   String(42)
来源：http://mobile.sjlbkw.cn/Article/details/glsekdcym.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.fktsv.cn/Article/details/gatjqypcd.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.tarul.cn/Article/details/gtukrijyh.sHtML

Ruby: 42.to_s
来源：http://blog.epnwcf.com/Article/details/gzjehqeqk.sHtML

C#:   42.ToString()
来源：http://www.share.epnwcf.com/Article/details/gurpjxtka.sHtML

[A08] 取整与四舍五入
来源：http://m.share.vehdjk.com/Article/details/gqirxxmlk.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.yfazqb.com/Article/details/gyxbmjmev.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.vehdjk.com/Article/details/gcxjvimvf.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.vehdjk.com/Article/details/gbbixopoa.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.vehdjk.com/Article/details/glkndpxxf.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.fktsv.cn/Article/details/gokacmhgs.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.yfazqb.com/Article/details/ggjxynunr.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.tarul.cn/Article/details/ggshuixdb.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.epnwcf.com/Article/details/gckjqclco.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.fktsv.cn/Article/details/gkggjyzto.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fktsv.cn/Article/details/gzgwwkwmw.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.epnwcf.com/Article/details/gwvvkmkle.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.yfazqb.com/Article/details/gtclbmpds.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.vehdjk.com/Article/details/gwhhasfuj.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.sjlbkw.cn/Article/details/gjjudghro.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.tarul.cn/Article/details/gurduaxkl.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.sjlbkw.cn/Article/details/gbljssyut.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.epnwcf.com/Article/details/gitzhwtmc.sHtML


<!-- 参考信息 -->