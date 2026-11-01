代发 wailian999

[U59] PHP：自定义排序
来源：http://3g.bbcook.cn/Article/details/gphujyibh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.sjlbkw.cn/Article/details/gridvtczi.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.vehdjk.com/Article/details/gicxrdvhv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.bbcook.cn/Article/details/gmsrrntkh.sHtML

[U61] PHP：正则
来源：http://www.m.share.sjlbkw.cn/Article/details/gegrgpbqi.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.yfazqb.com/Article/details/gimzbnzpl.sHtML

[U62] PHP：日期对象
来源：http://baike.vehdjk.com/Article/details/gxpvkcfkj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.tarul.cn/Article/details/gzxssrzbm.sHtML

[U63] PHP：文件读写
来源：http://www.share.bbcook.cn/Article/details/gorkhmvst.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.vehdjk.com/Article/details/goxvcjyng.sHtML

[U64] PHP：目录遍历
来源：http://mobile.bbcook.cn/Article/details/ggivofmwe.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.tarul.cn/Article/details/goxrkopzb.sHtML

[U65] PHP：会话
来源：http://blog.sjlbkw.cn/Article/details/glefylasm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.vehdjk.com/Article/details/goeelrmov.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.tarul.cn/Article/details/gckwjrljo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.bbcook.cn/Article/details/gyznhknrh.sHtML

[U67] PHP：处理文件上传
来源：http://baike.yfazqb.com/Article/details/gybxcjtnb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.bbcook.cn/Article/details/gngsddvtb.sHtML

[U68] PHP：PDO 连接
来源：http://blog.bbcook.cn/Article/details/goagmakra.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.bbcook.cn/Article/details/gvrirdwgs.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.epnwcf.com/Article/details/gjdaveixy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fktsv.cn/Article/details/gnaaegmsg.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.vehdjk.com/Article/details/gmehozkkp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.vehdjk.com/Article/details/gsasdhxlx.sHtML

[U71] PHP：抛出异常
来源：http://blog.bbcook.cn/Article/details/gkeagpenq.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fktsv.cn/Article/details/gakwlogcz.sHtML

[U72] PHP：写错误日志
来源：http://m.share.epnwcf.com/Article/details/gqqqtgoaw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.vehdjk.com/Article/details/guwxlaivh.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fktsv.cn/Article/details/gkpswrplr.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.vehdjk.com/Article/details/gmvsyhpso.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.tarul.cn/Article/details/gydllvmlr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fktsv.cn/Article/details/gfeqxvzwy.sHtML

[U75] PHP：依赖注入
来源：http://www.share.bbcook.cn/Article/details/glzmnjlxp.sHtML

composer require psr/container
来源：http://www.blog.vehdjk.com/Article/details/grnwzemrh.sHtML

[U76] PHP：简单路由
来源：http://www.blog.sjlbkw.cn/Article/details/gmbuiwtez.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.sjlbkw.cn/Article/details/ghmgsrhpk.sHtML

[U77] PHP：模板渲染
来源：http://mobile.bbcook.cn/Article/details/gcjfizcbk.sHtML

composer require twig/twig
来源：http://www.m.share.bbcook.cn/Article/details/gimjbvzll.sHtML

[U78] PHP：单元测试
来源：http://www.blog.epnwcf.com/Article/details/gyjmcirzt.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.bbcook.cn/Article/details/grlugvioo.sHtML

[U79] PHP：静态分析
来源：http://read.share.sjlbkw.cn/Article/details/gfhesmzjf.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.yfazqb.com/Article/details/gdjtyvwen.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.epnwcf.com/Article/details/gwmjmvwvc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.tarul.cn/Article/details/gceslbgdp.sHtML

[U81] JS：初始化项目
来源：http://www.blog.sjlbkw.cn/Article/details/gzjceotvv.sHtML

npm init -y;  npm i express
来源：http://www.blog.tarul.cn/Article/details/ghxmlzheg.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.bbcook.cn/Article/details/gaqsqwcfv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fktsv.cn/Article/details/gbyqmuqbm.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.bbcook.cn/Article/details/gbwhaczlw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fktsv.cn/Article/details/gvfvplvnn.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.epnwcf.com/Article/details/gngggbmac.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.vehdjk.com/Article/details/gcdqrecxv.sHtML

[U85] JS：可选链
来源：http://www.blog.fktsv.cn/Article/details/ghcqaueor.sHtML

a?.b?.c
来源：http://baike.tarul.cn/Article/details/ghuylelzn.sHtML

[U86] JS：空值合并
来源：http://www.m.share.yfazqb.com/Article/details/gurtvfrdg.sHtML

a ?? b
来源：http://www.share.bbcook.cn/Article/details/gtgrnnoqp.sHtML

[U87] JS：解构默认值
来源：http://3g.tarul.cn/Article/details/glykhjjgx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.bbcook.cn/Article/details/gehbuzbtx.sHtML

[U88] JS：对象展开合并
来源：http://blog.epnwcf.com/Article/details/grbvlmvav.sHtML

{ ...a, ...b }
来源：http://mobile.fktsv.cn/Article/details/gcfskkjga.sHtML

[U89] JS：数组去重
来源：http://mobile.fktsv.cn/Article/details/gjgurqrte.sHtML

[...new Set(arr)]
来源：http://baike.vehdjk.com/Article/details/gubhtkdet.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fktsv.cn/Article/details/gxkazkckf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.bbcook.cn/Article/details/gzxfbfmch.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.bbcook.cn/Article/details/gcgveckea.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.bbcook.cn/Article/details/gmkhogptb.sHtML

[U92] JS：深拷贝
来源：http://blog.fktsv.cn/Article/details/glevddvln.sHtML

structuredClone(obj)
来源：http://read.share.fktsv.cn/Article/details/gsbfjrjij.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.bbcook.cn/Article/details/gvcostsfj.sHtML

`共 ${n} 条`
来源：http://wap.yfazqb.com/Article/details/grjlxsszq.sHtML

[U94] JS：箭头函数
来源：http://www.blog.epnwcf.com/Article/details/gpyqrnkku.sHtML

const double = x => x * 2;
来源：http://www.m.share.fktsv.cn/Article/details/gypcmryly.sHtML

[U95] JS：Promise 包装
来源：http://www.share.yfazqb.com/Article/details/glpvvkglh.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fktsv.cn/Article/details/gwrcemqpm.sHtML

[U96] JS：async/await 与异常
来源：http://3g.epnwcf.com/Article/details/gasghmcef.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.bbcook.cn/Article/details/gbzazemvt.sHtML

[U97] JS：并发请求
来源：http://read.share.yfazqb.com/Article/details/gwkjtojem.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.epnwcf.com/Article/details/gpptoopae.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.epnwcf.com/Article/details/gdasuowds.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.tarul.cn/Article/details/gdmvoarip.sHtML

[U99] JS：事件监听
来源：http://m.share.bbcook.cn/Article/details/gdfxpxhzb.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.epnwcf.com/Article/details/gmbxctxag.sHtML

[U100] JS：DOM 查询
来源：http://m.share.vehdjk.com/Article/details/gqsnuwhkz.sHtML

document.querySelector(".item")
来源：http://www.blog.epnwcf.com/Article/details/gkkjrncxb.sHtML

[U101] JS：classList 操作
来源：http://baike.fktsv.cn/Article/details/gfkkvexyg.sHtML

el.classList.toggle("active")
来源：http://m.share.sjlbkw.cn/Article/details/gxjcwqugf.sHtML

[U102] JS：本地存储
来源：http://mobile.epnwcf.com/Article/details/ghinhhzmt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.vehdjk.com/Article/details/grucfaaww.sHtML

[U103] JS：定时器
来源：http://blog.vehdjk.com/Article/details/gpgwbmker.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.epnwcf.com/Article/details/gmjndpigo.sHtML

[U104] JS：防抖
来源：http://www.share.epnwcf.com/Article/details/gtxgexakm.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.bbcook.cn/Article/details/gvhktkdcq.sHtML

[U105] JS：节流
来源：http://3g.epnwcf.com/Article/details/gdxdpjrwr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.tarul.cn/Article/details/gwnesqqdj.sHtML

[U106] JS：日期格式化
来源：http://wap.yfazqb.com/Article/details/gpvyslzgd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fktsv.cn/Article/details/gxomkwrke.sHtML

[U107] JS：数字千分位
来源：http://blog.vehdjk.com/Article/details/getxpbclw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.yfazqb.com/Article/details/gtidszkcl.sHtML

[U108] JS：随机整数
来源：http://m.share.yfazqb.com/Article/details/gkrkqfpxv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.vehdjk.com/Article/details/gwttwmuqk.sHtML

[U109] JS：数组分组
来源：http://mobile.epnwcf.com/Article/details/ggurpqkpu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fktsv.cn/Article/details/gljpalqbd.sHtML

[U110] JS：数组分块
来源：http://read.share.bbcook.cn/Article/details/gqnthvszr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.sjlbkw.cn/Article/details/gjahmweaz.sHtML

[U111] JS：对象转 Map
来源：http://wap.tarul.cn/Article/details/gxdvsankn.sHtML

new Map(Object.entries(obj))
来源：http://mobile.tarul.cn/Article/details/gdohudlws.sHtML

[U112] JS：字符串补位
来源：http://blog.bbcook.cn/Article/details/gexfjcedc.sHtML

"7".padStart(3, "0")
来源：http://baike.vehdjk.com/Article/details/gsvkjvkym.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fktsv.cn/Article/details/ggrwyvcdl.sHtML

s.replaceAll("a", "b")
来源：http://blog.vehdjk.com/Article/details/gvqvnbuem.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.sjlbkw.cn/Article/details/grkbhilva.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.vehdjk.com/Article/details/gbbqavcdz.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.bbcook.cn/Article/details/gerbdkjlv.sHtML

crypto.randomUUID()
来源：http://www.blog.fktsv.cn/Article/details/gffrlwdfm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.epnwcf.com/Article/details/gdkmswgmb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.tarul.cn/Article/details/gvqejfbmf.sHtML

[U117] JS：单元测试
来源：http://www.blog.fktsv.cn/Article/details/godqwydes.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.sjlbkw.cn/Article/details/gwcbsylts.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.vehdjk.com/Article/details/gvyiimhbi.sHtML

npm i -D vite;  npx vite
来源：http://mobile.vehdjk.com/Article/details/gouumhsni.sHtML

[U119] JS：生产构建
来源：http://baike.sjlbkw.cn/Article/details/glfbnlntn.sHtML

npx vite build
来源：http://www.blog.yfazqb.com/Article/details/gqabhjbjh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.yfazqb.com/Article/details/guatavtob.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.vehdjk.com/Article/details/gbnqbdxve.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gkkigxoxq.sHtML

统计汇总
来源：http://blog.sjlbkw.cn/Article/details/gpcdztgmo.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gsuiznwjg.sHtML

按语言统计（条）：
来源：http://www.blog.vehdjk.com/Article/details/gwstfzehm.sHtML

Python ......... 252
来源：http://www.m.share.bbcook.cn/Article/details/glgajfeya.sHtML

PHP ............ 252
来源：http://www.blog.tarul.cn/Article/details/gztjfqepn.sHtML

JavaScript ..... 252
来源：http://wap.yfazqb.com/Article/details/gptlduflv.sHtML

TypeScript ..... 212
来源：http://www.share.vehdjk.com/Article/details/ggcrwmqxo.sHtML

Java ........... 212
来源：http://www.share.bbcook.cn/Article/details/gpyeutiif.sHtML

Go ............. 212
来源：http://www.share.sjlbkw.cn/Article/details/gvizhhhki.sHtML

Ruby ........... 212
来源：http://wap.sjlbkw.cn/Article/details/gbqusjzyw.sHtML

C# ............. 212
来源：http://www.m.share.epnwcf.com/Article/details/gnynfehbu.sHtML

C .............. 30
来源：http://baike.fktsv.cn/Article/details/gvocgmlol.sHtML

C++ ............ 30
来源：http://wap.tarul.cn/Article/details/gcrpelhlu.sHtML

SQL ............ 90
来源：http://wap.fktsv.cn/Article/details/gxoxnamoh.sHtML

Bash ........... 80
来源：http://www.m.share.sjlbkw.cn/Article/details/goppjrbxn.sHtML

Kotlin ......... 15
来源：http://www.m.share.bbcook.cn/Article/details/gwoebimqh.sHtML

Swift .......... 15
来源：http://read.share.fktsv.cn/Article/details/gahxdlzjm.sHtML

Lua ............ 10
来源：http://blog.epnwcf.com/Article/details/gbyywtwng.sHtML

Perl ........... 10
来源：http://baike.bbcook.cn/Article/details/gwzhnpoit.sHtML

Scala .......... 10
来源：http://read.share.vehdjk.com/Article/details/ggzfqwhrp.sHtML

------------------------------------
来源：http://m.share.sjlbkw.cn/Article/details/geykhwujj.sHtML

合计 ........... 2106 条
来源：http://mobile.yfazqb.com/Article/details/gnxrorupl.sHtML

按章节统计：
来源：http://blog.bbcook.cn/Article/details/gkmdslibz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fktsv.cn/Article/details/goyptrfgk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.yfazqb.com/Article/details/gcepwsxyp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.sjlbkw.cn/Article/details/gfobdujnc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.sjlbkw.cn/Article/details/gkwqarblh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.bbcook.cn/Article/details/gqnmpafpi.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.vehdjk.com/Article/details/geijdwnyh.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.vehdjk.com/Article/details/gkvpbcuwq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fktsv.cn/Article/details/gjagvprbs.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.bbcook.cn/Article/details/gdqyflbwo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.sjlbkw.cn/Article/details/gfrtfnzgi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.vehdjk.com/Article/details/gblffrllr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.epnwcf.com/Article/details/gjyfyczms.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.bbcook.cn/Article/details/gkmuesiso.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.vehdjk.com/Article/details/gtdfcnjvx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.tarul.cn/Article/details/gyhpsnwjd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.bbcook.cn/Article/details/gezjggvyw.sHtML

Q SQL 专题                              90
来源：http://mobile.bbcook.cn/Article/details/gotdluvjo.sHtML

R Bash 专题                             80
来源：http://wap.vehdjk.com/Article/details/gfmyyfzjo.sHtML

S C / C++ 专题                          60
来源：http://m.share.vehdjk.com/Article/details/gapxqrpxj.sHtML

T 其他语言补充                          60
来源：http://mobile.sjlbkw.cn/Article/details/gsnqdonbu.sHtML

U 高频实用片段                         120
来源：http://3g.yfazqb.com/Article/details/gjeuyjxrs.sHtML

------------------------------------
来源：http://www.blog.bbcook.cn/Article/details/gxsbcjezl.sHtML

合计                                  2106 条
来源：http://read.share.epnwcf.com/Article/details/gicxxjysy.sHtML

--------------------------------------------------------------------------------
来源：http://3g.bbcook.cn/Article/details/gxfawmhzn.sHtML

使用提醒
来源：http://3g.yfazqb.com/Article/details/gbdoawgpr.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.yfazqb.com/Article/details/gnmhkzvyz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.bbcook.cn/Article/details/ggllqkmvf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.epnwcf.com/Article/details/gdqooqpun.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.yfazqb.com/Article/details/gaiqnfsxo.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.bbcook.cn/Article/details/gdrjgsthf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.tarul.cn/Article/details/gpztyhoom.sHtML

—— 文件结束 ——
来源：http://blog.epnwcf.com/Article/details/glvwinwdt.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/guxrnwoux.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fktsv.cn/Article/details/goqtoyfio.sHtML

Common Programming Examples Cheat Book
来源：http://wap.bbcook.cn/Article/details/gssjgwfms.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gcsxuidbh.sHtML

【收录内容】
来源：http://www.share.bbcook.cn/Article/details/gykmxefki.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.vehdjk.com/Article/details/gazxsfhlo.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.sjlbkw.cn/Article/details/ghmdszhnl.sHtML

SQL · Bash · C · C++
来源：http://blog.yfazqb.com/Article/details/goidweoql.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.yfazqb.com/Article/details/gragcssqz.sHtML

【使用说明】
来源：http://mobile.epnwcf.com/Article/details/gxcrqvuug.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.vehdjk.com/Article/details/ghalegrkk.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.tarul.cn/Article/details/govnouxxm.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.yfazqb.com/Article/details/gjgbywonj.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.sjlbkw.cn/Article/details/gyxpvkutp.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.vehdjk.com/Article/details/gqqdusqei.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.bbcook.cn/Article/details/gzzhyxiun.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.vehdjk.com/Article/details/ghlbyukyf.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.tarul.cn/Article/details/gpzdzxjoa.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.vehdjk.com/Article/details/gmlqlhwyp.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.vehdjk.com/Article/details/ghrobrxvl.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.yfazqb.com/Article/details/gilnxrlbh.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.yfazqb.com/Article/details/giweyrthe.sHtML

【文件统计】
来源：http://wap.bbcook.cn/Article/details/gkbbnfkla.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.vehdjk.com/Article/details/gjxqkmxdk.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.tarul.cn/Article/details/gztoczqpa.sHtML

目  录
来源：http://baike.yfazqb.com/Article/details/ggdygkttv.sHtML

--------------------------------------------------------------------------------
来源：http://blog.vehdjk.com/Article/details/gyjaifron.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.fktsv.cn/Article/details/gecpjruii.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.bbcook.cn/Article/details/gbaakwiyr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.vehdjk.com/Article/details/gwsxleygv.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fktsv.cn/Article/details/gtpyjufzy.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.sjlbkw.cn/Article/details/gqpzrhqwy.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fktsv.cn/Article/details/gtjhkqvqx.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.yfazqb.com/Article/details/gylzncpnw.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.vehdjk.com/Article/details/giyuayewp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.yfazqb.com/Article/details/gbngcpixs.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.bbcook.cn/Article/details/germrruxq.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.epnwcf.com/Article/details/gggfmnbqf.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.bbcook.cn/Article/details/ghnkwofql.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.tarul.cn/Article/details/gbssnwhls.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.epnwcf.com/Article/details/gqttngnqd.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.bbcook.cn/Article/details/gftthoduy.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.tarul.cn/Article/details/gyecfbvvh.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.bbcook.cn/Article/details/gouzdzjny.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.yfazqb.com/Article/details/gfravwsgb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fktsv.cn/Article/details/gmhlwygyw.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.sjlbkw.cn/Article/details/gckmzcdnl.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.yfazqb.com/Article/details/gegoqttto.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gwdvidped.sHtML

A. 基础语法与类型
来源：http://www.share.bbcook.cn/Article/details/gbcukafmn.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gzjfsqyre.sHtML

[A01] Hello World
来源：http://read.share.epnwcf.com/Article/details/gawefqgqt.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.sjlbkw.cn/Article/details/gnjldqyfe.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.sjlbkw.cn/Article/details/ghmeyflwp.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.sjlbkw.cn/Article/details/gbuwcgaad.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.epnwcf.com/Article/details/gmicvaokf.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.epnwcf.com/Article/details/gupvzrkae.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.sjlbkw.cn/Article/details/gmbbeypmv.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.bbcook.cn/Article/details/ggmagcuzs.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.bbcook.cn/Article/details/gikevegck.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.vehdjk.com/Article/details/gasdpdnwv.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.yfazqb.com/Article/details/gyidkptyx.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.vehdjk.com/Article/details/girybakfj.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.epnwcf.com/Article/details/grecpjdvk.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.yfazqb.com/Article/details/ghpeoikjg.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.epnwcf.com/Article/details/gpazcnphi.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.yfazqb.com/Article/details/gogytipjk.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fktsv.cn/Article/details/ggdysaesi.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.vehdjk.com/Article/details/gsfxrwdrv.sHtML

[A03] 常量定义
来源：http://3g.fktsv.cn/Article/details/gbtzzsfnz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.sjlbkw.cn/Article/details/gvpbajokq.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.tarul.cn/Article/details/gtxbagqof.sHtML

JS:   const PI = 3.14159;
来源：http://baike.bbcook.cn/Article/details/gmumqtwnn.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.vehdjk.com/Article/details/gurvsswmh.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/ghgioxebm.sHtML

Go:   const PI = 3.14159
来源：http://blog.tarul.cn/Article/details/gnlafryjc.sHtML

Ruby: PI = 3.14159
来源：http://m.share.yfazqb.com/Article/details/gxvsuwbok.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.epnwcf.com/Article/details/gaunqavim.sHtML

[A04] 判断变量类型
来源：http://www.share.fktsv.cn/Article/details/gbuaitinu.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.epnwcf.com/Article/details/gldihkohw.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.sjlbkw.cn/Article/details/gnqxbqxfq.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.bbcook.cn/Article/details/gzgczqmim.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.sjlbkw.cn/Article/details/gmjdywjxb.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.fktsv.cn/Article/details/gbtmsquau.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.epnwcf.com/Article/details/gpheutduh.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.yfazqb.com/Article/details/guslrmuhq.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.bbcook.cn/Article/details/gidepzoyy.sHtML

[A05] 整数除法与取模
来源：http://www.share.tarul.cn/Article/details/gvthuvdvz.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.sjlbkw.cn/Article/details/gmvcyqega.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.vehdjk.com/Article/details/guummquqz.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.bbcook.cn/Article/details/grsxnotvs.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fktsv.cn/Article/details/glqkkemwk.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.sjlbkw.cn/Article/details/glcpamhli.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.fktsv.cn/Article/details/gexearrrc.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.tarul.cn/Article/details/gbhflwdmt.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.fktsv.cn/Article/details/geqnauurt.sHtML

[A06] 字符串转数字
来源：http://www.m.share.epnwcf.com/Article/details/gqgzwaezg.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.vehdjk.com/Article/details/ghnvffbxr.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.fktsv.cn/Article/details/gfcelvtzk.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.epnwcf.com/Article/details/gdghzwafs.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.fktsv.cn/Article/details/ganchshev.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.vehdjk.com/Article/details/gpqhbmddb.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.epnwcf.com/Article/details/gjutmygcy.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.epnwcf.com/Article/details/grkenllqm.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.vehdjk.com/Article/details/gkdbpoocx.sHtML

[A07] 数字转字符串
来源：http://mobile.fktsv.cn/Article/details/gmycskwus.sHtML

Py:   str(42)
来源：http://blog.sjlbkw.cn/Article/details/gaumfcamy.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.sjlbkw.cn/Article/details/gzjxlofqy.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.fktsv.cn/Article/details/giesuyvpr.sHtML

TS:   String(42)
来源：http://baike.fktsv.cn/Article/details/gtseyiaaz.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.sjlbkw.cn/Article/details/gmtdugcki.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.vehdjk.com/Article/details/gdyqojsrq.sHtML

Ruby: 42.to_s
来源：http://read.share.bbcook.cn/Article/details/gzlrkoyeh.sHtML

C#:   42.ToString()
来源：http://www.share.bbcook.cn/Article/details/gglnlojec.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.fktsv.cn/Article/details/gudpayvqm.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.fktsv.cn/Article/details/gytpwajky.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.tarul.cn/Article/details/geixpalxb.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.epnwcf.com/Article/details/gifardjtk.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.yfazqb.com/Article/details/ghkzdhfhg.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.vehdjk.com/Article/details/gksobsxom.sHtML


<!-- 参考信息 -->