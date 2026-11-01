代发 wailian999

[U53] PHP：空合并运算符
来源：http://read.share.tarul.cn/Article/details/gemezhtxt.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fktsv.cn/Article/details/gqwxpxzji.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.yfazqb.com/Article/details/gxddeluib.sHtML

$obj?->method()
来源：http://baike.epnwcf.com/Article/details/gwctpdnbv.sHtML

[U55] PHP：match 表达式
来源：http://baike.sjlbkw.cn/Article/details/gcudveorc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fktsv.cn/Article/details/gtuirwyvr.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.tarul.cn/Article/details/gylffxzev.sHtML

f(a: 1, b: 2)
来源：http://mobile.tarul.cn/Article/details/gfgqonaqz.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.sjlbkw.cn/Article/details/gzzbnljsx.sHtML

"值: {$a}"
来源：http://baike.fktsv.cn/Article/details/gwcsnpeaj.sHtML

[U58] PHP：数组三件套
来源：http://wap.epnwcf.com/Article/details/gfungqsfz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.sjlbkw.cn/Article/details/gkcriwhyv.sHtML

[U59] PHP：自定义排序
来源：http://www.share.bbcook.cn/Article/details/gacaztymi.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.sjlbkw.cn/Article/details/gjjverebi.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.tarul.cn/Article/details/ggixcpzvj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fktsv.cn/Article/details/gjsoydxcb.sHtML

[U61] PHP：正则
来源：http://www.share.yfazqb.com/Article/details/goqvtttym.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fktsv.cn/Article/details/gevprrjdv.sHtML

[U62] PHP：日期对象
来源：http://read.share.yfazqb.com/Article/details/gxrlfbqeq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.sjlbkw.cn/Article/details/gfnkqdrjo.sHtML

[U63] PHP：文件读写
来源：http://read.share.epnwcf.com/Article/details/gubfhlakb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.yfazqb.com/Article/details/gkijmtqlu.sHtML

[U64] PHP：目录遍历
来源：http://read.share.sjlbkw.cn/Article/details/gqrtwbged.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.sjlbkw.cn/Article/details/ghvdimszs.sHtML

[U65] PHP：会话
来源：http://wap.fktsv.cn/Article/details/gltpkvxok.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gcsoyzsxa.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.bbcook.cn/Article/details/gnexgefnu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.epnwcf.com/Article/details/goqkchxub.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fktsv.cn/Article/details/gsbqqedcx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fktsv.cn/Article/details/gelamxmfs.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.bbcook.cn/Article/details/gqyujygfi.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.vehdjk.com/Article/details/gacmdwttz.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.tarul.cn/Article/details/gmrccllyt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.bbcook.cn/Article/details/glxmrcgke.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.bbcook.cn/Article/details/gvtvzbeda.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.bbcook.cn/Article/details/gijhkmzni.sHtML

[U71] PHP：抛出异常
来源：http://mobile.sjlbkw.cn/Article/details/gnrbictfg.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.epnwcf.com/Article/details/gffnxupuh.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.tarul.cn/Article/details/gkvsiqsim.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.epnwcf.com/Article/details/grjioxmcm.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fktsv.cn/Article/details/gdypfilsc.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.bbcook.cn/Article/details/goxlvfdlu.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.vehdjk.com/Article/details/grafgicfs.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.yfazqb.com/Article/details/gtznvyzzb.sHtML

[U75] PHP：依赖注入
来源：http://wap.bbcook.cn/Article/details/gfpwvcxxs.sHtML

composer require psr/container
来源：http://read.share.sjlbkw.cn/Article/details/gqymvrjaa.sHtML

[U76] PHP：简单路由
来源：http://blog.epnwcf.com/Article/details/gisekqsgr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.sjlbkw.cn/Article/details/gzvbynxdo.sHtML

[U77] PHP：模板渲染
来源：http://3g.tarul.cn/Article/details/glavqansj.sHtML

composer require twig/twig
来源：http://wap.fktsv.cn/Article/details/gzagphinz.sHtML

[U78] PHP：单元测试
来源：http://blog.epnwcf.com/Article/details/ggghbidwr.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.vehdjk.com/Article/details/gmauvhbkf.sHtML

[U79] PHP：静态分析
来源：http://blog.bbcook.cn/Article/details/gapgsavtu.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.bbcook.cn/Article/details/gnaszfvgm.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.sjlbkw.cn/Article/details/gnifhtzcb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.epnwcf.com/Article/details/gfqxrqwqy.sHtML

[U81] JS：初始化项目
来源：http://www.share.bbcook.cn/Article/details/gktachfse.sHtML

npm init -y;  npm i express
来源：http://baike.sjlbkw.cn/Article/details/gcvjnjtxk.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fktsv.cn/Article/details/gqkezxfpa.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.vehdjk.com/Article/details/gjuatsbgt.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.bbcook.cn/Article/details/gistduhbl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.yfazqb.com/Article/details/gckfnpnqr.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.sjlbkw.cn/Article/details/gznjaawbl.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.tarul.cn/Article/details/gblhihmbs.sHtML

[U85] JS：可选链
来源：http://3g.vehdjk.com/Article/details/gxgjjnrxi.sHtML

a?.b?.c
来源：http://read.share.yfazqb.com/Article/details/gxliferzf.sHtML

[U86] JS：空值合并
来源：http://m.share.yfazqb.com/Article/details/gsvthsoui.sHtML

a ?? b
来源：http://wap.epnwcf.com/Article/details/gqpcgqgfo.sHtML

[U87] JS：解构默认值
来源：http://m.share.epnwcf.com/Article/details/gocqtcphl.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fktsv.cn/Article/details/ggazwvaxf.sHtML

[U88] JS：对象展开合并
来源：http://read.share.bbcook.cn/Article/details/gcsazirsl.sHtML

{ ...a, ...b }
来源：http://m.share.bbcook.cn/Article/details/gptyttvyi.sHtML

[U89] JS：数组去重
来源：http://baike.tarul.cn/Article/details/gitevqwcs.sHtML

[...new Set(arr)]
来源：http://mobile.tarul.cn/Article/details/ggsbbehnf.sHtML

[U90] JS：数字数组排序
来源：http://wap.bbcook.cn/Article/details/gyhfajmuf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.yfazqb.com/Article/details/gesnlnqux.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.tarul.cn/Article/details/gijlkocrr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.bbcook.cn/Article/details/gxmujtlkd.sHtML

[U92] JS：深拷贝
来源：http://www.share.tarul.cn/Article/details/gtgfqywij.sHtML

structuredClone(obj)
来源：http://www.share.epnwcf.com/Article/details/gbxilakoj.sHtML

[U93] JS：模板字符串
来源：http://blog.fktsv.cn/Article/details/gbvozumwa.sHtML

`共 ${n} 条`
来源：http://www.blog.vehdjk.com/Article/details/gzdkzlzls.sHtML

[U94] JS：箭头函数
来源：http://blog.epnwcf.com/Article/details/ggxkkhhap.sHtML

const double = x => x * 2;
来源：http://read.share.epnwcf.com/Article/details/gkswqzoak.sHtML

[U95] JS：Promise 包装
来源：http://blog.bbcook.cn/Article/details/gwmbsjqel.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fktsv.cn/Article/details/gagbabdtv.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.vehdjk.com/Article/details/gsegplijy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.epnwcf.com/Article/details/gqqckflmr.sHtML

[U97] JS：并发请求
来源：http://www.share.vehdjk.com/Article/details/gmpwpppeg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.yfazqb.com/Article/details/gvpnfjtic.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.sjlbkw.cn/Article/details/gaefxdmlp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.vehdjk.com/Article/details/gmuaoqklt.sHtML

[U99] JS：事件监听
来源：http://www.share.yfazqb.com/Article/details/gvtmbguyv.sHtML

el.addEventListener("click", e => {})
来源：http://wap.bbcook.cn/Article/details/gprzugjkk.sHtML

[U100] JS：DOM 查询
来源：http://wap.fktsv.cn/Article/details/gjfcazdcb.sHtML

document.querySelector(".item")
来源：http://www.blog.sjlbkw.cn/Article/details/gwhxeqcpr.sHtML

[U101] JS：classList 操作
来源：http://www.blog.sjlbkw.cn/Article/details/gbjoyhjfs.sHtML

el.classList.toggle("active")
来源：http://mobile.yfazqb.com/Article/details/gqezysvla.sHtML

[U102] JS：本地存储
来源：http://www.blog.bbcook.cn/Article/details/gukypaasv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fktsv.cn/Article/details/gbniyvkyk.sHtML

[U103] JS：定时器
来源：http://blog.tarul.cn/Article/details/gwjexzbbz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.vehdjk.com/Article/details/gdvjzuomh.sHtML

[U104] JS：防抖
来源：http://blog.fktsv.cn/Article/details/gdycrquxq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.yfazqb.com/Article/details/gedtfedle.sHtML

[U105] JS：节流
来源：http://blog.sjlbkw.cn/Article/details/gcnefdznr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.vehdjk.com/Article/details/gtoflllfq.sHtML

[U106] JS：日期格式化
来源：http://www.blog.sjlbkw.cn/Article/details/gxhcltebz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.tarul.cn/Article/details/gzlwklgli.sHtML

[U107] JS：数字千分位
来源：http://mobile.vehdjk.com/Article/details/gnxqsrkrz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.vehdjk.com/Article/details/gewswpebo.sHtML

[U108] JS：随机整数
来源：http://www.m.share.bbcook.cn/Article/details/gxurrwpxc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.epnwcf.com/Article/details/ghdmtloms.sHtML

[U109] JS：数组分组
来源：http://baike.tarul.cn/Article/details/ghpgfqhqk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.yfazqb.com/Article/details/gucjornkb.sHtML

[U110] JS：数组分块
来源：http://wap.tarul.cn/Article/details/gsexhkosw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.yfazqb.com/Article/details/gbjapwrqx.sHtML

[U111] JS：对象转 Map
来源：http://read.share.epnwcf.com/Article/details/gzsmzkktf.sHtML

new Map(Object.entries(obj))
来源：http://blog.epnwcf.com/Article/details/gkpuptkxv.sHtML

[U112] JS：字符串补位
来源：http://mobile.sjlbkw.cn/Article/details/gmuuppuzb.sHtML

"7".padStart(3, "0")
来源：http://blog.bbcook.cn/Article/details/gebezwxim.sHtML

[U113] JS：正则替换全部
来源：http://blog.vehdjk.com/Article/details/glzrbglvo.sHtML

s.replaceAll("a", "b")
来源：http://baike.tarul.cn/Article/details/gbdmrohoc.sHtML

[U114] JS：JSON 深比较
来源：http://baike.vehdjk.com/Article/details/grnnyetag.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.tarul.cn/Article/details/gjloxsmhw.sHtML

[U115] JS：生成 UUID
来源：http://mobile.sjlbkw.cn/Article/details/giorsfols.sHtML

crypto.randomUUID()
来源：http://www.blog.bbcook.cn/Article/details/gceqhjbqa.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.yfazqb.com/Article/details/gvmevnrpb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.epnwcf.com/Article/details/gkwtuemqd.sHtML

[U117] JS：单元测试
来源：http://wap.sjlbkw.cn/Article/details/gmmnfdfiy.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fktsv.cn/Article/details/gktkvupgn.sHtML

[U118] JS：开发服务器
来源：http://read.share.sjlbkw.cn/Article/details/gidtturow.sHtML

npm i -D vite;  npx vite
来源：http://3g.tarul.cn/Article/details/goalvdntv.sHtML

[U119] JS：生产构建
来源：http://m.share.tarul.cn/Article/details/ggiqkijpp.sHtML

npx vite build
来源：http://blog.yfazqb.com/Article/details/gsceesufm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.bbcook.cn/Article/details/gtankgxsa.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.sjlbkw.cn/Article/details/gnkuslbsk.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/ggecnedjl.sHtML

统计汇总
来源：http://m.share.epnwcf.com/Article/details/gepcmdnii.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gnpdfrcpk.sHtML

按语言统计（条）：
来源：http://baike.fktsv.cn/Article/details/gituxirto.sHtML

Python ......... 252
来源：http://blog.tarul.cn/Article/details/gfutnplgb.sHtML

PHP ............ 252
来源：http://wap.bbcook.cn/Article/details/glbrwscri.sHtML

JavaScript ..... 252
来源：http://3g.vehdjk.com/Article/details/gtrawvmjh.sHtML

TypeScript ..... 212
来源：http://blog.tarul.cn/Article/details/gggspcive.sHtML

Java ........... 212
来源：http://read.share.yfazqb.com/Article/details/ghxqkzkpb.sHtML

Go ............. 212
来源：http://read.share.vehdjk.com/Article/details/gmhaxxljq.sHtML

Ruby ........... 212
来源：http://m.share.epnwcf.com/Article/details/gyldgsqzc.sHtML

C# ............. 212
来源：http://read.share.bbcook.cn/Article/details/gefugzhin.sHtML

C .............. 30
来源：http://baike.fktsv.cn/Article/details/gzixuffll.sHtML

C++ ............ 30
来源：http://www.blog.tarul.cn/Article/details/gyhqtrrff.sHtML

SQL ............ 90
来源：http://blog.sjlbkw.cn/Article/details/gkqljxmqc.sHtML

Bash ........... 80
来源：http://www.blog.tarul.cn/Article/details/gnjozfndk.sHtML

Kotlin ......... 15
来源：http://baike.sjlbkw.cn/Article/details/gvuzbuern.sHtML

Swift .......... 15
来源：http://wap.tarul.cn/Article/details/gztwzqxmx.sHtML

Lua ............ 10
来源：http://blog.yfazqb.com/Article/details/gjvuqjmsw.sHtML

Perl ........... 10
来源：http://baike.yfazqb.com/Article/details/gxwutwzgu.sHtML

Scala .......... 10
来源：http://blog.vehdjk.com/Article/details/gvdrldmpq.sHtML

------------------------------------
来源：http://m.share.epnwcf.com/Article/details/ggnnznmcn.sHtML

合计 ........... 2106 条
来源：http://m.share.fktsv.cn/Article/details/gqxsisoxc.sHtML

按章节统计：
来源：http://www.share.epnwcf.com/Article/details/gjdplbcft.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.yfazqb.com/Article/details/gchusclbd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.vehdjk.com/Article/details/ghbxdubtk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.bbcook.cn/Article/details/gafgmcnew.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.epnwcf.com/Article/details/gkqaygggv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.sjlbkw.cn/Article/details/gaxcnegcr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.bbcook.cn/Article/details/grlejdbdj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.bbcook.cn/Article/details/gmihmxxpm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.epnwcf.com/Article/details/gwrjobohk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.sjlbkw.cn/Article/details/gfdqhckim.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.tarul.cn/Article/details/ghrixxkck.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.epnwcf.com/Article/details/gssdppdsy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.epnwcf.com/Article/details/grtewzdyi.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.sjlbkw.cn/Article/details/gvrewyzku.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.epnwcf.com/Article/details/gjefbeymo.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.tarul.cn/Article/details/gfjedzgxz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.sjlbkw.cn/Article/details/gxeqtpnwp.sHtML

Q SQL 专题                              90
来源：http://blog.epnwcf.com/Article/details/gtklkgdlq.sHtML

R Bash 专题                             80
来源：http://3g.tarul.cn/Article/details/gndrtfipd.sHtML

S C / C++ 专题                          60
来源：http://mobile.yfazqb.com/Article/details/gaemzazwd.sHtML

T 其他语言补充                          60
来源：http://3g.yfazqb.com/Article/details/gbaeqfxja.sHtML

U 高频实用片段                         120
来源：http://baike.tarul.cn/Article/details/gcwjcfswp.sHtML

------------------------------------
来源：http://mobile.fktsv.cn/Article/details/guklxfqyo.sHtML

合计                                  2106 条
来源：http://baike.bbcook.cn/Article/details/govpwnqwo.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.epnwcf.com/Article/details/gbngulkbp.sHtML

使用提醒
来源：http://3g.tarul.cn/Article/details/gftwsagcs.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/gvxcqkiye.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.sjlbkw.cn/Article/details/ghgvlsfmr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.sjlbkw.cn/Article/details/gfqxpuwnz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.bbcook.cn/Article/details/gfhwrtegd.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.sjlbkw.cn/Article/details/gxbrzzldi.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.bbcook.cn/Article/details/gibdtpukj.sHtML

—— 文件结束 ——
来源：http://www.share.epnwcf.com/Article/details/ggkxivkzn.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gqznorchy.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.yfazqb.com/Article/details/gdinkaofn.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.vehdjk.com/Article/details/ggvucqhoh.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gnryvecsb.sHtML

【收录内容】
来源：http://www.share.fktsv.cn/Article/details/ghyntqevb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.bbcook.cn/Article/details/glyckegfu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.tarul.cn/Article/details/gimotyrpd.sHtML

SQL · Bash · C · C++
来源：http://baike.tarul.cn/Article/details/ghasalfcl.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fktsv.cn/Article/details/gnpcepcca.sHtML

【使用说明】
来源：http://blog.epnwcf.com/Article/details/gyqbnrkqz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.epnwcf.com/Article/details/ghzezkkrm.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.tarul.cn/Article/details/grjtyiyfa.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.tarul.cn/Article/details/gcektemtp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.epnwcf.com/Article/details/gmqbxlrtb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.epnwcf.com/Article/details/gigdxmyoz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.vehdjk.com/Article/details/gvphjhwhx.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.vehdjk.com/Article/details/gxgffsdzo.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.yfazqb.com/Article/details/grbokxxnw.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.bbcook.cn/Article/details/gnygchvih.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.vehdjk.com/Article/details/glhdlzogm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.sjlbkw.cn/Article/details/ghvnnbufn.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fktsv.cn/Article/details/gbfstqtcn.sHtML

【文件统计】
来源：http://read.share.tarul.cn/Article/details/gnbvcdgna.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.vehdjk.com/Article/details/ggvvblxzc.sHtML

--------------------------------------------------------------------------------
来源：http://wap.bbcook.cn/Article/details/govzpvgfm.sHtML

目  录
来源：http://blog.epnwcf.com/Article/details/gwuibiais.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.epnwcf.com/Article/details/ggybkkvxa.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.tarul.cn/Article/details/guqljxkwt.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.epnwcf.com/Article/details/gfxkjumjk.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.vehdjk.com/Article/details/gwlpcinqf.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fktsv.cn/Article/details/gfopqwvmw.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.yfazqb.com/Article/details/giceqjtds.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.epnwcf.com/Article/details/glevhieqy.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.vehdjk.com/Article/details/goxterwbv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.epnwcf.com/Article/details/gnflobjaf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.yfazqb.com/Article/details/gcredniiu.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.epnwcf.com/Article/details/gjrdmeoea.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.epnwcf.com/Article/details/gkpdjgokh.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.tarul.cn/Article/details/gbsgkdzxg.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.fktsv.cn/Article/details/gzlvscyae.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.vehdjk.com/Article/details/gtibuknrs.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.bbcook.cn/Article/details/gvuyrsnrl.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.tarul.cn/Article/details/grdxyatam.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.vehdjk.com/Article/details/gnegpcbgu.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gbismpgau.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.fktsv.cn/Article/details/gwtrotmzt.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fktsv.cn/Article/details/ghibwjqjm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fktsv.cn/Article/details/grzskiypk.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gwgxbfygy.sHtML

A. 基础语法与类型
来源：http://3g.bbcook.cn/Article/details/gihsprdfk.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/glnjczqbh.sHtML

[A01] Hello World
来源：http://www.blog.bbcook.cn/Article/details/gehucfpiw.sHtML

Py:   print("Hello, World!")
来源：http://www.share.yfazqb.com/Article/details/gvpfvhyof.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.epnwcf.com/Article/details/givlxndic.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.bbcook.cn/Article/details/gmevkliny.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.sjlbkw.cn/Article/details/gexpvnogm.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.epnwcf.com/Article/details/gkpthbqnv.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.vehdjk.com/Article/details/ggejzyhnh.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.bbcook.cn/Article/details/gfywgwlat.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.epnwcf.com/Article/details/gmazhotqw.sHtML

[A02] 变量声明与赋值
来源：http://mobile.tarul.cn/Article/details/gofdmvvaw.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.yfazqb.com/Article/details/gddbmiggi.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.bbcook.cn/Article/details/gvhcmeksy.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.fktsv.cn/Article/details/gpxiffrqk.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.yfazqb.com/Article/details/glttzjebh.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.fktsv.cn/Article/details/gbyobkhne.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.yfazqb.com/Article/details/gvroxbpuf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.sjlbkw.cn/Article/details/gvblzunbw.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.vehdjk.com/Article/details/gpppipgdt.sHtML

[A03] 常量定义
来源：http://wap.epnwcf.com/Article/details/gzsvjfvvw.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.yfazqb.com/Article/details/gzdhcpibo.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.tarul.cn/Article/details/genotguhl.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.tarul.cn/Article/details/ggovgipvw.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.fktsv.cn/Article/details/glzasqgbf.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gtmkmlisu.sHtML

Go:   const PI = 3.14159
来源：http://baike.epnwcf.com/Article/details/gqnjocuiz.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.yfazqb.com/Article/details/gulktcqpn.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/gsnbzfjow.sHtML

[A04] 判断变量类型
来源：http://blog.yfazqb.com/Article/details/gtrqqnjsl.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.epnwcf.com/Article/details/gnszfrmqe.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.yfazqb.com/Article/details/gvosqwigh.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.fktsv.cn/Article/details/gbyylmuyu.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.vehdjk.com/Article/details/gxsyffksq.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.tarul.cn/Article/details/gasavecci.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.yfazqb.com/Article/details/gbaoviytf.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.fktsv.cn/Article/details/giawfmnqw.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.yfazqb.com/Article/details/gjoiseqyh.sHtML

[A05] 整数除法与取模
来源：http://blog.sjlbkw.cn/Article/details/gsajqtigx.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.fktsv.cn/Article/details/ggvrfjpzm.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.vehdjk.com/Article/details/glurputaf.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.epnwcf.com/Article/details/gybvxelzg.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.tarul.cn/Article/details/gooivbyjt.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gxzcucceg.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.fktsv.cn/Article/details/guzzqkywe.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.vehdjk.com/Article/details/gesskigop.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.yfazqb.com/Article/details/gdbcdvadg.sHtML

[A06] 字符串转数字
来源：http://wap.vehdjk.com/Article/details/gjnrtgpui.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.vehdjk.com/Article/details/gevybqqeq.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.fktsv.cn/Article/details/ghhkfjevu.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.sjlbkw.cn/Article/details/gsddczmty.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.fktsv.cn/Article/details/gtyetfpoc.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.fktsv.cn/Article/details/gjpcjxrqj.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.sjlbkw.cn/Article/details/gvetcinul.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.fktsv.cn/Article/details/gobgqqqxc.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.yfazqb.com/Article/details/gcwpaprpn.sHtML

[A07] 数字转字符串
来源：http://3g.yfazqb.com/Article/details/gajxcuygs.sHtML

Py:   str(42)
来源：http://www.share.sjlbkw.cn/Article/details/gvqkykmvt.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.vehdjk.com/Article/details/gpsbgtjzs.sHtML


<!-- 参考信息 -->