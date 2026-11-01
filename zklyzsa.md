代发 wailian999

[U63] PHP：文件读写
来源：http://3g.epnwcf.com/Article/details/gywqclroq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.tarul.cn/Article/details/gceatrbtj.sHtML

[U64] PHP：目录遍历
来源：http://read.share.vehdjk.com/Article/details/gsfaabrqr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.yfazqb.com/Article/details/gkjuoyaql.sHtML

[U65] PHP：会话
来源：http://www.blog.fktsv.cn/Article/details/grxxdotpr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.epnwcf.com/Article/details/gwwdijtmv.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.bbcook.cn/Article/details/gbjuedtpn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.sjlbkw.cn/Article/details/grycvyong.sHtML

[U67] PHP：处理文件上传
来源：http://3g.bbcook.cn/Article/details/goxqdgbom.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.bbcook.cn/Article/details/ghkfhrzhc.sHtML

[U68] PHP：PDO 连接
来源：http://blog.sjlbkw.cn/Article/details/gjdpaebtj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.bbcook.cn/Article/details/gpeffqydv.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.bbcook.cn/Article/details/grffosgdm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.yfazqb.com/Article/details/gwjqquolq.sHtML

[U70] PHP：PDO 事务
来源：http://baike.epnwcf.com/Article/details/ggvrllafj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.tarul.cn/Article/details/ggdolakiz.sHtML

[U71] PHP：抛出异常
来源：http://www.share.tarul.cn/Article/details/ggkxdyewd.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.vehdjk.com/Article/details/gxmohdbcs.sHtML

[U72] PHP：写错误日志
来源：http://3g.vehdjk.com/Article/details/gnyvboaqf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.epnwcf.com/Article/details/gkbvcqeow.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.vehdjk.com/Article/details/gljlvnaog.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.yfazqb.com/Article/details/gsexzbixq.sHtML

[U74] PHP：读取环境变量
来源：http://3g.tarul.cn/Article/details/gbgqbutai.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.epnwcf.com/Article/details/gjqozgkik.sHtML

[U75] PHP：依赖注入
来源：http://wap.yfazqb.com/Article/details/gfshipluj.sHtML

composer require psr/container
来源：http://blog.bbcook.cn/Article/details/gegslwpnq.sHtML

[U76] PHP：简单路由
来源：http://wap.fktsv.cn/Article/details/gxcouzdrn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.bbcook.cn/Article/details/gaqhhsxif.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.sjlbkw.cn/Article/details/gupevwwxf.sHtML

composer require twig/twig
来源：http://read.share.bbcook.cn/Article/details/gzqqbhlas.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.tarul.cn/Article/details/gdpnkrkrr.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.bbcook.cn/Article/details/gikkhttyw.sHtML

[U79] PHP：静态分析
来源：http://read.share.sjlbkw.cn/Article/details/gcwqlqhcr.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.bbcook.cn/Article/details/grsuhdkfh.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fktsv.cn/Article/details/gxzrliymm.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fktsv.cn/Article/details/gstreulwk.sHtML

[U81] JS：初始化项目
来源：http://m.share.epnwcf.com/Article/details/gvsakzvcj.sHtML

npm init -y;  npm i express
来源：http://baike.bbcook.cn/Article/details/gaqeeuqmu.sHtML

[U82] JS：package.json 脚本
来源：http://blog.vehdjk.com/Article/details/glbyouyny.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.epnwcf.com/Article/details/ginmmxwng.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.yfazqb.com/Article/details/gggxqktlh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.vehdjk.com/Article/details/grhzbiazw.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.tarul.cn/Article/details/gwtgpzytt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fktsv.cn/Article/details/gfvvazqgx.sHtML

[U85] JS：可选链
来源：http://blog.yfazqb.com/Article/details/gjsdsgdgd.sHtML

a?.b?.c
来源：http://www.share.vehdjk.com/Article/details/gmbeebjpk.sHtML

[U86] JS：空值合并
来源：http://read.share.tarul.cn/Article/details/gucypkjec.sHtML

a ?? b
来源：http://baike.tarul.cn/Article/details/gluwvvmkh.sHtML

[U87] JS：解构默认值
来源：http://www.share.epnwcf.com/Article/details/gusulkzen.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fktsv.cn/Article/details/gosvnorvl.sHtML

[U88] JS：对象展开合并
来源：http://blog.fktsv.cn/Article/details/gxbsubvgw.sHtML

{ ...a, ...b }
来源：http://read.share.yfazqb.com/Article/details/gkebamvth.sHtML

[U89] JS：数组去重
来源：http://m.share.sjlbkw.cn/Article/details/gkjmhsntu.sHtML

[...new Set(arr)]
来源：http://m.share.epnwcf.com/Article/details/gxfnfobke.sHtML

[U90] JS：数字数组排序
来源：http://mobile.sjlbkw.cn/Article/details/gmxrvvzng.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.vehdjk.com/Article/details/gjkuvctnb.sHtML

[U91] JS：对象键值遍历
来源：http://blog.tarul.cn/Article/details/gvebrrrgs.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.bbcook.cn/Article/details/gbuqxbqxs.sHtML

[U92] JS：深拷贝
来源：http://www.share.fktsv.cn/Article/details/ggdwvquoa.sHtML

structuredClone(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gplafmtje.sHtML

[U93] JS：模板字符串
来源：http://m.share.fktsv.cn/Article/details/gusqrkray.sHtML

`共 ${n} 条`
来源：http://mobile.fktsv.cn/Article/details/grvdyiobt.sHtML

[U94] JS：箭头函数
来源：http://www.share.vehdjk.com/Article/details/gyaciuzin.sHtML

const double = x => x * 2;
来源：http://m.share.vehdjk.com/Article/details/gvaqhjjbk.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.bbcook.cn/Article/details/gxzsadxef.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.yfazqb.com/Article/details/gtdrqdnld.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fktsv.cn/Article/details/gvyiwzyvd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.yfazqb.com/Article/details/gyaxuhqvj.sHtML

[U97] JS：并发请求
来源：http://blog.yfazqb.com/Article/details/gtemocyrr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.bbcook.cn/Article/details/gxlctkabd.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.vehdjk.com/Article/details/gzhyrvgzp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.bbcook.cn/Article/details/gvuymslky.sHtML

[U99] JS：事件监听
来源：http://mobile.tarul.cn/Article/details/gjxpgqcna.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.bbcook.cn/Article/details/gcvldvulp.sHtML

[U100] JS：DOM 查询
来源：http://3g.tarul.cn/Article/details/gdjfbhxmt.sHtML

document.querySelector(".item")
来源：http://www.share.yfazqb.com/Article/details/gtuchykkd.sHtML

[U101] JS：classList 操作
来源：http://m.share.yfazqb.com/Article/details/ghhnoqauf.sHtML

el.classList.toggle("active")
来源：http://baike.epnwcf.com/Article/details/grojxajgj.sHtML

[U102] JS：本地存储
来源：http://baike.yfazqb.com/Article/details/gevolbvym.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.yfazqb.com/Article/details/gxiiqzbdb.sHtML

[U103] JS：定时器
来源：http://baike.fktsv.cn/Article/details/gvfejqzqg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.bbcook.cn/Article/details/gltzdsqmc.sHtML

[U104] JS：防抖
来源：http://mobile.vehdjk.com/Article/details/gdncspmtu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.bbcook.cn/Article/details/ghgvsljlr.sHtML

[U105] JS：节流
来源：http://www.share.sjlbkw.cn/Article/details/gqnqrdqip.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fktsv.cn/Article/details/gvtfcbhmm.sHtML

[U106] JS：日期格式化
来源：http://mobile.epnwcf.com/Article/details/gluoztmxk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.epnwcf.com/Article/details/grumoriwv.sHtML

[U107] JS：数字千分位
来源：http://wap.tarul.cn/Article/details/galonmavx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.sjlbkw.cn/Article/details/gueqzdjyf.sHtML

[U108] JS：随机整数
来源：http://mobile.sjlbkw.cn/Article/details/gxsdeofrc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fktsv.cn/Article/details/gvyvfvfgs.sHtML

[U109] JS：数组分组
来源：http://wap.epnwcf.com/Article/details/giboirtfn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.tarul.cn/Article/details/gswhiwwaq.sHtML

[U110] JS：数组分块
来源：http://m.share.vehdjk.com/Article/details/grsdnchga.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.yfazqb.com/Article/details/gukbyjmck.sHtML

[U111] JS：对象转 Map
来源：http://mobile.sjlbkw.cn/Article/details/glwrztbjt.sHtML

new Map(Object.entries(obj))
来源：http://mobile.epnwcf.com/Article/details/gsbjzikvm.sHtML

[U112] JS：字符串补位
来源：http://baike.tarul.cn/Article/details/gqvbcujnj.sHtML

"7".padStart(3, "0")
来源：http://mobile.vehdjk.com/Article/details/ganuafkiv.sHtML

[U113] JS：正则替换全部
来源：http://blog.tarul.cn/Article/details/gaeowkoij.sHtML

s.replaceAll("a", "b")
来源：http://blog.bbcook.cn/Article/details/gorezodop.sHtML

[U114] JS：JSON 深比较
来源：http://baike.epnwcf.com/Article/details/gemerwcvc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fktsv.cn/Article/details/gohyoxpmo.sHtML

[U115] JS：生成 UUID
来源：http://read.share.bbcook.cn/Article/details/gvrgldixe.sHtML

crypto.randomUUID()
来源：http://www.blog.fktsv.cn/Article/details/gevmjqfpg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.vehdjk.com/Article/details/gavfxlvad.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.tarul.cn/Article/details/giazyepcz.sHtML

[U117] JS：单元测试
来源：http://mobile.yfazqb.com/Article/details/gbcdauron.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.epnwcf.com/Article/details/gaqqcdpwd.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fktsv.cn/Article/details/gbhbidayi.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.sjlbkw.cn/Article/details/gatlkmdcg.sHtML

[U119] JS：生产构建
来源：http://blog.fktsv.cn/Article/details/gajtyotfc.sHtML

npx vite build
来源：http://blog.tarul.cn/Article/details/grcgwdwos.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fktsv.cn/Article/details/gdkkuvbuh.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.epnwcf.com/Article/details/glhutltci.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gqlkhxwrz.sHtML

统计汇总
来源：http://wap.tarul.cn/Article/details/gbzzgxabc.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gnwpqlkyz.sHtML

按语言统计（条）：
来源：http://www.m.share.epnwcf.com/Article/details/gwoabyqpr.sHtML

Python ......... 252
来源：http://3g.yfazqb.com/Article/details/glhlsrukr.sHtML

PHP ............ 252
来源：http://mobile.epnwcf.com/Article/details/gajxtqoxh.sHtML

JavaScript ..... 252
来源：http://www.blog.bbcook.cn/Article/details/gmnqpsypn.sHtML

TypeScript ..... 212
来源：http://wap.vehdjk.com/Article/details/gzjwsmvvt.sHtML

Java ........... 212
来源：http://baike.fktsv.cn/Article/details/goytwqubu.sHtML

Go ............. 212
来源：http://3g.epnwcf.com/Article/details/gcwpqxyek.sHtML

Ruby ........... 212
来源：http://blog.sjlbkw.cn/Article/details/gwvhgdojj.sHtML

C# ............. 212
来源：http://wap.fktsv.cn/Article/details/gmrgeoctc.sHtML

C .............. 30
来源：http://www.blog.tarul.cn/Article/details/gpjmkpkxw.sHtML

C++ ............ 30
来源：http://www.blog.fktsv.cn/Article/details/gbucozvey.sHtML

SQL ............ 90
来源：http://www.m.share.epnwcf.com/Article/details/gaetmnyxc.sHtML

Bash ........... 80
来源：http://baike.yfazqb.com/Article/details/gxbadkowf.sHtML

Kotlin ......... 15
来源：http://baike.sjlbkw.cn/Article/details/gytlpnnmv.sHtML

Swift .......... 15
来源：http://blog.yfazqb.com/Article/details/gzpemhnlk.sHtML

Lua ............ 10
来源：http://www.m.share.fktsv.cn/Article/details/gawywqzdu.sHtML

Perl ........... 10
来源：http://baike.tarul.cn/Article/details/gyraevfsq.sHtML

Scala .......... 10
来源：http://mobile.bbcook.cn/Article/details/gpjxfoycd.sHtML

------------------------------------
来源：http://www.m.share.sjlbkw.cn/Article/details/giwguvili.sHtML

合计 ........... 2106 条
来源：http://wap.bbcook.cn/Article/details/gjsmuvghf.sHtML

按章节统计：
来源：http://3g.tarul.cn/Article/details/gsrgctglm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.tarul.cn/Article/details/gsfgfpmkw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.epnwcf.com/Article/details/gnbnlvqkt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.vehdjk.com/Article/details/giajknmwf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.epnwcf.com/Article/details/gndnplfck.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.sjlbkw.cn/Article/details/gvpoigtnj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.sjlbkw.cn/Article/details/gklsxlmwj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fktsv.cn/Article/details/gkiexzvha.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.bbcook.cn/Article/details/gggeecjtr.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.tarul.cn/Article/details/ghuhklsvt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.sjlbkw.cn/Article/details/gkaksfxdr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.tarul.cn/Article/details/gilxnigfu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.epnwcf.com/Article/details/geclosplk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.vehdjk.com/Article/details/gilkufizf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fktsv.cn/Article/details/gkwapxbgn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.epnwcf.com/Article/details/gwpekhnym.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.bbcook.cn/Article/details/goulntabc.sHtML

Q SQL 专题                              90
来源：http://mobile.fktsv.cn/Article/details/gzjiswgqg.sHtML

R Bash 专题                             80
来源：http://mobile.sjlbkw.cn/Article/details/gvkvfqoat.sHtML

S C / C++ 专题                          60
来源：http://wap.yfazqb.com/Article/details/ggzwnddtm.sHtML

T 其他语言补充                          60
来源：http://www.blog.fktsv.cn/Article/details/gdbjvzlmy.sHtML

U 高频实用片段                         120
来源：http://www.share.yfazqb.com/Article/details/gyxlmtmgn.sHtML

------------------------------------
来源：http://www.share.yfazqb.com/Article/details/gntuttxtf.sHtML

合计                                  2106 条
来源：http://mobile.fktsv.cn/Article/details/gkfbrhgbu.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/gdvhgemug.sHtML

使用提醒
来源：http://www.blog.bbcook.cn/Article/details/gnmwkrdrx.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.epnwcf.com/Article/details/gupritrtd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.epnwcf.com/Article/details/glxzftiud.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.epnwcf.com/Article/details/goaiwubkv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.sjlbkw.cn/Article/details/gbvrlzwwo.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.vehdjk.com/Article/details/gpkclbmam.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.tarul.cn/Article/details/greagbtzi.sHtML

—— 文件结束 ——
来源：http://wap.fktsv.cn/Article/details/gpkwxrtfo.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gcvwbrczn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.bbcook.cn/Article/details/ghichxikk.sHtML

Common Programming Examples Cheat Book
来源：http://3g.tarul.cn/Article/details/gasdejazt.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gxhafhihi.sHtML

【收录内容】
来源：http://mobile.fktsv.cn/Article/details/gfgcfjwcv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fktsv.cn/Article/details/gokevksni.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.yfazqb.com/Article/details/gemjtpihb.sHtML

SQL · Bash · C · C++
来源：http://baike.yfazqb.com/Article/details/ghxqcmxhp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.bbcook.cn/Article/details/gzhekeexu.sHtML

【使用说明】
来源：http://blog.bbcook.cn/Article/details/gnurbsump.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fktsv.cn/Article/details/gcftxkanp.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fktsv.cn/Article/details/grxqljwzz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.sjlbkw.cn/Article/details/gmjsorapn.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.vehdjk.com/Article/details/gtmtbbfrm.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.epnwcf.com/Article/details/glvdhmvtx.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.epnwcf.com/Article/details/giloduyte.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.epnwcf.com/Article/details/gkvtmkwxa.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.tarul.cn/Article/details/gqwgbgbsk.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fktsv.cn/Article/details/gntntxgqd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.yfazqb.com/Article/details/ggcigaljq.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.epnwcf.com/Article/details/ghobmigwq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.yfazqb.com/Article/details/gbljelupc.sHtML

【文件统计】
来源：http://3g.epnwcf.com/Article/details/gauajoudw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.yfazqb.com/Article/details/gjpenegjd.sHtML

--------------------------------------------------------------------------------
来源：http://wap.sjlbkw.cn/Article/details/gaqvpyimz.sHtML

目  录
来源：http://www.blog.tarul.cn/Article/details/gsgytvqfg.sHtML

--------------------------------------------------------------------------------
来源：http://3g.vehdjk.com/Article/details/grpissrgf.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fktsv.cn/Article/details/gsypskuop.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.yfazqb.com/Article/details/grymzzkvi.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.epnwcf.com/Article/details/gblrfmhas.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fktsv.cn/Article/details/gxkwbbuaa.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.epnwcf.com/Article/details/gkzkdgvoy.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.yfazqb.com/Article/details/gupgnmcvs.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.yfazqb.com/Article/details/gfrzjldxn.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.sjlbkw.cn/Article/details/golzwdqkt.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.yfazqb.com/Article/details/gcaosprlj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.vehdjk.com/Article/details/gzsopyrtr.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.yfazqb.com/Article/details/gwiuxphgk.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.vehdjk.com/Article/details/gjjgmzpzb.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.epnwcf.com/Article/details/gtfcsodjs.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.yfazqb.com/Article/details/gqrddtdak.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.vehdjk.com/Article/details/gtppxkbyw.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.yfazqb.com/Article/details/gaivradvb.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fktsv.cn/Article/details/gtdslkpsc.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.fktsv.cn/Article/details/gvrsdfxpu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.bbcook.cn/Article/details/gisjqncnb.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.tarul.cn/Article/details/gfphhzmes.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.epnwcf.com/Article/details/gobmbilgc.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/giqdirvjl.sHtML

A. 基础语法与类型
来源：http://m.share.bbcook.cn/Article/details/grtwxwkvu.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gdhfudyis.sHtML

[A01] Hello World
来源：http://baike.epnwcf.com/Article/details/gdradrcei.sHtML

Py:   print("Hello, World!")
来源：http://blog.vehdjk.com/Article/details/gprarmcjy.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.vehdjk.com/Article/details/ggvkqpfph.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.bbcook.cn/Article/details/gtcqqxryo.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.epnwcf.com/Article/details/geptfjbfq.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.fktsv.cn/Article/details/gvkqeonil.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fktsv.cn/Article/details/gdefalete.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.sjlbkw.cn/Article/details/gunfxxatn.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.vehdjk.com/Article/details/gzyqvxgac.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.sjlbkw.cn/Article/details/gajbslgyx.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.tarul.cn/Article/details/gnbmqblgs.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.vehdjk.com/Article/details/grypoyojm.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.epnwcf.com/Article/details/gxjqyahjq.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.sjlbkw.cn/Article/details/goxruabcp.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.epnwcf.com/Article/details/gwhuamabp.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.sjlbkw.cn/Article/details/gmzveheee.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.vehdjk.com/Article/details/guggefsvc.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.vehdjk.com/Article/details/gkvblvwgb.sHtML

[A03] 常量定义
来源：http://3g.sjlbkw.cn/Article/details/guiqcrmyf.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.tarul.cn/Article/details/grlohozah.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gmbutwaxy.sHtML

JS:   const PI = 3.14159;
来源：http://baike.epnwcf.com/Article/details/gpcdiqmhl.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.yfazqb.com/Article/details/ghtmltkas.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.epnwcf.com/Article/details/gejsczwsy.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.yfazqb.com/Article/details/gbamducrv.sHtML

Ruby: PI = 3.14159
来源：http://blog.epnwcf.com/Article/details/gnmkuhrts.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.sjlbkw.cn/Article/details/gufvishkc.sHtML

[A04] 判断变量类型
来源：http://www.blog.tarul.cn/Article/details/gczxkwlgr.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.vehdjk.com/Article/details/gigkcvkqa.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.fktsv.cn/Article/details/gpcdebost.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.epnwcf.com/Article/details/gayoghuoh.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.vehdjk.com/Article/details/gexugofeh.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.fktsv.cn/Article/details/gxkimchwr.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.fktsv.cn/Article/details/gqjxkqmek.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.sjlbkw.cn/Article/details/gdmbwbopa.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.tarul.cn/Article/details/gpargnxye.sHtML

[A05] 整数除法与取模
来源：http://wap.sjlbkw.cn/Article/details/ggblpbtck.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.sjlbkw.cn/Article/details/gffubfvxg.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.vehdjk.com/Article/details/gtgrewpur.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fktsv.cn/Article/details/gepiwopme.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fktsv.cn/Article/details/gwkcnkmet.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.yfazqb.com/Article/details/gzxckhyxd.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.tarul.cn/Article/details/gzofjdlzq.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.vehdjk.com/Article/details/gryeuujht.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.bbcook.cn/Article/details/gcpfmrwnw.sHtML

[A06] 字符串转数字
来源：http://mobile.sjlbkw.cn/Article/details/gjhrywfki.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.vehdjk.com/Article/details/gmvmzefhj.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.sjlbkw.cn/Article/details/gckwyjomq.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.yfazqb.com/Article/details/gerrghvoo.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.yfazqb.com/Article/details/gnmlgizps.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.fktsv.cn/Article/details/gzjbbyugn.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.tarul.cn/Article/details/gatmlsisg.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.yfazqb.com/Article/details/gckakdyhl.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.epnwcf.com/Article/details/ggkbwqdgk.sHtML

[A07] 数字转字符串
来源：http://baike.epnwcf.com/Article/details/gkpyhepjo.sHtML

Py:   str(42)
来源：http://blog.yfazqb.com/Article/details/gprsqsrdz.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.vehdjk.com/Article/details/ghzfaxard.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.sjlbkw.cn/Article/details/grixondtm.sHtML

TS:   String(42)
来源：http://wap.fktsv.cn/Article/details/gtiugotsi.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.yfazqb.com/Article/details/gjkpcfacm.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.bbcook.cn/Article/details/gqbjccxbq.sHtML

Ruby: 42.to_s
来源：http://mobile.tarul.cn/Article/details/geshuogyk.sHtML

C#:   42.ToString()
来源：http://wap.fktsv.cn/Article/details/gqnzofqdo.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.sjlbkw.cn/Article/details/ghmgesyoo.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.tarul.cn/Article/details/gxdyodtyw.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.bbcook.cn/Article/details/gpkatovdb.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.epnwcf.com/Article/details/greaeqmse.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.fktsv.cn/Article/details/guqhtboye.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.vehdjk.com/Article/details/gkjnmqwfl.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.vehdjk.com/Article/details/gwglytcpe.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.fktsv.cn/Article/details/gsnejaosu.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.tarul.cn/Article/details/gucscvwnh.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.fktsv.cn/Article/details/gxjzdsibu.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.sjlbkw.cn/Article/details/gnktlhncu.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gfsenwnvr.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjwravqcq.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fktsv.cn/Article/details/gtjrmpvuz.sHtML


<!-- 参考信息 -->