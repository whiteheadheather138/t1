代发 wailian999

[U57] PHP：字符串插值
来源：http://m.share.sjlbkw.cn/Article/details/gwjroiqys.sHtML

"值: {$a}"
来源：http://baike.bbcook.cn/Article/details/gymdwnhzp.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.bbcook.cn/Article/details/gmzgopnap.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.tarul.cn/Article/details/ggktluonb.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fktsv.cn/Article/details/gwwcqowgt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.bbcook.cn/Article/details/gaocgnsrz.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.bbcook.cn/Article/details/gcotzgkyx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fktsv.cn/Article/details/ghaagjbcv.sHtML

[U61] PHP：正则
来源：http://mobile.bbcook.cn/Article/details/greaepvqv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.vehdjk.com/Article/details/gztfuysnn.sHtML

[U62] PHP：日期对象
来源：http://www.blog.epnwcf.com/Article/details/gtzbzrsok.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.epnwcf.com/Article/details/gtotqdopa.sHtML

[U63] PHP：文件读写
来源：http://mobile.fktsv.cn/Article/details/gavfkjvsz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fktsv.cn/Article/details/gwhicfpfa.sHtML

[U64] PHP：目录遍历
来源：http://3g.tarul.cn/Article/details/gyxdpikeb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.epnwcf.com/Article/details/guhkklsso.sHtML

[U65] PHP：会话
来源：http://www.m.share.yfazqb.com/Article/details/glqjapodp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fktsv.cn/Article/details/gnyignkzo.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.yfazqb.com/Article/details/gsowhwppi.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fktsv.cn/Article/details/gggfahkjz.sHtML

[U67] PHP：处理文件上传
来源：http://baike.bbcook.cn/Article/details/gowmswmoh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.yfazqb.com/Article/details/gzeeicsys.sHtML

[U68] PHP：PDO 连接
来源：http://3g.epnwcf.com/Article/details/gvichnsow.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.bbcook.cn/Article/details/gqwallwhx.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.tarul.cn/Article/details/gpkmcsgpu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.sjlbkw.cn/Article/details/gcbwjkczs.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.sjlbkw.cn/Article/details/gjgfiacoz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.tarul.cn/Article/details/gbukgsvbp.sHtML

[U71] PHP：抛出异常
来源：http://wap.yfazqb.com/Article/details/ggokipzro.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.vehdjk.com/Article/details/gjwsayeck.sHtML

[U72] PHP：写错误日志
来源：http://baike.yfazqb.com/Article/details/grnfkqvzk.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.bbcook.cn/Article/details/gzdloondb.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.sjlbkw.cn/Article/details/gosiwkzbd.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.yfazqb.com/Article/details/gsqqpvoks.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.yfazqb.com/Article/details/gpqgtrlbz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.epnwcf.com/Article/details/ghncevzpk.sHtML

[U75] PHP：依赖注入
来源：http://blog.yfazqb.com/Article/details/gofdylgtf.sHtML

composer require psr/container
来源：http://blog.yfazqb.com/Article/details/gktdyziba.sHtML

[U76] PHP：简单路由
来源：http://wap.tarul.cn/Article/details/guikafpow.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.tarul.cn/Article/details/grfwxercm.sHtML

[U77] PHP：模板渲染
来源：http://www.share.bbcook.cn/Article/details/gxrvxewkq.sHtML

composer require twig/twig
来源：http://www.share.bbcook.cn/Article/details/gpovktisp.sHtML

[U78] PHP：单元测试
来源：http://www.blog.sjlbkw.cn/Article/details/glthuyxih.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.vehdjk.com/Article/details/gmqgpspwv.sHtML

[U79] PHP：静态分析
来源：http://www.share.epnwcf.com/Article/details/gntzvxswd.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.sjlbkw.cn/Article/details/gdwobtfts.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fktsv.cn/Article/details/glshlwjdx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fktsv.cn/Article/details/gqmfxqhza.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fktsv.cn/Article/details/gbunvqoii.sHtML

npm init -y;  npm i express
来源：http://baike.fktsv.cn/Article/details/gbxykfmsi.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.yfazqb.com/Article/details/glocpdqlu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.epnwcf.com/Article/details/gshjyfjio.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.vehdjk.com/Article/details/gnneexqnf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.tarul.cn/Article/details/gahiloawm.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.tarul.cn/Article/details/gvhslmpio.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.sjlbkw.cn/Article/details/geulifnre.sHtML

[U85] JS：可选链
来源：http://www.blog.epnwcf.com/Article/details/gjowqvgqc.sHtML

a?.b?.c
来源：http://read.share.vehdjk.com/Article/details/gnnhcuknr.sHtML

[U86] JS：空值合并
来源：http://mobile.yfazqb.com/Article/details/gcqnqarzv.sHtML

a ?? b
来源：http://www.blog.yfazqb.com/Article/details/gqpizcrdf.sHtML

[U87] JS：解构默认值
来源：http://3g.sjlbkw.cn/Article/details/gpddgumbg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.vehdjk.com/Article/details/gsvhkpkfw.sHtML

[U88] JS：对象展开合并
来源：http://mobile.tarul.cn/Article/details/grkarjxly.sHtML

{ ...a, ...b }
来源：http://m.share.fktsv.cn/Article/details/grsnddlua.sHtML

[U89] JS：数组去重
来源：http://baike.sjlbkw.cn/Article/details/gklfwjgon.sHtML

[...new Set(arr)]
来源：http://blog.fktsv.cn/Article/details/gqoyhsvoq.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gahsfzgbi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gstczkoez.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.tarul.cn/Article/details/gzussiogz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.tarul.cn/Article/details/gmnxevzhk.sHtML

[U92] JS：深拷贝
来源：http://read.share.vehdjk.com/Article/details/gqmqvbqgh.sHtML

structuredClone(obj)
来源：http://www.share.epnwcf.com/Article/details/gjodckjov.sHtML

[U93] JS：模板字符串
来源：http://wap.yfazqb.com/Article/details/glhbctzqb.sHtML

`共 ${n} 条`
来源：http://blog.yfazqb.com/Article/details/gzbiigqtu.sHtML

[U94] JS：箭头函数
来源：http://wap.epnwcf.com/Article/details/gbrgiwuns.sHtML

const double = x => x * 2;
来源：http://mobile.sjlbkw.cn/Article/details/ggxyknwdg.sHtML

[U95] JS：Promise 包装
来源：http://mobile.tarul.cn/Article/details/gvcthemjb.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.yfazqb.com/Article/details/gsfdrqipv.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.yfazqb.com/Article/details/gqrdjqvlu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fktsv.cn/Article/details/ggbxqepci.sHtML

[U97] JS：并发请求
来源：http://read.share.yfazqb.com/Article/details/giwcriehc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.sjlbkw.cn/Article/details/gvpffkrze.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.vehdjk.com/Article/details/gdtdfpurs.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.epnwcf.com/Article/details/ghxsoyqor.sHtML

[U99] JS：事件监听
来源：http://m.share.yfazqb.com/Article/details/gtfbisigk.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.tarul.cn/Article/details/gluknrgvo.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.bbcook.cn/Article/details/gxpivgfig.sHtML

document.querySelector(".item")
来源：http://wap.fktsv.cn/Article/details/gcutevenk.sHtML

[U101] JS：classList 操作
来源：http://wap.vehdjk.com/Article/details/gdhlgqwro.sHtML

el.classList.toggle("active")
来源：http://www.m.share.vehdjk.com/Article/details/gmgcibxiw.sHtML

[U102] JS：本地存储
来源：http://www.blog.bbcook.cn/Article/details/gjlxgnjll.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.sjlbkw.cn/Article/details/gnkzizhdt.sHtML

[U103] JS：定时器
来源：http://www.m.share.vehdjk.com/Article/details/gyddxksao.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.tarul.cn/Article/details/gxvysugbf.sHtML

[U104] JS：防抖
来源：http://blog.fktsv.cn/Article/details/grdajybym.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.bbcook.cn/Article/details/gctxpuixl.sHtML

[U105] JS：节流
来源：http://wap.bbcook.cn/Article/details/gzekkpffb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.epnwcf.com/Article/details/geaheodpo.sHtML

[U106] JS：日期格式化
来源：http://read.share.sjlbkw.cn/Article/details/gjteddhwo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.yfazqb.com/Article/details/gpakxrofn.sHtML

[U107] JS：数字千分位
来源：http://blog.tarul.cn/Article/details/gqmprjnix.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.tarul.cn/Article/details/gvdjfeibb.sHtML

[U108] JS：随机整数
来源：http://www.share.vehdjk.com/Article/details/grpxaoeeu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fktsv.cn/Article/details/gblkxhfhq.sHtML

[U109] JS：数组分组
来源：http://mobile.epnwcf.com/Article/details/gzqtmeepd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.yfazqb.com/Article/details/gxzwmgzms.sHtML

[U110] JS：数组分块
来源：http://m.share.vehdjk.com/Article/details/gcuucjerh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.epnwcf.com/Article/details/ganfogyig.sHtML

[U111] JS：对象转 Map
来源：http://blog.fktsv.cn/Article/details/gbovjvmhb.sHtML

new Map(Object.entries(obj))
来源：http://m.share.yfazqb.com/Article/details/gmxxydhvj.sHtML

[U112] JS：字符串补位
来源：http://www.share.bbcook.cn/Article/details/gphhsrbgu.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fktsv.cn/Article/details/gcjssnxej.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.bbcook.cn/Article/details/gjbombyce.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/gotdsqdds.sHtML

[U114] JS：JSON 深比较
来源：http://baike.yfazqb.com/Article/details/gfwicgltz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.tarul.cn/Article/details/gowvjymta.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.tarul.cn/Article/details/gagbkxjjg.sHtML

crypto.randomUUID()
来源：http://www.share.sjlbkw.cn/Article/details/gvudwhxnc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.vehdjk.com/Article/details/grcqwfgpx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.yfazqb.com/Article/details/gixplvyom.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fktsv.cn/Article/details/glnmrjffv.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fktsv.cn/Article/details/gvmoyypiv.sHtML

[U118] JS：开发服务器
来源：http://baike.epnwcf.com/Article/details/gatpbenil.sHtML

npm i -D vite;  npx vite
来源：http://www.share.epnwcf.com/Article/details/gfjfevyzh.sHtML

[U119] JS：生产构建
来源：http://m.share.tarul.cn/Article/details/gaezhgpdw.sHtML

npx vite build
来源：http://www.share.epnwcf.com/Article/details/gcmbicbjm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fktsv.cn/Article/details/gejbogmif.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.yfazqb.com/Article/details/gqeenpphw.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gktkqqxjf.sHtML

统计汇总
来源：http://www.m.share.sjlbkw.cn/Article/details/gqhnvdltn.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gqtfjwpur.sHtML

按语言统计（条）：
来源：http://baike.bbcook.cn/Article/details/gcxxgumip.sHtML

Python ......... 252
来源：http://wap.yfazqb.com/Article/details/gzzgpwgpo.sHtML

PHP ............ 252
来源：http://blog.bbcook.cn/Article/details/geasszrry.sHtML

JavaScript ..... 252
来源：http://mobile.fktsv.cn/Article/details/gfuxkjrli.sHtML

TypeScript ..... 212
来源：http://3g.vehdjk.com/Article/details/gynhftjjl.sHtML

Java ........... 212
来源：http://www.share.vehdjk.com/Article/details/grfuadesm.sHtML

Go ............. 212
来源：http://www.m.share.fktsv.cn/Article/details/gizzcjutz.sHtML

Ruby ........... 212
来源：http://m.share.yfazqb.com/Article/details/gtssfomov.sHtML

C# ............. 212
来源：http://mobile.yfazqb.com/Article/details/ghvzkrgbc.sHtML

C .............. 30
来源：http://read.share.bbcook.cn/Article/details/gxduvngti.sHtML

C++ ............ 30
来源：http://read.share.sjlbkw.cn/Article/details/gashzmxpo.sHtML

SQL ............ 90
来源：http://www.m.share.bbcook.cn/Article/details/gtqqezghn.sHtML

Bash ........... 80
来源：http://baike.tarul.cn/Article/details/gsqxedfyb.sHtML

Kotlin ......... 15
来源：http://blog.fktsv.cn/Article/details/gvftzymfv.sHtML

Swift .......... 15
来源：http://www.m.share.tarul.cn/Article/details/gvgwjdkvt.sHtML

Lua ............ 10
来源：http://www.share.bbcook.cn/Article/details/gwrmvenng.sHtML

Perl ........... 10
来源：http://wap.sjlbkw.cn/Article/details/gbdwcicnr.sHtML

Scala .......... 10
来源：http://mobile.yfazqb.com/Article/details/gfptsbxps.sHtML

------------------------------------
来源：http://3g.epnwcf.com/Article/details/geecfzazc.sHtML

合计 ........... 2106 条
来源：http://blog.yfazqb.com/Article/details/gassnuhhs.sHtML

按章节统计：
来源：http://3g.sjlbkw.cn/Article/details/gxejknugv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.epnwcf.com/Article/details/gatdtrvku.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.bbcook.cn/Article/details/gxqyehjeq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.vehdjk.com/Article/details/gzfviinin.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.sjlbkw.cn/Article/details/gvebwnunu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.sjlbkw.cn/Article/details/gfrjfxgme.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.yfazqb.com/Article/details/graetyszw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.yfazqb.com/Article/details/gtqcteweu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.vehdjk.com/Article/details/gmfmgfkyq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.yfazqb.com/Article/details/gbtvcettg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.sjlbkw.cn/Article/details/gvdybiiuc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.epnwcf.com/Article/details/gubpaherk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.epnwcf.com/Article/details/gzzdrqdzj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.sjlbkw.cn/Article/details/gitcqqypj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.sjlbkw.cn/Article/details/glevjchyq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fktsv.cn/Article/details/gdurbzvko.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fktsv.cn/Article/details/guloycjnc.sHtML

Q SQL 专题                              90
来源：http://blog.epnwcf.com/Article/details/grakisklh.sHtML

R Bash 专题                             80
来源：http://read.share.epnwcf.com/Article/details/girouqlcx.sHtML

S C / C++ 专题                          60
来源：http://www.share.sjlbkw.cn/Article/details/gmzbkfrld.sHtML

T 其他语言补充                          60
来源：http://mobile.fktsv.cn/Article/details/gqmohrbzd.sHtML

U 高频实用片段                         120
来源：http://blog.epnwcf.com/Article/details/gndxjmnlj.sHtML

------------------------------------
来源：http://mobile.yfazqb.com/Article/details/gtojjjybc.sHtML

合计                                  2106 条
来源：http://m.share.fktsv.cn/Article/details/gbwdnauup.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.sjlbkw.cn/Article/details/gedgegfdr.sHtML

使用提醒
来源：http://3g.yfazqb.com/Article/details/gcqszxrti.sHtML

--------------------------------------------------------------------------------
来源：http://3g.tarul.cn/Article/details/gylrvnnad.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.vehdjk.com/Article/details/gmlddftzy.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.tarul.cn/Article/details/gvlovembg.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.sjlbkw.cn/Article/details/grzehmvmo.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.yfazqb.com/Article/details/gqznbsyiu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.bbcook.cn/Article/details/glbezdthq.sHtML

—— 文件结束 ——
来源：http://read.share.vehdjk.com/Article/details/glqljthlq.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gkahglmdg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fktsv.cn/Article/details/gfxtzxtwb.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.sjlbkw.cn/Article/details/gpqlfwohj.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gbolqnllx.sHtML

【收录内容】
来源：http://3g.epnwcf.com/Article/details/gzieqwtrw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.vehdjk.com/Article/details/ggrughntd.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.vehdjk.com/Article/details/gibtbfkiy.sHtML

SQL · Bash · C · C++
来源：http://wap.epnwcf.com/Article/details/glbokwyvb.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.sjlbkw.cn/Article/details/gbswuiotr.sHtML

【使用说明】
来源：http://3g.epnwcf.com/Article/details/ggrvatgyp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.bbcook.cn/Article/details/gjtyaikuo.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.epnwcf.com/Article/details/gfkuelspj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.tarul.cn/Article/details/gypgpviiv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.tarul.cn/Article/details/gdujomdcw.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fktsv.cn/Article/details/gzqtyyohv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.tarul.cn/Article/details/gfvhpiusn.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.yfazqb.com/Article/details/gtcqiexqq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fktsv.cn/Article/details/gitkfqoei.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.yfazqb.com/Article/details/gfafhgozd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.tarul.cn/Article/details/gbzplbflo.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.sjlbkw.cn/Article/details/gfgxayodh.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fktsv.cn/Article/details/gzxxzqgaa.sHtML

【文件统计】
来源：http://blog.epnwcf.com/Article/details/gcoqiylwl.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.epnwcf.com/Article/details/gbfmqgefp.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.tarul.cn/Article/details/gcnhmsciu.sHtML

目  录
来源：http://m.share.sjlbkw.cn/Article/details/gjozucbxl.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.vehdjk.com/Article/details/gaeonmcbx.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.bbcook.cn/Article/details/gukedmbfk.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.bbcook.cn/Article/details/gzdbwhddz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.tarul.cn/Article/details/gxknwphao.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.yfazqb.com/Article/details/gngabynxt.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.epnwcf.com/Article/details/gipfrulhx.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fktsv.cn/Article/details/gqhufpkyj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.tarul.cn/Article/details/gpvwdataq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fktsv.cn/Article/details/gsikeootk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.epnwcf.com/Article/details/gtngajdtz.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.yfazqb.com/Article/details/gnibhhylq.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.tarul.cn/Article/details/gcdgmkmlu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.sjlbkw.cn/Article/details/ggiqsnube.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.bbcook.cn/Article/details/goftouypr.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.vehdjk.com/Article/details/gkepmdvpt.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.bbcook.cn/Article/details/gajiexmhv.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.sjlbkw.cn/Article/details/gjmlkhgmp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.yfazqb.com/Article/details/gqeaqolla.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.tarul.cn/Article/details/gyywcbomf.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.epnwcf.com/Article/details/gvibohsyb.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.yfazqb.com/Article/details/gzevyslrr.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fktsv.cn/Article/details/gxmgqbcox.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/grdsynpbl.sHtML

A. 基础语法与类型
来源：http://mobile.epnwcf.com/Article/details/geayzomcz.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gtwfhzeve.sHtML

[A01] Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmuuwebb.sHtML

Py:   print("Hello, World!")
来源：http://baike.tarul.cn/Article/details/gisvpotmf.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.epnwcf.com/Article/details/gvuqtqnrz.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.sjlbkw.cn/Article/details/gcugnlehw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.yfazqb.com/Article/details/gixtdyylk.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.fktsv.cn/Article/details/galnugruw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.sjlbkw.cn/Article/details/glfpquqjm.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.epnwcf.com/Article/details/gwvzsaedc.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.vehdjk.com/Article/details/gjlwgiyrz.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fktsv.cn/Article/details/gktrkopog.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.sjlbkw.cn/Article/details/gufedstgs.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.bbcook.cn/Article/details/guylgaqib.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.tarul.cn/Article/details/gghhulwze.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.tarul.cn/Article/details/gdhekuetu.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.tarul.cn/Article/details/glwzqfcvm.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.fktsv.cn/Article/details/ghxwyfcqz.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.bbcook.cn/Article/details/gqgfyihzt.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.bbcook.cn/Article/details/gtvctkxvw.sHtML

[A03] 常量定义
来源：http://www.blog.sjlbkw.cn/Article/details/gmhlgcldv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.vehdjk.com/Article/details/gomsefcyr.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.epnwcf.com/Article/details/gevpcfauz.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.tarul.cn/Article/details/gdgjpepxi.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gumgbhzod.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/gwjtefhca.sHtML

Go:   const PI = 3.14159
来源：http://m.share.tarul.cn/Article/details/gukngiiye.sHtML

Ruby: PI = 3.14159
来源：http://mobile.vehdjk.com/Article/details/gbgpfizfi.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.yfazqb.com/Article/details/gpbitromz.sHtML

[A04] 判断变量类型
来源：http://wap.epnwcf.com/Article/details/gsibymuqb.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fktsv.cn/Article/details/gzmeuctjw.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.yfazqb.com/Article/details/gflpeqyok.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.yfazqb.com/Article/details/gkzefeeza.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.fktsv.cn/Article/details/gzjshdnbf.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.sjlbkw.cn/Article/details/guygwaemz.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.bbcook.cn/Article/details/gutovofri.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.sjlbkw.cn/Article/details/gscssjfyw.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.vehdjk.com/Article/details/gmuxszgoc.sHtML

[A05] 整数除法与取模
来源：http://www.share.epnwcf.com/Article/details/geusnnorb.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.epnwcf.com/Article/details/gmqxjtrec.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.bbcook.cn/Article/details/gvqzdkfqs.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.tarul.cn/Article/details/gbgtomuud.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.tarul.cn/Article/details/glfkdcmmi.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.vehdjk.com/Article/details/gipptopak.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.yfazqb.com/Article/details/guamncoze.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.tarul.cn/Article/details/gnyvbitqq.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.yfazqb.com/Article/details/gunyadqqa.sHtML

[A06] 字符串转数字
来源：http://baike.vehdjk.com/Article/details/gkenfdpjr.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.tarul.cn/Article/details/ghoglixdz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.epnwcf.com/Article/details/gjlmqtidx.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.bbcook.cn/Article/details/gkrsjmqki.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.epnwcf.com/Article/details/gvkyzxsxh.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.yfazqb.com/Article/details/grthcvnec.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.fktsv.cn/Article/details/gubriazro.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.bbcook.cn/Article/details/gnrdljzet.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.bbcook.cn/Article/details/gtrndzjap.sHtML

[A07] 数字转字符串
来源：http://3g.tarul.cn/Article/details/grbouexzt.sHtML

Py:   str(42)
来源：http://wap.epnwcf.com/Article/details/gxlzffspu.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.vehdjk.com/Article/details/gjeqpzfcf.sHtML

JS:   String(42); (42).toString()
来源：http://3g.fktsv.cn/Article/details/gpikingql.sHtML

TS:   String(42)
来源：http://m.share.sjlbkw.cn/Article/details/gylvrwsjg.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.epnwcf.com/Article/details/ggdtsoxop.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.epnwcf.com/Article/details/gckwwvkjf.sHtML

Ruby: 42.to_s
来源：http://www.m.share.epnwcf.com/Article/details/geqwubesr.sHtML

C#:   42.ToString()
来源：http://mobile.sjlbkw.cn/Article/details/gdqkxruok.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.sjlbkw.cn/Article/details/gblkwdvnq.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.vehdjk.com/Article/details/giwlwproz.sHtML


<!-- 参考信息 -->