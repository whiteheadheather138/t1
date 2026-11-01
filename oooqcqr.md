代发 wailian999

[U63] PHP：文件读写
来源：http://www.share.tarul.cn/Article/details/gaflooulu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.yfazqb.com/Article/details/galwoyqtd.sHtML

[U64] PHP：目录遍历
来源：http://baike.epnwcf.com/Article/details/geykgwgzw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.yfazqb.com/Article/details/gxpgjwfyw.sHtML

[U65] PHP：会话
来源：http://www.share.yfazqb.com/Article/details/gnskjpyfg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/gwoibrfuf.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.bbcook.cn/Article/details/gmkgvyssz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.epnwcf.com/Article/details/ghawfvycn.sHtML

[U67] PHP：处理文件上传
来源：http://baike.sjlbkw.cn/Article/details/gldupvzto.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.tarul.cn/Article/details/gcaxbxxgx.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fktsv.cn/Article/details/gxkizurcu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fktsv.cn/Article/details/gthbcsolk.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.yfazqb.com/Article/details/ggchnrldo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.tarul.cn/Article/details/gzrwkmwix.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fktsv.cn/Article/details/gvvoraytu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.epnwcf.com/Article/details/gvvpzviqb.sHtML

[U71] PHP：抛出异常
来源：http://baike.bbcook.cn/Article/details/glxtahimm.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fktsv.cn/Article/details/geprvmxlh.sHtML

[U72] PHP：写错误日志
来源：http://baike.fktsv.cn/Article/details/gqsksprlq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.sjlbkw.cn/Article/details/gqwgtbvhm.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fktsv.cn/Article/details/ghqgjodtc.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.vehdjk.com/Article/details/gxzvtjgij.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fktsv.cn/Article/details/gmlplhebe.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.tarul.cn/Article/details/gfuoorjqc.sHtML

[U75] PHP：依赖注入
来源：http://m.share.tarul.cn/Article/details/gzxbfeqrs.sHtML

composer require psr/container
来源：http://www.blog.vehdjk.com/Article/details/gditouewb.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fktsv.cn/Article/details/gnfbiafyc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fktsv.cn/Article/details/gyblduwom.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fktsv.cn/Article/details/givofxsfi.sHtML

composer require twig/twig
来源：http://blog.tarul.cn/Article/details/gezcqreqf.sHtML

[U78] PHP：单元测试
来源：http://m.share.sjlbkw.cn/Article/details/gefjsgrhb.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.vehdjk.com/Article/details/gaewqlxbk.sHtML

[U79] PHP：静态分析
来源：http://read.share.vehdjk.com/Article/details/gpmkvihqc.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.bbcook.cn/Article/details/gknrkptto.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fktsv.cn/Article/details/ggbrthyyn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.tarul.cn/Article/details/giwxwfsch.sHtML

[U81] JS：初始化项目
来源：http://mobile.vehdjk.com/Article/details/grujyntme.sHtML

npm init -y;  npm i express
来源：http://read.share.yfazqb.com/Article/details/gxhkiidtd.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.tarul.cn/Article/details/gyjditipy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.epnwcf.com/Article/details/ghikoaqdz.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.sjlbkw.cn/Article/details/gqwkluqvk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.tarul.cn/Article/details/galzswvfj.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.sjlbkw.cn/Article/details/ggcdgyuln.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.bbcook.cn/Article/details/gcfbipzzf.sHtML

[U85] JS：可选链
来源：http://www.m.share.epnwcf.com/Article/details/ghdvqwnqz.sHtML

a?.b?.c
来源：http://www.share.vehdjk.com/Article/details/glcngrhgu.sHtML

[U86] JS：空值合并
来源：http://www.share.yfazqb.com/Article/details/gudiccthj.sHtML

a ?? b
来源：http://www.blog.vehdjk.com/Article/details/gmlsdkxcf.sHtML

[U87] JS：解构默认值
来源：http://baike.epnwcf.com/Article/details/gyttfpmab.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.vehdjk.com/Article/details/gcrxhmjfc.sHtML

[U88] JS：对象展开合并
来源：http://wap.sjlbkw.cn/Article/details/gjppbfsvd.sHtML

{ ...a, ...b }
来源：http://read.share.tarul.cn/Article/details/goyhlktwn.sHtML

[U89] JS：数组去重
来源：http://baike.bbcook.cn/Article/details/gjqksxqus.sHtML

[...new Set(arr)]
来源：http://wap.sjlbkw.cn/Article/details/ghkfkqrcj.sHtML

[U90] JS：数字数组排序
来源：http://blog.bbcook.cn/Article/details/gaahagnrn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.vehdjk.com/Article/details/ghnvddtpb.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.tarul.cn/Article/details/gpvtksnkh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.yfazqb.com/Article/details/gkolfmhls.sHtML

[U92] JS：深拷贝
来源：http://www.share.yfazqb.com/Article/details/gvozmtfug.sHtML

structuredClone(obj)
来源：http://3g.yfazqb.com/Article/details/gfhoexbgv.sHtML

[U93] JS：模板字符串
来源：http://3g.fktsv.cn/Article/details/gdkevxutg.sHtML

`共 ${n} 条`
来源：http://www.m.share.bbcook.cn/Article/details/gkaqudxzx.sHtML

[U94] JS：箭头函数
来源：http://blog.epnwcf.com/Article/details/gparoqyla.sHtML

const double = x => x * 2;
来源：http://3g.yfazqb.com/Article/details/gvqcwiwzv.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.vehdjk.com/Article/details/gjsevkrlo.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.bbcook.cn/Article/details/goqioblmf.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.vehdjk.com/Article/details/gcafpftrf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.bbcook.cn/Article/details/gcdqoytiq.sHtML

[U97] JS：并发请求
来源：http://baike.bbcook.cn/Article/details/gtrndmbvo.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gujiwlmzr.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.vehdjk.com/Article/details/gvvffwqlr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.sjlbkw.cn/Article/details/gjqemxixo.sHtML

[U99] JS：事件监听
来源：http://www.blog.vehdjk.com/Article/details/gmuzjaygl.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.bbcook.cn/Article/details/gxwfltoav.sHtML

[U100] JS：DOM 查询
来源：http://www.share.epnwcf.com/Article/details/gpxjxoikq.sHtML

document.querySelector(".item")
来源：http://baike.bbcook.cn/Article/details/ggbvtncqo.sHtML

[U101] JS：classList 操作
来源：http://www.blog.bbcook.cn/Article/details/gdszacuuh.sHtML

el.classList.toggle("active")
来源：http://www.blog.tarul.cn/Article/details/gceuyatiq.sHtML

[U102] JS：本地存储
来源：http://wap.epnwcf.com/Article/details/gorrlojqa.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.epnwcf.com/Article/details/gcnakvcss.sHtML

[U103] JS：定时器
来源：http://www.m.share.yfazqb.com/Article/details/gtccducbj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.yfazqb.com/Article/details/gxhomsftm.sHtML

[U104] JS：防抖
来源：http://www.m.share.fktsv.cn/Article/details/gzaqzimdj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.tarul.cn/Article/details/gucazupmc.sHtML

[U105] JS：节流
来源：http://mobile.sjlbkw.cn/Article/details/gdwfdicmm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fktsv.cn/Article/details/gxpvgbsya.sHtML

[U106] JS：日期格式化
来源：http://m.share.yfazqb.com/Article/details/gnhmkvole.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fktsv.cn/Article/details/gwxxjldlp.sHtML

[U107] JS：数字千分位
来源：http://blog.bbcook.cn/Article/details/gikwelzys.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fktsv.cn/Article/details/gjsvpyiml.sHtML

[U108] JS：随机整数
来源：http://wap.fktsv.cn/Article/details/gwplekgyz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.epnwcf.com/Article/details/gezduzegy.sHtML

[U109] JS：数组分组
来源：http://wap.yfazqb.com/Article/details/ghujshfmr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.vehdjk.com/Article/details/gwmepitcq.sHtML

[U110] JS：数组分块
来源：http://blog.fktsv.cn/Article/details/gochwvbef.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.yfazqb.com/Article/details/gghthtdal.sHtML

[U111] JS：对象转 Map
来源：http://read.share.sjlbkw.cn/Article/details/gwusobzkk.sHtML

new Map(Object.entries(obj))
来源：http://read.share.yfazqb.com/Article/details/gcvhrlwkf.sHtML

[U112] JS：字符串补位
来源：http://3g.yfazqb.com/Article/details/gvjgrcvlc.sHtML

"7".padStart(3, "0")
来源：http://3g.yfazqb.com/Article/details/gaubegnmo.sHtML

[U113] JS：正则替换全部
来源：http://www.share.epnwcf.com/Article/details/grbdgsbem.sHtML

s.replaceAll("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gbatljkxn.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.epnwcf.com/Article/details/gatvuestl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.tarul.cn/Article/details/gnmoyxhwy.sHtML

[U115] JS：生成 UUID
来源：http://baike.bbcook.cn/Article/details/gmaikeugv.sHtML

crypto.randomUUID()
来源：http://blog.epnwcf.com/Article/details/gliwprmre.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.bbcook.cn/Article/details/gjogcwjdg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.yfazqb.com/Article/details/ggacdfhcu.sHtML

[U117] JS：单元测试
来源：http://mobile.yfazqb.com/Article/details/gqnschmul.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.epnwcf.com/Article/details/gqjcgijcb.sHtML

[U118] JS：开发服务器
来源：http://3g.yfazqb.com/Article/details/gqgpdgmvp.sHtML

npm i -D vite;  npx vite
来源：http://wap.sjlbkw.cn/Article/details/gylwannys.sHtML

[U119] JS：生产构建
来源：http://mobile.epnwcf.com/Article/details/ghzcjiqge.sHtML

npx vite build
来源：http://www.share.tarul.cn/Article/details/gwhgpgepw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.bbcook.cn/Article/details/glugpscxv.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fktsv.cn/Article/details/gvgyudwrl.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gpibvisrd.sHtML

统计汇总
来源：http://mobile.sjlbkw.cn/Article/details/gkqogzjpv.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/grbzozbek.sHtML

按语言统计（条）：
来源：http://mobile.fktsv.cn/Article/details/gjfvzxbiv.sHtML

Python ......... 252
来源：http://3g.fktsv.cn/Article/details/gsiimgwzw.sHtML

PHP ............ 252
来源：http://baike.tarul.cn/Article/details/gimpjjhdk.sHtML

JavaScript ..... 252
来源：http://read.share.epnwcf.com/Article/details/gmzqntbwh.sHtML

TypeScript ..... 212
来源：http://baike.yfazqb.com/Article/details/gnyqtffxd.sHtML

Java ........... 212
来源：http://www.blog.bbcook.cn/Article/details/gkjqiqvlt.sHtML

Go ............. 212
来源：http://read.share.sjlbkw.cn/Article/details/gglzlssct.sHtML

Ruby ........... 212
来源：http://www.share.fktsv.cn/Article/details/gfmzuvoxb.sHtML

C# ............. 212
来源：http://mobile.tarul.cn/Article/details/gmlcstezm.sHtML

C .............. 30
来源：http://3g.yfazqb.com/Article/details/gwnqcetpt.sHtML

C++ ............ 30
来源：http://www.m.share.epnwcf.com/Article/details/gwfqaepmt.sHtML

SQL ............ 90
来源：http://wap.vehdjk.com/Article/details/ggrkjndds.sHtML

Bash ........... 80
来源：http://m.share.sjlbkw.cn/Article/details/gmbppzhds.sHtML

Kotlin ......... 15
来源：http://wap.sjlbkw.cn/Article/details/gqsnsmmox.sHtML

Swift .......... 15
来源：http://mobile.sjlbkw.cn/Article/details/guvsdukmh.sHtML

Lua ............ 10
来源：http://www.share.vehdjk.com/Article/details/gndheyzst.sHtML

Perl ........... 10
来源：http://www.share.vehdjk.com/Article/details/gmejhywlw.sHtML

Scala .......... 10
来源：http://3g.yfazqb.com/Article/details/gcnwvwmju.sHtML

------------------------------------
来源：http://www.share.yfazqb.com/Article/details/gssrtrbmh.sHtML

合计 ........... 2106 条
来源：http://www.blog.fktsv.cn/Article/details/gvtlvsmon.sHtML

按章节统计：
来源：http://mobile.sjlbkw.cn/Article/details/gkijrphpf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.vehdjk.com/Article/details/grnsrzhxh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.yfazqb.com/Article/details/goinyrcfy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fktsv.cn/Article/details/ggqhudody.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.epnwcf.com/Article/details/goijburjj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.tarul.cn/Article/details/geeowpnli.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.tarul.cn/Article/details/gkpvztske.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.epnwcf.com/Article/details/gzxecieof.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.yfazqb.com/Article/details/gcsepgwoe.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.sjlbkw.cn/Article/details/gcgkwaniw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.epnwcf.com/Article/details/gjfuxczdq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.tarul.cn/Article/details/giszvtwzk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.sjlbkw.cn/Article/details/geunfvowg.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.tarul.cn/Article/details/gexvekoat.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.tarul.cn/Article/details/gtgmawfad.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.yfazqb.com/Article/details/gfbdniyvv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fktsv.cn/Article/details/gsaijtqnh.sHtML

Q SQL 专题                              90
来源：http://www.share.epnwcf.com/Article/details/gcoqeehzg.sHtML

R Bash 专题                             80
来源：http://blog.epnwcf.com/Article/details/gjhoacjhq.sHtML

S C / C++ 专题                          60
来源：http://read.share.vehdjk.com/Article/details/gkretndny.sHtML

T 其他语言补充                          60
来源：http://m.share.fktsv.cn/Article/details/guvhkhwgu.sHtML

U 高频实用片段                         120
来源：http://wap.tarul.cn/Article/details/gjrgmpkot.sHtML

------------------------------------
来源：http://read.share.bbcook.cn/Article/details/gyzkbxgcp.sHtML

合计                                  2106 条
来源：http://mobile.bbcook.cn/Article/details/grjravtvs.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.sjlbkw.cn/Article/details/gdjsnxxbo.sHtML

使用提醒
来源：http://www.blog.yfazqb.com/Article/details/gqjndnwpd.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.tarul.cn/Article/details/gyynqlsti.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.sjlbkw.cn/Article/details/gwhlsuixy.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.sjlbkw.cn/Article/details/gkgmhnufg.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.yfazqb.com/Article/details/gbyyhnjsv.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.tarul.cn/Article/details/glvcvaryv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.yfazqb.com/Article/details/gfvkjbdtu.sHtML

—— 文件结束 ——
来源：http://baike.vehdjk.com/Article/details/gydhyslyo.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/ggkxwlgty.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.bbcook.cn/Article/details/gwcwubmfe.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.epnwcf.com/Article/details/gojyhzvuz.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gbzmzygia.sHtML

【收录内容】
来源：http://m.share.yfazqb.com/Article/details/giqnopkol.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.epnwcf.com/Article/details/gyfzpieyf.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.tarul.cn/Article/details/gjzlewzvk.sHtML

SQL · Bash · C · C++
来源：http://www.share.bbcook.cn/Article/details/ghpydsszv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fktsv.cn/Article/details/ggggotvjk.sHtML

【使用说明】
来源：http://m.share.sjlbkw.cn/Article/details/gzjadgler.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fktsv.cn/Article/details/gqcsbtkop.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.epnwcf.com/Article/details/gfudpltcc.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.vehdjk.com/Article/details/gzvbaussv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.tarul.cn/Article/details/gsliegzoc.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.bbcook.cn/Article/details/gthunfrlo.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.sjlbkw.cn/Article/details/gqqejsdws.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.epnwcf.com/Article/details/gydtmdprl.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.yfazqb.com/Article/details/gzmrrqtcc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.sjlbkw.cn/Article/details/gxceahmez.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.epnwcf.com/Article/details/gxdhimafp.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.epnwcf.com/Article/details/gvkqtnczd.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.epnwcf.com/Article/details/gjrwjhdsg.sHtML

【文件统计】
来源：http://wap.vehdjk.com/Article/details/gmsdnfghl.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.tarul.cn/Article/details/glsklftfa.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.vehdjk.com/Article/details/gntdfcoon.sHtML

目  录
来源：http://m.share.sjlbkw.cn/Article/details/giafhgkag.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.vehdjk.com/Article/details/gymfbbhys.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.bbcook.cn/Article/details/gvtjnyzoq.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.sjlbkw.cn/Article/details/gryeqsnmd.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.sjlbkw.cn/Article/details/gnmismopi.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.yfazqb.com/Article/details/gttrucxgp.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.tarul.cn/Article/details/gnosmouao.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.bbcook.cn/Article/details/gzbyqdxif.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.epnwcf.com/Article/details/gslmvfdzt.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.vehdjk.com/Article/details/gjlampjuw.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.yfazqb.com/Article/details/gkgtyediu.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.vehdjk.com/Article/details/gudvebryo.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.tarul.cn/Article/details/gyshrucmd.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.tarul.cn/Article/details/giremwrfv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.epnwcf.com/Article/details/grvfxvfcb.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.vehdjk.com/Article/details/gldguqnzk.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.fktsv.cn/Article/details/ggpvbnjch.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.yfazqb.com/Article/details/gtmnsnwsl.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.sjlbkw.cn/Article/details/glkkbzrpl.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.fktsv.cn/Article/details/gvkclcnwy.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.sjlbkw.cn/Article/details/gfgrzhnfr.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.vehdjk.com/Article/details/gdertvgns.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.epnwcf.com/Article/details/grewzcpwv.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gofztfebx.sHtML

A. 基础语法与类型
来源：http://www.share.vehdjk.com/Article/details/gqazxcgjd.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gktfcnkyh.sHtML

[A01] Hello World
来源：http://blog.epnwcf.com/Article/details/gwogzfuvw.sHtML

Py:   print("Hello, World!")
来源：http://read.share.bbcook.cn/Article/details/gcemmffcj.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.sjlbkw.cn/Article/details/gduyvxjzi.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.fktsv.cn/Article/details/ghfkksfwa.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.tarul.cn/Article/details/giuivjfmc.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.sjlbkw.cn/Article/details/gqbpmmhij.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.vehdjk.com/Article/details/gmuchpxpc.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.tarul.cn/Article/details/giuifnqvn.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.vehdjk.com/Article/details/gnciqqxhk.sHtML

[A02] 变量声明与赋值
来源：http://wap.epnwcf.com/Article/details/gltlxolcd.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fktsv.cn/Article/details/gjzltqksc.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.tarul.cn/Article/details/gpcvqepxr.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.epnwcf.com/Article/details/gcsgfdxey.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.yfazqb.com/Article/details/gzfrzwqdd.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.tarul.cn/Article/details/ghrktubty.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.sjlbkw.cn/Article/details/gunidrqli.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.epnwcf.com/Article/details/gdpsfntuw.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.tarul.cn/Article/details/gfqftmusg.sHtML

[A03] 常量定义
来源：http://mobile.epnwcf.com/Article/details/gcrehwxwu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.yfazqb.com/Article/details/gzhqvdnpf.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/gpyxrhwnc.sHtML

JS:   const PI = 3.14159;
来源：http://blog.yfazqb.com/Article/details/grhzthhjt.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.vehdjk.com/Article/details/gwsqpmyqc.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.yfazqb.com/Article/details/gpooapjch.sHtML

Go:   const PI = 3.14159
来源：http://baike.epnwcf.com/Article/details/gynwyakeq.sHtML

Ruby: PI = 3.14159
来源：http://m.share.tarul.cn/Article/details/glenfylen.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/gqbhjdijl.sHtML

[A04] 判断变量类型
来源：http://blog.tarul.cn/Article/details/gleekocwt.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.epnwcf.com/Article/details/gnvxykscq.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.epnwcf.com/Article/details/geurvgryo.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.vehdjk.com/Article/details/gjjhqhnkb.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.bbcook.cn/Article/details/gnwkyzbwp.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.sjlbkw.cn/Article/details/gegdcurmr.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.yfazqb.com/Article/details/gzvgyfggk.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.bbcook.cn/Article/details/gxsghlnju.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.yfazqb.com/Article/details/gavwirmqk.sHtML

[A05] 整数除法与取模
来源：http://read.share.epnwcf.com/Article/details/gjonihdqg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.bbcook.cn/Article/details/ggfysxhyt.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.tarul.cn/Article/details/gbvqprwyb.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.sjlbkw.cn/Article/details/giufdlfoi.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fktsv.cn/Article/details/guzgmykwl.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.yfazqb.com/Article/details/ghwidqryr.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.bbcook.cn/Article/details/gitqnvbbw.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.bbcook.cn/Article/details/gmctvzjxw.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.vehdjk.com/Article/details/gwxokphhx.sHtML

[A06] 字符串转数字
来源：http://blog.vehdjk.com/Article/details/geoeymvhv.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.tarul.cn/Article/details/grjciammx.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.sjlbkw.cn/Article/details/grsmlntlk.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.vehdjk.com/Article/details/ghweninni.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.sjlbkw.cn/Article/details/gothrkjgp.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.vehdjk.com/Article/details/grvoomzvt.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.fktsv.cn/Article/details/ggmdysjgp.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.yfazqb.com/Article/details/gaqpinmzj.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.fktsv.cn/Article/details/gnkbbhabd.sHtML

[A07] 数字转字符串
来源：http://wap.sjlbkw.cn/Article/details/gddmfoznn.sHtML

Py:   str(42)
来源：http://m.share.sjlbkw.cn/Article/details/ggayystar.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.tarul.cn/Article/details/ghpdtsnuk.sHtML

JS:   String(42); (42).toString()
来源：http://wap.vehdjk.com/Article/details/geujgxbto.sHtML

TS:   String(42)
来源：http://read.share.fktsv.cn/Article/details/gdghyoqgh.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.epnwcf.com/Article/details/gzfabfiot.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.fktsv.cn/Article/details/gdowokobl.sHtML

Ruby: 42.to_s
来源：http://blog.fktsv.cn/Article/details/gggbmgsdw.sHtML

C#:   42.ToString()
来源：http://m.share.yfazqb.com/Article/details/gethxwubz.sHtML

[A08] 取整与四舍五入
来源：http://read.share.sjlbkw.cn/Article/details/gbmzxvagi.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.epnwcf.com/Article/details/gvxoezwsl.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.vehdjk.com/Article/details/gowtjigtj.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.vehdjk.com/Article/details/glhefuaax.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.epnwcf.com/Article/details/gqzkdvrjl.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.fktsv.cn/Article/details/gyijbakuh.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.fktsv.cn/Article/details/gfogoeorq.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.fktsv.cn/Article/details/gzbgviich.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.fktsv.cn/Article/details/gfouymkhf.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.epnwcf.com/Article/details/gobdmakep.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/grhguifkx.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.tarul.cn/Article/details/gokysudpb.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.fktsv.cn/Article/details/grvkirpeg.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.fktsv.cn/Article/details/glpuwstoi.sHtML


<!-- 参考信息 -->