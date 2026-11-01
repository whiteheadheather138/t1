代发 wailian999

[U63] PHP：文件读写
来源：http://mobile.vehdjk.com/Article/details/gchfsfpco.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.tarul.cn/Article/details/gaqqjvtpp.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.epnwcf.com/Article/details/gxqkgyzzy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.sjlbkw.cn/Article/details/gowsazsde.sHtML

[U65] PHP：会话
来源：http://m.share.bbcook.cn/Article/details/gnvumzwgy.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.vehdjk.com/Article/details/gcmvskfde.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.vehdjk.com/Article/details/gmxkefgto.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.epnwcf.com/Article/details/gdbicrmbw.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fktsv.cn/Article/details/gldgksnto.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.yfazqb.com/Article/details/gdcdfbnmu.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.sjlbkw.cn/Article/details/gtlzcjzaw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.tarul.cn/Article/details/gigdyyplw.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.sjlbkw.cn/Article/details/glqslmjqz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.tarul.cn/Article/details/gwrcbxbkd.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fktsv.cn/Article/details/gaoksvyzm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.vehdjk.com/Article/details/gmdhstkey.sHtML

[U71] PHP：抛出异常
来源：http://mobile.yfazqb.com/Article/details/ggikztvmo.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.sjlbkw.cn/Article/details/govhwjkrf.sHtML

[U72] PHP：写错误日志
来源：http://baike.vehdjk.com/Article/details/gdsggoaex.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fktsv.cn/Article/details/gcrawxwkn.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.vehdjk.com/Article/details/gywyxasvo.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.epnwcf.com/Article/details/ghcgfxqzo.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.bbcook.cn/Article/details/gmuwefxts.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fktsv.cn/Article/details/gljgwqohk.sHtML

[U75] PHP：依赖注入
来源：http://www.share.yfazqb.com/Article/details/gwlaxfgoe.sHtML

composer require psr/container
来源：http://www.blog.vehdjk.com/Article/details/gppctxoyf.sHtML

[U76] PHP：简单路由
来源：http://www.share.fktsv.cn/Article/details/gatlerhyk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.yfazqb.com/Article/details/gbltqloal.sHtML

[U77] PHP：模板渲染
来源：http://3g.fktsv.cn/Article/details/glqrlcimn.sHtML

composer require twig/twig
来源：http://wap.sjlbkw.cn/Article/details/gyfncyezu.sHtML

[U78] PHP：单元测试
来源：http://www.share.bbcook.cn/Article/details/gingmmzbm.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fktsv.cn/Article/details/gtlhptgyl.sHtML

[U79] PHP：静态分析
来源：http://read.share.sjlbkw.cn/Article/details/gzwjzylbq.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.vehdjk.com/Article/details/gsegqlfry.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.epnwcf.com/Article/details/gkbekeryy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fktsv.cn/Article/details/ghvdjggrb.sHtML

[U81] JS：初始化项目
来源：http://blog.fktsv.cn/Article/details/genzmnast.sHtML

npm init -y;  npm i express
来源：http://blog.fktsv.cn/Article/details/gwbfebgtf.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.sjlbkw.cn/Article/details/gfodyzwwf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.sjlbkw.cn/Article/details/gblhgvpuq.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.tarul.cn/Article/details/gpzpjagjj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.epnwcf.com/Article/details/gqmsjlqpj.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.bbcook.cn/Article/details/ganhnkkmf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.yfazqb.com/Article/details/gboptkrfv.sHtML

[U85] JS：可选链
来源：http://www.share.fktsv.cn/Article/details/gorufkskr.sHtML

a?.b?.c
来源：http://read.share.yfazqb.com/Article/details/gjvcxqxmb.sHtML

[U86] JS：空值合并
来源：http://wap.fktsv.cn/Article/details/ghnbhvmlz.sHtML

a ?? b
来源：http://www.share.yfazqb.com/Article/details/griuaswzy.sHtML

[U87] JS：解构默认值
来源：http://m.share.vehdjk.com/Article/details/ghzsrpnoi.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.vehdjk.com/Article/details/gssfohnna.sHtML

[U88] JS：对象展开合并
来源：http://wap.bbcook.cn/Article/details/gcqnptjnx.sHtML

{ ...a, ...b }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggzxoepnl.sHtML

[U89] JS：数组去重
来源：http://mobile.fktsv.cn/Article/details/guwrqpmlj.sHtML

[...new Set(arr)]
来源：http://baike.sjlbkw.cn/Article/details/ganxrmsvy.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.epnwcf.com/Article/details/gdwiswypv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.yfazqb.com/Article/details/glxspyudn.sHtML

[U91] JS：对象键值遍历
来源：http://wap.bbcook.cn/Article/details/gxjzgeffq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.bbcook.cn/Article/details/gvokyzxwi.sHtML

[U92] JS：深拷贝
来源：http://mobile.fktsv.cn/Article/details/gmidglqyl.sHtML

structuredClone(obj)
来源：http://www.blog.tarul.cn/Article/details/gonvqihne.sHtML

[U93] JS：模板字符串
来源：http://3g.epnwcf.com/Article/details/glqyohtkq.sHtML

`共 ${n} 条`
来源：http://www.blog.bbcook.cn/Article/details/griilbzdo.sHtML

[U94] JS：箭头函数
来源：http://wap.sjlbkw.cn/Article/details/guclbsdce.sHtML

const double = x => x * 2;
来源：http://wap.yfazqb.com/Article/details/gkctpjntu.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.bbcook.cn/Article/details/gfyqjahfe.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.vehdjk.com/Article/details/goenkwxhg.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.epnwcf.com/Article/details/gigyxznww.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.tarul.cn/Article/details/geibslgiw.sHtML

[U97] JS：并发请求
来源：http://wap.bbcook.cn/Article/details/gvbsjozyt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.bbcook.cn/Article/details/gnnrwpdrh.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.epnwcf.com/Article/details/glhnokkzh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.sjlbkw.cn/Article/details/gghthrzei.sHtML

[U99] JS：事件监听
来源：http://www.m.share.sjlbkw.cn/Article/details/giuddyzct.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.vehdjk.com/Article/details/gvezylrdy.sHtML

[U100] JS：DOM 查询
来源：http://mobile.sjlbkw.cn/Article/details/gpnzczedi.sHtML

document.querySelector(".item")
来源：http://wap.yfazqb.com/Article/details/grfpqzgvx.sHtML

[U101] JS：classList 操作
来源：http://3g.vehdjk.com/Article/details/gefhnbamc.sHtML

el.classList.toggle("active")
来源：http://read.share.sjlbkw.cn/Article/details/ghlksmubv.sHtML

[U102] JS：本地存储
来源：http://blog.tarul.cn/Article/details/gikwngbjm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.tarul.cn/Article/details/godkayygy.sHtML

[U103] JS：定时器
来源：http://baike.vehdjk.com/Article/details/gmhxoqawb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.yfazqb.com/Article/details/ghockkqsq.sHtML

[U104] JS：防抖
来源：http://wap.bbcook.cn/Article/details/gdvrezkvu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fktsv.cn/Article/details/gwfjufomk.sHtML

[U105] JS：节流
来源：http://3g.bbcook.cn/Article/details/gpvmelrzs.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.epnwcf.com/Article/details/gqkmzzotf.sHtML

[U106] JS：日期格式化
来源：http://mobile.fktsv.cn/Article/details/gpaprupkr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.epnwcf.com/Article/details/gjzjyzawg.sHtML

[U107] JS：数字千分位
来源：http://read.share.yfazqb.com/Article/details/gspvitxov.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.yfazqb.com/Article/details/ggbzeomjy.sHtML

[U108] JS：随机整数
来源：http://3g.vehdjk.com/Article/details/gfoswgmfd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.bbcook.cn/Article/details/gxvanlyoi.sHtML

[U109] JS：数组分组
来源：http://read.share.yfazqb.com/Article/details/gzslqrijt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.yfazqb.com/Article/details/gigsiwfyz.sHtML

[U110] JS：数组分块
来源：http://baike.yfazqb.com/Article/details/gpzdasziq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.tarul.cn/Article/details/gieacxess.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.yfazqb.com/Article/details/grrwohgyr.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fktsv.cn/Article/details/gxoojudvz.sHtML

[U112] JS：字符串补位
来源：http://www.blog.bbcook.cn/Article/details/gtputstvh.sHtML

"7".padStart(3, "0")
来源：http://mobile.bbcook.cn/Article/details/gavbezxnj.sHtML

[U113] JS：正则替换全部
来源：http://m.share.sjlbkw.cn/Article/details/gsmhqngdc.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/glhjhybim.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.epnwcf.com/Article/details/gqozmldei.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fktsv.cn/Article/details/gqobjrapa.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.tarul.cn/Article/details/gupvyzfex.sHtML

crypto.randomUUID()
来源：http://wap.vehdjk.com/Article/details/guhajplpj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.sjlbkw.cn/Article/details/gjkuzxgwn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhgffapl.sHtML

[U117] JS：单元测试
来源：http://www.blog.tarul.cn/Article/details/gtcafnfec.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fktsv.cn/Article/details/gyhpnkktm.sHtML

[U118] JS：开发服务器
来源：http://www.share.vehdjk.com/Article/details/gsdbewyjp.sHtML

npm i -D vite;  npx vite
来源：http://baike.tarul.cn/Article/details/gwiraroec.sHtML

[U119] JS：生产构建
来源：http://read.share.sjlbkw.cn/Article/details/gqgpwxgtt.sHtML

npx vite build
来源：http://read.share.epnwcf.com/Article/details/grklvfepk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fktsv.cn/Article/details/ggqiytovv.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.vehdjk.com/Article/details/gmejimvsg.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gyaubgozf.sHtML

统计汇总
来源：http://www.m.share.bbcook.cn/Article/details/ghvpmfgun.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gukjddrfj.sHtML

按语言统计（条）：
来源：http://blog.sjlbkw.cn/Article/details/ghdfazbgp.sHtML

Python ......... 252
来源：http://www.m.share.yfazqb.com/Article/details/gmkerdqhp.sHtML

PHP ............ 252
来源：http://m.share.tarul.cn/Article/details/gtoihcndu.sHtML

JavaScript ..... 252
来源：http://read.share.sjlbkw.cn/Article/details/gtocsdywk.sHtML

TypeScript ..... 212
来源：http://m.share.fktsv.cn/Article/details/gmpbegxbg.sHtML

Java ........... 212
来源：http://www.m.share.bbcook.cn/Article/details/golifvrzw.sHtML

Go ............. 212
来源：http://m.share.yfazqb.com/Article/details/gwvtxwraz.sHtML

Ruby ........... 212
来源：http://baike.sjlbkw.cn/Article/details/gqklqgnbe.sHtML

C# ............. 212
来源：http://read.share.fktsv.cn/Article/details/gzwfjtakp.sHtML

C .............. 30
来源：http://www.share.epnwcf.com/Article/details/gmnbaxhgh.sHtML

C++ ............ 30
来源：http://baike.yfazqb.com/Article/details/gfnourkpw.sHtML

SQL ............ 90
来源：http://www.share.yfazqb.com/Article/details/gpxxlqgdg.sHtML

Bash ........... 80
来源：http://wap.tarul.cn/Article/details/gtuwphnco.sHtML

Kotlin ......... 15
来源：http://www.blog.epnwcf.com/Article/details/gglrekhai.sHtML

Swift .......... 15
来源：http://read.share.bbcook.cn/Article/details/gdhwlcstq.sHtML

Lua ............ 10
来源：http://mobile.bbcook.cn/Article/details/gijdhohpc.sHtML

Perl ........... 10
来源：http://www.m.share.bbcook.cn/Article/details/gvigpfksf.sHtML

Scala .......... 10
来源：http://wap.tarul.cn/Article/details/gikxogrhq.sHtML

------------------------------------
来源：http://read.share.sjlbkw.cn/Article/details/ggzkqlkoe.sHtML

合计 ........... 2106 条
来源：http://3g.sjlbkw.cn/Article/details/gfhphsoyl.sHtML

按章节统计：
来源：http://baike.yfazqb.com/Article/details/gjuaflopx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.sjlbkw.cn/Article/details/gmwplthux.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.yfazqb.com/Article/details/gesgxotyh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.yfazqb.com/Article/details/gmjvoobom.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fktsv.cn/Article/details/grlxyhaxr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.tarul.cn/Article/details/gvejfmdmv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.sjlbkw.cn/Article/details/gdnuidbnf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fktsv.cn/Article/details/gfhifarec.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fktsv.cn/Article/details/gouamrier.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.bbcook.cn/Article/details/gasmimdsy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.vehdjk.com/Article/details/gfcjfmtjf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.bbcook.cn/Article/details/gsdiuucva.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fktsv.cn/Article/details/gdhlvxtrb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.sjlbkw.cn/Article/details/gidpkneqg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.bbcook.cn/Article/details/ghwfddmwz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.epnwcf.com/Article/details/gtuafbvyg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.yfazqb.com/Article/details/gyrydepog.sHtML

Q SQL 专题                              90
来源：http://read.share.epnwcf.com/Article/details/glohklgtu.sHtML

R Bash 专题                             80
来源：http://m.share.vehdjk.com/Article/details/gyofskoxp.sHtML

S C / C++ 专题                          60
来源：http://3g.fktsv.cn/Article/details/gagjnhgrb.sHtML

T 其他语言补充                          60
来源：http://baike.bbcook.cn/Article/details/ggoesyord.sHtML

U 高频实用片段                         120
来源：http://wap.epnwcf.com/Article/details/guosowkws.sHtML

------------------------------------
来源：http://www.share.vehdjk.com/Article/details/gdobjaugg.sHtML

合计                                  2106 条
来源：http://www.m.share.fktsv.cn/Article/details/gtgsrzimg.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.vehdjk.com/Article/details/golagzitd.sHtML

使用提醒
来源：http://mobile.vehdjk.com/Article/details/giwzcsjdp.sHtML

--------------------------------------------------------------------------------
来源：http://baike.sjlbkw.cn/Article/details/gflwizxej.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.epnwcf.com/Article/details/gmecjresz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.vehdjk.com/Article/details/gqjuwuhwl.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.epnwcf.com/Article/details/gksssauyn.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.vehdjk.com/Article/details/gbvhumkyi.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.vehdjk.com/Article/details/gtttefvxx.sHtML

—— 文件结束 ——
来源：http://mobile.tarul.cn/Article/details/gpzgjxtif.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gvwdnydvd.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.vehdjk.com/Article/details/guczrzkvi.sHtML

Common Programming Examples Cheat Book
来源：http://baike.sjlbkw.cn/Article/details/glfnuhijk.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/grspvvpgm.sHtML

【收录内容】
来源：http://baike.vehdjk.com/Article/details/ghmwmojik.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fktsv.cn/Article/details/gyjpqvmxi.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.epnwcf.com/Article/details/gpwjknfne.sHtML

SQL · Bash · C · C++
来源：http://www.share.fktsv.cn/Article/details/gjxtyuqdo.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.bbcook.cn/Article/details/gvbukhbgf.sHtML

【使用说明】
来源：http://wap.epnwcf.com/Article/details/gskgpqszw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.vehdjk.com/Article/details/gpankfwcv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.bbcook.cn/Article/details/guzblawab.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.epnwcf.com/Article/details/gajjhlyzk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.epnwcf.com/Article/details/gpjivkisl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.yfazqb.com/Article/details/gcofzdbfb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.epnwcf.com/Article/details/gyaaebbgp.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.tarul.cn/Article/details/glnmetnnn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.yfazqb.com/Article/details/gxevljvnc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.vehdjk.com/Article/details/gaarpmanr.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.yfazqb.com/Article/details/gloowprub.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.epnwcf.com/Article/details/gpayodpda.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.vehdjk.com/Article/details/gqccedqbd.sHtML

【文件统计】
来源：http://www.share.fktsv.cn/Article/details/gdslapwmr.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.bbcook.cn/Article/details/gneetqjtm.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fktsv.cn/Article/details/gumzelbwq.sHtML

目  录
来源：http://www.share.tarul.cn/Article/details/gdqboxyze.sHtML

--------------------------------------------------------------------------------
来源：http://blog.epnwcf.com/Article/details/gwtsthcqv.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.bbcook.cn/Article/details/gfgentqex.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.yfazqb.com/Article/details/galuanrbz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fktsv.cn/Article/details/gwngwqadk.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.vehdjk.com/Article/details/grdcuipni.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.yfazqb.com/Article/details/guvqvkrwn.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.tarul.cn/Article/details/gaynkzssj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.epnwcf.com/Article/details/gewwvgpew.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.yfazqb.com/Article/details/gtkvlwjgi.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.vehdjk.com/Article/details/girddmunv.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.fktsv.cn/Article/details/gcfnfxmve.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fktsv.cn/Article/details/ggpcfwufr.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.tarul.cn/Article/details/gmhueaxwl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.yfazqb.com/Article/details/gyxwrotbp.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.tarul.cn/Article/details/gmzuczflj.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.tarul.cn/Article/details/gtgeivsbr.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.yfazqb.com/Article/details/gxkvyistz.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.yfazqb.com/Article/details/gnmfylmzs.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.yfazqb.com/Article/details/ggfasjisu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.epnwcf.com/Article/details/gvinzwqbx.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.tarul.cn/Article/details/ghelcjjxw.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.vehdjk.com/Article/details/gmwrzozdi.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gqxxedtfz.sHtML

A. 基础语法与类型
来源：http://www.share.epnwcf.com/Article/details/gvwzddjnj.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/geubjyxqj.sHtML

[A01] Hello World
来源：http://read.share.sjlbkw.cn/Article/details/guhjzcerl.sHtML

Py:   print("Hello, World!")
来源：http://mobile.bbcook.cn/Article/details/gtxidjpkn.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.tarul.cn/Article/details/gfqmojfmg.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.epnwcf.com/Article/details/gaxlovqsa.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.vehdjk.com/Article/details/gyqdavzll.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.vehdjk.com/Article/details/gydjouhku.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.fktsv.cn/Article/details/gywjldmnu.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.epnwcf.com/Article/details/gzprrpxwu.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.yfazqb.com/Article/details/givmohtax.sHtML

[A02] 变量声明与赋值
来源：http://mobile.fktsv.cn/Article/details/ggcouecoi.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.vehdjk.com/Article/details/giuqcnwtt.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.bbcook.cn/Article/details/gbslsnzxg.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.tarul.cn/Article/details/gauoxryun.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.vehdjk.com/Article/details/gozjshabd.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.yfazqb.com/Article/details/gfuvugdua.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.yfazqb.com/Article/details/gddupphcc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fktsv.cn/Article/details/gbgaouwsc.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.fktsv.cn/Article/details/glfqhyddg.sHtML

[A03] 常量定义
来源：http://www.m.share.fktsv.cn/Article/details/grslhgqwm.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.epnwcf.com/Article/details/grfanswyp.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.yfazqb.com/Article/details/gtzcupatv.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gyxbupeur.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/gftzspxpf.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.yfazqb.com/Article/details/gepicbjbo.sHtML

Go:   const PI = 3.14159
来源：http://read.share.vehdjk.com/Article/details/gjajkqkge.sHtML

Ruby: PI = 3.14159
来源：http://baike.tarul.cn/Article/details/gohndryuh.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.bbcook.cn/Article/details/gmgzrcjhy.sHtML

[A04] 判断变量类型
来源：http://mobile.vehdjk.com/Article/details/gdbaeuegn.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.yfazqb.com/Article/details/gecbwruun.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.fktsv.cn/Article/details/gktaiphtz.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.yfazqb.com/Article/details/gbftadtkg.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.bbcook.cn/Article/details/gmgjvnral.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.bbcook.cn/Article/details/gqeaxhfnh.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.bbcook.cn/Article/details/gnujzjxej.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.vehdjk.com/Article/details/gfgujjarm.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.sjlbkw.cn/Article/details/guhxtassa.sHtML

[A05] 整数除法与取模
来源：http://baike.yfazqb.com/Article/details/gkgfcakik.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.tarul.cn/Article/details/gydidhyvk.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.bbcook.cn/Article/details/glmtjovit.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fktsv.cn/Article/details/gkplydgfk.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.bbcook.cn/Article/details/ghhraaghp.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.tarul.cn/Article/details/gwskrgupj.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.yfazqb.com/Article/details/gwzlazznz.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.tarul.cn/Article/details/ghlcexadd.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.epnwcf.com/Article/details/gnhmfetgf.sHtML

[A06] 字符串转数字
来源：http://baike.tarul.cn/Article/details/gudoifwaa.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.epnwcf.com/Article/details/gutgvrryf.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.epnwcf.com/Article/details/gknyozwvz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.tarul.cn/Article/details/glwtqjzeh.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.bbcook.cn/Article/details/gtjzokjmb.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.bbcook.cn/Article/details/gqujhbhar.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.fktsv.cn/Article/details/gznifmthz.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.fktsv.cn/Article/details/gojnvasjo.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.bbcook.cn/Article/details/gyrdgkhzv.sHtML

[A07] 数字转字符串
来源：http://mobile.fktsv.cn/Article/details/goczbibmr.sHtML

Py:   str(42)
来源：http://mobile.vehdjk.com/Article/details/gsmxswqvb.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.tarul.cn/Article/details/gsmvcqfkb.sHtML

JS:   String(42); (42).toString()
来源：http://3g.sjlbkw.cn/Article/details/gfidtbyqn.sHtML

TS:   String(42)
来源：http://www.m.share.fktsv.cn/Article/details/gyaseblzd.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.epnwcf.com/Article/details/gpcghudoz.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.bbcook.cn/Article/details/glxrsutjd.sHtML

Ruby: 42.to_s
来源：http://baike.fktsv.cn/Article/details/gjnbbzihj.sHtML

C#:   42.ToString()
来源：http://blog.bbcook.cn/Article/details/gksbrltzj.sHtML

[A08] 取整与四舍五入
来源：http://baike.bbcook.cn/Article/details/gkhkxjsqw.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.bbcook.cn/Article/details/ghfubsvlc.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.vehdjk.com/Article/details/gzohlylcc.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.yfazqb.com/Article/details/gwskyfoib.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.sjlbkw.cn/Article/details/gxfnoxecm.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.bbcook.cn/Article/details/gypvwzpls.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.fktsv.cn/Article/details/gsuczljbk.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.fktsv.cn/Article/details/grlzzoegj.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.vehdjk.com/Article/details/giqpfkrdd.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.epnwcf.com/Article/details/gszlkurhw.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.bbcook.cn/Article/details/gyxwwgewk.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.epnwcf.com/Article/details/gthcxflel.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.fktsv.cn/Article/details/gjfrvujsj.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.epnwcf.com/Article/details/gdbtqjnle.sHtML


<!-- 参考信息 -->