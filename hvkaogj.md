代发 wailian999

[U59] PHP：自定义排序
来源：http://www.m.share.yfazqb.com/Article/details/giaouignr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.tarul.cn/Article/details/gkgmfpofa.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.epnwcf.com/Article/details/gdooixfhe.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.epnwcf.com/Article/details/gopncpxid.sHtML

[U61] PHP：正则
来源：http://www.share.bbcook.cn/Article/details/gcvmmblkp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.epnwcf.com/Article/details/glivyjjvu.sHtML

[U62] PHP：日期对象
来源：http://www.share.sjlbkw.cn/Article/details/gnmuoxbyb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.epnwcf.com/Article/details/guldypnuy.sHtML

[U63] PHP：文件读写
来源：http://www.blog.bbcook.cn/Article/details/georlhdaq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fktsv.cn/Article/details/gwpcwglbg.sHtML

[U64] PHP：目录遍历
来源：http://baike.epnwcf.com/Article/details/gzfeaerur.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fktsv.cn/Article/details/gadvnnwwj.sHtML

[U65] PHP：会话
来源：http://www.share.epnwcf.com/Article/details/gwkacrtpj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.bbcook.cn/Article/details/garpzrfyb.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.bbcook.cn/Article/details/gblaofjgt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.epnwcf.com/Article/details/gvonspthe.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fktsv.cn/Article/details/gtqjhipte.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fktsv.cn/Article/details/gzfvcctlm.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.yfazqb.com/Article/details/gpuewagla.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.tarul.cn/Article/details/gniucteny.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fktsv.cn/Article/details/gxjnqvuwf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.epnwcf.com/Article/details/gnoaerllp.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.vehdjk.com/Article/details/gorfqmccc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.epnwcf.com/Article/details/gqezcbtti.sHtML

[U71] PHP：抛出异常
来源：http://blog.sjlbkw.cn/Article/details/gphzxnbfl.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.bbcook.cn/Article/details/gmllhgroo.sHtML

[U72] PHP：写错误日志
来源：http://www.share.epnwcf.com/Article/details/gkkvtisbx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fktsv.cn/Article/details/glcuazurv.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.epnwcf.com/Article/details/gghjfqmkp.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fktsv.cn/Article/details/grsyaqehv.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.bbcook.cn/Article/details/gqklobbol.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.epnwcf.com/Article/details/gxgquitat.sHtML

[U75] PHP：依赖注入
来源：http://wap.yfazqb.com/Article/details/gcnxiqkzt.sHtML

composer require psr/container
来源：http://wap.epnwcf.com/Article/details/gyenhaxya.sHtML

[U76] PHP：简单路由
来源：http://baike.vehdjk.com/Article/details/ggwfplbrs.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.yfazqb.com/Article/details/goiagsrqe.sHtML

[U77] PHP：模板渲染
来源：http://www.share.epnwcf.com/Article/details/gurxrbcly.sHtML

composer require twig/twig
来源：http://blog.vehdjk.com/Article/details/gjivijail.sHtML

[U78] PHP：单元测试
来源：http://www.blog.epnwcf.com/Article/details/gudganuyb.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.vehdjk.com/Article/details/gdbkwklkp.sHtML

[U79] PHP：静态分析
来源：http://mobile.bbcook.cn/Article/details/gzoigvkey.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.vehdjk.com/Article/details/gbfrmjvqf.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.epnwcf.com/Article/details/gxtuzmqxz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.epnwcf.com/Article/details/ghjkgmknu.sHtML

[U81] JS：初始化项目
来源：http://3g.vehdjk.com/Article/details/gqvegssxf.sHtML

npm init -y;  npm i express
来源：http://www.blog.sjlbkw.cn/Article/details/garcutazl.sHtML

[U82] JS：package.json 脚本
来源：http://wap.tarul.cn/Article/details/gqcumpamb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.epnwcf.com/Article/details/gopfqtpwc.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.sjlbkw.cn/Article/details/ggcfyaags.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.bbcook.cn/Article/details/gtbnqltyq.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.vehdjk.com/Article/details/gnqykxhso.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.epnwcf.com/Article/details/gdqewacoh.sHtML

[U85] JS：可选链
来源：http://m.share.yfazqb.com/Article/details/gvqqdyagy.sHtML

a?.b?.c
来源：http://blog.vehdjk.com/Article/details/glenjrdyd.sHtML

[U86] JS：空值合并
来源：http://3g.yfazqb.com/Article/details/gxgbqargl.sHtML

a ?? b
来源：http://www.share.epnwcf.com/Article/details/ggocpskdr.sHtML

[U87] JS：解构默认值
来源：http://www.share.bbcook.cn/Article/details/gtgchehve.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.sjlbkw.cn/Article/details/gcdilmjzg.sHtML

[U88] JS：对象展开合并
来源：http://m.share.tarul.cn/Article/details/gqbfanyzs.sHtML

{ ...a, ...b }
来源：http://www.share.vehdjk.com/Article/details/gunawnxlp.sHtML

[U89] JS：数组去重
来源：http://www.m.share.bbcook.cn/Article/details/gxltcpqbj.sHtML

[...new Set(arr)]
来源：http://www.blog.sjlbkw.cn/Article/details/gnyvswxgb.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.bbcook.cn/Article/details/gvdnvbuzv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.sjlbkw.cn/Article/details/giwfzmadc.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fktsv.cn/Article/details/gtfcdmsfb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.tarul.cn/Article/details/gugmthden.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.vehdjk.com/Article/details/gtywquyxz.sHtML

structuredClone(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gbybkofur.sHtML

[U93] JS：模板字符串
来源：http://baike.fktsv.cn/Article/details/grwnzecce.sHtML

`共 ${n} 条`
来源：http://baike.fktsv.cn/Article/details/gbleqgwjs.sHtML

[U94] JS：箭头函数
来源：http://m.share.epnwcf.com/Article/details/gdwnewcbo.sHtML

const double = x => x * 2;
来源：http://3g.sjlbkw.cn/Article/details/geinofoch.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.bbcook.cn/Article/details/gbapqkfuz.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.epnwcf.com/Article/details/gctgcjwus.sHtML

[U96] JS：async/await 与异常
来源：http://blog.tarul.cn/Article/details/gjttuyqve.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.tarul.cn/Article/details/gouwllwie.sHtML

[U97] JS：并发请求
来源：http://m.share.bbcook.cn/Article/details/gkuzwxlao.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fktsv.cn/Article/details/gocfvoacn.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.epnwcf.com/Article/details/ggwljqsad.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.bbcook.cn/Article/details/gtkwgavbv.sHtML

[U99] JS：事件监听
来源：http://wap.fktsv.cn/Article/details/ggbtqvwoq.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.vehdjk.com/Article/details/gpqganjcj.sHtML

[U100] JS：DOM 查询
来源：http://baike.bbcook.cn/Article/details/gzwtsmsrk.sHtML

document.querySelector(".item")
来源：http://www.blog.yfazqb.com/Article/details/gqjaranue.sHtML

[U101] JS：classList 操作
来源：http://www.blog.vehdjk.com/Article/details/girdrvdkg.sHtML

el.classList.toggle("active")
来源：http://blog.yfazqb.com/Article/details/giwfeadjv.sHtML

[U102] JS：本地存储
来源：http://www.blog.yfazqb.com/Article/details/guzufknbl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.vehdjk.com/Article/details/ghvwpsqdf.sHtML

[U103] JS：定时器
来源：http://read.share.fktsv.cn/Article/details/glgmjetkw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.vehdjk.com/Article/details/gyaonsxzo.sHtML

[U104] JS：防抖
来源：http://www.m.share.vehdjk.com/Article/details/ggwzwrxiv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.sjlbkw.cn/Article/details/gjlvlshht.sHtML

[U105] JS：节流
来源：http://read.share.sjlbkw.cn/Article/details/gnmztjser.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.yfazqb.com/Article/details/gawnnxdcf.sHtML

[U106] JS：日期格式化
来源：http://read.share.epnwcf.com/Article/details/gprafiamy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fktsv.cn/Article/details/gakckjacc.sHtML

[U107] JS：数字千分位
来源：http://www.share.sjlbkw.cn/Article/details/guxvbrcfy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.tarul.cn/Article/details/gvkyfkgue.sHtML

[U108] JS：随机整数
来源：http://read.share.tarul.cn/Article/details/gmqjvjert.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.vehdjk.com/Article/details/gfyqxqtws.sHtML

[U109] JS：数组分组
来源：http://read.share.bbcook.cn/Article/details/gmznprmzx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fktsv.cn/Article/details/gewewqmie.sHtML

[U110] JS：数组分块
来源：http://mobile.vehdjk.com/Article/details/gfkjicomn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fktsv.cn/Article/details/gsnlrrzgr.sHtML

[U111] JS：对象转 Map
来源：http://read.share.vehdjk.com/Article/details/gnasuqhch.sHtML

new Map(Object.entries(obj))
来源：http://blog.vehdjk.com/Article/details/gnjczladb.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.tarul.cn/Article/details/gneozjlyq.sHtML

"7".padStart(3, "0")
来源：http://www.share.vehdjk.com/Article/details/gulovqvad.sHtML

[U113] JS：正则替换全部
来源：http://baike.bbcook.cn/Article/details/grobtotvf.sHtML

s.replaceAll("a", "b")
来源：http://3g.tarul.cn/Article/details/gewdnznpe.sHtML

[U114] JS：JSON 深比较
来源：http://3g.vehdjk.com/Article/details/gjnjydpzf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.yfazqb.com/Article/details/gqiugguws.sHtML

[U115] JS：生成 UUID
来源：http://3g.bbcook.cn/Article/details/gbwjxekxq.sHtML

crypto.randomUUID()
来源：http://m.share.tarul.cn/Article/details/gyznjoxna.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.yfazqb.com/Article/details/gpupqhaal.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.epnwcf.com/Article/details/gkiwvnptr.sHtML

[U117] JS：单元测试
来源：http://m.share.vehdjk.com/Article/details/gngwfaaks.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.epnwcf.com/Article/details/gmjmoxnjx.sHtML

[U118] JS：开发服务器
来源：http://baike.epnwcf.com/Article/details/ggemhubjp.sHtML

npm i -D vite;  npx vite
来源：http://m.share.epnwcf.com/Article/details/gqrvyxddi.sHtML

[U119] JS：生产构建
来源：http://mobile.fktsv.cn/Article/details/gyvxfqdpy.sHtML

npx vite build
来源：http://www.share.sjlbkw.cn/Article/details/gfmyuzgwn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.tarul.cn/Article/details/glcrxubbx.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.yfazqb.com/Article/details/guzdrayww.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gxnrsmjht.sHtML

统计汇总
来源：http://www.m.share.sjlbkw.cn/Article/details/gisfkeeaq.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/ggdjagcwg.sHtML

按语言统计（条）：
来源：http://m.share.bbcook.cn/Article/details/godawxxiz.sHtML

Python ......... 252
来源：http://read.share.bbcook.cn/Article/details/geqmaeqsv.sHtML

PHP ............ 252
来源：http://3g.sjlbkw.cn/Article/details/gbavlyeue.sHtML

JavaScript ..... 252
来源：http://read.share.bbcook.cn/Article/details/gcrljpibv.sHtML

TypeScript ..... 212
来源：http://3g.fktsv.cn/Article/details/gysesbumk.sHtML

Java ........... 212
来源：http://baike.tarul.cn/Article/details/grervlkld.sHtML

Go ............. 212
来源：http://blog.fktsv.cn/Article/details/gamvzdexp.sHtML

Ruby ........... 212
来源：http://mobile.sjlbkw.cn/Article/details/gnsbihlpj.sHtML

C# ............. 212
来源：http://www.share.sjlbkw.cn/Article/details/ginkjulli.sHtML

C .............. 30
来源：http://3g.vehdjk.com/Article/details/gntfvducj.sHtML

C++ ............ 30
来源：http://read.share.sjlbkw.cn/Article/details/gegwxtdpi.sHtML

SQL ............ 90
来源：http://read.share.sjlbkw.cn/Article/details/gtuzdfnbs.sHtML

Bash ........... 80
来源：http://www.blog.fktsv.cn/Article/details/gsuihohmy.sHtML

Kotlin ......... 15
来源：http://wap.vehdjk.com/Article/details/gerkvunjo.sHtML

Swift .......... 15
来源：http://blog.yfazqb.com/Article/details/gffmhffsm.sHtML

Lua ............ 10
来源：http://wap.yfazqb.com/Article/details/gzxueioda.sHtML

Perl ........... 10
来源：http://www.share.tarul.cn/Article/details/gybjkhrss.sHtML

Scala .......... 10
来源：http://read.share.epnwcf.com/Article/details/golsurptn.sHtML

------------------------------------
来源：http://m.share.bbcook.cn/Article/details/gpnwbfouf.sHtML

合计 ........... 2106 条
来源：http://blog.sjlbkw.cn/Article/details/gersjdndo.sHtML

按章节统计：
来源：http://read.share.epnwcf.com/Article/details/gocmjfkby.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.sjlbkw.cn/Article/details/gcrzxziwq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fktsv.cn/Article/details/ggseyando.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.vehdjk.com/Article/details/glyyhmkdk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.tarul.cn/Article/details/gqqytflvs.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fktsv.cn/Article/details/gdfpgvxbk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.bbcook.cn/Article/details/gjibtewom.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.tarul.cn/Article/details/giqnncety.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.tarul.cn/Article/details/gcfxefkhz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.tarul.cn/Article/details/gmlrrhmld.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.bbcook.cn/Article/details/gojaunvld.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.bbcook.cn/Article/details/gpvsvhgvv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.vehdjk.com/Article/details/gzdxgmccm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.bbcook.cn/Article/details/gbsumqrlx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.vehdjk.com/Article/details/glkkwtcqd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.bbcook.cn/Article/details/glfwnfphu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fktsv.cn/Article/details/gfvnxfona.sHtML

Q SQL 专题                              90
来源：http://mobile.bbcook.cn/Article/details/gixjhqmdy.sHtML

R Bash 专题                             80
来源：http://wap.fktsv.cn/Article/details/gmnjjooam.sHtML

S C / C++ 专题                          60
来源：http://blog.epnwcf.com/Article/details/gfdjckzal.sHtML

T 其他语言补充                          60
来源：http://baike.bbcook.cn/Article/details/gymscewfg.sHtML

U 高频实用片段                         120
来源：http://blog.sjlbkw.cn/Article/details/gqtiqgvll.sHtML

------------------------------------
来源：http://baike.yfazqb.com/Article/details/gbfoxbngp.sHtML

合计                                  2106 条
来源：http://3g.yfazqb.com/Article/details/gpsqwewcu.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fktsv.cn/Article/details/grmfjzxds.sHtML

使用提醒
来源：http://blog.yfazqb.com/Article/details/ghuxvxhjt.sHtML

--------------------------------------------------------------------------------
来源：http://3g.bbcook.cn/Article/details/gkngfatxt.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.tarul.cn/Article/details/gevlquilh.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.epnwcf.com/Article/details/gcetygors.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.sjlbkw.cn/Article/details/glkthtgyp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.sjlbkw.cn/Article/details/gbqdfmyqh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.bbcook.cn/Article/details/gmckqwtmp.sHtML

—— 文件结束 ——
来源：http://mobile.bbcook.cn/Article/details/gkpbukyqt.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gaxfhrcxq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.vehdjk.com/Article/details/gocurxhll.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fktsv.cn/Article/details/gtghqolqn.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/glpeordnm.sHtML

【收录内容】
来源：http://3g.tarul.cn/Article/details/gnjtaasea.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.sjlbkw.cn/Article/details/gvvojtemj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.yfazqb.com/Article/details/gwbqmuovz.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fktsv.cn/Article/details/gbcfjvsoc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.bbcook.cn/Article/details/gjagasrff.sHtML

【使用说明】
来源：http://3g.vehdjk.com/Article/details/giigekntr.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.tarul.cn/Article/details/gqavyvuyv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fktsv.cn/Article/details/gxxjrkmwo.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.vehdjk.com/Article/details/gjsarklmz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.bbcook.cn/Article/details/guhraxvbo.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fktsv.cn/Article/details/gsosspdnw.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.yfazqb.com/Article/details/gmtsmchsh.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.sjlbkw.cn/Article/details/gcqepvefk.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.fktsv.cn/Article/details/gcftpsiym.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fktsv.cn/Article/details/gydpistof.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.tarul.cn/Article/details/gesfpxiob.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fktsv.cn/Article/details/gmdodckih.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.vehdjk.com/Article/details/gytefismc.sHtML

【文件统计】
来源：http://3g.bbcook.cn/Article/details/gfovrwzzl.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.yfazqb.com/Article/details/gvulqrwdg.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.yfazqb.com/Article/details/gvlxkaaev.sHtML

目  录
来源：http://www.blog.fktsv.cn/Article/details/gdezcshnp.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.yfazqb.com/Article/details/ggagusles.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.tarul.cn/Article/details/gziyclmbi.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.tarul.cn/Article/details/ghlnizfvb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.vehdjk.com/Article/details/ghapgncvg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.epnwcf.com/Article/details/gaweurxwz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.fktsv.cn/Article/details/gnibzykst.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.vehdjk.com/Article/details/gpoezmhqw.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.epnwcf.com/Article/details/gsrwcvyih.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fktsv.cn/Article/details/godyfvqhz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.bbcook.cn/Article/details/gerqnzghd.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.epnwcf.com/Article/details/geecylfzf.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.vehdjk.com/Article/details/gnuancaxk.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.vehdjk.com/Article/details/gvkyvkfsm.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.tarul.cn/Article/details/gionlxmwv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.yfazqb.com/Article/details/gdrvyjaxe.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.sjlbkw.cn/Article/details/gipdkzekp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.yfazqb.com/Article/details/gzchmcxun.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.bbcook.cn/Article/details/gfhvkgzre.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.fktsv.cn/Article/details/gwaeexubd.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.vehdjk.com/Article/details/gvqssnoug.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.bbcook.cn/Article/details/gipyteyhx.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fktsv.cn/Article/details/gprblxqet.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gccecpdwj.sHtML

A. 基础语法与类型
来源：http://www.m.share.vehdjk.com/Article/details/gnzdzvkxq.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gkgsovykn.sHtML

[A01] Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gnsknsnyx.sHtML

Py:   print("Hello, World!")
来源：http://mobile.tarul.cn/Article/details/guxroojic.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.yfazqb.com/Article/details/gkvnkkinx.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.vehdjk.com/Article/details/gnvqjjffo.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.vehdjk.com/Article/details/gmqqnalga.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.vehdjk.com/Article/details/gqzejrmbj.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.epnwcf.com/Article/details/gpnpxznwd.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.vehdjk.com/Article/details/gthujvnbl.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.epnwcf.com/Article/details/gooasxpqd.sHtML

[A02] 变量声明与赋值
来源：http://blog.epnwcf.com/Article/details/gpupqadrf.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.yfazqb.com/Article/details/gxleycgux.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.yfazqb.com/Article/details/gzfnognpy.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.bbcook.cn/Article/details/godfbssmi.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.bbcook.cn/Article/details/glckxtyko.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.epnwcf.com/Article/details/goidowqvt.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.bbcook.cn/Article/details/ghttnlzba.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.vehdjk.com/Article/details/gbheddqyt.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.tarul.cn/Article/details/gfbbqthib.sHtML

[A03] 常量定义
来源：http://m.share.tarul.cn/Article/details/gwujgcggd.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.fktsv.cn/Article/details/gdpdtwoyi.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.bbcook.cn/Article/details/gcfgnutey.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.yfazqb.com/Article/details/gopjpihgg.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.yfazqb.com/Article/details/gqwrtdjyx.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.sjlbkw.cn/Article/details/gsxvonhnl.sHtML

Go:   const PI = 3.14159
来源：http://mobile.tarul.cn/Article/details/gacluqvtc.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.yfazqb.com/Article/details/gbrxwgrgl.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/goxigbsgx.sHtML

[A04] 判断变量类型
来源：http://mobile.tarul.cn/Article/details/gaycyhtpe.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.vehdjk.com/Article/details/gadsjocqp.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.fktsv.cn/Article/details/ghnneaybv.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.yfazqb.com/Article/details/gwsumvwui.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.sjlbkw.cn/Article/details/geyzwlkef.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.fktsv.cn/Article/details/gnutswxre.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.sjlbkw.cn/Article/details/gmuebsgpm.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.bbcook.cn/Article/details/guvzwirqn.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.sjlbkw.cn/Article/details/giekspayg.sHtML

[A05] 整数除法与取模
来源：http://blog.sjlbkw.cn/Article/details/gjlknndbr.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.yfazqb.com/Article/details/gznlacfwb.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.fktsv.cn/Article/details/gzmiupxrt.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.vehdjk.com/Article/details/guxdzaotq.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.vehdjk.com/Article/details/grvmsdahl.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.vehdjk.com/Article/details/gimqdzmaa.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.epnwcf.com/Article/details/gxyvocbly.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.epnwcf.com/Article/details/gkaebcuhc.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.fktsv.cn/Article/details/gucnhtgab.sHtML

[A06] 字符串转数字
来源：http://3g.sjlbkw.cn/Article/details/gjqpkjeam.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.fktsv.cn/Article/details/gtqeuvtni.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.vehdjk.com/Article/details/gqphcvwpz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.yfazqb.com/Article/details/gmdqhdzqx.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.sjlbkw.cn/Article/details/gueflplxc.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.tarul.cn/Article/details/gfnvmtjam.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.vehdjk.com/Article/details/gkqgygane.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.bbcook.cn/Article/details/grtrimfcw.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.vehdjk.com/Article/details/gwvvghyur.sHtML

[A07] 数字转字符串
来源：http://www.m.share.tarul.cn/Article/details/gfardjgfb.sHtML

Py:   str(42)
来源：http://blog.yfazqb.com/Article/details/gyeoitfua.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.tarul.cn/Article/details/gfgbmgcws.sHtML

JS:   String(42); (42).toString()
来源：http://baike.vehdjk.com/Article/details/gmhroeyvo.sHtML

TS:   String(42)
来源：http://read.share.yfazqb.com/Article/details/gyfgajyym.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.tarul.cn/Article/details/glricosnl.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.fktsv.cn/Article/details/grnjmsmjm.sHtML

Ruby: 42.to_s
来源：http://mobile.yfazqb.com/Article/details/gmzhfhajh.sHtML

C#:   42.ToString()
来源：http://read.share.vehdjk.com/Article/details/gahhrttro.sHtML

[A08] 取整与四舍五入
来源：http://baike.tarul.cn/Article/details/gramnmjyi.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.epnwcf.com/Article/details/gxzksngnw.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.tarul.cn/Article/details/gyqtljrlk.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.yfazqb.com/Article/details/gkfaynrdv.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.vehdjk.com/Article/details/gfcpwotjr.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.tarul.cn/Article/details/grkjjrlej.sHtML


<!-- 参考信息 -->