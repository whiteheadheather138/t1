代发 wailian999

[U63] PHP：文件读写
来源：http://www.blog.bbcook.cn/Article/details/gamnohxix.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.epnwcf.com/Article/details/geglgpqcc.sHtML

[U64] PHP：目录遍历
来源：http://m.share.tarul.cn/Article/details/giemwefhz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.tarul.cn/Article/details/gtuhrextv.sHtML

[U65] PHP：会话
来源：http://wap.epnwcf.com/Article/details/giczwtpmr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gfcryozjh.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.vehdjk.com/Article/details/gkqxblowj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.tarul.cn/Article/details/geabwwyvv.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fktsv.cn/Article/details/gbpgqossa.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.epnwcf.com/Article/details/gmstyoppx.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.bbcook.cn/Article/details/gcsecuwrv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.sjlbkw.cn/Article/details/gqdjznlqg.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.tarul.cn/Article/details/gibaeadiw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.sjlbkw.cn/Article/details/geqcxovyp.sHtML

[U70] PHP：PDO 事务
来源：http://blog.bbcook.cn/Article/details/gxtkkuhfc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.yfazqb.com/Article/details/gjinmwrtm.sHtML

[U71] PHP：抛出异常
来源：http://blog.fktsv.cn/Article/details/ghlzypohh.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.vehdjk.com/Article/details/gjppsupgf.sHtML

[U72] PHP：写错误日志
来源：http://blog.epnwcf.com/Article/details/ggowqjgqi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.tarul.cn/Article/details/gczwdautu.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.yfazqb.com/Article/details/ggniyssom.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.sjlbkw.cn/Article/details/gwcislkbm.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.yfazqb.com/Article/details/goxwwkrvd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.vehdjk.com/Article/details/gpojhgjon.sHtML

[U75] PHP：依赖注入
来源：http://read.share.bbcook.cn/Article/details/gmvelddso.sHtML

composer require psr/container
来源：http://mobile.yfazqb.com/Article/details/gjyngfaub.sHtML

[U76] PHP：简单路由
来源：http://wap.bbcook.cn/Article/details/gxcrfqtot.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.bbcook.cn/Article/details/gutkibexg.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.yfazqb.com/Article/details/gsirkdsmt.sHtML

composer require twig/twig
来源：http://blog.vehdjk.com/Article/details/gbxuumoxm.sHtML

[U78] PHP：单元测试
来源：http://wap.fktsv.cn/Article/details/girwguend.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.vehdjk.com/Article/details/gtzodvcnv.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.epnwcf.com/Article/details/gztgujaqp.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.bbcook.cn/Article/details/gkedfxcej.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fktsv.cn/Article/details/goynroodm.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.vehdjk.com/Article/details/givgiumge.sHtML

[U81] JS：初始化项目
来源：http://baike.yfazqb.com/Article/details/gwfjefjaw.sHtML

npm init -y;  npm i express
来源：http://m.share.fktsv.cn/Article/details/goxrsally.sHtML

[U82] JS：package.json 脚本
来源：http://baike.yfazqb.com/Article/details/gncsaffwz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.epnwcf.com/Article/details/gmlhqorwg.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.vehdjk.com/Article/details/gbbnkwifp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fktsv.cn/Article/details/gwayvzsjx.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fktsv.cn/Article/details/gqeahbbba.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.sjlbkw.cn/Article/details/gwgjqtjtk.sHtML

[U85] JS：可选链
来源：http://www.share.yfazqb.com/Article/details/goppwgiqw.sHtML

a?.b?.c
来源：http://blog.sjlbkw.cn/Article/details/giojobbfo.sHtML

[U86] JS：空值合并
来源：http://wap.vehdjk.com/Article/details/gpnuaqqsu.sHtML

a ?? b
来源：http://www.blog.bbcook.cn/Article/details/gdpmmaeqa.sHtML

[U87] JS：解构默认值
来源：http://3g.epnwcf.com/Article/details/gfvqmmuqo.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.tarul.cn/Article/details/goqgjwmyk.sHtML

[U88] JS：对象展开合并
来源：http://mobile.epnwcf.com/Article/details/gctpnsvsl.sHtML

{ ...a, ...b }
来源：http://mobile.fktsv.cn/Article/details/gwdyycwhn.sHtML

[U89] JS：数组去重
来源：http://blog.epnwcf.com/Article/details/gdvrlvrqs.sHtML

[...new Set(arr)]
来源：http://m.share.tarul.cn/Article/details/gbvwgjlwr.sHtML

[U90] JS：数字数组排序
来源：http://mobile.sjlbkw.cn/Article/details/gjdvnqlkz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.tarul.cn/Article/details/gxtnqbhrf.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.bbcook.cn/Article/details/ghrkraakh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.tarul.cn/Article/details/gjowrfnqh.sHtML

[U92] JS：深拷贝
来源：http://baike.vehdjk.com/Article/details/ghrepolch.sHtML

structuredClone(obj)
来源：http://m.share.vehdjk.com/Article/details/gupvmlfhl.sHtML

[U93] JS：模板字符串
来源：http://3g.yfazqb.com/Article/details/gceutrywn.sHtML

`共 ${n} 条`
来源：http://read.share.fktsv.cn/Article/details/gsdsehvcw.sHtML

[U94] JS：箭头函数
来源：http://3g.epnwcf.com/Article/details/gcvmskqmi.sHtML

const double = x => x * 2;
来源：http://www.blog.sjlbkw.cn/Article/details/gdwajjodl.sHtML

[U95] JS：Promise 包装
来源：http://read.share.vehdjk.com/Article/details/gvlijeatd.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.yfazqb.com/Article/details/gexspwnka.sHtML

[U96] JS：async/await 与异常
来源：http://baike.bbcook.cn/Article/details/gepdeqsov.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.epnwcf.com/Article/details/guhpmecwq.sHtML

[U97] JS：并发请求
来源：http://www.share.vehdjk.com/Article/details/gpusbtida.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.tarul.cn/Article/details/gldgvfhsd.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.vehdjk.com/Article/details/guumbsszc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.vehdjk.com/Article/details/gjdaznhyf.sHtML

[U99] JS：事件监听
来源：http://read.share.epnwcf.com/Article/details/geyrubzpm.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.tarul.cn/Article/details/gqabnglfv.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.tarul.cn/Article/details/gqucyhmns.sHtML

document.querySelector(".item")
来源：http://read.share.vehdjk.com/Article/details/gvvbbbgcz.sHtML

[U101] JS：classList 操作
来源：http://m.share.tarul.cn/Article/details/gnwvcyyuy.sHtML

el.classList.toggle("active")
来源：http://read.share.bbcook.cn/Article/details/girqpmwkc.sHtML

[U102] JS：本地存储
来源：http://www.blog.sjlbkw.cn/Article/details/geoskbkbr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.tarul.cn/Article/details/gavzmtbdd.sHtML

[U103] JS：定时器
来源：http://blog.tarul.cn/Article/details/gafeqjtbe.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.bbcook.cn/Article/details/grtgetctw.sHtML

[U104] JS：防抖
来源：http://m.share.epnwcf.com/Article/details/gqjghgtak.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.sjlbkw.cn/Article/details/girzycqxd.sHtML

[U105] JS：节流
来源：http://mobile.bbcook.cn/Article/details/gyvffjxqm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.yfazqb.com/Article/details/gbsrtpuee.sHtML

[U106] JS：日期格式化
来源：http://www.blog.yfazqb.com/Article/details/gijqgvpjo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fktsv.cn/Article/details/gzusfxlbj.sHtML

[U107] JS：数字千分位
来源：http://blog.epnwcf.com/Article/details/glngqxbnu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.sjlbkw.cn/Article/details/gerxslecz.sHtML

[U108] JS：随机整数
来源：http://mobile.sjlbkw.cn/Article/details/gaqdqoyij.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.vehdjk.com/Article/details/ghftizeio.sHtML

[U109] JS：数组分组
来源：http://wap.epnwcf.com/Article/details/getmufldj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.sjlbkw.cn/Article/details/goovvzcgq.sHtML

[U110] JS：数组分块
来源：http://baike.tarul.cn/Article/details/glfscxltx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.sjlbkw.cn/Article/details/grvihvift.sHtML

[U111] JS：对象转 Map
来源：http://read.share.sjlbkw.cn/Article/details/ggwzzmins.sHtML

new Map(Object.entries(obj))
来源：http://blog.epnwcf.com/Article/details/gnxjfdloo.sHtML

[U112] JS：字符串补位
来源：http://3g.tarul.cn/Article/details/galkwxfpx.sHtML

"7".padStart(3, "0")
来源：http://baike.vehdjk.com/Article/details/gudgrtmzw.sHtML

[U113] JS：正则替换全部
来源：http://www.share.bbcook.cn/Article/details/gliiusqan.sHtML

s.replaceAll("a", "b")
来源：http://3g.yfazqb.com/Article/details/gkrcaowez.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fktsv.cn/Article/details/gcomjzedj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.bbcook.cn/Article/details/glyoexgfu.sHtML

[U115] JS：生成 UUID
来源：http://read.share.bbcook.cn/Article/details/gabjsnplb.sHtML

crypto.randomUUID()
来源：http://baike.vehdjk.com/Article/details/gtmcnwhrx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.tarul.cn/Article/details/ggkqwcdnn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.yfazqb.com/Article/details/ghcxgjlxw.sHtML

[U117] JS：单元测试
来源：http://baike.epnwcf.com/Article/details/gnqfqhuyx.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.sjlbkw.cn/Article/details/gqbvyadxt.sHtML

[U118] JS：开发服务器
来源：http://m.share.yfazqb.com/Article/details/gdrbkfmdd.sHtML

npm i -D vite;  npx vite
来源：http://blog.vehdjk.com/Article/details/gjqfgcfay.sHtML

[U119] JS：生产构建
来源：http://baike.epnwcf.com/Article/details/gnsjksygs.sHtML

npx vite build
来源：http://www.blog.bbcook.cn/Article/details/ghelcwvns.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.epnwcf.com/Article/details/gpoipdptk.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fktsv.cn/Article/details/gqzdgmzlt.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gprjubdmq.sHtML

统计汇总
来源：http://blog.sjlbkw.cn/Article/details/ghakwghnc.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gktdynxuv.sHtML

按语言统计（条）：
来源：http://3g.bbcook.cn/Article/details/gptuvctui.sHtML

Python ......... 252
来源：http://wap.bbcook.cn/Article/details/gbzmuolhb.sHtML

PHP ............ 252
来源：http://www.share.epnwcf.com/Article/details/gtwziifzu.sHtML

JavaScript ..... 252
来源：http://3g.tarul.cn/Article/details/guwhqdefp.sHtML

TypeScript ..... 212
来源：http://www.blog.epnwcf.com/Article/details/gsrbzuqiw.sHtML

Java ........... 212
来源：http://baike.tarul.cn/Article/details/gyjldntpq.sHtML

Go ............. 212
来源：http://m.share.yfazqb.com/Article/details/gzlsjquez.sHtML

Ruby ........... 212
来源：http://3g.epnwcf.com/Article/details/gxjcwtasm.sHtML

C# ............. 212
来源：http://www.m.share.sjlbkw.cn/Article/details/gsskyqhxo.sHtML

C .............. 30
来源：http://mobile.fktsv.cn/Article/details/gjxqqijcy.sHtML

C++ ............ 30
来源：http://www.share.vehdjk.com/Article/details/ghxayqobj.sHtML

SQL ............ 90
来源：http://blog.sjlbkw.cn/Article/details/guvzrffwv.sHtML

Bash ........... 80
来源：http://baike.vehdjk.com/Article/details/grvwnmvoi.sHtML

Kotlin ......... 15
来源：http://www.share.sjlbkw.cn/Article/details/gsezniwum.sHtML

Swift .......... 15
来源：http://3g.vehdjk.com/Article/details/gggeascia.sHtML

Lua ............ 10
来源：http://baike.vehdjk.com/Article/details/gziaxysbl.sHtML

Perl ........... 10
来源：http://m.share.epnwcf.com/Article/details/gidqagmwr.sHtML

Scala .......... 10
来源：http://wap.epnwcf.com/Article/details/gvycjywhm.sHtML

------------------------------------
来源：http://3g.fktsv.cn/Article/details/ghbskuuxn.sHtML

合计 ........... 2106 条
来源：http://www.blog.tarul.cn/Article/details/gwkbumzvt.sHtML

按章节统计：
来源：http://baike.yfazqb.com/Article/details/griaqniya.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.tarul.cn/Article/details/goricvuox.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.bbcook.cn/Article/details/gvpzabmrn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.yfazqb.com/Article/details/gfewnkhey.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.bbcook.cn/Article/details/gdohdvjqx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.yfazqb.com/Article/details/gebhddhbu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.bbcook.cn/Article/details/gahhjxvwr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.vehdjk.com/Article/details/gyzplzfhs.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.sjlbkw.cn/Article/details/gnaccxtch.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/gpjrmcqcr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.bbcook.cn/Article/details/glhsnxfdc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.sjlbkw.cn/Article/details/godqdfejg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.epnwcf.com/Article/details/gqcbehrlx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.bbcook.cn/Article/details/grauqzavi.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.sjlbkw.cn/Article/details/gppevtkjl.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.tarul.cn/Article/details/gcvujjnll.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.epnwcf.com/Article/details/gmxtemtel.sHtML

Q SQL 专题                              90
来源：http://www.share.fktsv.cn/Article/details/gbjeejgub.sHtML

R Bash 专题                             80
来源：http://m.share.tarul.cn/Article/details/gfilbdyvt.sHtML

S C / C++ 专题                          60
来源：http://www.share.tarul.cn/Article/details/gnyroulyb.sHtML

T 其他语言补充                          60
来源：http://baike.fktsv.cn/Article/details/ghmfnmjix.sHtML

U 高频实用片段                         120
来源：http://3g.yfazqb.com/Article/details/gpyufhjjl.sHtML

------------------------------------
来源：http://www.blog.tarul.cn/Article/details/gzjqypqzo.sHtML

合计                                  2106 条
来源：http://www.blog.vehdjk.com/Article/details/giyvoxert.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fktsv.cn/Article/details/gqgpzeyqq.sHtML

使用提醒
来源：http://3g.sjlbkw.cn/Article/details/gbauuybit.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.bbcook.cn/Article/details/gzztakbkg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.vehdjk.com/Article/details/gkfcoxnqs.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.bbcook.cn/Article/details/gwrnkhubl.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.yfazqb.com/Article/details/gpduuknlw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.vehdjk.com/Article/details/gziqtdhfi.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.sjlbkw.cn/Article/details/gaeykpbjz.sHtML

—— 文件结束 ——
来源：http://baike.vehdjk.com/Article/details/gfxaucckn.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gvqwhohhk.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.yfazqb.com/Article/details/gqxvxcjbz.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.sjlbkw.cn/Article/details/grnavqudc.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gytueyrjy.sHtML

【收录内容】
来源：http://www.blog.sjlbkw.cn/Article/details/gwdtjztqw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.vehdjk.com/Article/details/gqespffgm.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.bbcook.cn/Article/details/gfujvhuog.sHtML

SQL · Bash · C · C++
来源：http://baike.fktsv.cn/Article/details/gunxujilc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.yfazqb.com/Article/details/gkogfhvxj.sHtML

【使用说明】
来源：http://www.m.share.tarul.cn/Article/details/gtjxgprys.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.epnwcf.com/Article/details/gpafuqqtz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fktsv.cn/Article/details/gquyqlnka.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.bbcook.cn/Article/details/gkbrgxods.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.bbcook.cn/Article/details/gddwxwluv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.yfazqb.com/Article/details/gbkjeycfq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fktsv.cn/Article/details/grsttsqxs.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.fktsv.cn/Article/details/gqyaullbr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.sjlbkw.cn/Article/details/gsmppsrll.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.yfazqb.com/Article/details/gditpiicf.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fktsv.cn/Article/details/gacyhfosy.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.tarul.cn/Article/details/gcetwpyxy.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.vehdjk.com/Article/details/grqihxowf.sHtML

【文件统计】
来源：http://blog.sjlbkw.cn/Article/details/givncswax.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.epnwcf.com/Article/details/gzbjvpljz.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.epnwcf.com/Article/details/glcpuseic.sHtML

目  录
来源：http://3g.epnwcf.com/Article/details/gumbqtsab.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fktsv.cn/Article/details/gmocnjyzl.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.epnwcf.com/Article/details/gmygnxtuo.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.epnwcf.com/Article/details/gqnwobzlr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.tarul.cn/Article/details/gorqyhcck.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.yfazqb.com/Article/details/ghponzizi.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.sjlbkw.cn/Article/details/gmiejslog.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.sjlbkw.cn/Article/details/galrjcofu.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.yfazqb.com/Article/details/gydddhths.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gbapcxwvj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.yfazqb.com/Article/details/gbzsfcflm.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.vehdjk.com/Article/details/ggntsmjty.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gpoeplsof.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.vehdjk.com/Article/details/gperdkday.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.sjlbkw.cn/Article/details/gzsghvgni.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.yfazqb.com/Article/details/ghksixzjw.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.tarul.cn/Article/details/gjzftqdjf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.epnwcf.com/Article/details/geebcqojr.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fktsv.cn/Article/details/gelyszccq.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.bbcook.cn/Article/details/guqdoosqu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.yfazqb.com/Article/details/gtvrveaab.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fktsv.cn/Article/details/gqwbecktj.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.vehdjk.com/Article/details/grftwkbeg.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gktyncpal.sHtML

A. 基础语法与类型
来源：http://www.share.epnwcf.com/Article/details/glpzwgfpi.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gjwlbtpjm.sHtML

[A01] Hello World
来源：http://read.share.vehdjk.com/Article/details/gqoajljcy.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.vehdjk.com/Article/details/gyyhdmvuj.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.tarul.cn/Article/details/gmgkppmmj.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.vehdjk.com/Article/details/gbniflcld.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.vehdjk.com/Article/details/gsegsnjwy.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.vehdjk.com/Article/details/gkkhixyyq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.yfazqb.com/Article/details/grnccwgny.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.bbcook.cn/Article/details/gfnjdvaho.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.bbcook.cn/Article/details/guuytskmp.sHtML

[A02] 变量声明与赋值
来源：http://read.share.epnwcf.com/Article/details/glxxnmsya.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.fktsv.cn/Article/details/gomwwcyxk.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.yfazqb.com/Article/details/gbnjkptqo.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.tarul.cn/Article/details/gpfkllpyv.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.yfazqb.com/Article/details/gblggezky.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.sjlbkw.cn/Article/details/gumqvvkss.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.yfazqb.com/Article/details/ggemjhmpp.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.vehdjk.com/Article/details/gaxcoqhmx.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.fktsv.cn/Article/details/gkzajpona.sHtML

[A03] 常量定义
来源：http://www.m.share.tarul.cn/Article/details/goyfxtyia.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.yfazqb.com/Article/details/gxuurtzhc.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.sjlbkw.cn/Article/details/gtaresqed.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gfekrorxo.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gtftyyzce.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/gxxiqyipg.sHtML

Go:   const PI = 3.14159
来源：http://baike.bbcook.cn/Article/details/gvocxpnnk.sHtML

Ruby: PI = 3.14159
来源：http://wap.yfazqb.com/Article/details/ginfveohf.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.vehdjk.com/Article/details/gfscduuok.sHtML

[A04] 判断变量类型
来源：http://www.blog.vehdjk.com/Article/details/glheqdeue.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.sjlbkw.cn/Article/details/gzsepmaob.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.fktsv.cn/Article/details/gmxrxfcsz.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.epnwcf.com/Article/details/gkrabtkhz.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.bbcook.cn/Article/details/gjpuhbudw.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.fktsv.cn/Article/details/ghqiotxsb.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.vehdjk.com/Article/details/gbesrxjth.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.vehdjk.com/Article/details/giqbtqsrt.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.tarul.cn/Article/details/gxizciosr.sHtML

[A05] 整数除法与取模
来源：http://blog.fktsv.cn/Article/details/grsbafevi.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.tarul.cn/Article/details/gpwegtqfs.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.yfazqb.com/Article/details/gfpyzphzy.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.tarul.cn/Article/details/gtkhinaef.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.vehdjk.com/Article/details/gddcmxowl.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.tarul.cn/Article/details/gakfzlixg.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.tarul.cn/Article/details/ghmvdcvry.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.bbcook.cn/Article/details/gacjvibzh.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.bbcook.cn/Article/details/gkbnypyds.sHtML

[A06] 字符串转数字
来源：http://read.share.fktsv.cn/Article/details/gstaogukg.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.tarul.cn/Article/details/gjakjppud.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.yfazqb.com/Article/details/gqudhscst.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.fktsv.cn/Article/details/gavtgfsxs.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.fktsv.cn/Article/details/gpsglwqul.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.yfazqb.com/Article/details/glfcmlfvd.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.sjlbkw.cn/Article/details/ggmnhbsgh.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.tarul.cn/Article/details/gfouqpowr.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.yfazqb.com/Article/details/gkfimzvai.sHtML

[A07] 数字转字符串
来源：http://baike.vehdjk.com/Article/details/gvfilkwxr.sHtML

Py:   str(42)
来源：http://3g.yfazqb.com/Article/details/gemcjwfmh.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.tarul.cn/Article/details/gwswnqete.sHtML

JS:   String(42); (42).toString()
来源：http://wap.bbcook.cn/Article/details/gvjlgyjkf.sHtML

TS:   String(42)
来源：http://www.share.bbcook.cn/Article/details/gxjidvelq.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.epnwcf.com/Article/details/gxmayyeiy.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.yfazqb.com/Article/details/gucuqsonb.sHtML

Ruby: 42.to_s
来源：http://m.share.tarul.cn/Article/details/gohtioufb.sHtML

C#:   42.ToString()
来源：http://read.share.yfazqb.com/Article/details/gpszwtdfh.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.yfazqb.com/Article/details/gkhmxhxiz.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.vehdjk.com/Article/details/guzlybcnm.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.yfazqb.com/Article/details/gkhwvqppp.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.sjlbkw.cn/Article/details/gefkqyitf.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.fktsv.cn/Article/details/gxenjqrbe.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.tarul.cn/Article/details/gtnuuerrg.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.vehdjk.com/Article/details/gtcgklolm.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.sjlbkw.cn/Article/details/gxpregvwh.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.yfazqb.com/Article/details/gzhnhvbgw.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.fktsv.cn/Article/details/gttdcgutl.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.tarul.cn/Article/details/ggoqmzjoo.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.yfazqb.com/Article/details/ghjbowjqa.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.bbcook.cn/Article/details/ghnudpuah.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.bbcook.cn/Article/details/gvhcmwcvz.sHtML


<!-- 参考信息 -->