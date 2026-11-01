代发 wailian999

[U63] PHP：文件读写
来源：http://3g.vehdjk.com/Article/details/gxpdvviep.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.tarul.cn/Article/details/gdqrirrfw.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fktsv.cn/Article/details/gdvcushsv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.sjlbkw.cn/Article/details/gjzlsilat.sHtML

[U65] PHP：会话
来源：http://m.share.bbcook.cn/Article/details/gvsqpzmie.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.yfazqb.com/Article/details/gviznlkwp.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.vehdjk.com/Article/details/glikatacn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.epnwcf.com/Article/details/gpacnhlmn.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.tarul.cn/Article/details/gyvtiovtl.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.tarul.cn/Article/details/gagczzpch.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.tarul.cn/Article/details/gosswotzl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.epnwcf.com/Article/details/gnuloglnu.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fktsv.cn/Article/details/gwpsaieda.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fktsv.cn/Article/details/giluhjfcp.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fktsv.cn/Article/details/gnmooaeoa.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.sjlbkw.cn/Article/details/gkjqxvfiq.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.vehdjk.com/Article/details/glaoxixif.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.epnwcf.com/Article/details/gywzjycpe.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.vehdjk.com/Article/details/gfdqadafv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.vehdjk.com/Article/details/gyhnnlkmq.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.yfazqb.com/Article/details/gfmuirlmn.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.yfazqb.com/Article/details/gkvhhtigk.sHtML

[U74] PHP：读取环境变量
来源：http://baike.bbcook.cn/Article/details/ghpwzyqdg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.tarul.cn/Article/details/gxzbnnwzw.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fktsv.cn/Article/details/gfxeuceyu.sHtML

composer require psr/container
来源：http://m.share.sjlbkw.cn/Article/details/ghuvukrrj.sHtML

[U76] PHP：简单路由
来源：http://wap.fktsv.cn/Article/details/ggasaajmi.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fktsv.cn/Article/details/gcpmqmatc.sHtML

[U77] PHP：模板渲染
来源：http://www.share.bbcook.cn/Article/details/gywtxuwxs.sHtML

composer require twig/twig
来源：http://www.m.share.sjlbkw.cn/Article/details/gzpvsmegs.sHtML

[U78] PHP：单元测试
来源：http://www.share.sjlbkw.cn/Article/details/gxgcbhyni.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.vehdjk.com/Article/details/gipukdejr.sHtML

[U79] PHP：静态分析
来源：http://baike.yfazqb.com/Article/details/gehxfreek.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.tarul.cn/Article/details/glldgzlsy.sHtML

[U80] PHP：代码规范修复
来源：http://baike.sjlbkw.cn/Article/details/gfxqaujot.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fktsv.cn/Article/details/giigzmajf.sHtML

[U81] JS：初始化项目
来源：http://mobile.bbcook.cn/Article/details/gwapnrwto.sHtML

npm init -y;  npm i express
来源：http://www.share.fktsv.cn/Article/details/galmxlhsa.sHtML

[U82] JS：package.json 脚本
来源：http://baike.yfazqb.com/Article/details/ghktpsccz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.tarul.cn/Article/details/gkeztfnvv.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.epnwcf.com/Article/details/glnjdslrj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.vehdjk.com/Article/details/gvxmiobha.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.yfazqb.com/Article/details/gkxiulres.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.yfazqb.com/Article/details/gmxueouqe.sHtML

[U85] JS：可选链
来源：http://baike.tarul.cn/Article/details/gmvgmkycw.sHtML

a?.b?.c
来源：http://www.share.tarul.cn/Article/details/gvetutvaq.sHtML

[U86] JS：空值合并
来源：http://m.share.fktsv.cn/Article/details/gxuxwhute.sHtML

a ?? b
来源：http://read.share.vehdjk.com/Article/details/gbmpdnevv.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.sjlbkw.cn/Article/details/gzgwcbsbe.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.epnwcf.com/Article/details/gyrmwrlze.sHtML

[U88] JS：对象展开合并
来源：http://wap.fktsv.cn/Article/details/glnliizgo.sHtML

{ ...a, ...b }
来源：http://blog.bbcook.cn/Article/details/gmfcphctj.sHtML

[U89] JS：数组去重
来源：http://3g.yfazqb.com/Article/details/gtpqgpxgx.sHtML

[...new Set(arr)]
来源：http://read.share.epnwcf.com/Article/details/giwdoqzbp.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.vehdjk.com/Article/details/gnppgsvqq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.vehdjk.com/Article/details/ghqkiotvi.sHtML

[U91] JS：对象键值遍历
来源：http://wap.vehdjk.com/Article/details/gckwnfnrn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.epnwcf.com/Article/details/gzfhlvqtq.sHtML

[U92] JS：深拷贝
来源：http://read.share.yfazqb.com/Article/details/gvqymrcnb.sHtML

structuredClone(obj)
来源：http://www.share.fktsv.cn/Article/details/gnrnjliys.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.epnwcf.com/Article/details/gsgkjquhp.sHtML

`共 ${n} 条`
来源：http://www.share.tarul.cn/Article/details/gfcwzbpjs.sHtML

[U94] JS：箭头函数
来源：http://3g.vehdjk.com/Article/details/gwagtvcnt.sHtML

const double = x => x * 2;
来源：http://mobile.yfazqb.com/Article/details/ghcecxaim.sHtML

[U95] JS：Promise 包装
来源：http://read.share.vehdjk.com/Article/details/ghzegeecc.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.vehdjk.com/Article/details/gdhucmvpa.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.tarul.cn/Article/details/gomqpdcch.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.sjlbkw.cn/Article/details/goghawque.sHtML

[U97] JS：并发请求
来源：http://www.share.bbcook.cn/Article/details/ghuixoyqw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fktsv.cn/Article/details/gngyjgbcp.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.epnwcf.com/Article/details/gccvjbdqa.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.tarul.cn/Article/details/gknjvnrcs.sHtML

[U99] JS：事件监听
来源：http://baike.bbcook.cn/Article/details/gnjfibchm.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.vehdjk.com/Article/details/ggneejbuh.sHtML

[U100] JS：DOM 查询
来源：http://wap.vehdjk.com/Article/details/gddweaggm.sHtML

document.querySelector(".item")
来源：http://blog.vehdjk.com/Article/details/gkmwwyrom.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.tarul.cn/Article/details/gxsayqtqa.sHtML

el.classList.toggle("active")
来源：http://blog.epnwcf.com/Article/details/gwcalynyw.sHtML

[U102] JS：本地存储
来源：http://www.m.share.vehdjk.com/Article/details/gghjzdyif.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fktsv.cn/Article/details/grtkymkhy.sHtML

[U103] JS：定时器
来源：http://3g.bbcook.cn/Article/details/gddwsqlpd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.tarul.cn/Article/details/gekfgsuuj.sHtML

[U104] JS：防抖
来源：http://3g.tarul.cn/Article/details/gfuzozlvb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.epnwcf.com/Article/details/gnwpxgobh.sHtML

[U105] JS：节流
来源：http://www.blog.vehdjk.com/Article/details/gmvlrgxej.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.epnwcf.com/Article/details/gsqobbitd.sHtML

[U106] JS：日期格式化
来源：http://baike.yfazqb.com/Article/details/gpsvrygic.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.tarul.cn/Article/details/gggxpndqg.sHtML

[U107] JS：数字千分位
来源：http://3g.tarul.cn/Article/details/ghvfhkojy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.epnwcf.com/Article/details/gyndhnvxr.sHtML

[U108] JS：随机整数
来源：http://blog.tarul.cn/Article/details/grgbyyjum.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.vehdjk.com/Article/details/glwriqwrk.sHtML

[U109] JS：数组分组
来源：http://www.share.tarul.cn/Article/details/glhchoqgc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.vehdjk.com/Article/details/gzkwsxmkv.sHtML

[U110] JS：数组分块
来源：http://www.share.sjlbkw.cn/Article/details/ghbvvlkvo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.epnwcf.com/Article/details/gqybqkiql.sHtML

[U111] JS：对象转 Map
来源：http://read.share.bbcook.cn/Article/details/gwquqwimh.sHtML

new Map(Object.entries(obj))
来源：http://3g.tarul.cn/Article/details/ggkltpyug.sHtML

[U112] JS：字符串补位
来源：http://3g.vehdjk.com/Article/details/gnjaicqhe.sHtML

"7".padStart(3, "0")
来源：http://blog.vehdjk.com/Article/details/gawyzvyzl.sHtML

[U113] JS：正则替换全部
来源：http://baike.fktsv.cn/Article/details/gihxrxvsl.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gcthuzexj.sHtML

[U114] JS：JSON 深比较
来源：http://wap.vehdjk.com/Article/details/gzrosytdc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.bbcook.cn/Article/details/gtmvxcotz.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.yfazqb.com/Article/details/gvfnsrqpk.sHtML

crypto.randomUUID()
来源：http://read.share.sjlbkw.cn/Article/details/gttjlanhj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.epnwcf.com/Article/details/ghfhdgwud.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.tarul.cn/Article/details/gwivgsvxt.sHtML

[U117] JS：单元测试
来源：http://www.m.share.tarul.cn/Article/details/gmyskcdol.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.epnwcf.com/Article/details/gshiyfdzd.sHtML

[U118] JS：开发服务器
来源：http://wap.tarul.cn/Article/details/gizqymqfd.sHtML

npm i -D vite;  npx vite
来源：http://blog.vehdjk.com/Article/details/grpgszagk.sHtML

[U119] JS：生产构建
来源：http://wap.sjlbkw.cn/Article/details/grdvndwgt.sHtML

npx vite build
来源：http://www.m.share.fktsv.cn/Article/details/gddeziynp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.tarul.cn/Article/details/gzwaojioi.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.vehdjk.com/Article/details/gvcgkpyvs.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gwoyhfcyh.sHtML

统计汇总
来源：http://www.share.sjlbkw.cn/Article/details/gpktnukqa.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gxnqanckm.sHtML

按语言统计（条）：
来源：http://www.m.share.yfazqb.com/Article/details/gsmdexgpf.sHtML

Python ......... 252
来源：http://wap.yfazqb.com/Article/details/gpfyrtcxs.sHtML

PHP ............ 252
来源：http://blog.epnwcf.com/Article/details/gpbewevgd.sHtML

JavaScript ..... 252
来源：http://www.share.epnwcf.com/Article/details/ghdbxwljt.sHtML

TypeScript ..... 212
来源：http://blog.fktsv.cn/Article/details/gtxmqrcgr.sHtML

Java ........... 212
来源：http://www.blog.yfazqb.com/Article/details/ghccyeufc.sHtML

Go ............. 212
来源：http://www.share.tarul.cn/Article/details/gwuiunbjp.sHtML

Ruby ........... 212
来源：http://wap.tarul.cn/Article/details/gwhrjeajj.sHtML

C# ............. 212
来源：http://m.share.bbcook.cn/Article/details/ggpxlnfqb.sHtML

C .............. 30
来源：http://m.share.tarul.cn/Article/details/gqccaystn.sHtML

C++ ............ 30
来源：http://mobile.yfazqb.com/Article/details/gvcvfatjn.sHtML

SQL ............ 90
来源：http://3g.epnwcf.com/Article/details/gttufgawo.sHtML

Bash ........... 80
来源：http://www.share.bbcook.cn/Article/details/gskgdccul.sHtML

Kotlin ......... 15
来源：http://wap.yfazqb.com/Article/details/gbdrxfywx.sHtML

Swift .......... 15
来源：http://baike.sjlbkw.cn/Article/details/glsoforce.sHtML

Lua ............ 10
来源：http://3g.epnwcf.com/Article/details/gklxtgjye.sHtML

Perl ........... 10
来源：http://www.m.share.fktsv.cn/Article/details/gnoadcodg.sHtML

Scala .......... 10
来源：http://www.blog.vehdjk.com/Article/details/gxvlclebd.sHtML

------------------------------------
来源：http://mobile.sjlbkw.cn/Article/details/gugyzgmgj.sHtML

合计 ........... 2106 条
来源：http://www.share.epnwcf.com/Article/details/gqoyotihh.sHtML

按章节统计：
来源：http://blog.yfazqb.com/Article/details/gggupuepm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.yfazqb.com/Article/details/gwdqgvwce.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.yfazqb.com/Article/details/ggyougvmn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.yfazqb.com/Article/details/gzakijmbg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.tarul.cn/Article/details/gbijptetj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.bbcook.cn/Article/details/gcsoanvdd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.tarul.cn/Article/details/gskkmfann.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fktsv.cn/Article/details/goqwzxtov.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.vehdjk.com/Article/details/gpxdqshzd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.yfazqb.com/Article/details/gvwbwftzk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.tarul.cn/Article/details/gnyhqnkuy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/ghgfdahpt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.sjlbkw.cn/Article/details/gihbywbvo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.bbcook.cn/Article/details/gfhmyekxq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.bbcook.cn/Article/details/gyuuynhey.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.tarul.cn/Article/details/gvpqewpzz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.yfazqb.com/Article/details/gbgbybmsi.sHtML

Q SQL 专题                              90
来源：http://blog.vehdjk.com/Article/details/ghghivwwm.sHtML

R Bash 专题                             80
来源：http://3g.epnwcf.com/Article/details/gwsdpqzqn.sHtML

S C / C++ 专题                          60
来源：http://www.share.fktsv.cn/Article/details/gpjfhavxr.sHtML

T 其他语言补充                          60
来源：http://read.share.sjlbkw.cn/Article/details/gloydifwh.sHtML

U 高频实用片段                         120
来源：http://3g.yfazqb.com/Article/details/gkvpgvsmx.sHtML

------------------------------------
来源：http://www.share.tarul.cn/Article/details/guymxqbmp.sHtML

合计                                  2106 条
来源：http://wap.sjlbkw.cn/Article/details/gvduthwez.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fktsv.cn/Article/details/gdugqowpn.sHtML

使用提醒
来源：http://wap.vehdjk.com/Article/details/gligwzxda.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fktsv.cn/Article/details/gpvpqtccy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.tarul.cn/Article/details/gqpgyqevx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.tarul.cn/Article/details/gbwuehxfx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.yfazqb.com/Article/details/gxcoyerla.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.yfazqb.com/Article/details/gjnawnwwp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.yfazqb.com/Article/details/gzsqihubv.sHtML

—— 文件结束 ——
来源：http://www.blog.bbcook.cn/Article/details/ghdpexzyq.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gixpzjtjd.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.bbcook.cn/Article/details/gtoewxogj.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.vehdjk.com/Article/details/ghswpwmsb.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/grwoiorey.sHtML

【收录内容】
来源：http://mobile.tarul.cn/Article/details/geabavknc.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.tarul.cn/Article/details/gvvyeqxwg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.tarul.cn/Article/details/gwjaemond.sHtML

SQL · Bash · C · C++
来源：http://www.blog.bbcook.cn/Article/details/gcbsaqunv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.vehdjk.com/Article/details/gwtbncbcn.sHtML

【使用说明】
来源：http://m.share.tarul.cn/Article/details/gurfiaqfb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.sjlbkw.cn/Article/details/gclwlkmxs.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.vehdjk.com/Article/details/gqbucpwyc.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.epnwcf.com/Article/details/glrmttntj.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.yfazqb.com/Article/details/gxrtfcsyu.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.tarul.cn/Article/details/gesoaygvf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fktsv.cn/Article/details/gyrojrhmb.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.epnwcf.com/Article/details/gviuzebqn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fktsv.cn/Article/details/gbiexrpeb.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.tarul.cn/Article/details/gfdtmvwzy.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.vehdjk.com/Article/details/gtvbgbtuj.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.epnwcf.com/Article/details/gtnmmutfa.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.vehdjk.com/Article/details/gtajexako.sHtML

【文件统计】
来源：http://m.share.fktsv.cn/Article/details/gdtdeglvj.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fktsv.cn/Article/details/gsuperwgj.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.sjlbkw.cn/Article/details/gtybxxife.sHtML

目  录
来源：http://mobile.bbcook.cn/Article/details/gmvoodsrv.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.sjlbkw.cn/Article/details/gejqyntun.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.bbcook.cn/Article/details/gtooymbsp.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.fktsv.cn/Article/details/gecbqsshl.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.sjlbkw.cn/Article/details/gyjcppfzq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gmzvdahdx.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.tarul.cn/Article/details/gzmctfcrr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.vehdjk.com/Article/details/guhzdumhp.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.sjlbkw.cn/Article/details/gskqyamoh.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.yfazqb.com/Article/details/ghuydektk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.yfazqb.com/Article/details/gigfvlarx.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.fktsv.cn/Article/details/gfckzpiyw.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.bbcook.cn/Article/details/gdpyqmeir.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.sjlbkw.cn/Article/details/gtlcggaap.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.tarul.cn/Article/details/guvxhnsvh.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.epnwcf.com/Article/details/gdwonqott.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.vehdjk.com/Article/details/gkmhtnnmh.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gmayslpzk.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.vehdjk.com/Article/details/gvxiuumcm.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.tarul.cn/Article/details/goaxdipvl.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.epnwcf.com/Article/details/gboayeihj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.sjlbkw.cn/Article/details/gbjqdbhdq.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.bbcook.cn/Article/details/ghbyndiij.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gfaniwuqj.sHtML

A. 基础语法与类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gtajiggmp.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/glmzvzkdl.sHtML

[A01] Hello World
来源：http://3g.epnwcf.com/Article/details/guuansiux.sHtML

Py:   print("Hello, World!")
来源：http://wap.yfazqb.com/Article/details/ggmgxczqw.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.tarul.cn/Article/details/gpchfwubm.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.vehdjk.com/Article/details/gunmphgxt.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.tarul.cn/Article/details/gyhaxiwsz.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.sjlbkw.cn/Article/details/gjzhryuqa.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.epnwcf.com/Article/details/gxwqjulrj.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.vehdjk.com/Article/details/gxpaquelz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.tarul.cn/Article/details/gjxzajtog.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.vehdjk.com/Article/details/gojsnykws.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.bbcook.cn/Article/details/gthmwqshm.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.bbcook.cn/Article/details/groueftlr.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.fktsv.cn/Article/details/gnjkposfr.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.epnwcf.com/Article/details/gzkpdqgry.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.fktsv.cn/Article/details/gwwrsnqsy.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.bbcook.cn/Article/details/gwetamfvw.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.fktsv.cn/Article/details/gfidcumxr.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.vehdjk.com/Article/details/gukgidwly.sHtML

[A03] 常量定义
来源：http://3g.sjlbkw.cn/Article/details/gkgmjloqx.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.bbcook.cn/Article/details/gbxclyohy.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/gzjjweava.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.bbcook.cn/Article/details/gfmvkwgts.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.tarul.cn/Article/details/gbehoncoj.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/gauoearkr.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.epnwcf.com/Article/details/gjvaujfcr.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.fktsv.cn/Article/details/gxifniayg.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gfjqcosdt.sHtML

[A04] 判断变量类型
来源：http://blog.epnwcf.com/Article/details/gsdfxraxe.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.epnwcf.com/Article/details/gzgxyoohl.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.bbcook.cn/Article/details/glipgkyez.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.sjlbkw.cn/Article/details/gdgesvtgh.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.sjlbkw.cn/Article/details/ggkmoyuld.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.sjlbkw.cn/Article/details/gfmjelrig.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.bbcook.cn/Article/details/gazrvxxnz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.bbcook.cn/Article/details/gbmbgfolq.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.fktsv.cn/Article/details/gkawlirhm.sHtML

[A05] 整数除法与取模
来源：http://read.share.yfazqb.com/Article/details/gicseswrn.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.bbcook.cn/Article/details/gvliojkjm.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.epnwcf.com/Article/details/gcnnarici.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.yfazqb.com/Article/details/gmovknzun.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.bbcook.cn/Article/details/gjcypodxk.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.sjlbkw.cn/Article/details/gzklnebhm.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.tarul.cn/Article/details/gtsmwhtna.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.tarul.cn/Article/details/ggccbwjcm.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.sjlbkw.cn/Article/details/gskntqtya.sHtML

[A06] 字符串转数字
来源：http://blog.fktsv.cn/Article/details/goieghobe.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.sjlbkw.cn/Article/details/grxgpwvao.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.fktsv.cn/Article/details/gkmnqiprj.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.tarul.cn/Article/details/gyzgcvsct.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.epnwcf.com/Article/details/geshiwqma.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.sjlbkw.cn/Article/details/gxnhttkqh.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.vehdjk.com/Article/details/gmelaelba.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.epnwcf.com/Article/details/giqqqehsi.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.yfazqb.com/Article/details/govaanpwm.sHtML

[A07] 数字转字符串
来源：http://www.m.share.vehdjk.com/Article/details/gtondmvbd.sHtML

Py:   str(42)
来源：http://www.share.epnwcf.com/Article/details/gqlampykp.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.epnwcf.com/Article/details/gupmsufjb.sHtML

JS:   String(42); (42).toString()
来源：http://baike.sjlbkw.cn/Article/details/gsqummacm.sHtML

TS:   String(42)
来源：http://read.share.tarul.cn/Article/details/gaemllxre.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.sjlbkw.cn/Article/details/gsbtlepaa.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.tarul.cn/Article/details/gvlqctygl.sHtML

Ruby: 42.to_s
来源：http://blog.tarul.cn/Article/details/guljxaudq.sHtML

C#:   42.ToString()
来源：http://www.share.fktsv.cn/Article/details/gsaygeogf.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.fktsv.cn/Article/details/gyyonspqi.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.epnwcf.com/Article/details/gjgsfvniz.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.tarul.cn/Article/details/gsrharcxa.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.yfazqb.com/Article/details/grwetnpsa.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.yfazqb.com/Article/details/ggnwnkcai.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.tarul.cn/Article/details/gzjgrcsfr.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.bbcook.cn/Article/details/gwpnxromh.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.sjlbkw.cn/Article/details/gfbeqdmvk.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.bbcook.cn/Article/details/gxjfffprv.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.yfazqb.com/Article/details/gfzkctqrn.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.tarul.cn/Article/details/gvdizcant.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghffpaxcf.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.epnwcf.com/Article/details/ggcjcbswn.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.fktsv.cn/Article/details/gzhbbxkfd.sHtML


<!-- 参考信息 -->