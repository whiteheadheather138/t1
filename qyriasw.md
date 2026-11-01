代发 wailian999

[U59] PHP：自定义排序
来源：http://baike.bbcook.cn/Article/details/gshljgcot.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.vehdjk.com/Article/details/gavkhxpqy.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.sjlbkw.cn/Article/details/grwfhfkgj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fktsv.cn/Article/details/gitbeorrp.sHtML

[U61] PHP：正则
来源：http://blog.tarul.cn/Article/details/gpwdxbhsy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.tarul.cn/Article/details/gnauqtiow.sHtML

[U62] PHP：日期对象
来源：http://www.share.bbcook.cn/Article/details/gdmijssdt.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.vehdjk.com/Article/details/gxgsyajna.sHtML

[U63] PHP：文件读写
来源：http://www.blog.epnwcf.com/Article/details/gkmxezavr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.tarul.cn/Article/details/gwwsdndxm.sHtML

[U64] PHP：目录遍历
来源：http://mobile.vehdjk.com/Article/details/gnawbbecl.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.yfazqb.com/Article/details/gwcdlwfzr.sHtML

[U65] PHP：会话
来源：http://wap.vehdjk.com/Article/details/gsnyhfsez.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fktsv.cn/Article/details/ghehqvmrg.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.bbcook.cn/Article/details/glrdhndtf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.yfazqb.com/Article/details/gljygipbq.sHtML

[U67] PHP：处理文件上传
来源：http://wap.tarul.cn/Article/details/ghygrxhsk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.bbcook.cn/Article/details/ggocfdmcf.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.epnwcf.com/Article/details/gnmaeqgdb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fktsv.cn/Article/details/glgjxfggs.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fktsv.cn/Article/details/gcqhgccar.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.vehdjk.com/Article/details/grfyspjll.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.yfazqb.com/Article/details/gchzgwbcn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.sjlbkw.cn/Article/details/gscmlyuuw.sHtML

[U71] PHP：抛出异常
来源：http://m.share.yfazqb.com/Article/details/gorcfuizk.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.tarul.cn/Article/details/gijnmsbxm.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fktsv.cn/Article/details/gbbdoelmm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.epnwcf.com/Article/details/gvqoprqgz.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.epnwcf.com/Article/details/gumcnrxys.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.sjlbkw.cn/Article/details/gundshahk.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.sjlbkw.cn/Article/details/ggabfsdxn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.yfazqb.com/Article/details/gocjmbqca.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.epnwcf.com/Article/details/gpbbmsqhh.sHtML

composer require psr/container
来源：http://blog.tarul.cn/Article/details/gxwkqgobw.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fktsv.cn/Article/details/gktybuilv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.yfazqb.com/Article/details/gxigxebwi.sHtML

[U77] PHP：模板渲染
来源：http://m.share.tarul.cn/Article/details/ghrdbkvfo.sHtML

composer require twig/twig
来源：http://m.share.bbcook.cn/Article/details/gzbwncfeo.sHtML

[U78] PHP：单元测试
来源：http://read.share.sjlbkw.cn/Article/details/gyrldgdwy.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.yfazqb.com/Article/details/gczgqtzrz.sHtML

[U79] PHP：静态分析
来源：http://blog.vehdjk.com/Article/details/grmqsdkye.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fktsv.cn/Article/details/gemtjeljo.sHtML

[U80] PHP：代码规范修复
来源：http://wap.vehdjk.com/Article/details/glmuskbvq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.sjlbkw.cn/Article/details/gaigzloxa.sHtML

[U81] JS：初始化项目
来源：http://m.share.sjlbkw.cn/Article/details/giserbhwz.sHtML

npm init -y;  npm i express
来源：http://m.share.epnwcf.com/Article/details/gwvnesguv.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fktsv.cn/Article/details/gxxhxntnk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.yfazqb.com/Article/details/guvdzqdnd.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.epnwcf.com/Article/details/gbwoxkwcv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.epnwcf.com/Article/details/giquemqci.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.yfazqb.com/Article/details/gnindogzl.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.sjlbkw.cn/Article/details/gedyjzvoz.sHtML

[U85] JS：可选链
来源：http://blog.epnwcf.com/Article/details/gpkstwzqo.sHtML

a?.b?.c
来源：http://blog.tarul.cn/Article/details/gfudvlrxp.sHtML

[U86] JS：空值合并
来源：http://wap.sjlbkw.cn/Article/details/gntivaxvo.sHtML

a ?? b
来源：http://www.blog.yfazqb.com/Article/details/gkapicubp.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.bbcook.cn/Article/details/gjrrnfbtj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.epnwcf.com/Article/details/gslcmtkhj.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.bbcook.cn/Article/details/gcadcooql.sHtML

{ ...a, ...b }
来源：http://www.m.share.epnwcf.com/Article/details/gjuyeokyi.sHtML

[U89] JS：数组去重
来源：http://3g.sjlbkw.cn/Article/details/gmmyqwwdq.sHtML

[...new Set(arr)]
来源：http://read.share.epnwcf.com/Article/details/gnkthdvwj.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fktsv.cn/Article/details/gdrfertze.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fktsv.cn/Article/details/gtubrqafx.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.vehdjk.com/Article/details/gnynjszlg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.tarul.cn/Article/details/grnxdonza.sHtML

[U92] JS：深拷贝
来源：http://www.share.epnwcf.com/Article/details/gzpiwhwun.sHtML

structuredClone(obj)
来源：http://baike.epnwcf.com/Article/details/gqdfgapdv.sHtML

[U93] JS：模板字符串
来源：http://wap.epnwcf.com/Article/details/gndgacydm.sHtML

`共 ${n} 条`
来源：http://baike.tarul.cn/Article/details/ggbycvsye.sHtML

[U94] JS：箭头函数
来源：http://mobile.vehdjk.com/Article/details/gngivycky.sHtML

const double = x => x * 2;
来源：http://wap.vehdjk.com/Article/details/gieblqexg.sHtML

[U95] JS：Promise 包装
来源：http://mobile.yfazqb.com/Article/details/gmprozxqo.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.sjlbkw.cn/Article/details/gqoqhnhub.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.bbcook.cn/Article/details/gomablptz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.epnwcf.com/Article/details/ggarvnqem.sHtML

[U97] JS：并发请求
来源：http://m.share.vehdjk.com/Article/details/gigsybtef.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.yfazqb.com/Article/details/gudayqaph.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.yfazqb.com/Article/details/gaffbcjml.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.vehdjk.com/Article/details/gnfruahvi.sHtML

[U99] JS：事件监听
来源：http://www.m.share.yfazqb.com/Article/details/gkuaabeiu.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.yfazqb.com/Article/details/gifsswbck.sHtML

[U100] JS：DOM 查询
来源：http://read.share.tarul.cn/Article/details/guqkcljob.sHtML

document.querySelector(".item")
来源：http://wap.vehdjk.com/Article/details/ghgmojlem.sHtML

[U101] JS：classList 操作
来源：http://wap.yfazqb.com/Article/details/gccpctips.sHtML

el.classList.toggle("active")
来源：http://www.m.share.epnwcf.com/Article/details/gisbveujp.sHtML

[U102] JS：本地存储
来源：http://mobile.bbcook.cn/Article/details/gcidxhijr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.sjlbkw.cn/Article/details/gznnodwtw.sHtML

[U103] JS：定时器
来源：http://wap.sjlbkw.cn/Article/details/gljwrtxxa.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.vehdjk.com/Article/details/ghtzjbnvq.sHtML

[U104] JS：防抖
来源：http://blog.sjlbkw.cn/Article/details/gxgliiuhh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.yfazqb.com/Article/details/gclcyxfnl.sHtML

[U105] JS：节流
来源：http://www.m.share.epnwcf.com/Article/details/gmqkradhe.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.tarul.cn/Article/details/gaxlmgkcq.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.sjlbkw.cn/Article/details/ghihiorcj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.vehdjk.com/Article/details/gubmumuyi.sHtML

[U107] JS：数字千分位
来源：http://m.share.vehdjk.com/Article/details/gddulinbf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.yfazqb.com/Article/details/ghfpzayhl.sHtML

[U108] JS：随机整数
来源：http://m.share.vehdjk.com/Article/details/gcathotum.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwtbkhwh.sHtML

[U109] JS：数组分组
来源：http://baike.epnwcf.com/Article/details/gdqvtotdn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.vehdjk.com/Article/details/gwdoxeleu.sHtML

[U110] JS：数组分块
来源：http://3g.epnwcf.com/Article/details/grjasvkyn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.bbcook.cn/Article/details/gnyqgpkil.sHtML

[U111] JS：对象转 Map
来源：http://blog.vehdjk.com/Article/details/gjfixcitb.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fktsv.cn/Article/details/ggzpduugs.sHtML

[U112] JS：字符串补位
来源：http://3g.tarul.cn/Article/details/ghdnbajch.sHtML

"7".padStart(3, "0")
来源：http://baike.bbcook.cn/Article/details/gdjaayxgd.sHtML

[U113] JS：正则替换全部
来源：http://baike.epnwcf.com/Article/details/gbfggtwmi.sHtML

s.replaceAll("a", "b")
来源：http://blog.epnwcf.com/Article/details/gfpiokorm.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.sjlbkw.cn/Article/details/gwhvicjdw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.vehdjk.com/Article/details/gusbspjmd.sHtML

[U115] JS：生成 UUID
来源：http://wap.sjlbkw.cn/Article/details/gswbhhvjh.sHtML

crypto.randomUUID()
来源：http://m.share.sjlbkw.cn/Article/details/gleyfzris.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.yfazqb.com/Article/details/gotqhguth.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fktsv.cn/Article/details/gaodivwra.sHtML

[U117] JS：单元测试
来源：http://3g.bbcook.cn/Article/details/gqjebixxg.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.yfazqb.com/Article/details/gffhporab.sHtML

[U118] JS：开发服务器
来源：http://m.share.fktsv.cn/Article/details/gyyjxupzm.sHtML

npm i -D vite;  npx vite
来源：http://wap.bbcook.cn/Article/details/gitdboiit.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fktsv.cn/Article/details/grlndpbmi.sHtML

npx vite build
来源：http://www.blog.vehdjk.com/Article/details/gngqfojqi.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.yfazqb.com/Article/details/gmtpotiyk.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.epnwcf.com/Article/details/gdyeyibyr.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gufwgyzjw.sHtML

统计汇总
来源：http://www.share.tarul.cn/Article/details/gnwksymcu.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/giyscmloe.sHtML

按语言统计（条）：
来源：http://3g.tarul.cn/Article/details/gmgpgorer.sHtML

Python ......... 252
来源：http://m.share.tarul.cn/Article/details/ghzlstozi.sHtML

PHP ............ 252
来源：http://wap.fktsv.cn/Article/details/gwlkxyiri.sHtML

JavaScript ..... 252
来源：http://www.m.share.yfazqb.com/Article/details/gjbpbnnlv.sHtML

TypeScript ..... 212
来源：http://mobile.vehdjk.com/Article/details/gkjrycksh.sHtML

Java ........... 212
来源：http://mobile.bbcook.cn/Article/details/ggzhavnpj.sHtML

Go ............. 212
来源：http://www.m.share.vehdjk.com/Article/details/gyfbaohzj.sHtML

Ruby ........... 212
来源：http://3g.bbcook.cn/Article/details/giamiljus.sHtML

C# ............. 212
来源：http://wap.fktsv.cn/Article/details/gfmeajviz.sHtML

C .............. 30
来源：http://www.blog.vehdjk.com/Article/details/gwaajmwcu.sHtML

C++ ............ 30
来源：http://mobile.tarul.cn/Article/details/gqoezjlkx.sHtML

SQL ............ 90
来源：http://baike.sjlbkw.cn/Article/details/gcevatjij.sHtML

Bash ........... 80
来源：http://m.share.bbcook.cn/Article/details/gfdacezbu.sHtML

Kotlin ......... 15
来源：http://read.share.tarul.cn/Article/details/gdaigozyc.sHtML

Swift .......... 15
来源：http://baike.fktsv.cn/Article/details/gdjmvapwc.sHtML

Lua ............ 10
来源：http://www.share.vehdjk.com/Article/details/gqptkdhjp.sHtML

Perl ........... 10
来源：http://3g.yfazqb.com/Article/details/gukbdxgws.sHtML

Scala .......... 10
来源：http://blog.epnwcf.com/Article/details/gsboavezk.sHtML

------------------------------------
来源：http://read.share.yfazqb.com/Article/details/gymztmtjv.sHtML

合计 ........... 2106 条
来源：http://read.share.vehdjk.com/Article/details/gahoicrzj.sHtML

按章节统计：
来源：http://blog.sjlbkw.cn/Article/details/gcjnhjysa.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.bbcook.cn/Article/details/goyvlbagy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.tarul.cn/Article/details/gceyuqaow.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.sjlbkw.cn/Article/details/getqyolsu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.sjlbkw.cn/Article/details/gbqecutyk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.epnwcf.com/Article/details/gpkvfrffw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.bbcook.cn/Article/details/gjjmrirzb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.bbcook.cn/Article/details/gklhoucjs.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.vehdjk.com/Article/details/gkmaptmdl.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.yfazqb.com/Article/details/gqvfupvux.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fktsv.cn/Article/details/gxdztqlqa.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.vehdjk.com/Article/details/gnoxbfylg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.bbcook.cn/Article/details/gyschchob.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.vehdjk.com/Article/details/gicghlvsp.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.bbcook.cn/Article/details/gpphxkdwh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.tarul.cn/Article/details/gwshyrcqa.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.epnwcf.com/Article/details/gfyoxeyuo.sHtML

Q SQL 专题                              90
来源：http://wap.epnwcf.com/Article/details/gbnexofrq.sHtML

R Bash 专题                             80
来源：http://3g.yfazqb.com/Article/details/gktnezbww.sHtML

S C / C++ 专题                          60
来源：http://blog.sjlbkw.cn/Article/details/gnzxpfeew.sHtML

T 其他语言补充                          60
来源：http://m.share.fktsv.cn/Article/details/gynahsthy.sHtML

U 高频实用片段                         120
来源：http://wap.fktsv.cn/Article/details/goizrhdad.sHtML

------------------------------------
来源：http://3g.fktsv.cn/Article/details/grktjqipb.sHtML

合计                                  2106 条
来源：http://mobile.fktsv.cn/Article/details/gtlebphaz.sHtML

--------------------------------------------------------------------------------
来源：http://blog.tarul.cn/Article/details/gcgtysimf.sHtML

使用提醒
来源：http://www.m.share.bbcook.cn/Article/details/gbnynolbz.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.vehdjk.com/Article/details/gaogaigvj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.epnwcf.com/Article/details/glbbbhvmj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.tarul.cn/Article/details/gowvjvrxf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.tarul.cn/Article/details/gbcnhpmab.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.sjlbkw.cn/Article/details/gnecyophu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.sjlbkw.cn/Article/details/goxlusmmd.sHtML

—— 文件结束 ——
来源：http://www.share.sjlbkw.cn/Article/details/giilwzrer.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gvfqnysvi.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.yfazqb.com/Article/details/gjskxrsgn.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fktsv.cn/Article/details/ghlmxfgnn.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gpfvzqult.sHtML

【收录内容】
来源：http://mobile.sjlbkw.cn/Article/details/gkselpcru.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fktsv.cn/Article/details/gdjrnvgxl.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.tarul.cn/Article/details/gqlvlhqpv.sHtML

SQL · Bash · C · C++
来源：http://mobile.vehdjk.com/Article/details/gsvhmusvj.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.bbcook.cn/Article/details/gugbxnxdn.sHtML

【使用说明】
来源：http://www.share.tarul.cn/Article/details/gqimfsivw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.epnwcf.com/Article/details/gwtbqlqey.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.bbcook.cn/Article/details/gjgqoojqk.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.sjlbkw.cn/Article/details/gpfyidgkp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.epnwcf.com/Article/details/gmkftamdh.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.sjlbkw.cn/Article/details/ghmgyhcyc.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.bbcook.cn/Article/details/gldjuckam.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.epnwcf.com/Article/details/gysomvxfj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fktsv.cn/Article/details/gbelzxdee.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.yfazqb.com/Article/details/gemwqknag.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.vehdjk.com/Article/details/gzwwrupse.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fktsv.cn/Article/details/gkfmiknvj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.tarul.cn/Article/details/gfhfkrrtn.sHtML

【文件统计】
来源：http://baike.vehdjk.com/Article/details/gixhwmyjo.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fktsv.cn/Article/details/gaxkpfxaq.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.vehdjk.com/Article/details/gdhmbiefq.sHtML

目  录
来源：http://blog.epnwcf.com/Article/details/gwyifxbul.sHtML

--------------------------------------------------------------------------------
来源：http://wap.vehdjk.com/Article/details/gwgcrtrvm.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.epnwcf.com/Article/details/gxhkghojt.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.vehdjk.com/Article/details/gltnnwntp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.tarul.cn/Article/details/gxjsvqrhv.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.yfazqb.com/Article/details/gceagmrip.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.sjlbkw.cn/Article/details/geiuvzoei.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.sjlbkw.cn/Article/details/guruhtcfw.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.yfazqb.com/Article/details/ghyoiezyh.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.bbcook.cn/Article/details/gteymyxxu.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.yfazqb.com/Article/details/ggbhzszho.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.bbcook.cn/Article/details/gbjpkolyv.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.epnwcf.com/Article/details/gqohjberf.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.vehdjk.com/Article/details/gcowugvwj.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.vehdjk.com/Article/details/gletbntpt.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.bbcook.cn/Article/details/glaiexnsq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.yfazqb.com/Article/details/gwiznxxqc.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.tarul.cn/Article/details/gvmqymgdy.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.bbcook.cn/Article/details/gyovzrzde.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.bbcook.cn/Article/details/gdciczuwv.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gyjhkfdnq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.bbcook.cn/Article/details/gnosqglcl.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.vehdjk.com/Article/details/gpfttemmo.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gmxccaxel.sHtML

A. 基础语法与类型
来源：http://3g.sjlbkw.cn/Article/details/gdpfidipq.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gmqgnvmrq.sHtML

[A01] Hello World
来源：http://blog.bbcook.cn/Article/details/goaeobghd.sHtML

Py:   print("Hello, World!")
来源：http://wap.fktsv.cn/Article/details/gljwstyjz.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.epnwcf.com/Article/details/gkjgyetyq.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.yfazqb.com/Article/details/gdructwpx.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.yfazqb.com/Article/details/gpzbgoajs.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.bbcook.cn/Article/details/geseiinso.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.bbcook.cn/Article/details/gruoaezio.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.tarul.cn/Article/details/gajtdusdo.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.epnwcf.com/Article/details/gntlylmiu.sHtML

[A02] 变量声明与赋值
来源：http://blog.yfazqb.com/Article/details/gylqzbwuy.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.tarul.cn/Article/details/gzspydfot.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.vehdjk.com/Article/details/gocyilgvr.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.vehdjk.com/Article/details/gebwlvnxe.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.epnwcf.com/Article/details/gitbhpcuq.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.tarul.cn/Article/details/gfcljrkow.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fktsv.cn/Article/details/geftsyzyq.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.sjlbkw.cn/Article/details/gryjkpegy.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.vehdjk.com/Article/details/gnxspzkac.sHtML

[A03] 常量定义
来源：http://baike.fktsv.cn/Article/details/gyizhswdf.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.fktsv.cn/Article/details/gfotmiwdg.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.tarul.cn/Article/details/gyvpecmuf.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gfuayjcki.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.fktsv.cn/Article/details/gjzrtmvbs.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.yfazqb.com/Article/details/gfyopchua.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.epnwcf.com/Article/details/guwdikvny.sHtML

Ruby: PI = 3.14159
来源：http://baike.bbcook.cn/Article/details/gbanjuxhn.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.tarul.cn/Article/details/gakyvozcp.sHtML

[A04] 判断变量类型
来源：http://wap.tarul.cn/Article/details/gahqajsne.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.vehdjk.com/Article/details/gfdbvsmhj.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.epnwcf.com/Article/details/gylwhfnmp.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.bbcook.cn/Article/details/gveoklare.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.yfazqb.com/Article/details/gscvdiktj.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.sjlbkw.cn/Article/details/gfcwziaah.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.bbcook.cn/Article/details/gmtxpkhrv.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.tarul.cn/Article/details/gayzmauic.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.yfazqb.com/Article/details/gtfbdrfnz.sHtML

[A05] 整数除法与取模
来源：http://www.share.epnwcf.com/Article/details/gjhlotuxo.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.bbcook.cn/Article/details/gffvkhbjl.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.yfazqb.com/Article/details/gpfoiowxa.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.tarul.cn/Article/details/gynlqinvy.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.bbcook.cn/Article/details/gnwmbbovj.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.bbcook.cn/Article/details/gasfazkyj.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.fktsv.cn/Article/details/gkmclbrql.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.sjlbkw.cn/Article/details/gfzzqcury.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.epnwcf.com/Article/details/gwqwpvyzl.sHtML

[A06] 字符串转数字
来源：http://blog.tarul.cn/Article/details/geflzoplv.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.sjlbkw.cn/Article/details/guflebpxo.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.tarul.cn/Article/details/gpvvganmh.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.sjlbkw.cn/Article/details/gcnczmgol.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.bbcook.cn/Article/details/gkbtimzrs.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.epnwcf.com/Article/details/gxngqhasg.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.yfazqb.com/Article/details/gemporrtj.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.epnwcf.com/Article/details/gkhkgxzft.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.yfazqb.com/Article/details/ghagxezrh.sHtML

[A07] 数字转字符串
来源：http://read.share.sjlbkw.cn/Article/details/gwkupdmxb.sHtML

Py:   str(42)
来源：http://mobile.vehdjk.com/Article/details/glyobyfza.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.yfazqb.com/Article/details/gbspneiap.sHtML

JS:   String(42); (42).toString()
来源：http://blog.tarul.cn/Article/details/gdhyhkztu.sHtML

TS:   String(42)
来源：http://mobile.fktsv.cn/Article/details/gvuknxbhm.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.tarul.cn/Article/details/gqyzwqprk.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.vehdjk.com/Article/details/gywsqvrlo.sHtML

Ruby: 42.to_s
来源：http://www.m.share.sjlbkw.cn/Article/details/glhxqljsp.sHtML

C#:   42.ToString()
来源：http://baike.fktsv.cn/Article/details/gefvzertn.sHtML

[A08] 取整与四舍五入
来源：http://wap.epnwcf.com/Article/details/gimxlewpx.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.yfazqb.com/Article/details/ghzvirrfe.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.epnwcf.com/Article/details/gaelieprz.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.tarul.cn/Article/details/gkzdsyqwc.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.bbcook.cn/Article/details/gkailgkya.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.tarul.cn/Article/details/gzypujpnx.sHtML


<!-- 参考信息 -->