代发 wailian999

[U59] PHP：自定义排序
来源：http://3g.yfazqb.com/Article/details/gxqwtjldb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.yfazqb.com/Article/details/ghskxsngn.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.vehdjk.com/Article/details/ggjavpfgu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.epnwcf.com/Article/details/gfewgdupf.sHtML

[U61] PHP：正则
来源：http://read.share.tarul.cn/Article/details/ggbstuyww.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.vehdjk.com/Article/details/gekcqbldn.sHtML

[U62] PHP：日期对象
来源：http://3g.yfazqb.com/Article/details/gpqedzuwn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.vehdjk.com/Article/details/guuitxudb.sHtML

[U63] PHP：文件读写
来源：http://read.share.bbcook.cn/Article/details/ghgghhdsh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.epnwcf.com/Article/details/gsdraldda.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fktsv.cn/Article/details/grcedhxth.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.vehdjk.com/Article/details/gghkgzzmi.sHtML

[U65] PHP：会话
来源：http://wap.fktsv.cn/Article/details/gobxhsnbk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/gbdatpoyu.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.tarul.cn/Article/details/ggrpsyhwf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.tarul.cn/Article/details/gywmeahgg.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.epnwcf.com/Article/details/gqdxpdapu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.yfazqb.com/Article/details/gbnnpmrpe.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.yfazqb.com/Article/details/gdmjregob.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.yfazqb.com/Article/details/grqjtldxj.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.vehdjk.com/Article/details/gzzjmghhk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.vehdjk.com/Article/details/gyzersorq.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.sjlbkw.cn/Article/details/gzuqbpouy.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.tarul.cn/Article/details/gculyqvwx.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.tarul.cn/Article/details/gjisxehxb.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.vehdjk.com/Article/details/gljdsvqrh.sHtML

[U72] PHP：写错误日志
来源：http://3g.epnwcf.com/Article/details/giwzozxdh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.tarul.cn/Article/details/gmhhymhio.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.vehdjk.com/Article/details/gatlokgnl.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.sjlbkw.cn/Article/details/gnhxyfjgf.sHtML

[U74] PHP：读取环境变量
来源：http://blog.tarul.cn/Article/details/gfbrfzvkz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.bbcook.cn/Article/details/gnvgnrpjo.sHtML

[U75] PHP：依赖注入
来源：http://3g.yfazqb.com/Article/details/gcqegfusv.sHtML

composer require psr/container
来源：http://www.blog.fktsv.cn/Article/details/gdyotnixx.sHtML

[U76] PHP：简单路由
来源：http://www.blog.yfazqb.com/Article/details/gkrivhscr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.sjlbkw.cn/Article/details/gxbmuiprr.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fktsv.cn/Article/details/glokgrfbe.sHtML

composer require twig/twig
来源：http://mobile.fktsv.cn/Article/details/gyfvrgxfq.sHtML

[U78] PHP：单元测试
来源：http://www.share.epnwcf.com/Article/details/grosshnbn.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.vehdjk.com/Article/details/gandluzug.sHtML

[U79] PHP：静态分析
来源：http://www.blog.bbcook.cn/Article/details/gxyjzomzj.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.yfazqb.com/Article/details/gbxrcqaqu.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.epnwcf.com/Article/details/gqodhyqah.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.vehdjk.com/Article/details/giwesxmvt.sHtML

[U81] JS：初始化项目
来源：http://read.share.yfazqb.com/Article/details/golzdeuaq.sHtML

npm init -y;  npm i express
来源：http://mobile.yfazqb.com/Article/details/ggueqckhy.sHtML

[U82] JS：package.json 脚本
来源：http://3g.yfazqb.com/Article/details/gscnisbvg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.vehdjk.com/Article/details/guyvcdmys.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.epnwcf.com/Article/details/gtigxpjuu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.tarul.cn/Article/details/gpyrcxtuz.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.bbcook.cn/Article/details/gkilwkyff.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.vehdjk.com/Article/details/gnowfaltg.sHtML

[U85] JS：可选链
来源：http://blog.tarul.cn/Article/details/grwhczedq.sHtML

a?.b?.c
来源：http://www.m.share.fktsv.cn/Article/details/gflojtapy.sHtML

[U86] JS：空值合并
来源：http://mobile.yfazqb.com/Article/details/gzqqxwpoo.sHtML

a ?? b
来源：http://3g.yfazqb.com/Article/details/gkvqcdtyj.sHtML

[U87] JS：解构默认值
来源：http://3g.fktsv.cn/Article/details/gqotodrhr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.tarul.cn/Article/details/gzgxctapx.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fktsv.cn/Article/details/gnvgwiwyq.sHtML

{ ...a, ...b }
来源：http://www.share.vehdjk.com/Article/details/ghhzwaksi.sHtML

[U89] JS：数组去重
来源：http://blog.yfazqb.com/Article/details/gcppycajk.sHtML

[...new Set(arr)]
来源：http://www.m.share.sjlbkw.cn/Article/details/gnsesxnvo.sHtML

[U90] JS：数字数组排序
来源：http://wap.vehdjk.com/Article/details/gssgdojno.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.epnwcf.com/Article/details/gqrpmvgsi.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.yfazqb.com/Article/details/ghjswondn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.sjlbkw.cn/Article/details/gakllhefj.sHtML

[U92] JS：深拷贝
来源：http://baike.tarul.cn/Article/details/gvqzirwqb.sHtML

structuredClone(obj)
来源：http://mobile.bbcook.cn/Article/details/gizkknoyn.sHtML

[U93] JS：模板字符串
来源：http://baike.vehdjk.com/Article/details/gtqqcigtr.sHtML

`共 ${n} 条`
来源：http://blog.epnwcf.com/Article/details/glbstabjv.sHtML

[U94] JS：箭头函数
来源：http://blog.sjlbkw.cn/Article/details/gmdtojmqg.sHtML

const double = x => x * 2;
来源：http://3g.epnwcf.com/Article/details/gbxbpzxem.sHtML

[U95] JS：Promise 包装
来源：http://wap.fktsv.cn/Article/details/gelwhycnr.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.tarul.cn/Article/details/gcbgamsqf.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.bbcook.cn/Article/details/godnjhsky.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.bbcook.cn/Article/details/gyftjdcnq.sHtML

[U97] JS：并发请求
来源：http://read.share.sjlbkw.cn/Article/details/gsttvumzp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.epnwcf.com/Article/details/gndwmhjjh.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.sjlbkw.cn/Article/details/glxepibvb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.sjlbkw.cn/Article/details/ghaigftjk.sHtML

[U99] JS：事件监听
来源：http://baike.sjlbkw.cn/Article/details/guqyjnzwj.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.yfazqb.com/Article/details/gqbxdarib.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fktsv.cn/Article/details/gjxpqgwxd.sHtML

document.querySelector(".item")
来源：http://mobile.epnwcf.com/Article/details/grfdemlli.sHtML

[U101] JS：classList 操作
来源：http://m.share.sjlbkw.cn/Article/details/gwkgqavrl.sHtML

el.classList.toggle("active")
来源：http://3g.bbcook.cn/Article/details/gglgqunbh.sHtML

[U102] JS：本地存储
来源：http://3g.epnwcf.com/Article/details/gzmwunzde.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.yfazqb.com/Article/details/givzfztwj.sHtML

[U103] JS：定时器
来源：http://www.m.share.bbcook.cn/Article/details/gizrhjptz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fktsv.cn/Article/details/ghkyerhfv.sHtML

[U104] JS：防抖
来源：http://www.m.share.bbcook.cn/Article/details/gshrzxnjv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.bbcook.cn/Article/details/gvwkpkczp.sHtML

[U105] JS：节流
来源：http://mobile.yfazqb.com/Article/details/gvajkieul.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.yfazqb.com/Article/details/gixlpkrlc.sHtML

[U106] JS：日期格式化
来源：http://3g.vehdjk.com/Article/details/gttpwznxl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fktsv.cn/Article/details/gocgtkfkb.sHtML

[U107] JS：数字千分位
来源：http://3g.epnwcf.com/Article/details/gnycfkrqf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.yfazqb.com/Article/details/gurpyrlru.sHtML

[U108] JS：随机整数
来源：http://www.share.fktsv.cn/Article/details/gvrmtzvcd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fktsv.cn/Article/details/gpwfaqmez.sHtML

[U109] JS：数组分组
来源：http://wap.tarul.cn/Article/details/gtvujppny.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.sjlbkw.cn/Article/details/gkwmuonhe.sHtML

[U110] JS：数组分块
来源：http://m.share.bbcook.cn/Article/details/ggkzcginn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.bbcook.cn/Article/details/gfihecxkn.sHtML

[U111] JS：对象转 Map
来源：http://baike.yfazqb.com/Article/details/gtqygitja.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.vehdjk.com/Article/details/guugdranu.sHtML

[U112] JS：字符串补位
来源：http://read.share.sjlbkw.cn/Article/details/gzhcizrsq.sHtML

"7".padStart(3, "0")
来源：http://m.share.yfazqb.com/Article/details/grzgqziha.sHtML

[U113] JS：正则替换全部
来源：http://read.share.yfazqb.com/Article/details/gqkihkviv.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gpokighhz.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.sjlbkw.cn/Article/details/gecvrambd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.vehdjk.com/Article/details/gjoxyqhgj.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fktsv.cn/Article/details/gabhgarod.sHtML

crypto.randomUUID()
来源：http://baike.bbcook.cn/Article/details/gnfyuvxaj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fktsv.cn/Article/details/gxpkgnglz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.bbcook.cn/Article/details/gfecgipzr.sHtML

[U117] JS：单元测试
来源：http://wap.bbcook.cn/Article/details/gkfiaglhr.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fktsv.cn/Article/details/giwuoqzyq.sHtML

[U118] JS：开发服务器
来源：http://blog.yfazqb.com/Article/details/gapydclae.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.tarul.cn/Article/details/gugpxavvl.sHtML

[U119] JS：生产构建
来源：http://mobile.yfazqb.com/Article/details/gpgwuqgbo.sHtML

npx vite build
来源：http://www.blog.sjlbkw.cn/Article/details/gqzxvtjil.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.yfazqb.com/Article/details/gnhsviuzq.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.tarul.cn/Article/details/gzgtdbyij.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gvniapfbb.sHtML

统计汇总
来源：http://wap.yfazqb.com/Article/details/gzrzygvzi.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gmbbpievb.sHtML

按语言统计（条）：
来源：http://3g.tarul.cn/Article/details/gpagzdtna.sHtML

Python ......... 252
来源：http://read.share.sjlbkw.cn/Article/details/gimopyamc.sHtML

PHP ............ 252
来源：http://wap.fktsv.cn/Article/details/gnjoxtefk.sHtML

JavaScript ..... 252
来源：http://mobile.sjlbkw.cn/Article/details/gmjewrgoj.sHtML

TypeScript ..... 212
来源：http://www.m.share.fktsv.cn/Article/details/gsbqaumxb.sHtML

Java ........... 212
来源：http://www.blog.fktsv.cn/Article/details/goepicxrg.sHtML

Go ............. 212
来源：http://www.blog.yfazqb.com/Article/details/gzoytcige.sHtML

Ruby ........... 212
来源：http://www.m.share.tarul.cn/Article/details/gpqfoszfw.sHtML

C# ............. 212
来源：http://baike.sjlbkw.cn/Article/details/gzsvihazp.sHtML

C .............. 30
来源：http://3g.yfazqb.com/Article/details/grunhfkjp.sHtML

C++ ............ 30
来源：http://www.blog.fktsv.cn/Article/details/gxpqcpfqy.sHtML

SQL ............ 90
来源：http://www.share.tarul.cn/Article/details/gexmlfqiv.sHtML

Bash ........... 80
来源：http://blog.bbcook.cn/Article/details/guesnjkpz.sHtML

Kotlin ......... 15
来源：http://m.share.sjlbkw.cn/Article/details/gdcjrzbfr.sHtML

Swift .......... 15
来源：http://m.share.bbcook.cn/Article/details/gdthnqlre.sHtML

Lua ............ 10
来源：http://baike.fktsv.cn/Article/details/gwxbdzkhs.sHtML

Perl ........... 10
来源：http://wap.tarul.cn/Article/details/gkjsvqkgr.sHtML

Scala .......... 10
来源：http://www.blog.tarul.cn/Article/details/gvgkjecwv.sHtML

------------------------------------
来源：http://www.blog.epnwcf.com/Article/details/gkstbnhgz.sHtML

合计 ........... 2106 条
来源：http://baike.sjlbkw.cn/Article/details/ghwrywavt.sHtML

按章节统计：
来源：http://m.share.bbcook.cn/Article/details/gdeefnsip.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fktsv.cn/Article/details/gfqvwqjto.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.tarul.cn/Article/details/gvnofqrvn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.sjlbkw.cn/Article/details/gyboentqp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.yfazqb.com/Article/details/gtfjokihj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.bbcook.cn/Article/details/gcqvwjulk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.bbcook.cn/Article/details/gptnsdbpy.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.sjlbkw.cn/Article/details/gpgkgbqyl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.epnwcf.com/Article/details/ggyuekqtx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.bbcook.cn/Article/details/gxyjsmahj.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.bbcook.cn/Article/details/gjudkiimo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.bbcook.cn/Article/details/gzpakbksy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.bbcook.cn/Article/details/glpwgwuhy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fktsv.cn/Article/details/gfqrciyqr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fktsv.cn/Article/details/glkkwyowh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.epnwcf.com/Article/details/guvnjowkp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.tarul.cn/Article/details/gomrrifhn.sHtML

Q SQL 专题                              90
来源：http://read.share.vehdjk.com/Article/details/giahmtjbt.sHtML

R Bash 专题                             80
来源：http://blog.vehdjk.com/Article/details/gmehmmnmq.sHtML

S C / C++ 专题                          60
来源：http://m.share.sjlbkw.cn/Article/details/guwsjzutc.sHtML

T 其他语言补充                          60
来源：http://www.share.bbcook.cn/Article/details/gymzxhlel.sHtML

U 高频实用片段                         120
来源：http://read.share.epnwcf.com/Article/details/gtnnzmgfh.sHtML

------------------------------------
来源：http://m.share.bbcook.cn/Article/details/gibqatmaa.sHtML

合计                                  2106 条
来源：http://www.m.share.bbcook.cn/Article/details/gnpvlidzb.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.yfazqb.com/Article/details/gbavkgbsx.sHtML

使用提醒
来源：http://www.blog.fktsv.cn/Article/details/gwlwrzxjv.sHtML

--------------------------------------------------------------------------------
来源：http://baike.sjlbkw.cn/Article/details/gdvoildan.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.sjlbkw.cn/Article/details/gcxlbdohl.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.epnwcf.com/Article/details/gpyyugzam.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.epnwcf.com/Article/details/gtwjldszp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.sjlbkw.cn/Article/details/gabgdgdhw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.epnwcf.com/Article/details/gnvmhrmez.sHtML

—— 文件结束 ——
来源：http://www.m.share.fktsv.cn/Article/details/gswbobsae.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gsznucsto.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.bbcook.cn/Article/details/grutlvozn.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fktsv.cn/Article/details/gxyvvcqwf.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gvtezaaor.sHtML

【收录内容】
来源：http://www.m.share.fktsv.cn/Article/details/gpgqxqdfn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.yfazqb.com/Article/details/gloddadjp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.bbcook.cn/Article/details/gmbjbnlcx.sHtML

SQL · Bash · C · C++
来源：http://www.share.epnwcf.com/Article/details/gavogeaqz.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.bbcook.cn/Article/details/gemnzqncy.sHtML

【使用说明】
来源：http://www.blog.vehdjk.com/Article/details/gsenzbyok.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.sjlbkw.cn/Article/details/gzvjnsibo.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.bbcook.cn/Article/details/gloraunmk.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.yfazqb.com/Article/details/gvpjokmqs.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.epnwcf.com/Article/details/gojtvdktx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.epnwcf.com/Article/details/gpovohimv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.vehdjk.com/Article/details/gogfatkuj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.yfazqb.com/Article/details/gjuogquzr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.epnwcf.com/Article/details/gbdkrrabs.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.vehdjk.com/Article/details/gjzpndkaa.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.sjlbkw.cn/Article/details/grckuenwx.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fktsv.cn/Article/details/gjlyyotri.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.bbcook.cn/Article/details/gfkhjijag.sHtML

【文件统计】
来源：http://www.m.share.bbcook.cn/Article/details/gbemmqdiq.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.vehdjk.com/Article/details/gukxkkjqf.sHtML

--------------------------------------------------------------------------------
来源：http://baike.epnwcf.com/Article/details/genikpjhh.sHtML

目  录
来源：http://www.m.share.tarul.cn/Article/details/gbrmphbtf.sHtML

--------------------------------------------------------------------------------
来源：http://3g.sjlbkw.cn/Article/details/gpawfmmoy.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.yfazqb.com/Article/details/gyzslqrqr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.tarul.cn/Article/details/gfguwuhkx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.bbcook.cn/Article/details/gauewmoan.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.sjlbkw.cn/Article/details/gtxluykhr.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.yfazqb.com/Article/details/govotxuhr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.tarul.cn/Article/details/gbnngxdpg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fktsv.cn/Article/details/gvxmonuas.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.yfazqb.com/Article/details/gtezrhtez.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gnwxwbedm.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.vehdjk.com/Article/details/gboyisqcr.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.vehdjk.com/Article/details/gyebktvel.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.vehdjk.com/Article/details/glkolwnef.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.yfazqb.com/Article/details/geneqojhp.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.tarul.cn/Article/details/gwkzdkabn.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.bbcook.cn/Article/details/gisrktbpv.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.yfazqb.com/Article/details/gytvnbflq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.fktsv.cn/Article/details/gxjdjjseu.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.sjlbkw.cn/Article/details/gfpkedebk.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.tarul.cn/Article/details/ghuezuequ.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.tarul.cn/Article/details/gdsqdixss.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fktsv.cn/Article/details/gdjwiwiei.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gspjjqnij.sHtML

A. 基础语法与类型
来源：http://read.share.sjlbkw.cn/Article/details/gpssszwep.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gyzdsqyro.sHtML

[A01] Hello World
来源：http://baike.tarul.cn/Article/details/gbjphhvwv.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.yfazqb.com/Article/details/gvuianvrt.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.bbcook.cn/Article/details/gafdkhzya.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.fktsv.cn/Article/details/gbsvrkjzy.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.yfazqb.com/Article/details/ghugutmut.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.yfazqb.com/Article/details/gifnusljv.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.vehdjk.com/Article/details/giwyyihqt.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.fktsv.cn/Article/details/gmaroqsll.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.yfazqb.com/Article/details/gcfebwogr.sHtML

[A02] 变量声明与赋值
来源：http://blog.fktsv.cn/Article/details/glmnvnwwo.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.tarul.cn/Article/details/gmzkvmkzr.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.vehdjk.com/Article/details/gsahnhuyv.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.sjlbkw.cn/Article/details/gosycipfq.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.tarul.cn/Article/details/giiuiilak.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.vehdjk.com/Article/details/gnrenweje.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.bbcook.cn/Article/details/giyreqbzo.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.bbcook.cn/Article/details/gicqzccrk.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.fktsv.cn/Article/details/ggkuilbxi.sHtML

[A03] 常量定义
来源：http://read.share.epnwcf.com/Article/details/gtmmeavhu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.sjlbkw.cn/Article/details/gvrennexs.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.epnwcf.com/Article/details/gsjdjdzxg.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.yfazqb.com/Article/details/gzhrtnnqv.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.tarul.cn/Article/details/gfzdgdjdk.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.fktsv.cn/Article/details/genzptgoj.sHtML

Go:   const PI = 3.14159
来源：http://www.share.vehdjk.com/Article/details/gskhogqrf.sHtML

Ruby: PI = 3.14159
来源：http://wap.bbcook.cn/Article/details/gehavpkbs.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.epnwcf.com/Article/details/gvelouvmx.sHtML

[A04] 判断变量类型
来源：http://www.blog.epnwcf.com/Article/details/gsrotupbd.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.fktsv.cn/Article/details/gjaqnupqm.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.bbcook.cn/Article/details/gsaiiwrlh.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.yfazqb.com/Article/details/gmgtgiaco.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.fktsv.cn/Article/details/gsnmlimjr.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.sjlbkw.cn/Article/details/gydmrrwsn.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.tarul.cn/Article/details/gndppqkxc.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.epnwcf.com/Article/details/gylsnvkks.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.vehdjk.com/Article/details/geccoxftb.sHtML

[A05] 整数除法与取模
来源：http://www.blog.yfazqb.com/Article/details/gphlxyscq.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gjuxfeemg.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.vehdjk.com/Article/details/gbfzpwrjm.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fktsv.cn/Article/details/giofzfecy.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.tarul.cn/Article/details/gpzwrdmmk.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.bbcook.cn/Article/details/gflntfmav.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.tarul.cn/Article/details/gdgosqhwa.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.sjlbkw.cn/Article/details/gpsrtdlgg.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.bbcook.cn/Article/details/gtgedpjat.sHtML

[A06] 字符串转数字
来源：http://www.share.yfazqb.com/Article/details/genelthms.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.bbcook.cn/Article/details/geqgoggdq.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.epnwcf.com/Article/details/gkfprmyox.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.epnwcf.com/Article/details/gziuflfjs.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.tarul.cn/Article/details/grpwidyug.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.fktsv.cn/Article/details/gpnoqqftw.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.yfazqb.com/Article/details/ghzvlzikn.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.bbcook.cn/Article/details/gspfjeuoq.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.yfazqb.com/Article/details/gqmyuxnqj.sHtML

[A07] 数字转字符串
来源：http://www.m.share.epnwcf.com/Article/details/gqhbzwhrb.sHtML

Py:   str(42)
来源：http://read.share.vehdjk.com/Article/details/gwzugvazo.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.epnwcf.com/Article/details/gcysaxltl.sHtML

JS:   String(42); (42).toString()
来源：http://wap.epnwcf.com/Article/details/gnquvimyg.sHtML

TS:   String(42)
来源：http://www.m.share.yfazqb.com/Article/details/gacmnmmso.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.sjlbkw.cn/Article/details/gmarndmxj.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.fktsv.cn/Article/details/gqpzxnafb.sHtML

Ruby: 42.to_s
来源：http://read.share.yfazqb.com/Article/details/gfkxomyyg.sHtML

C#:   42.ToString()
来源：http://3g.fktsv.cn/Article/details/gbzjmscai.sHtML

[A08] 取整与四舍五入
来源：http://www.share.yfazqb.com/Article/details/gqaoczjcg.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.tarul.cn/Article/details/gxcqdwmou.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.fktsv.cn/Article/details/girlfoolu.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.sjlbkw.cn/Article/details/gilhaejzp.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.vehdjk.com/Article/details/gcbbdrqyy.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.vehdjk.com/Article/details/grdzckkhh.sHtML


<!-- 参考信息 -->