代发 wailian999

[U59] PHP：自定义排序
来源：http://wap.sjlbkw.cn/Article/details/gswmljrcc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.epnwcf.com/Article/details/gvomvyehz.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.epnwcf.com/Article/details/gzynmmhac.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.sjlbkw.cn/Article/details/gdhpnosav.sHtML

[U61] PHP：正则
来源：http://blog.yfazqb.com/Article/details/gludrqlwm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.epnwcf.com/Article/details/gnsbubuiq.sHtML

[U62] PHP：日期对象
来源：http://www.blog.yfazqb.com/Article/details/gmiqewufe.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fktsv.cn/Article/details/gkcmtficc.sHtML

[U63] PHP：文件读写
来源：http://wap.fktsv.cn/Article/details/ghvkbczcd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.yfazqb.com/Article/details/gkfobrwsf.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fktsv.cn/Article/details/gnvftqtvb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.sjlbkw.cn/Article/details/gtrbplnui.sHtML

[U65] PHP：会话
来源：http://www.share.sjlbkw.cn/Article/details/gunomamkq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.tarul.cn/Article/details/gapliiodj.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.sjlbkw.cn/Article/details/gmzgyxexm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.yfazqb.com/Article/details/gdrtxtbxf.sHtML

[U67] PHP：处理文件上传
来源：http://wap.yfazqb.com/Article/details/goywgtxkq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.bbcook.cn/Article/details/gavzazbjo.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.vehdjk.com/Article/details/gfrskycce.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.yfazqb.com/Article/details/gjpzcypsw.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.vehdjk.com/Article/details/gupnxljue.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.vehdjk.com/Article/details/gwnlgrvql.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.sjlbkw.cn/Article/details/glpwrmeav.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.bbcook.cn/Article/details/gqullrtcj.sHtML

[U71] PHP：抛出异常
来源：http://read.share.yfazqb.com/Article/details/gpthhlvmo.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fktsv.cn/Article/details/gxindegym.sHtML

[U72] PHP：写错误日志
来源：http://mobile.bbcook.cn/Article/details/gemfvhcnn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.sjlbkw.cn/Article/details/gplzqakqh.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.yfazqb.com/Article/details/gmpcvgirb.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.vehdjk.com/Article/details/gjcsqfath.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.vehdjk.com/Article/details/gcqcevvur.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.epnwcf.com/Article/details/gcmerndnd.sHtML

[U75] PHP：依赖注入
来源：http://m.share.yfazqb.com/Article/details/gbgaftbpo.sHtML

composer require psr/container
来源：http://m.share.sjlbkw.cn/Article/details/gpvonaczt.sHtML

[U76] PHP：简单路由
来源：http://m.share.yfazqb.com/Article/details/gytyyyjet.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.bbcook.cn/Article/details/gnijqnejf.sHtML

[U77] PHP：模板渲染
来源：http://www.share.bbcook.cn/Article/details/gucjbnvip.sHtML

composer require twig/twig
来源：http://wap.bbcook.cn/Article/details/gnhovrriu.sHtML

[U78] PHP：单元测试
来源：http://blog.tarul.cn/Article/details/gnxkipdtg.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fktsv.cn/Article/details/gnabxfblo.sHtML

[U79] PHP：静态分析
来源：http://blog.vehdjk.com/Article/details/giuqqcuim.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.vehdjk.com/Article/details/gyiqsmlup.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.epnwcf.com/Article/details/giyluwdkn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.epnwcf.com/Article/details/gsartlosd.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.bbcook.cn/Article/details/gghwnlioz.sHtML

npm init -y;  npm i express
来源：http://www.share.vehdjk.com/Article/details/gclkbtvqm.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fktsv.cn/Article/details/gpqqqambr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fktsv.cn/Article/details/gbwycqwjs.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.bbcook.cn/Article/details/gjztnqrnx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.yfazqb.com/Article/details/gdvouvfvw.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.yfazqb.com/Article/details/gwkuozxor.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.sjlbkw.cn/Article/details/gqadmsnxj.sHtML

[U85] JS：可选链
来源：http://wap.fktsv.cn/Article/details/guxpcdnyk.sHtML

a?.b?.c
来源：http://wap.vehdjk.com/Article/details/gybjtijub.sHtML

[U86] JS：空值合并
来源：http://3g.bbcook.cn/Article/details/gqxemfssq.sHtML

a ?? b
来源：http://www.share.tarul.cn/Article/details/gdfmdrcyx.sHtML

[U87] JS：解构默认值
来源：http://www.blog.epnwcf.com/Article/details/gjdmwqgxc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.epnwcf.com/Article/details/gdwuewpob.sHtML

[U88] JS：对象展开合并
来源：http://3g.fktsv.cn/Article/details/ghxlnzeqf.sHtML

{ ...a, ...b }
来源：http://blog.tarul.cn/Article/details/ghaowynxl.sHtML

[U89] JS：数组去重
来源：http://baike.yfazqb.com/Article/details/gumjavkst.sHtML

[...new Set(arr)]
来源：http://wap.yfazqb.com/Article/details/gbvzgdlij.sHtML

[U90] JS：数字数组排序
来源：http://www.share.sjlbkw.cn/Article/details/gcuuawset.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.sjlbkw.cn/Article/details/gpkjwlmki.sHtML

[U91] JS：对象键值遍历
来源：http://baike.bbcook.cn/Article/details/gfwqmujoo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.tarul.cn/Article/details/gawreczct.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.bbcook.cn/Article/details/gfqeivafm.sHtML

structuredClone(obj)
来源：http://3g.vehdjk.com/Article/details/gisxmadaj.sHtML

[U93] JS：模板字符串
来源：http://blog.epnwcf.com/Article/details/gvhdinhnq.sHtML

`共 ${n} 条`
来源：http://mobile.tarul.cn/Article/details/gkcgffiyt.sHtML

[U94] JS：箭头函数
来源：http://3g.bbcook.cn/Article/details/gaqklovoi.sHtML

const double = x => x * 2;
来源：http://mobile.epnwcf.com/Article/details/gkkuzdreq.sHtML

[U95] JS：Promise 包装
来源：http://wap.bbcook.cn/Article/details/gmmzauhuv.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.vehdjk.com/Article/details/gyuewiryp.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.epnwcf.com/Article/details/gubygerca.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.yfazqb.com/Article/details/gwqevohyg.sHtML

[U97] JS：并发请求
来源：http://wap.vehdjk.com/Article/details/gspkzxzys.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.epnwcf.com/Article/details/gxrldtoqp.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.yfazqb.com/Article/details/gpibxqlnn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.epnwcf.com/Article/details/grminecin.sHtML

[U99] JS：事件监听
来源：http://baike.fktsv.cn/Article/details/giuhwlvro.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.tarul.cn/Article/details/grcurooyg.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.vehdjk.com/Article/details/gfdaoofne.sHtML

document.querySelector(".item")
来源：http://read.share.tarul.cn/Article/details/gninbsuxx.sHtML

[U101] JS：classList 操作
来源：http://www.blog.yfazqb.com/Article/details/gwgwpkuyd.sHtML

el.classList.toggle("active")
来源：http://www.share.fktsv.cn/Article/details/grzrnkhbe.sHtML

[U102] JS：本地存储
来源：http://www.share.yfazqb.com/Article/details/gtufqkesi.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.tarul.cn/Article/details/gvmlmdtsk.sHtML

[U103] JS：定时器
来源：http://www.m.share.yfazqb.com/Article/details/gkabwdrki.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.sjlbkw.cn/Article/details/gcmbeuynv.sHtML

[U104] JS：防抖
来源：http://www.share.fktsv.cn/Article/details/gfmxgrfsl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.epnwcf.com/Article/details/gkaauppge.sHtML

[U105] JS：节流
来源：http://m.share.sjlbkw.cn/Article/details/gpngozofn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.sjlbkw.cn/Article/details/gqtlzapvg.sHtML

[U106] JS：日期格式化
来源：http://m.share.yfazqb.com/Article/details/ghpzfidfq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.yfazqb.com/Article/details/gtkazsvng.sHtML

[U107] JS：数字千分位
来源：http://www.share.sjlbkw.cn/Article/details/gejtlvcmd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.tarul.cn/Article/details/gannkqxly.sHtML

[U108] JS：随机整数
来源：http://blog.epnwcf.com/Article/details/gjtghkzmh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fktsv.cn/Article/details/gddlccjzc.sHtML

[U109] JS：数组分组
来源：http://baike.epnwcf.com/Article/details/gzdmgujon.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.epnwcf.com/Article/details/giskbmmud.sHtML

[U110] JS：数组分块
来源：http://wap.sjlbkw.cn/Article/details/guxizgzpd.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.tarul.cn/Article/details/guemfmsgt.sHtML

[U111] JS：对象转 Map
来源：http://baike.sjlbkw.cn/Article/details/gzczdodvi.sHtML

new Map(Object.entries(obj))
来源：http://baike.fktsv.cn/Article/details/gtqkorkeh.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fktsv.cn/Article/details/gvuejnovu.sHtML

"7".padStart(3, "0")
来源：http://wap.yfazqb.com/Article/details/gxpkktwyg.sHtML

[U113] JS：正则替换全部
来源：http://wap.fktsv.cn/Article/details/gombgguvl.sHtML

s.replaceAll("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gnklsivlu.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.epnwcf.com/Article/details/gdiyvjspp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.tarul.cn/Article/details/gfvxslgkq.sHtML

[U115] JS：生成 UUID
来源：http://www.share.bbcook.cn/Article/details/gqnlcsujr.sHtML

crypto.randomUUID()
来源：http://www.share.vehdjk.com/Article/details/ggvhlshlb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fktsv.cn/Article/details/gvipgfodh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fktsv.cn/Article/details/gsrvdpijz.sHtML

[U117] JS：单元测试
来源：http://m.share.epnwcf.com/Article/details/gfrzsgmoj.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fktsv.cn/Article/details/ghasvecvl.sHtML

[U118] JS：开发服务器
来源：http://www.blog.epnwcf.com/Article/details/gynxbbbmt.sHtML

npm i -D vite;  npx vite
来源：http://m.share.bbcook.cn/Article/details/groxgivkc.sHtML

[U119] JS：生产构建
来源：http://mobile.epnwcf.com/Article/details/gnautcsms.sHtML

npx vite build
来源：http://wap.bbcook.cn/Article/details/gvqvlgwxd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.bbcook.cn/Article/details/gftlfvxxq.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.sjlbkw.cn/Article/details/gepmnfdel.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gwkoswrlp.sHtML

统计汇总
来源：http://read.share.yfazqb.com/Article/details/gnuxtwlqv.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gxaeztykt.sHtML

按语言统计（条）：
来源：http://3g.bbcook.cn/Article/details/gyrvwnmcm.sHtML

Python ......... 252
来源：http://baike.bbcook.cn/Article/details/gwzabqjzo.sHtML

PHP ............ 252
来源：http://mobile.epnwcf.com/Article/details/gqxupgtsm.sHtML

JavaScript ..... 252
来源：http://3g.sjlbkw.cn/Article/details/gbuksmkwl.sHtML

TypeScript ..... 212
来源：http://mobile.yfazqb.com/Article/details/ghfpapjyi.sHtML

Java ........... 212
来源：http://wap.yfazqb.com/Article/details/ghhzqnofx.sHtML

Go ............. 212
来源：http://www.share.vehdjk.com/Article/details/gisxxggdx.sHtML

Ruby ........... 212
来源：http://www.m.share.epnwcf.com/Article/details/gdnrfrlqu.sHtML

C# ............. 212
来源：http://baike.vehdjk.com/Article/details/gleeqsaik.sHtML

C .............. 30
来源：http://3g.sjlbkw.cn/Article/details/gpvtgmtph.sHtML

C++ ............ 30
来源：http://read.share.fktsv.cn/Article/details/gppobcvlf.sHtML

SQL ............ 90
来源：http://3g.tarul.cn/Article/details/gvcrxpgje.sHtML

Bash ........... 80
来源：http://www.blog.vehdjk.com/Article/details/gngxbujfc.sHtML

Kotlin ......... 15
来源：http://wap.epnwcf.com/Article/details/gtosanlah.sHtML

Swift .......... 15
来源：http://m.share.tarul.cn/Article/details/gomtwurfx.sHtML

Lua ............ 10
来源：http://baike.bbcook.cn/Article/details/gcnmfiugh.sHtML

Perl ........... 10
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqvgsnjh.sHtML

Scala .......... 10
来源：http://mobile.fktsv.cn/Article/details/gltsugxek.sHtML

------------------------------------
来源：http://blog.vehdjk.com/Article/details/gtetexbew.sHtML

合计 ........... 2106 条
来源：http://3g.sjlbkw.cn/Article/details/gudnkeewf.sHtML

按章节统计：
来源：http://read.share.sjlbkw.cn/Article/details/gevfpptfj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.epnwcf.com/Article/details/grnoemwtt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.tarul.cn/Article/details/gbuvdulbu.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fktsv.cn/Article/details/gdlwfrdkt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fktsv.cn/Article/details/gutqnykew.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fktsv.cn/Article/details/glxjbnfvu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.yfazqb.com/Article/details/gotgqyknd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.sjlbkw.cn/Article/details/gjtsbymje.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.tarul.cn/Article/details/gjnekngdd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.bbcook.cn/Article/details/gwwqempsv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.bbcook.cn/Article/details/gzrdvlwoz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.vehdjk.com/Article/details/gixunqgwi.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.tarul.cn/Article/details/gdqfhnhkf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.tarul.cn/Article/details/gtaoyszza.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.tarul.cn/Article/details/gkwoaoncp.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.epnwcf.com/Article/details/ggtuukuvc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.tarul.cn/Article/details/gkwrrkfxr.sHtML

Q SQL 专题                              90
来源：http://3g.bbcook.cn/Article/details/gmhbxebbd.sHtML

R Bash 专题                             80
来源：http://wap.tarul.cn/Article/details/gtazteymt.sHtML

S C / C++ 专题                          60
来源：http://wap.tarul.cn/Article/details/gjmzwnpsw.sHtML

T 其他语言补充                          60
来源：http://blog.epnwcf.com/Article/details/gwvludfbu.sHtML

U 高频实用片段                         120
来源：http://www.blog.epnwcf.com/Article/details/gnnwujpfn.sHtML

------------------------------------
来源：http://www.share.tarul.cn/Article/details/gsdwkbmqj.sHtML

合计                                  2106 条
来源：http://www.m.share.sjlbkw.cn/Article/details/gjyaiiezx.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.sjlbkw.cn/Article/details/gfestfint.sHtML

使用提醒
来源：http://www.blog.vehdjk.com/Article/details/gchiymlak.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.epnwcf.com/Article/details/gifinxjuc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.tarul.cn/Article/details/gnoxjcldm.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.tarul.cn/Article/details/geaognclg.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.tarul.cn/Article/details/glqojgchx.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.epnwcf.com/Article/details/grvywhgey.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.sjlbkw.cn/Article/details/gwjwugysj.sHtML

—— 文件结束 ——
来源：http://www.blog.bbcook.cn/Article/details/gqjioklut.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gvpxwszca.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.sjlbkw.cn/Article/details/gvmnbrmbd.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.yfazqb.com/Article/details/ggktwebhk.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gyoqvildv.sHtML

【收录内容】
来源：http://www.share.bbcook.cn/Article/details/gugjsfvbw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.tarul.cn/Article/details/gaibexpov.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fktsv.cn/Article/details/gbvfxipag.sHtML

SQL · Bash · C · C++
来源：http://m.share.vehdjk.com/Article/details/gtfsoymup.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.epnwcf.com/Article/details/ghflejywq.sHtML

【使用说明】
来源：http://mobile.bbcook.cn/Article/details/gfptzhtbr.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.yfazqb.com/Article/details/gfvtuhyzz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.sjlbkw.cn/Article/details/gsfnazbdu.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.vehdjk.com/Article/details/geukalrnc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.tarul.cn/Article/details/gtsvobwwj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.vehdjk.com/Article/details/grybwwcyi.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.epnwcf.com/Article/details/gtheinwbe.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fktsv.cn/Article/details/gzimdvbsw.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fktsv.cn/Article/details/gyfgaiiqg.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.sjlbkw.cn/Article/details/girqacpmc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.vehdjk.com/Article/details/gynhlwupj.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.bbcook.cn/Article/details/guepnjdnn.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.sjlbkw.cn/Article/details/gfndcgnov.sHtML

【文件统计】
来源：http://read.share.epnwcf.com/Article/details/gccujnvqx.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.epnwcf.com/Article/details/gwsihyeec.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.yfazqb.com/Article/details/gxboirwmt.sHtML

目  录
来源：http://www.m.share.vehdjk.com/Article/details/grupsoydf.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.yfazqb.com/Article/details/gxyuxlldi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.vehdjk.com/Article/details/gosawufng.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.sjlbkw.cn/Article/details/gbmmndvzb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fktsv.cn/Article/details/gvbmzvrfg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.tarul.cn/Article/details/gqdzvvgmf.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.vehdjk.com/Article/details/glncicoqk.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.yfazqb.com/Article/details/goioebjcs.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.tarul.cn/Article/details/gqjhnspei.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.vehdjk.com/Article/details/gzmsnkbjm.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.sjlbkw.cn/Article/details/gkmythhbf.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.yfazqb.com/Article/details/gqkdvkqkm.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.tarul.cn/Article/details/gycermyzb.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.tarul.cn/Article/details/glewvnadp.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.epnwcf.com/Article/details/gmqsavrra.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.bbcook.cn/Article/details/gfsiopbih.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.bbcook.cn/Article/details/gesxcizta.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.epnwcf.com/Article/details/goggjancw.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.vehdjk.com/Article/details/gxrhhummi.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.epnwcf.com/Article/details/gspsstnzf.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.yfazqb.com/Article/details/gqbdoofcm.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.sjlbkw.cn/Article/details/gltnwwvow.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.tarul.cn/Article/details/gtezureqf.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gtlkqncus.sHtML

A. 基础语法与类型
来源：http://mobile.vehdjk.com/Article/details/gasnvpxhf.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gzorwqcih.sHtML

[A01] Hello World
来源：http://www.blog.fktsv.cn/Article/details/gtdhaidhi.sHtML

Py:   print("Hello, World!")
来源：http://baike.fktsv.cn/Article/details/guuyplnzm.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.bbcook.cn/Article/details/gckrukdkr.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.tarul.cn/Article/details/goqwxbbvy.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.epnwcf.com/Article/details/guqlhchkx.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.sjlbkw.cn/Article/details/gpiusznyr.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.bbcook.cn/Article/details/gcyqvhdhd.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.fktsv.cn/Article/details/gekmeexcs.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.vehdjk.com/Article/details/gbkinbhow.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.epnwcf.com/Article/details/glriybukm.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.sjlbkw.cn/Article/details/gnxnmsnca.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.vehdjk.com/Article/details/gdnmxpmpz.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.yfazqb.com/Article/details/gtprigmto.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.yfazqb.com/Article/details/gozkbdktg.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.sjlbkw.cn/Article/details/gejouvacj.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.vehdjk.com/Article/details/gnbuosbzn.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.tarul.cn/Article/details/gccyciogc.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.yfazqb.com/Article/details/getrofltf.sHtML

[A03] 常量定义
来源：http://www.share.vehdjk.com/Article/details/gsncounru.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.vehdjk.com/Article/details/gvbwkwirp.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.tarul.cn/Article/details/gcxnrehfs.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.bbcook.cn/Article/details/gpqmyeakq.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.sjlbkw.cn/Article/details/gjohyfslf.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.fktsv.cn/Article/details/gwphswnuk.sHtML

Go:   const PI = 3.14159
来源：http://blog.bbcook.cn/Article/details/gttlzfkec.sHtML

Ruby: PI = 3.14159
来源：http://baike.yfazqb.com/Article/details/gpveorfru.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.vehdjk.com/Article/details/ghxsgjfkk.sHtML

[A04] 判断变量类型
来源：http://www.share.bbcook.cn/Article/details/gqzaixrre.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.vehdjk.com/Article/details/gwzljidfw.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.vehdjk.com/Article/details/gfzrjyzxd.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.sjlbkw.cn/Article/details/gynnddevz.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.epnwcf.com/Article/details/ghozxxbjz.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.vehdjk.com/Article/details/gudyhnilo.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.fktsv.cn/Article/details/gurvkzzmh.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.epnwcf.com/Article/details/gzwcrvnfe.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.fktsv.cn/Article/details/gpylqkmaz.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.fktsv.cn/Article/details/gzswdnigc.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.sjlbkw.cn/Article/details/gefavfnrn.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.fktsv.cn/Article/details/glqjmrgis.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.vehdjk.com/Article/details/gkhqacgyc.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.epnwcf.com/Article/details/giycjyvar.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.sjlbkw.cn/Article/details/gwxwosbks.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.epnwcf.com/Article/details/gybgwvxqs.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.tarul.cn/Article/details/gtgneetak.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.vehdjk.com/Article/details/ghmzrqxzb.sHtML

[A06] 字符串转数字
来源：http://blog.epnwcf.com/Article/details/gtctvveai.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.yfazqb.com/Article/details/gasntwqiv.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.fktsv.cn/Article/details/gfosewkcz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.epnwcf.com/Article/details/giozmklqy.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.yfazqb.com/Article/details/gwbbpzeuv.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.vehdjk.com/Article/details/gaiyibhrv.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.vehdjk.com/Article/details/gsxmvemnt.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.bbcook.cn/Article/details/gyzmrheeu.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.bbcook.cn/Article/details/gntksuiny.sHtML

[A07] 数字转字符串
来源：http://mobile.sjlbkw.cn/Article/details/gydqzuydm.sHtML

Py:   str(42)
来源：http://m.share.yfazqb.com/Article/details/gvzfnckra.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.tarul.cn/Article/details/gvsswqlbc.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.sjlbkw.cn/Article/details/giroqmdeb.sHtML

TS:   String(42)
来源：http://www.m.share.fktsv.cn/Article/details/gaffppgdp.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.bbcook.cn/Article/details/ggjpznwiy.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.yfazqb.com/Article/details/gcnnngfbi.sHtML

Ruby: 42.to_s
来源：http://read.share.sjlbkw.cn/Article/details/geqahdwyv.sHtML

C#:   42.ToString()
来源：http://m.share.epnwcf.com/Article/details/gjmauvwmg.sHtML

[A08] 取整与四舍五入
来源：http://www.share.fktsv.cn/Article/details/gwwbyfkdx.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.sjlbkw.cn/Article/details/gxxiugijq.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.bbcook.cn/Article/details/gvnqoapdi.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.bbcook.cn/Article/details/gichcqgng.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.yfazqb.com/Article/details/ggnscgrdo.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.epnwcf.com/Article/details/giauwruix.sHtML


<!-- 参考信息 -->