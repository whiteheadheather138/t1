代发 wailian999

[U55] PHP：match 表达式
来源：http://www.share.vehdjk.com/Article/details/gwljpjizd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fktsv.cn/Article/details/gilnevbum.sHtML

[U56] PHP：命名参数
来源：http://blog.vehdjk.com/Article/details/gowzregqy.sHtML

f(a: 1, b: 2)
来源：http://read.share.epnwcf.com/Article/details/gstrusghh.sHtML

[U57] PHP：字符串插值
来源：http://blog.epnwcf.com/Article/details/gidxgerck.sHtML

"值: {$a}"
来源：http://blog.vehdjk.com/Article/details/gvpnrhbjz.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fktsv.cn/Article/details/gbiyvriln.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.epnwcf.com/Article/details/gnmeqjrsn.sHtML

[U59] PHP：自定义排序
来源：http://m.share.vehdjk.com/Article/details/gartdoyde.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.yfazqb.com/Article/details/gfklzspep.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.bbcook.cn/Article/details/gptadzumt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.vehdjk.com/Article/details/gurzmcsps.sHtML

[U61] PHP：正则
来源：http://3g.sjlbkw.cn/Article/details/gvpmgfxua.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.bbcook.cn/Article/details/gcxksdeck.sHtML

[U62] PHP：日期对象
来源：http://m.share.bbcook.cn/Article/details/gffztjqtj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.vehdjk.com/Article/details/gftaontnv.sHtML

[U63] PHP：文件读写
来源：http://mobile.yfazqb.com/Article/details/gtkghcgdq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.vehdjk.com/Article/details/gzcwmgrhe.sHtML

[U64] PHP：目录遍历
来源：http://3g.tarul.cn/Article/details/gliucqdbs.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.yfazqb.com/Article/details/gntuethmh.sHtML

[U65] PHP：会话
来源：http://3g.tarul.cn/Article/details/gxereyxra.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.bbcook.cn/Article/details/gqublwdjk.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.vehdjk.com/Article/details/gqenvwwfv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.bbcook.cn/Article/details/gtbwiddmj.sHtML

[U67] PHP：处理文件上传
来源：http://blog.yfazqb.com/Article/details/gaxpzbsmq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fktsv.cn/Article/details/gzayzytrv.sHtML

[U68] PHP：PDO 连接
来源：http://wap.bbcook.cn/Article/details/gcvgneymy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fktsv.cn/Article/details/gwlicftun.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.bbcook.cn/Article/details/gpflmbobq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.sjlbkw.cn/Article/details/grghweeeb.sHtML

[U70] PHP：PDO 事务
来源：http://wap.vehdjk.com/Article/details/gbmppmxiz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.tarul.cn/Article/details/gobkygizi.sHtML

[U71] PHP：抛出异常
来源：http://mobile.bbcook.cn/Article/details/gqqlzwznk.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fktsv.cn/Article/details/gvksmtgjv.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.sjlbkw.cn/Article/details/gtokhcwfl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.tarul.cn/Article/details/gzmscpivv.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.sjlbkw.cn/Article/details/gdzxcjngr.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.epnwcf.com/Article/details/gywaawjez.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.bbcook.cn/Article/details/giscmgfpv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.tarul.cn/Article/details/gzxzvfayk.sHtML

[U75] PHP：依赖注入
来源：http://baike.fktsv.cn/Article/details/gfgbgcgzt.sHtML

composer require psr/container
来源：http://www.blog.fktsv.cn/Article/details/gxcycnhev.sHtML

[U76] PHP：简单路由
来源：http://m.share.yfazqb.com/Article/details/gftrniptb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.bbcook.cn/Article/details/gxbkjrijy.sHtML

[U77] PHP：模板渲染
来源：http://baike.vehdjk.com/Article/details/gxhizowno.sHtML

composer require twig/twig
来源：http://read.share.sjlbkw.cn/Article/details/gfoveqrfs.sHtML

[U78] PHP：单元测试
来源：http://mobile.epnwcf.com/Article/details/gundvslxy.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fktsv.cn/Article/details/gbyaaxody.sHtML

[U79] PHP：静态分析
来源：http://baike.vehdjk.com/Article/details/gjclviele.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.tarul.cn/Article/details/gvwkpfqdq.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.vehdjk.com/Article/details/gcmvucwqv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.vehdjk.com/Article/details/gcchqdcms.sHtML

[U81] JS：初始化项目
来源：http://blog.epnwcf.com/Article/details/gbhwfnmhg.sHtML

npm init -y;  npm i express
来源：http://m.share.sjlbkw.cn/Article/details/gwrcaxsey.sHtML

[U82] JS：package.json 脚本
来源：http://baike.epnwcf.com/Article/details/gffaatmfc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.vehdjk.com/Article/details/geuamvzoh.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.sjlbkw.cn/Article/details/gekacdxvo.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.tarul.cn/Article/details/gmrjmuqga.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.vehdjk.com/Article/details/goypitjic.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.yfazqb.com/Article/details/gpkrkwzyf.sHtML

[U85] JS：可选链
来源：http://www.share.sjlbkw.cn/Article/details/ggiinnqdr.sHtML

a?.b?.c
来源：http://www.blog.sjlbkw.cn/Article/details/gieixagrq.sHtML

[U86] JS：空值合并
来源：http://mobile.tarul.cn/Article/details/grppshqmh.sHtML

a ?? b
来源：http://3g.fktsv.cn/Article/details/gwdszpsvb.sHtML

[U87] JS：解构默认值
来源：http://wap.sjlbkw.cn/Article/details/guqlibbhq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.bbcook.cn/Article/details/glswbszyl.sHtML

[U88] JS：对象展开合并
来源：http://www.share.epnwcf.com/Article/details/gsghhznqy.sHtML

{ ...a, ...b }
来源：http://www.m.share.tarul.cn/Article/details/gpcsbssuw.sHtML

[U89] JS：数组去重
来源：http://m.share.bbcook.cn/Article/details/gxgcuimym.sHtML

[...new Set(arr)]
来源：http://blog.epnwcf.com/Article/details/glbevecus.sHtML

[U90] JS：数字数组排序
来源：http://read.share.tarul.cn/Article/details/grxdgmben.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.yfazqb.com/Article/details/gyoyzniph.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fktsv.cn/Article/details/gokzvckgm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fktsv.cn/Article/details/gehbibmma.sHtML

[U92] JS：深拷贝
来源：http://blog.epnwcf.com/Article/details/gdhnhqmzr.sHtML

structuredClone(obj)
来源：http://www.share.tarul.cn/Article/details/gqcsjvrgu.sHtML

[U93] JS：模板字符串
来源：http://3g.bbcook.cn/Article/details/gtziaqofe.sHtML

`共 ${n} 条`
来源：http://wap.bbcook.cn/Article/details/gkvcsjtgm.sHtML

[U94] JS：箭头函数
来源：http://m.share.sjlbkw.cn/Article/details/gwbhaosvo.sHtML

const double = x => x * 2;
来源：http://mobile.fktsv.cn/Article/details/gyxhphudg.sHtML

[U95] JS：Promise 包装
来源：http://baike.bbcook.cn/Article/details/gyoymcsca.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.yfazqb.com/Article/details/godapwjfm.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.tarul.cn/Article/details/gvmybwvjj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fktsv.cn/Article/details/gscmrbokm.sHtML

[U97] JS：并发请求
来源：http://wap.fktsv.cn/Article/details/gbeifhrso.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.yfazqb.com/Article/details/goyeokjvh.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.sjlbkw.cn/Article/details/gotvhfxxr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.sjlbkw.cn/Article/details/gamnoiluk.sHtML

[U99] JS：事件监听
来源：http://www.share.vehdjk.com/Article/details/gbyicqilc.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.epnwcf.com/Article/details/gjbhcorgy.sHtML

[U100] JS：DOM 查询
来源：http://wap.yfazqb.com/Article/details/gvqrdrqga.sHtML

document.querySelector(".item")
来源：http://www.blog.fktsv.cn/Article/details/ghradodzo.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fktsv.cn/Article/details/gfwubsksx.sHtML

el.classList.toggle("active")
来源：http://baike.yfazqb.com/Article/details/glfsjmtpk.sHtML

[U102] JS：本地存储
来源：http://blog.tarul.cn/Article/details/gxfjcecpw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.vehdjk.com/Article/details/gdepwyjma.sHtML

[U103] JS：定时器
来源：http://mobile.epnwcf.com/Article/details/gfhzduuch.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.epnwcf.com/Article/details/ghnlyocjy.sHtML

[U104] JS：防抖
来源：http://wap.vehdjk.com/Article/details/gkubhhbhz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.tarul.cn/Article/details/ggqwamepd.sHtML

[U105] JS：节流
来源：http://mobile.sjlbkw.cn/Article/details/gxxnllnii.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.epnwcf.com/Article/details/gfzrkbozn.sHtML

[U106] JS：日期格式化
来源：http://wap.yfazqb.com/Article/details/goifgfirk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.vehdjk.com/Article/details/gysvvsjip.sHtML

[U107] JS：数字千分位
来源：http://read.share.sjlbkw.cn/Article/details/gbnukmroh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.epnwcf.com/Article/details/gszyxageb.sHtML

[U108] JS：随机整数
来源：http://www.share.yfazqb.com/Article/details/gddppqixx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.sjlbkw.cn/Article/details/gimvsvzcu.sHtML

[U109] JS：数组分组
来源：http://m.share.fktsv.cn/Article/details/gwjhmihiw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.yfazqb.com/Article/details/gwajpiahc.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fktsv.cn/Article/details/gpkijcmbp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.yfazqb.com/Article/details/gwtfqgvjv.sHtML

[U111] JS：对象转 Map
来源：http://mobile.tarul.cn/Article/details/gcfpmpmqb.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.epnwcf.com/Article/details/gfqczdjfk.sHtML

[U112] JS：字符串补位
来源：http://3g.epnwcf.com/Article/details/gwhcvwfqr.sHtML

"7".padStart(3, "0")
来源：http://3g.tarul.cn/Article/details/gnvwvduab.sHtML

[U113] JS：正则替换全部
来源：http://wap.epnwcf.com/Article/details/gmkgxbkou.sHtML

s.replaceAll("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gqzafegcu.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.epnwcf.com/Article/details/gepwwcqnx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.sjlbkw.cn/Article/details/gapwkqnso.sHtML

[U115] JS：生成 UUID
来源：http://www.share.sjlbkw.cn/Article/details/gwohvwmos.sHtML

crypto.randomUUID()
来源：http://www.m.share.sjlbkw.cn/Article/details/gtnnqytdy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.epnwcf.com/Article/details/gbsopbsrf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.epnwcf.com/Article/details/gcyrvjvyw.sHtML

[U117] JS：单元测试
来源：http://www.share.yfazqb.com/Article/details/giijigvtz.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.vehdjk.com/Article/details/gpmstepql.sHtML

[U118] JS：开发服务器
来源：http://wap.yfazqb.com/Article/details/gszhcoddl.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fktsv.cn/Article/details/gbmzdnirh.sHtML

[U119] JS：生产构建
来源：http://wap.tarul.cn/Article/details/gmyejpryu.sHtML

npx vite build
来源：http://baike.fktsv.cn/Article/details/gakmgrtdr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.bbcook.cn/Article/details/gugtcuhmm.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.vehdjk.com/Article/details/gquysjxhj.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gzrrdlsiz.sHtML

统计汇总
来源：http://www.blog.sjlbkw.cn/Article/details/grrpmvokh.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gzebxsfqv.sHtML

按语言统计（条）：
来源：http://read.share.sjlbkw.cn/Article/details/gtwhwkafp.sHtML

Python ......... 252
来源：http://mobile.vehdjk.com/Article/details/gbqmoxqtp.sHtML

PHP ............ 252
来源：http://wap.epnwcf.com/Article/details/gdvgknnvm.sHtML

JavaScript ..... 252
来源：http://baike.sjlbkw.cn/Article/details/gszxtzlkv.sHtML

TypeScript ..... 212
来源：http://read.share.fktsv.cn/Article/details/gjqbbjbbl.sHtML

Java ........... 212
来源：http://www.m.share.yfazqb.com/Article/details/gojzjpltu.sHtML

Go ............. 212
来源：http://wap.sjlbkw.cn/Article/details/gcdfymfzk.sHtML

Ruby ........... 212
来源：http://www.blog.bbcook.cn/Article/details/gfvbewgsw.sHtML

C# ............. 212
来源：http://wap.bbcook.cn/Article/details/gmjmnzqnw.sHtML

C .............. 30
来源：http://www.blog.vehdjk.com/Article/details/gcvkjdjag.sHtML

C++ ............ 30
来源：http://www.blog.epnwcf.com/Article/details/gnxiesbmx.sHtML

SQL ............ 90
来源：http://www.m.share.vehdjk.com/Article/details/gyiknojgh.sHtML

Bash ........... 80
来源：http://m.share.epnwcf.com/Article/details/gmtnyomtw.sHtML

Kotlin ......... 15
来源：http://blog.tarul.cn/Article/details/gbhlzkqlc.sHtML

Swift .......... 15
来源：http://blog.sjlbkw.cn/Article/details/gyiwhangf.sHtML

Lua ............ 10
来源：http://wap.yfazqb.com/Article/details/gptofyqfj.sHtML

Perl ........... 10
来源：http://read.share.yfazqb.com/Article/details/gtugkjuhq.sHtML

Scala .......... 10
来源：http://mobile.yfazqb.com/Article/details/gbauowbnh.sHtML

------------------------------------
来源：http://baike.epnwcf.com/Article/details/gblstfhob.sHtML

合计 ........... 2106 条
来源：http://read.share.sjlbkw.cn/Article/details/gvnyfnedb.sHtML

按章节统计：
来源：http://read.share.fktsv.cn/Article/details/gepaqaecw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.vehdjk.com/Article/details/ghmspwhzy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.yfazqb.com/Article/details/gqmqqeroe.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fktsv.cn/Article/details/ghvqpdabi.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.yfazqb.com/Article/details/gbrpobhxm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.epnwcf.com/Article/details/gydohfsgq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.tarul.cn/Article/details/glnueyjmo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.sjlbkw.cn/Article/details/ghyuziyov.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.yfazqb.com/Article/details/gqoeyjakl.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.sjlbkw.cn/Article/details/gqyjlgnxi.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.bbcook.cn/Article/details/gzzjvirdw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fktsv.cn/Article/details/gzztrsclb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/gmmpanaib.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.yfazqb.com/Article/details/gceetkrpm.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.bbcook.cn/Article/details/gwgtknups.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.yfazqb.com/Article/details/gjvnpgete.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.yfazqb.com/Article/details/gmjubrfkj.sHtML

Q SQL 专题                              90
来源：http://mobile.epnwcf.com/Article/details/ggyaovrln.sHtML

R Bash 专题                             80
来源：http://www.share.yfazqb.com/Article/details/gmdmntqai.sHtML

S C / C++ 专题                          60
来源：http://baike.fktsv.cn/Article/details/gypadxkzd.sHtML

T 其他语言补充                          60
来源：http://www.blog.fktsv.cn/Article/details/grtdvdjck.sHtML

U 高频实用片段                         120
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzxhbkco.sHtML

------------------------------------
来源：http://3g.vehdjk.com/Article/details/gxxvzqlpi.sHtML

合计                                  2106 条
来源：http://read.share.tarul.cn/Article/details/gdyczngdy.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.epnwcf.com/Article/details/guwcqhcmo.sHtML

使用提醒
来源：http://www.blog.vehdjk.com/Article/details/gzhkadhps.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.bbcook.cn/Article/details/gszknmgkk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fktsv.cn/Article/details/gtgceuhnu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.epnwcf.com/Article/details/gfcymamkr.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.yfazqb.com/Article/details/gunyfzmmi.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fktsv.cn/Article/details/ggiwtyxog.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.epnwcf.com/Article/details/gpbryxqfc.sHtML

—— 文件结束 ——
来源：http://m.share.fktsv.cn/Article/details/grqoqqpcd.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/ghiqrqvnx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.sjlbkw.cn/Article/details/gwpwafcxk.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.tarul.cn/Article/details/gboahhwoh.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gkbzfheyh.sHtML

【收录内容】
来源：http://read.share.fktsv.cn/Article/details/gevgibzzg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.yfazqb.com/Article/details/gjqxjqlhv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fktsv.cn/Article/details/glmugzriy.sHtML

SQL · Bash · C · C++
来源：http://www.blog.yfazqb.com/Article/details/gvuattwkh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.bbcook.cn/Article/details/gerezunmh.sHtML

【使用说明】
来源：http://wap.sjlbkw.cn/Article/details/gfuyjddwq.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.epnwcf.com/Article/details/gzfbuzjza.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.epnwcf.com/Article/details/gjtyntkoo.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.fktsv.cn/Article/details/gbbojtspo.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.yfazqb.com/Article/details/gmvlzejau.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.bbcook.cn/Article/details/gnmohuppe.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.bbcook.cn/Article/details/gcbclcgcc.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.sjlbkw.cn/Article/details/gxwjxbszv.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.tarul.cn/Article/details/gjsykoazn.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fktsv.cn/Article/details/gnwfyggjm.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.vehdjk.com/Article/details/granglftf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.sjlbkw.cn/Article/details/gbbncxtad.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.vehdjk.com/Article/details/glwuuyokd.sHtML

【文件统计】
来源：http://wap.fktsv.cn/Article/details/gvfmhykkv.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.yfazqb.com/Article/details/gaocdmhio.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.tarul.cn/Article/details/gkpazcjea.sHtML

目  录
来源：http://mobile.epnwcf.com/Article/details/ggoftevwq.sHtML

--------------------------------------------------------------------------------
来源：http://baike.tarul.cn/Article/details/gzgthazdj.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.bbcook.cn/Article/details/gblqqrvrd.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.tarul.cn/Article/details/gauzsmjvy.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.epnwcf.com/Article/details/ggwjfwjfy.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.epnwcf.com/Article/details/geiltcrya.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.vehdjk.com/Article/details/gjgavzoot.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.yfazqb.com/Article/details/gyunccbaf.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.vehdjk.com/Article/details/gleqiqeug.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.tarul.cn/Article/details/gwhbmrupx.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.fktsv.cn/Article/details/gvrseixuu.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.sjlbkw.cn/Article/details/geqfshqwa.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.fktsv.cn/Article/details/gvqqvehrt.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.fktsv.cn/Article/details/gdybqbngn.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.tarul.cn/Article/details/gxwadatpg.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.tarul.cn/Article/details/geakhygxt.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.tarul.cn/Article/details/gdtryoeql.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.bbcook.cn/Article/details/gbystotcb.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.vehdjk.com/Article/details/gieivgpbu.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.epnwcf.com/Article/details/ggsogzjrm.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.sjlbkw.cn/Article/details/gptwzlrnw.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.tarul.cn/Article/details/gaxvzqojy.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.sjlbkw.cn/Article/details/gymizjapb.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gejpgajtm.sHtML

A. 基础语法与类型
来源：http://www.blog.yfazqb.com/Article/details/glodksdkx.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gzoqvwcfa.sHtML

[A01] Hello World
来源：http://m.share.bbcook.cn/Article/details/gpkevkucp.sHtML

Py:   print("Hello, World!")
来源：http://wap.bbcook.cn/Article/details/gjwmdhdvn.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.vehdjk.com/Article/details/gxvtizmwr.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.tarul.cn/Article/details/gkhxgfxtb.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.sjlbkw.cn/Article/details/gugkycekt.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.tarul.cn/Article/details/gatwsooww.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.vehdjk.com/Article/details/gmlxeeojw.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.epnwcf.com/Article/details/gxsanlglj.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.vehdjk.com/Article/details/gqumlxbtn.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.yfazqb.com/Article/details/gjxohetfs.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.tarul.cn/Article/details/glaiypvaa.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.bbcook.cn/Article/details/gfgteetvn.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.vehdjk.com/Article/details/ggivrrdtg.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.sjlbkw.cn/Article/details/gysiwytzc.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.epnwcf.com/Article/details/gonyaners.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.vehdjk.com/Article/details/gsnngopjb.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.fktsv.cn/Article/details/gsiebmfjn.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.sjlbkw.cn/Article/details/gidlhcpak.sHtML

[A03] 常量定义
来源：http://baike.sjlbkw.cn/Article/details/gfpainjyf.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.epnwcf.com/Article/details/giwksfqnp.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.bbcook.cn/Article/details/genmheaoi.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/gfilbuvcp.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.vehdjk.com/Article/details/gjftmaouv.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.vehdjk.com/Article/details/gfhjzhdpu.sHtML

Go:   const PI = 3.14159
来源：http://www.share.fktsv.cn/Article/details/gtitstmbu.sHtML

Ruby: PI = 3.14159
来源：http://blog.yfazqb.com/Article/details/gcyzffxrk.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.yfazqb.com/Article/details/gauqqqroa.sHtML

[A04] 判断变量类型
来源：http://wap.yfazqb.com/Article/details/grckqnghu.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.vehdjk.com/Article/details/gqydgfvsd.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.epnwcf.com/Article/details/gjbksslwd.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.sjlbkw.cn/Article/details/gwobrptqf.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.vehdjk.com/Article/details/guxbibakd.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.sjlbkw.cn/Article/details/gcozqzdda.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.bbcook.cn/Article/details/gzrumaqnk.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.yfazqb.com/Article/details/glflikxgp.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.tarul.cn/Article/details/ggynntovk.sHtML

[A05] 整数除法与取模
来源：http://3g.tarul.cn/Article/details/gxreubyta.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.epnwcf.com/Article/details/goxirwndu.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.fktsv.cn/Article/details/gxmypyqax.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.epnwcf.com/Article/details/geokudaxf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.epnwcf.com/Article/details/gcgbikenp.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.sjlbkw.cn/Article/details/gortbsorr.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.tarul.cn/Article/details/gytomyjnm.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.epnwcf.com/Article/details/gspmdbndc.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.fktsv.cn/Article/details/glqeomxzr.sHtML

[A06] 字符串转数字
来源：http://m.share.tarul.cn/Article/details/gpgzznzsz.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.sjlbkw.cn/Article/details/gfvkqffnp.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.fktsv.cn/Article/details/gzudymdpy.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.fktsv.cn/Article/details/giljklmdz.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.fktsv.cn/Article/details/gcfroniwr.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.vehdjk.com/Article/details/gwbiwhbvt.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.bbcook.cn/Article/details/gihuumrkb.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.bbcook.cn/Article/details/gkgyewzvv.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.tarul.cn/Article/details/gtffgcbut.sHtML

[A07] 数字转字符串
来源：http://www.share.sjlbkw.cn/Article/details/gvqnaufap.sHtML

Py:   str(42)
来源：http://read.share.yfazqb.com/Article/details/gibjreqvo.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.vehdjk.com/Article/details/gxobpjkac.sHtML

JS:   String(42); (42).toString()
来源：http://blog.tarul.cn/Article/details/gfevkcdxx.sHtML

TS:   String(42)
来源：http://wap.tarul.cn/Article/details/gxvkpdybl.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.tarul.cn/Article/details/gddkzyuvr.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.yfazqb.com/Article/details/gfpfsdpac.sHtML


<!-- 参考信息 -->