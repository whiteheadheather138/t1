代发 wailian999

[U61] PHP：正则
来源：http://www.blog.vehdjk.com/Article/details/gmtdxsuct.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.tarul.cn/Article/details/gmamgtzum.sHtML

[U62] PHP：日期对象
来源：http://www.blog.sjlbkw.cn/Article/details/gyqcflrwi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.yfazqb.com/Article/details/gesvcjwdy.sHtML

[U63] PHP：文件读写
来源：http://www.share.tarul.cn/Article/details/gjyyuqdgg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.vehdjk.com/Article/details/gbkoawops.sHtML

[U64] PHP：目录遍历
来源：http://mobile.yfazqb.com/Article/details/gvttdliyh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.bbcook.cn/Article/details/gaetywegd.sHtML

[U65] PHP：会话
来源：http://read.share.epnwcf.com/Article/details/gvdhevdzu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.vehdjk.com/Article/details/gwvnjcxfm.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.sjlbkw.cn/Article/details/gcflhnlnd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.bbcook.cn/Article/details/gkqvdnaxx.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.tarul.cn/Article/details/gevitmnid.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.vehdjk.com/Article/details/gyzbhxbds.sHtML

[U68] PHP：PDO 连接
来源：http://blog.vehdjk.com/Article/details/gnpeptsba.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.bbcook.cn/Article/details/gnovanwks.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.tarul.cn/Article/details/grvkuqxbs.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.bbcook.cn/Article/details/gjdubtcbe.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.bbcook.cn/Article/details/gkcatgvwa.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.bbcook.cn/Article/details/gsnbzhdlr.sHtML

[U71] PHP：抛出异常
来源：http://blog.fktsv.cn/Article/details/gaascacva.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.yfazqb.com/Article/details/gcvczhily.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fktsv.cn/Article/details/gyhbfpyze.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.sjlbkw.cn/Article/details/gpiqgrvoq.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.vehdjk.com/Article/details/ggwntmdlb.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fktsv.cn/Article/details/gyyoyqksy.sHtML

[U74] PHP：读取环境变量
来源：http://3g.bbcook.cn/Article/details/gdovvxhlz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.bbcook.cn/Article/details/gkxkgtcen.sHtML

[U75] PHP：依赖注入
来源：http://baike.bbcook.cn/Article/details/gekgikvpo.sHtML

composer require psr/container
来源：http://3g.tarul.cn/Article/details/gfacdoqis.sHtML

[U76] PHP：简单路由
来源：http://3g.sjlbkw.cn/Article/details/gnuvxpbor.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.tarul.cn/Article/details/geaoiekuw.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.bbcook.cn/Article/details/gnkimhjtt.sHtML

composer require twig/twig
来源：http://blog.fktsv.cn/Article/details/gksypbwbg.sHtML

[U78] PHP：单元测试
来源：http://read.share.vehdjk.com/Article/details/gmljfdoaf.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.bbcook.cn/Article/details/gculiyhfo.sHtML

[U79] PHP：静态分析
来源：http://www.share.tarul.cn/Article/details/gwyvhthei.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.yfazqb.com/Article/details/gnesahtrn.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.tarul.cn/Article/details/gftixopeh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.sjlbkw.cn/Article/details/gsomkvxvw.sHtML

[U81] JS：初始化项目
来源：http://baike.sjlbkw.cn/Article/details/gaubpdnwl.sHtML

npm init -y;  npm i express
来源：http://mobile.yfazqb.com/Article/details/glvkofiam.sHtML

[U82] JS：package.json 脚本
来源：http://3g.yfazqb.com/Article/details/gdkryphic.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.bbcook.cn/Article/details/gxdsgyxeq.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.tarul.cn/Article/details/gsypivpzo.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fktsv.cn/Article/details/gdjiojaxc.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.vehdjk.com/Article/details/gtpwiuwzw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.vehdjk.com/Article/details/gzootodih.sHtML

[U85] JS：可选链
来源：http://blog.epnwcf.com/Article/details/gryaxcxxz.sHtML

a?.b?.c
来源：http://read.share.tarul.cn/Article/details/gpdcpmuxt.sHtML

[U86] JS：空值合并
来源：http://wap.tarul.cn/Article/details/gipounnnt.sHtML

a ?? b
来源：http://blog.sjlbkw.cn/Article/details/gtzfgmsti.sHtML

[U87] JS：解构默认值
来源：http://baike.tarul.cn/Article/details/gebgatcxg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.bbcook.cn/Article/details/grurjgjes.sHtML

[U88] JS：对象展开合并
来源：http://blog.epnwcf.com/Article/details/gwhzlfwyv.sHtML

{ ...a, ...b }
来源：http://m.share.bbcook.cn/Article/details/glpovqqhm.sHtML

[U89] JS：数组去重
来源：http://baike.yfazqb.com/Article/details/gfyzarigm.sHtML

[...new Set(arr)]
来源：http://read.share.tarul.cn/Article/details/gdqmlccuv.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.bbcook.cn/Article/details/gtdeibyhl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.bbcook.cn/Article/details/gvkqqhull.sHtML

[U91] JS：对象键值遍历
来源：http://3g.epnwcf.com/Article/details/grfofkatq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.bbcook.cn/Article/details/gbuienwvp.sHtML

[U92] JS：深拷贝
来源：http://mobile.yfazqb.com/Article/details/gvvfbuyar.sHtML

structuredClone(obj)
来源：http://wap.bbcook.cn/Article/details/gzdrbhhaw.sHtML

[U93] JS：模板字符串
来源：http://mobile.yfazqb.com/Article/details/gtjcnygxs.sHtML

`共 ${n} 条`
来源：http://wap.yfazqb.com/Article/details/gnvclydtl.sHtML

[U94] JS：箭头函数
来源：http://3g.bbcook.cn/Article/details/gxfqsdiyb.sHtML

const double = x => x * 2;
来源：http://m.share.vehdjk.com/Article/details/glkmnzuou.sHtML

[U95] JS：Promise 包装
来源：http://m.share.sjlbkw.cn/Article/details/gwtbyqfoh.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fktsv.cn/Article/details/gurhicxek.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.vehdjk.com/Article/details/gteexhryr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.tarul.cn/Article/details/gqugtxtzq.sHtML

[U97] JS：并发请求
来源：http://m.share.vehdjk.com/Article/details/gffyuzqvn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fktsv.cn/Article/details/gjdwvvtic.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fktsv.cn/Article/details/gzrlsojmj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.sjlbkw.cn/Article/details/glwjxzrgv.sHtML

[U99] JS：事件监听
来源：http://www.m.share.yfazqb.com/Article/details/geawyzetb.sHtML

el.addEventListener("click", e => {})
来源：http://blog.yfazqb.com/Article/details/gygonqmyy.sHtML

[U100] JS：DOM 查询
来源：http://www.share.vehdjk.com/Article/details/gteeipkoj.sHtML

document.querySelector(".item")
来源：http://m.share.yfazqb.com/Article/details/gwugetzcv.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.yfazqb.com/Article/details/gektiudue.sHtML

el.classList.toggle("active")
来源：http://www.blog.fktsv.cn/Article/details/gocfkrxev.sHtML

[U102] JS：本地存储
来源：http://mobile.sjlbkw.cn/Article/details/gyeujryty.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fktsv.cn/Article/details/glttyonnm.sHtML

[U103] JS：定时器
来源：http://mobile.epnwcf.com/Article/details/gxkldnzxu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.tarul.cn/Article/details/giqvtkiya.sHtML

[U104] JS：防抖
来源：http://www.m.share.yfazqb.com/Article/details/glqbdeucd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.yfazqb.com/Article/details/gerwpbicx.sHtML

[U105] JS：节流
来源：http://wap.sjlbkw.cn/Article/details/gkeenjxuh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.vehdjk.com/Article/details/gyzlnewlb.sHtML

[U106] JS：日期格式化
来源：http://m.share.tarul.cn/Article/details/gdadvpton.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.sjlbkw.cn/Article/details/gecvtvcps.sHtML

[U107] JS：数字千分位
来源：http://www.share.epnwcf.com/Article/details/gnoerdxcl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.vehdjk.com/Article/details/gsqtkwkmv.sHtML

[U108] JS：随机整数
来源：http://read.share.yfazqb.com/Article/details/gmmwelymp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.bbcook.cn/Article/details/gfojfahqo.sHtML

[U109] JS：数组分组
来源：http://blog.tarul.cn/Article/details/gbpwniwmo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.epnwcf.com/Article/details/gncpwloci.sHtML

[U110] JS：数组分块
来源：http://m.share.fktsv.cn/Article/details/gztvpojdq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.vehdjk.com/Article/details/gfupvfvya.sHtML

[U111] JS：对象转 Map
来源：http://blog.vehdjk.com/Article/details/gozxluouj.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.bbcook.cn/Article/details/gutnifoqn.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.yfazqb.com/Article/details/guthmukjy.sHtML

"7".padStart(3, "0")
来源：http://3g.bbcook.cn/Article/details/gxndlvaxm.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.sjlbkw.cn/Article/details/gvfqrfeyp.sHtML

s.replaceAll("a", "b")
来源：http://m.share.vehdjk.com/Article/details/gbahuhgqh.sHtML

[U114] JS：JSON 深比较
来源：http://blog.epnwcf.com/Article/details/gbfmidimo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fktsv.cn/Article/details/ghcxxdrea.sHtML

[U115] JS：生成 UUID
来源：http://www.share.sjlbkw.cn/Article/details/gcqyvfbut.sHtML

crypto.randomUUID()
来源：http://baike.epnwcf.com/Article/details/gwonoqctb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.bbcook.cn/Article/details/gsbjevbeo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.tarul.cn/Article/details/gelvzhqmo.sHtML

[U117] JS：单元测试
来源：http://m.share.epnwcf.com/Article/details/ghbfcokgw.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.sjlbkw.cn/Article/details/ggnowfuor.sHtML

[U118] JS：开发服务器
来源：http://www.share.fktsv.cn/Article/details/ghrdvlctv.sHtML

npm i -D vite;  npx vite
来源：http://3g.vehdjk.com/Article/details/glqhfbssu.sHtML

[U119] JS：生产构建
来源：http://read.share.fktsv.cn/Article/details/gararyppv.sHtML

npx vite build
来源：http://www.share.yfazqb.com/Article/details/giwvlhvgs.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.epnwcf.com/Article/details/gnolvyuku.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fktsv.cn/Article/details/ggntltvof.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gnqudndvo.sHtML

统计汇总
来源：http://mobile.vehdjk.com/Article/details/gihzsnqrz.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gxlbbcood.sHtML

按语言统计（条）：
来源：http://read.share.epnwcf.com/Article/details/gewgrwznj.sHtML

Python ......... 252
来源：http://baike.fktsv.cn/Article/details/gqbkftqps.sHtML

PHP ............ 252
来源：http://3g.epnwcf.com/Article/details/gxtdazqxh.sHtML

JavaScript ..... 252
来源：http://baike.epnwcf.com/Article/details/gyjmytwuj.sHtML

TypeScript ..... 212
来源：http://baike.fktsv.cn/Article/details/gbvlsnvmo.sHtML

Java ........... 212
来源：http://www.m.share.sjlbkw.cn/Article/details/grzdbfrhz.sHtML

Go ............. 212
来源：http://baike.vehdjk.com/Article/details/gfhnjslad.sHtML

Ruby ........... 212
来源：http://www.share.sjlbkw.cn/Article/details/gxvtwkcwy.sHtML

C# ............. 212
来源：http://3g.yfazqb.com/Article/details/gcpbnvqra.sHtML

C .............. 30
来源：http://m.share.fktsv.cn/Article/details/gcbyobwsi.sHtML

C++ ............ 30
来源：http://www.blog.epnwcf.com/Article/details/gelsprsec.sHtML

SQL ............ 90
来源：http://baike.bbcook.cn/Article/details/guphcymiq.sHtML

Bash ........... 80
来源：http://www.share.tarul.cn/Article/details/gtpldchkv.sHtML

Kotlin ......... 15
来源：http://baike.yfazqb.com/Article/details/gewbcoycf.sHtML

Swift .......... 15
来源：http://blog.fktsv.cn/Article/details/gwrheaxbs.sHtML

Lua ............ 10
来源：http://blog.tarul.cn/Article/details/gmkxhkkjd.sHtML

Perl ........... 10
来源：http://www.share.yfazqb.com/Article/details/gkwijweal.sHtML

Scala .......... 10
来源：http://baike.yfazqb.com/Article/details/glnojmvbp.sHtML

------------------------------------
来源：http://www.m.share.tarul.cn/Article/details/gvzprlqpx.sHtML

合计 ........... 2106 条
来源：http://www.share.tarul.cn/Article/details/gtanslnxp.sHtML

按章节统计：
来源：http://www.share.vehdjk.com/Article/details/gpsueqorx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.epnwcf.com/Article/details/gmyozrzxm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.tarul.cn/Article/details/gycznfefa.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.tarul.cn/Article/details/gzxpthynm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.sjlbkw.cn/Article/details/gcwxfltod.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.yfazqb.com/Article/details/glrhaisrr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.yfazqb.com/Article/details/gdywhytmd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.sjlbkw.cn/Article/details/gveadpjsp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fktsv.cn/Article/details/gfogjtynu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.tarul.cn/Article/details/gmjsiyjwv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.sjlbkw.cn/Article/details/gofnlpafq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.yfazqb.com/Article/details/gwhaimytn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.epnwcf.com/Article/details/gvafmaovq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.vehdjk.com/Article/details/gfnirtbdz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fktsv.cn/Article/details/gofkanywb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.bbcook.cn/Article/details/gfnsqwnla.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fktsv.cn/Article/details/gofrwfran.sHtML

Q SQL 专题                              90
来源：http://3g.sjlbkw.cn/Article/details/gbsidebky.sHtML

R Bash 专题                             80
来源：http://mobile.tarul.cn/Article/details/gajfugaex.sHtML

S C / C++ 专题                          60
来源：http://3g.epnwcf.com/Article/details/gnxnxphjw.sHtML

T 其他语言补充                          60
来源：http://www.m.share.yfazqb.com/Article/details/gfiqlkuoe.sHtML

U 高频实用片段                         120
来源：http://mobile.fktsv.cn/Article/details/gxjsrxnmq.sHtML

------------------------------------
来源：http://read.share.sjlbkw.cn/Article/details/govrzooge.sHtML

合计                                  2106 条
来源：http://m.share.bbcook.cn/Article/details/gwgfihiub.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.sjlbkw.cn/Article/details/gvahhphiy.sHtML

使用提醒
来源：http://baike.tarul.cn/Article/details/gazvsziwl.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/gaijdpzma.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.vehdjk.com/Article/details/gveilhsbm.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.vehdjk.com/Article/details/gchhmjacj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.sjlbkw.cn/Article/details/gecainmlt.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fktsv.cn/Article/details/gognjjqgr.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fktsv.cn/Article/details/ggqrxvegl.sHtML

—— 文件结束 ——
来源：http://m.share.epnwcf.com/Article/details/gxkgbrzku.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/glanyqudv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.yfazqb.com/Article/details/ggypqdrub.sHtML

Common Programming Examples Cheat Book
来源：http://3g.tarul.cn/Article/details/gvjbvbcpr.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/grttecpsx.sHtML

【收录内容】
来源：http://www.blog.yfazqb.com/Article/details/gziebmvvp.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.bbcook.cn/Article/details/gazwqzphx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.tarul.cn/Article/details/ghtesctyc.sHtML

SQL · Bash · C · C++
来源：http://m.share.epnwcf.com/Article/details/gnfpymzrk.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.bbcook.cn/Article/details/gouzouyuf.sHtML

【使用说明】
来源：http://mobile.sjlbkw.cn/Article/details/gxtcqyzjz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.yfazqb.com/Article/details/gyhmsomgy.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.tarul.cn/Article/details/gjzjzsyun.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.tarul.cn/Article/details/gnvsaudzu.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.bbcook.cn/Article/details/gctjfqkxa.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.vehdjk.com/Article/details/gmbgfrevm.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.sjlbkw.cn/Article/details/gaguhwgoc.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.bbcook.cn/Article/details/gqfowbkxo.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.vehdjk.com/Article/details/giwexxknj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fktsv.cn/Article/details/gcebvogfe.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.tarul.cn/Article/details/gcraolzue.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.sjlbkw.cn/Article/details/gwhzumxyg.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.sjlbkw.cn/Article/details/gpgnqsaft.sHtML

【文件统计】
来源：http://blog.yfazqb.com/Article/details/grjydwnnj.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.vehdjk.com/Article/details/ggchdtomk.sHtML

--------------------------------------------------------------------------------
来源：http://blog.vehdjk.com/Article/details/gjaayfsss.sHtML

目  录
来源：http://www.share.tarul.cn/Article/details/gfnopqbsc.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.yfazqb.com/Article/details/gncdehzds.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.fktsv.cn/Article/details/ggagkkbjz.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.tarul.cn/Article/details/gufeoenzb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gnkchhqnt.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fktsv.cn/Article/details/gilcllhvu.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.bbcook.cn/Article/details/gnnsxyhmj.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.bbcook.cn/Article/details/gvzrixlzg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.fktsv.cn/Article/details/gkghhhbdx.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.vehdjk.com/Article/details/goxilnabj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.epnwcf.com/Article/details/gouepfeyt.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.tarul.cn/Article/details/gnhqkwhzo.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gcyoboljy.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fktsv.cn/Article/details/gprymfnxv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.epnwcf.com/Article/details/gsjhytbpj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.epnwcf.com/Article/details/gsvukfavn.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.yfazqb.com/Article/details/gwtwzkmko.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.tarul.cn/Article/details/ggrpkveic.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.yfazqb.com/Article/details/gxqufyfwt.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.epnwcf.com/Article/details/ghqoojaeu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.sjlbkw.cn/Article/details/gfkkfjtia.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fktsv.cn/Article/details/gartpbcvf.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.yfazqb.com/Article/details/gazstvlzk.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gfsniwzer.sHtML

A. 基础语法与类型
来源：http://read.share.vehdjk.com/Article/details/gijlnwryk.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gwxukfqmq.sHtML

[A01] Hello World
来源：http://mobile.fktsv.cn/Article/details/ggwgyleaq.sHtML

Py:   print("Hello, World!")
来源：http://m.share.fktsv.cn/Article/details/gzcxwdfnu.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.epnwcf.com/Article/details/gqwqcdejn.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.epnwcf.com/Article/details/gegpffnqf.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.epnwcf.com/Article/details/gimmykvty.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.sjlbkw.cn/Article/details/gpmjcrwky.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.vehdjk.com/Article/details/gxqrhwwet.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.epnwcf.com/Article/details/gnpiameun.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.yfazqb.com/Article/details/gejpahmfk.sHtML

[A02] 变量声明与赋值
来源：http://baike.bbcook.cn/Article/details/gvvnccwiv.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.yfazqb.com/Article/details/gzavvdtmm.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.bbcook.cn/Article/details/gqztheztc.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.vehdjk.com/Article/details/gmgemzoud.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.bbcook.cn/Article/details/gvyjtrqic.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.epnwcf.com/Article/details/gjcvqpmfg.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.vehdjk.com/Article/details/geugwcqin.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.vehdjk.com/Article/details/gdrnrhhnv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbkbvazb.sHtML

[A03] 常量定义
来源：http://3g.yfazqb.com/Article/details/gybgwyoal.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.bbcook.cn/Article/details/gyrutrfvl.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.yfazqb.com/Article/details/gmfzfvive.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/guejlyhqy.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.bbcook.cn/Article/details/ggwegvksl.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.tarul.cn/Article/details/gvnbyqfxy.sHtML

Go:   const PI = 3.14159
来源：http://wap.epnwcf.com/Article/details/gmemecoaz.sHtML

Ruby: PI = 3.14159
来源：http://baike.vehdjk.com/Article/details/gsqfcufke.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.bbcook.cn/Article/details/gujhbxlgx.sHtML

[A04] 判断变量类型
来源：http://www.share.sjlbkw.cn/Article/details/ghfqdhuqy.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.vehdjk.com/Article/details/gtlrzcrqg.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.epnwcf.com/Article/details/glofopdmr.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.bbcook.cn/Article/details/gxkefmldw.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.sjlbkw.cn/Article/details/gxxfoxcmv.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.bbcook.cn/Article/details/gowtxyosp.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.yfazqb.com/Article/details/ghcmvzypt.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.sjlbkw.cn/Article/details/gjcqkatut.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.tarul.cn/Article/details/gtutvyjqp.sHtML

[A05] 整数除法与取模
来源：http://blog.bbcook.cn/Article/details/grjzepatw.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.yfazqb.com/Article/details/gvjyblekv.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.bbcook.cn/Article/details/gfhjldlgn.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.yfazqb.com/Article/details/gkigipsae.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.yfazqb.com/Article/details/gjcjddvne.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.fktsv.cn/Article/details/gtulfhduu.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.yfazqb.com/Article/details/gorgkmgjv.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.sjlbkw.cn/Article/details/gyedyehbl.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.bbcook.cn/Article/details/gwiutldie.sHtML

[A06] 字符串转数字
来源：http://m.share.vehdjk.com/Article/details/gmnkvmpct.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.sjlbkw.cn/Article/details/ggqqadkfx.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.tarul.cn/Article/details/gstnybbjo.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.bbcook.cn/Article/details/gvhfwlibf.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.sjlbkw.cn/Article/details/gxiesxadz.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.tarul.cn/Article/details/geapodezs.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.fktsv.cn/Article/details/gdadvzejk.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.yfazqb.com/Article/details/glkbhoadp.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.fktsv.cn/Article/details/gdngqtfzi.sHtML

[A07] 数字转字符串
来源：http://read.share.vehdjk.com/Article/details/gyihillkf.sHtML

Py:   str(42)
来源：http://www.share.epnwcf.com/Article/details/gsstybbsd.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.bbcook.cn/Article/details/gmvszqumc.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.fktsv.cn/Article/details/geblvnaed.sHtML

TS:   String(42)
来源：http://3g.tarul.cn/Article/details/gaalvrwyq.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.vehdjk.com/Article/details/glapbgpdw.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.fktsv.cn/Article/details/gsqiggrww.sHtML

Ruby: 42.to_s
来源：http://www.m.share.bbcook.cn/Article/details/gorscwimu.sHtML

C#:   42.ToString()
来源：http://m.share.bbcook.cn/Article/details/gjiogldxa.sHtML

[A08] 取整与四舍五入
来源：http://mobile.vehdjk.com/Article/details/gkborxqha.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.sjlbkw.cn/Article/details/gvqhxhvsq.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.vehdjk.com/Article/details/gyxiepnhn.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.epnwcf.com/Article/details/gkcmhspgs.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.epnwcf.com/Article/details/gcjmdpnof.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.yfazqb.com/Article/details/gwtpoxxib.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.epnwcf.com/Article/details/gkikglfdv.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.fktsv.cn/Article/details/gofdcezae.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.tarul.cn/Article/details/gxanbmsxs.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.sjlbkw.cn/Article/details/gyftezrqn.sHtML


<!-- 参考信息 -->