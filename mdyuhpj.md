代发 wailian999

[U57] PHP：字符串插值
来源：http://3g.vehdjk.com/Article/details/ggjezrdxk.sHtML

"值: {$a}"
来源：http://www.blog.fktsv.cn/Article/details/gijqeybqh.sHtML

[U58] PHP：数组三件套
来源：http://m.share.yfazqb.com/Article/details/giomninun.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.vehdjk.com/Article/details/gzjsftzfe.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.bbcook.cn/Article/details/ggczcclfn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.sjlbkw.cn/Article/details/gxedaobpc.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.bbcook.cn/Article/details/grpzpnrrj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.sjlbkw.cn/Article/details/gcyumwytd.sHtML

[U61] PHP：正则
来源：http://www.m.share.vehdjk.com/Article/details/gzycofgez.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.yfazqb.com/Article/details/gptjekxzp.sHtML

[U62] PHP：日期对象
来源：http://blog.bbcook.cn/Article/details/girqetkbj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.bbcook.cn/Article/details/gvcwnltgu.sHtML

[U63] PHP：文件读写
来源：http://www.share.sjlbkw.cn/Article/details/gvlmjybqt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.vehdjk.com/Article/details/ggyootqrc.sHtML

[U64] PHP：目录遍历
来源：http://mobile.bbcook.cn/Article/details/gkohkqvmf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.vehdjk.com/Article/details/ggvnacysk.sHtML

[U65] PHP：会话
来源：http://m.share.tarul.cn/Article/details/gqrpabwuf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.bbcook.cn/Article/details/gyttupapq.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.vehdjk.com/Article/details/ggmfzelxe.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fktsv.cn/Article/details/gvkeofrqd.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.bbcook.cn/Article/details/gshtuooch.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.sjlbkw.cn/Article/details/gboakpmxb.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.tarul.cn/Article/details/gtpyamkpm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fktsv.cn/Article/details/glypbmacm.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.yfazqb.com/Article/details/gvrsrkdgx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.epnwcf.com/Article/details/gjydckwru.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.sjlbkw.cn/Article/details/gxqkeggnw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.vehdjk.com/Article/details/gujkwrxnz.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fktsv.cn/Article/details/glicvuccz.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.sjlbkw.cn/Article/details/guhdmlmtl.sHtML

[U72] PHP：写错误日志
来源：http://m.share.sjlbkw.cn/Article/details/gqfvckotg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.vehdjk.com/Article/details/gugjbyclh.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.yfazqb.com/Article/details/gzbzjeahe.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.tarul.cn/Article/details/gzdwbbepb.sHtML

[U74] PHP：读取环境变量
来源：http://wap.sjlbkw.cn/Article/details/gedkvdfsg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.epnwcf.com/Article/details/gkbhfnyhf.sHtML

[U75] PHP：依赖注入
来源：http://mobile.bbcook.cn/Article/details/gbddqrvml.sHtML

composer require psr/container
来源：http://wap.yfazqb.com/Article/details/gvtjpcrbe.sHtML

[U76] PHP：简单路由
来源：http://3g.sjlbkw.cn/Article/details/ghecmxzmt.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.tarul.cn/Article/details/ghciysxhe.sHtML

[U77] PHP：模板渲染
来源：http://m.share.yfazqb.com/Article/details/gfcllhtoi.sHtML

composer require twig/twig
来源：http://mobile.fktsv.cn/Article/details/gohfepcai.sHtML

[U78] PHP：单元测试
来源：http://blog.epnwcf.com/Article/details/gindjajnw.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.epnwcf.com/Article/details/gdmvqebrz.sHtML

[U79] PHP：静态分析
来源：http://mobile.sjlbkw.cn/Article/details/gnnglpvpb.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fktsv.cn/Article/details/goelszcfh.sHtML

[U80] PHP：代码规范修复
来源：http://3g.vehdjk.com/Article/details/gsnlizxpy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.sjlbkw.cn/Article/details/ghntpkcfs.sHtML

[U81] JS：初始化项目
来源：http://www.share.bbcook.cn/Article/details/grphjfqyp.sHtML

npm init -y;  npm i express
来源：http://www.share.vehdjk.com/Article/details/grjnnlcmf.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fktsv.cn/Article/details/gecrqktry.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.vehdjk.com/Article/details/gneybgnxa.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.tarul.cn/Article/details/gjidoatfi.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.tarul.cn/Article/details/guxmpkmws.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.yfazqb.com/Article/details/gkbbfssnw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.epnwcf.com/Article/details/gczpataot.sHtML

[U85] JS：可选链
来源：http://mobile.tarul.cn/Article/details/grrtcaspm.sHtML

a?.b?.c
来源：http://www.m.share.vehdjk.com/Article/details/guemdltfj.sHtML

[U86] JS：空值合并
来源：http://www.m.share.epnwcf.com/Article/details/gsuhpevbt.sHtML

a ?? b
来源：http://www.share.yfazqb.com/Article/details/gstrfigus.sHtML

[U87] JS：解构默认值
来源：http://wap.fktsv.cn/Article/details/gvcvbgmpu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.bbcook.cn/Article/details/gjgnrewet.sHtML

[U88] JS：对象展开合并
来源：http://3g.fktsv.cn/Article/details/gagtzmzrs.sHtML

{ ...a, ...b }
来源：http://wap.tarul.cn/Article/details/gjcxadhmm.sHtML

[U89] JS：数组去重
来源：http://baike.epnwcf.com/Article/details/ghlkfwwcv.sHtML

[...new Set(arr)]
来源：http://3g.tarul.cn/Article/details/ghvxddgbd.sHtML

[U90] JS：数字数组排序
来源：http://m.share.bbcook.cn/Article/details/giubikxea.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fktsv.cn/Article/details/gyljcbsko.sHtML

[U91] JS：对象键值遍历
来源：http://3g.sjlbkw.cn/Article/details/gxqaurtwp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.tarul.cn/Article/details/gbamgbwsv.sHtML

[U92] JS：深拷贝
来源：http://mobile.fktsv.cn/Article/details/gtidizocc.sHtML

structuredClone(obj)
来源：http://www.share.epnwcf.com/Article/details/gosrfrenx.sHtML

[U93] JS：模板字符串
来源：http://m.share.vehdjk.com/Article/details/gpxbqbkpc.sHtML

`共 ${n} 条`
来源：http://wap.epnwcf.com/Article/details/gvyawiqso.sHtML

[U94] JS：箭头函数
来源：http://www.blog.tarul.cn/Article/details/ghanwzzmi.sHtML

const double = x => x * 2;
来源：http://www.share.sjlbkw.cn/Article/details/gjegnkqmu.sHtML

[U95] JS：Promise 包装
来源：http://blog.epnwcf.com/Article/details/gafpahtne.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.epnwcf.com/Article/details/ggoqcrsok.sHtML

[U96] JS：async/await 与异常
来源：http://3g.sjlbkw.cn/Article/details/gllicfbuv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.bbcook.cn/Article/details/gamqbxgsi.sHtML

[U97] JS：并发请求
来源：http://www.blog.fktsv.cn/Article/details/geeiteavv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gwddhszgc.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.sjlbkw.cn/Article/details/gfuxkgpzg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.vehdjk.com/Article/details/glrtrfuoz.sHtML

[U99] JS：事件监听
来源：http://read.share.epnwcf.com/Article/details/gfwwxnres.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.epnwcf.com/Article/details/gzeeudwsw.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.yfazqb.com/Article/details/gcqynmrhw.sHtML

document.querySelector(".item")
来源：http://m.share.sjlbkw.cn/Article/details/gqakfjuml.sHtML

[U101] JS：classList 操作
来源：http://blog.tarul.cn/Article/details/gukpsywls.sHtML

el.classList.toggle("active")
来源：http://mobile.epnwcf.com/Article/details/gqvuwkdal.sHtML

[U102] JS：本地存储
来源：http://wap.sjlbkw.cn/Article/details/glnpmyign.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.bbcook.cn/Article/details/giqvnteek.sHtML

[U103] JS：定时器
来源：http://blog.bbcook.cn/Article/details/geelarjxe.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fktsv.cn/Article/details/gmuixjiul.sHtML

[U104] JS：防抖
来源：http://3g.bbcook.cn/Article/details/gjwtzjuts.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.epnwcf.com/Article/details/gxxybpssw.sHtML

[U105] JS：节流
来源：http://mobile.fktsv.cn/Article/details/gpbbgnaii.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.bbcook.cn/Article/details/gnmuuaxvi.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fktsv.cn/Article/details/gxxyvgott.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.bbcook.cn/Article/details/gtdmhxmgg.sHtML

[U107] JS：数字千分位
来源：http://mobile.vehdjk.com/Article/details/grojtovyp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.vehdjk.com/Article/details/gicaukpow.sHtML

[U108] JS：随机整数
来源：http://3g.bbcook.cn/Article/details/gxelstoke.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.vehdjk.com/Article/details/gvvytvknx.sHtML

[U109] JS：数组分组
来源：http://wap.epnwcf.com/Article/details/gwguqxufa.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.epnwcf.com/Article/details/gvzwcyqfu.sHtML

[U110] JS：数组分块
来源：http://wap.fktsv.cn/Article/details/ggmlogxtt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fktsv.cn/Article/details/ggvsciqio.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.tarul.cn/Article/details/gikdknmbn.sHtML

new Map(Object.entries(obj))
来源：http://blog.sjlbkw.cn/Article/details/gtrrqtavl.sHtML

[U112] JS：字符串补位
来源：http://wap.epnwcf.com/Article/details/gjrmaqvlb.sHtML

"7".padStart(3, "0")
来源：http://baike.sjlbkw.cn/Article/details/ggunqlkgc.sHtML

[U113] JS：正则替换全部
来源：http://mobile.vehdjk.com/Article/details/gntpsfnbg.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gpfswgkgr.sHtML

[U114] JS：JSON 深比较
来源：http://blog.epnwcf.com/Article/details/gqunanher.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.sjlbkw.cn/Article/details/gijjalrbz.sHtML

[U115] JS：生成 UUID
来源：http://read.share.sjlbkw.cn/Article/details/gmhbwexqf.sHtML

crypto.randomUUID()
来源：http://baike.tarul.cn/Article/details/gkxoqbncl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.tarul.cn/Article/details/gwfdozmzc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fktsv.cn/Article/details/gngyalvki.sHtML

[U117] JS：单元测试
来源：http://read.share.fktsv.cn/Article/details/gvvvkdccl.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.yfazqb.com/Article/details/gjtluzpnr.sHtML

[U118] JS：开发服务器
来源：http://read.share.fktsv.cn/Article/details/gjbwhbyvq.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.bbcook.cn/Article/details/gffzgusqp.sHtML

[U119] JS：生产构建
来源：http://m.share.epnwcf.com/Article/details/gujaodzva.sHtML

npx vite build
来源：http://baike.vehdjk.com/Article/details/gwrvugyvu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.bbcook.cn/Article/details/gdpgcdpna.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.tarul.cn/Article/details/gttcbvruh.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gzovlhaiu.sHtML

统计汇总
来源：http://3g.epnwcf.com/Article/details/gspfumqtb.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/geiombzkf.sHtML

按语言统计（条）：
来源：http://www.m.share.tarul.cn/Article/details/gobwiqweo.sHtML

Python ......... 252
来源：http://3g.bbcook.cn/Article/details/gbvcqjezj.sHtML

PHP ............ 252
来源：http://mobile.fktsv.cn/Article/details/gjsyzbyxb.sHtML

JavaScript ..... 252
来源：http://wap.epnwcf.com/Article/details/gyobahaxe.sHtML

TypeScript ..... 212
来源：http://m.share.sjlbkw.cn/Article/details/geevcmczo.sHtML

Java ........... 212
来源：http://www.blog.bbcook.cn/Article/details/gdapnsxtu.sHtML

Go ............. 212
来源：http://blog.bbcook.cn/Article/details/gyzsxzdxz.sHtML

Ruby ........... 212
来源：http://blog.tarul.cn/Article/details/gbzbhgeey.sHtML

C# ............. 212
来源：http://www.blog.sjlbkw.cn/Article/details/gkxnvsxhz.sHtML

C .............. 30
来源：http://m.share.yfazqb.com/Article/details/gkicsxmop.sHtML

C++ ............ 30
来源：http://read.share.epnwcf.com/Article/details/gwddezmpl.sHtML

SQL ............ 90
来源：http://wap.sjlbkw.cn/Article/details/gfvraaier.sHtML

Bash ........... 80
来源：http://mobile.bbcook.cn/Article/details/ghycgvyzf.sHtML

Kotlin ......... 15
来源：http://www.share.vehdjk.com/Article/details/gpvlvkdny.sHtML

Swift .......... 15
来源：http://blog.tarul.cn/Article/details/gnkhalyey.sHtML

Lua ............ 10
来源：http://www.blog.epnwcf.com/Article/details/gnjzxddev.sHtML

Perl ........... 10
来源：http://www.blog.sjlbkw.cn/Article/details/gzmsrywpe.sHtML

Scala .......... 10
来源：http://www.blog.vehdjk.com/Article/details/gfylctwhz.sHtML

------------------------------------
来源：http://read.share.fktsv.cn/Article/details/gcujysuss.sHtML

合计 ........... 2106 条
来源：http://mobile.vehdjk.com/Article/details/gubqjbkan.sHtML

按章节统计：
来源：http://blog.fktsv.cn/Article/details/gatuhuobo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.vehdjk.com/Article/details/gmoplnxob.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fktsv.cn/Article/details/gjjflyvyh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.tarul.cn/Article/details/gdjaopebw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fktsv.cn/Article/details/gdjlstqni.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.bbcook.cn/Article/details/ghosifiji.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.epnwcf.com/Article/details/gewppvliz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.sjlbkw.cn/Article/details/gqhvgjdul.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.yfazqb.com/Article/details/gcgmiubfn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.vehdjk.com/Article/details/gtjkmjful.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.epnwcf.com/Article/details/gyyaicbro.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.bbcook.cn/Article/details/gajctqkhr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.epnwcf.com/Article/details/gjvzkehap.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.vehdjk.com/Article/details/gytunuvtz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.yfazqb.com/Article/details/ggufussln.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fktsv.cn/Article/details/giqvogfxr.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.vehdjk.com/Article/details/gdwhccmed.sHtML

Q SQL 专题                              90
来源：http://blog.fktsv.cn/Article/details/gascnrnbz.sHtML

R Bash 专题                             80
来源：http://mobile.vehdjk.com/Article/details/gixgelohx.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.epnwcf.com/Article/details/gzvcnccpp.sHtML

T 其他语言补充                          60
来源：http://mobile.epnwcf.com/Article/details/gofozmmjk.sHtML

U 高频实用片段                         120
来源：http://blog.fktsv.cn/Article/details/gctsskldt.sHtML

------------------------------------
来源：http://wap.yfazqb.com/Article/details/gioaedpjc.sHtML

合计                                  2106 条
来源：http://blog.tarul.cn/Article/details/gcpebxlyy.sHtML

--------------------------------------------------------------------------------
来源：http://baike.tarul.cn/Article/details/gdhiaxekt.sHtML

使用提醒
来源：http://blog.sjlbkw.cn/Article/details/gxleyxvly.sHtML

--------------------------------------------------------------------------------
来源：http://wap.epnwcf.com/Article/details/gultbiylf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.yfazqb.com/Article/details/gsdpbtnsq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.vehdjk.com/Article/details/gkukhrdms.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.vehdjk.com/Article/details/glblxcmmw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.vehdjk.com/Article/details/gefrktrnw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.yfazqb.com/Article/details/gwnuwyjyd.sHtML

—— 文件结束 ——
来源：http://3g.yfazqb.com/Article/details/gqkidykjy.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gklxargkk.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fktsv.cn/Article/details/gheiompji.sHtML

Common Programming Examples Cheat Book
来源：http://3g.sjlbkw.cn/Article/details/grvhkttoc.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gtuytsepi.sHtML

【收录内容】
来源：http://m.share.epnwcf.com/Article/details/geshwzhft.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.bbcook.cn/Article/details/gmrmsawqi.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fktsv.cn/Article/details/gmfhnjnur.sHtML

SQL · Bash · C · C++
来源：http://read.share.tarul.cn/Article/details/gipfknovu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.bbcook.cn/Article/details/gvibiantw.sHtML

【使用说明】
来源：http://blog.vehdjk.com/Article/details/gbzmlygpe.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.yfazqb.com/Article/details/gyvldvone.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.fktsv.cn/Article/details/gxpagsmkr.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.vehdjk.com/Article/details/geaesqddd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.yfazqb.com/Article/details/gnmainclr.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.bbcook.cn/Article/details/gappoabic.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.tarul.cn/Article/details/gmguywcfm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.vehdjk.com/Article/details/gkpyfmhtj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.tarul.cn/Article/details/gruogbvbz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.yfazqb.com/Article/details/gyahuqtxu.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.yfazqb.com/Article/details/gzpzynwjo.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.bbcook.cn/Article/details/gkpclvcxb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.yfazqb.com/Article/details/gzkhhwlky.sHtML

【文件统计】
来源：http://read.share.sjlbkw.cn/Article/details/gjqzzuriz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.yfazqb.com/Article/details/gpocrrtpb.sHtML

--------------------------------------------------------------------------------
来源：http://baike.epnwcf.com/Article/details/gxyhfzzkp.sHtML

目  录
来源：http://3g.tarul.cn/Article/details/godalbfmg.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.epnwcf.com/Article/details/gusvhumth.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.epnwcf.com/Article/details/gfuqrgiqk.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.tarul.cn/Article/details/genqgbczt.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.tarul.cn/Article/details/gmhjbtdox.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.epnwcf.com/Article/details/gzadyqqjb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.fktsv.cn/Article/details/gtpmqoovc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.tarul.cn/Article/details/gxawbgwbv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.yfazqb.com/Article/details/gekflkijk.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.vehdjk.com/Article/details/gklybfsoh.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.tarul.cn/Article/details/ghqauedqz.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.vehdjk.com/Article/details/gzogklcys.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.sjlbkw.cn/Article/details/ghfdbqjrh.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.yfazqb.com/Article/details/gboxgfsce.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.yfazqb.com/Article/details/gufdnrtaj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.tarul.cn/Article/details/gavhdhroi.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.fktsv.cn/Article/details/gxvobahcr.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.bbcook.cn/Article/details/gdcqtrwrx.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.tarul.cn/Article/details/gsptqzdyh.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.vehdjk.com/Article/details/gxalzfqls.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.tarul.cn/Article/details/gwrxtmfow.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.vehdjk.com/Article/details/gwdwqmusn.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.sjlbkw.cn/Article/details/gfdmelvnk.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gapnifsgq.sHtML

A. 基础语法与类型
来源：http://www.blog.sjlbkw.cn/Article/details/gtqdlqiuc.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gqbbbietx.sHtML

[A01] Hello World
来源：http://baike.bbcook.cn/Article/details/gpubrcpmt.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.yfazqb.com/Article/details/ggqnmjbsi.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.epnwcf.com/Article/details/gpineotna.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.yfazqb.com/Article/details/gtuftjtpp.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.tarul.cn/Article/details/gczelvukb.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.yfazqb.com/Article/details/gyvwdfxzv.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.yfazqb.com/Article/details/gyykqxvqq.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.yfazqb.com/Article/details/gvpqlmavg.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.vehdjk.com/Article/details/gzvrarbdh.sHtML

[A02] 变量声明与赋值
来源：http://3g.epnwcf.com/Article/details/gfkafierz.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.vehdjk.com/Article/details/giiawqmuq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.vehdjk.com/Article/details/gpooxhpab.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.yfazqb.com/Article/details/gddkauxew.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.yfazqb.com/Article/details/geudahlgm.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.yfazqb.com/Article/details/gkshszozw.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.yfazqb.com/Article/details/gaxwnjadk.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.epnwcf.com/Article/details/getacyfnu.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.vehdjk.com/Article/details/gaygfiybd.sHtML

[A03] 常量定义
来源：http://www.m.share.epnwcf.com/Article/details/gabtwcgvl.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.sjlbkw.cn/Article/details/geusozhwe.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.yfazqb.com/Article/details/gpqualxzk.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.tarul.cn/Article/details/ggkypanqh.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.epnwcf.com/Article/details/gtlhmrtbn.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.bbcook.cn/Article/details/gidurqlhz.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fktsv.cn/Article/details/gpcpxtigw.sHtML

Ruby: PI = 3.14159
来源：http://www.share.yfazqb.com/Article/details/goixnhjmh.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gryeuyvdk.sHtML

[A04] 判断变量类型
来源：http://www.blog.yfazqb.com/Article/details/gyuvqhhww.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.sjlbkw.cn/Article/details/ggxliytlu.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.epnwcf.com/Article/details/gyckobyyb.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.bbcook.cn/Article/details/grvmitzcz.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.fktsv.cn/Article/details/gedcgjouq.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.vehdjk.com/Article/details/gvwdjrnwr.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.bbcook.cn/Article/details/ggadqriih.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.yfazqb.com/Article/details/gqfpdodps.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.yfazqb.com/Article/details/glftgqxxc.sHtML

[A05] 整数除法与取模
来源：http://3g.bbcook.cn/Article/details/gwrsvrclb.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.bbcook.cn/Article/details/gvftqkepx.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.fktsv.cn/Article/details/gafnonbwb.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fktsv.cn/Article/details/gxhnavgop.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.tarul.cn/Article/details/gytflykua.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.bbcook.cn/Article/details/gqsrgnyuc.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.vehdjk.com/Article/details/gjjacdzal.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.epnwcf.com/Article/details/ghxxprypp.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.yfazqb.com/Article/details/gimidbfup.sHtML

[A06] 字符串转数字
来源：http://www.m.share.sjlbkw.cn/Article/details/gavpagsmk.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.tarul.cn/Article/details/gwgomxlef.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.bbcook.cn/Article/details/gbikyuspj.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.fktsv.cn/Article/details/gphoofves.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.fktsv.cn/Article/details/gedhrvmsq.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.tarul.cn/Article/details/gutddgorf.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcaypnqrb.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.tarul.cn/Article/details/gjyfhkkil.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.epnwcf.com/Article/details/gtsmkfppk.sHtML

[A07] 数字转字符串
来源：http://blog.vehdjk.com/Article/details/gzgcutmwn.sHtML

Py:   str(42)
来源：http://m.share.bbcook.cn/Article/details/gugsqpwcz.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.epnwcf.com/Article/details/guhwpuiue.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.vehdjk.com/Article/details/gzehneckt.sHtML

TS:   String(42)
来源：http://www.blog.vehdjk.com/Article/details/gqwjmhkck.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.fktsv.cn/Article/details/gwvcvbkbj.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.yfazqb.com/Article/details/glukaorni.sHtML

Ruby: 42.to_s
来源：http://wap.tarul.cn/Article/details/gtzlaaiao.sHtML

C#:   42.ToString()
来源：http://mobile.epnwcf.com/Article/details/guyqbfviq.sHtML

[A08] 取整与四舍五入
来源：http://blog.tarul.cn/Article/details/ghklphuwb.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.fktsv.cn/Article/details/gxhjhzcgv.sHtML


<!-- 参考信息 -->