代发 wailian999

[U55] PHP：match 表达式
来源：http://www.m.share.fktsv.cn/Article/details/ggnysffza.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.sjlbkw.cn/Article/details/gtglsdjsw.sHtML

[U56] PHP：命名参数
来源：http://www.share.tarul.cn/Article/details/gcsnfmwxt.sHtML

f(a: 1, b: 2)
来源：http://wap.yfazqb.com/Article/details/gjpiuhkpp.sHtML

[U57] PHP：字符串插值
来源：http://3g.sjlbkw.cn/Article/details/gzzvgpqhh.sHtML

"值: {$a}"
来源：http://blog.fktsv.cn/Article/details/gvkvoosfi.sHtML

[U58] PHP：数组三件套
来源：http://wap.bbcook.cn/Article/details/gukeijcoa.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.epnwcf.com/Article/details/geismnksl.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.yfazqb.com/Article/details/gwngzubqt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gofiorxrg.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.sjlbkw.cn/Article/details/gdrsicqfu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.sjlbkw.cn/Article/details/gtpnflsty.sHtML

[U61] PHP：正则
来源：http://blog.yfazqb.com/Article/details/gvzxsjmlf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.epnwcf.com/Article/details/gdfwqekvs.sHtML

[U62] PHP：日期对象
来源：http://www.blog.bbcook.cn/Article/details/gnllladqw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.sjlbkw.cn/Article/details/ggvkesqdr.sHtML

[U63] PHP：文件读写
来源：http://read.share.bbcook.cn/Article/details/gfrxmszef.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fktsv.cn/Article/details/gpvzycqec.sHtML

[U64] PHP：目录遍历
来源：http://read.share.vehdjk.com/Article/details/goibkdaox.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.yfazqb.com/Article/details/gqzczkraq.sHtML

[U65] PHP：会话
来源：http://blog.yfazqb.com/Article/details/gzxsavtbc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gpusrwrnz.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.bbcook.cn/Article/details/grgveehfd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.tarul.cn/Article/details/gvlpjszsa.sHtML

[U67] PHP：处理文件上传
来源：http://3g.tarul.cn/Article/details/ghcdcvxmh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.vehdjk.com/Article/details/grmcwhfcb.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.tarul.cn/Article/details/gfhpgkgmw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.tarul.cn/Article/details/gfaldgocy.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.bbcook.cn/Article/details/gyuyexzel.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.bbcook.cn/Article/details/gehtncwfo.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.sjlbkw.cn/Article/details/ghmvsfefb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fktsv.cn/Article/details/ggmgttbut.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.sjlbkw.cn/Article/details/gujnycpmn.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.tarul.cn/Article/details/ghioacdct.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.sjlbkw.cn/Article/details/ggpepylpc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.yfazqb.com/Article/details/gsvbbngjz.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.sjlbkw.cn/Article/details/gmjimrnnt.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.bbcook.cn/Article/details/goevmmkgz.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.tarul.cn/Article/details/gaptkpbhk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.bbcook.cn/Article/details/gqraynzix.sHtML

[U75] PHP：依赖注入
来源：http://baike.fktsv.cn/Article/details/gpzxwhugf.sHtML

composer require psr/container
来源：http://www.share.vehdjk.com/Article/details/gxemorgxr.sHtML

[U76] PHP：简单路由
来源：http://www.share.vehdjk.com/Article/details/gownwbmkb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.yfazqb.com/Article/details/gdtvlyevm.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.tarul.cn/Article/details/gvasbgbag.sHtML

composer require twig/twig
来源：http://read.share.vehdjk.com/Article/details/geujuuwec.sHtML

[U78] PHP：单元测试
来源：http://blog.epnwcf.com/Article/details/gsbsjblmg.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.bbcook.cn/Article/details/gqododgvt.sHtML

[U79] PHP：静态分析
来源：http://www.share.vehdjk.com/Article/details/gosgqbjhk.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.epnwcf.com/Article/details/gghtzqcrw.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fktsv.cn/Article/details/garrscvpk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.bbcook.cn/Article/details/gphdenbsq.sHtML

[U81] JS：初始化项目
来源：http://www.share.vehdjk.com/Article/details/gxxlrajsm.sHtML

npm init -y;  npm i express
来源：http://baike.sjlbkw.cn/Article/details/ghtcxvjjs.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.yfazqb.com/Article/details/gcpigfrim.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.yfazqb.com/Article/details/grtztcopb.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.bbcook.cn/Article/details/gpuwyifgt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.vehdjk.com/Article/details/ghmjnazyf.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.vehdjk.com/Article/details/gbwazitqr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.sjlbkw.cn/Article/details/gvhcngbml.sHtML

[U85] JS：可选链
来源：http://read.share.sjlbkw.cn/Article/details/gyuzvnxvl.sHtML

a?.b?.c
来源：http://www.blog.sjlbkw.cn/Article/details/gwbuzrpzd.sHtML

[U86] JS：空值合并
来源：http://mobile.sjlbkw.cn/Article/details/gkazxejxc.sHtML

a ?? b
来源：http://m.share.yfazqb.com/Article/details/gaxvsqpoe.sHtML

[U87] JS：解构默认值
来源：http://3g.tarul.cn/Article/details/gjzoqqwxa.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.vehdjk.com/Article/details/gttcozgfu.sHtML

[U88] JS：对象展开合并
来源：http://read.share.sjlbkw.cn/Article/details/gofuhbllv.sHtML

{ ...a, ...b }
来源：http://read.share.tarul.cn/Article/details/gwbrlomly.sHtML

[U89] JS：数组去重
来源：http://m.share.epnwcf.com/Article/details/gsxwichce.sHtML

[...new Set(arr)]
来源：http://read.share.yfazqb.com/Article/details/gxrisrjcr.sHtML

[U90] JS：数字数组排序
来源：http://mobile.bbcook.cn/Article/details/gkxstmmqk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fktsv.cn/Article/details/gpmzdndqv.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fktsv.cn/Article/details/gzoqljoix.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.tarul.cn/Article/details/gfwhujerq.sHtML

[U92] JS：深拷贝
来源：http://m.share.vehdjk.com/Article/details/gpciicsxv.sHtML

structuredClone(obj)
来源：http://wap.yfazqb.com/Article/details/gcnppfrzq.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.yfazqb.com/Article/details/gjdnzlzvm.sHtML

`共 ${n} 条`
来源：http://www.share.epnwcf.com/Article/details/gavzoqdom.sHtML

[U94] JS：箭头函数
来源：http://blog.bbcook.cn/Article/details/gkbnccxpc.sHtML

const double = x => x * 2;
来源：http://m.share.bbcook.cn/Article/details/gvduxmhed.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.tarul.cn/Article/details/gbncjezcb.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.bbcook.cn/Article/details/gjkmeqalp.sHtML

[U96] JS：async/await 与异常
来源：http://wap.vehdjk.com/Article/details/ghiiyolgk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.bbcook.cn/Article/details/ghnumbkwd.sHtML

[U97] JS：并发请求
来源：http://wap.epnwcf.com/Article/details/gqrixfimr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.tarul.cn/Article/details/gnirgyvqc.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.sjlbkw.cn/Article/details/gndgimaph.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.sjlbkw.cn/Article/details/gmuffuiyq.sHtML

[U99] JS：事件监听
来源：http://mobile.bbcook.cn/Article/details/gdcggbzra.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fktsv.cn/Article/details/gztbwxkcb.sHtML

[U100] JS：DOM 查询
来源：http://mobile.epnwcf.com/Article/details/grhakkyiw.sHtML

document.querySelector(".item")
来源：http://m.share.vehdjk.com/Article/details/gqzrqlmml.sHtML

[U101] JS：classList 操作
来源：http://www.blog.epnwcf.com/Article/details/gwcwlbqxx.sHtML

el.classList.toggle("active")
来源：http://read.share.bbcook.cn/Article/details/gwdyceitq.sHtML

[U102] JS：本地存储
来源：http://baike.sjlbkw.cn/Article/details/godjchxqw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.tarul.cn/Article/details/gjywnycxl.sHtML

[U103] JS：定时器
来源：http://3g.sjlbkw.cn/Article/details/gkakwnwip.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.sjlbkw.cn/Article/details/geilpwtoq.sHtML

[U104] JS：防抖
来源：http://www.share.vehdjk.com/Article/details/gkozymecf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.bbcook.cn/Article/details/gopljlpiy.sHtML

[U105] JS：节流
来源：http://read.share.sjlbkw.cn/Article/details/gribtamru.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.tarul.cn/Article/details/galvrszrv.sHtML

[U106] JS：日期格式化
来源：http://wap.vehdjk.com/Article/details/glfookmld.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.vehdjk.com/Article/details/gchrrjedd.sHtML

[U107] JS：数字千分位
来源：http://wap.tarul.cn/Article/details/gmhrixtoz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.bbcook.cn/Article/details/gmwwooeoj.sHtML

[U108] JS：随机整数
来源：http://wap.yfazqb.com/Article/details/gzlfhzrqf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.epnwcf.com/Article/details/gudlspgyl.sHtML

[U109] JS：数组分组
来源：http://baike.vehdjk.com/Article/details/glnycybcr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.vehdjk.com/Article/details/gcqcancry.sHtML

[U110] JS：数组分块
来源：http://read.share.sjlbkw.cn/Article/details/gwxuicvcr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.vehdjk.com/Article/details/gbmppypbn.sHtML

[U111] JS：对象转 Map
来源：http://baike.fktsv.cn/Article/details/gjlzflgsz.sHtML

new Map(Object.entries(obj))
来源：http://mobile.epnwcf.com/Article/details/gpktsttng.sHtML

[U112] JS：字符串补位
来源：http://blog.vehdjk.com/Article/details/gwanbmthg.sHtML

"7".padStart(3, "0")
来源：http://wap.yfazqb.com/Article/details/gqnqyasbo.sHtML

[U113] JS：正则替换全部
来源：http://3g.tarul.cn/Article/details/gwtpmrvsu.sHtML

s.replaceAll("a", "b")
来源：http://blog.fktsv.cn/Article/details/gczzgmxna.sHtML

[U114] JS：JSON 深比较
来源：http://blog.yfazqb.com/Article/details/gwdhfvoit.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.tarul.cn/Article/details/gyohcjmtq.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fktsv.cn/Article/details/grvcygnej.sHtML

crypto.randomUUID()
来源：http://baike.fktsv.cn/Article/details/gvrmkjmga.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.yfazqb.com/Article/details/gzlxburjr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fktsv.cn/Article/details/grlynqnhh.sHtML

[U117] JS：单元测试
来源：http://read.share.sjlbkw.cn/Article/details/gzjbmigtf.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.tarul.cn/Article/details/gghscnmlm.sHtML

[U118] JS：开发服务器
来源：http://mobile.yfazqb.com/Article/details/gjvviiuah.sHtML

npm i -D vite;  npx vite
来源：http://3g.fktsv.cn/Article/details/gejcjnlgl.sHtML

[U119] JS：生产构建
来源：http://m.share.yfazqb.com/Article/details/guohrsasz.sHtML

npx vite build
来源：http://www.share.sjlbkw.cn/Article/details/gbsdknwvl.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.tarul.cn/Article/details/gwensalzy.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.tarul.cn/Article/details/gdakgkwat.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gaiwagtkb.sHtML

统计汇总
来源：http://www.share.fktsv.cn/Article/details/gqwewitkg.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gapwlpdgf.sHtML

按语言统计（条）：
来源：http://www.blog.epnwcf.com/Article/details/gfnfqxlnq.sHtML

Python ......... 252
来源：http://www.share.sjlbkw.cn/Article/details/gheralzfd.sHtML

PHP ............ 252
来源：http://read.share.sjlbkw.cn/Article/details/gxfeykvzc.sHtML

JavaScript ..... 252
来源：http://mobile.bbcook.cn/Article/details/gemticipr.sHtML

TypeScript ..... 212
来源：http://wap.vehdjk.com/Article/details/gedugacvp.sHtML

Java ........... 212
来源：http://blog.sjlbkw.cn/Article/details/gqbirtgie.sHtML

Go ............. 212
来源：http://mobile.vehdjk.com/Article/details/gljjwtbhg.sHtML

Ruby ........... 212
来源：http://www.m.share.bbcook.cn/Article/details/gesblzimn.sHtML

C# ............. 212
来源：http://www.blog.vehdjk.com/Article/details/gkuufeutu.sHtML

C .............. 30
来源：http://baike.epnwcf.com/Article/details/gwjqzkqes.sHtML

C++ ............ 30
来源：http://mobile.yfazqb.com/Article/details/gdigvgyqq.sHtML

SQL ............ 90
来源：http://wap.vehdjk.com/Article/details/gpxdrjyai.sHtML

Bash ........... 80
来源：http://read.share.tarul.cn/Article/details/guphrdsvz.sHtML

Kotlin ......... 15
来源：http://wap.vehdjk.com/Article/details/gkytzxnkp.sHtML

Swift .......... 15
来源：http://wap.tarul.cn/Article/details/gilncmttv.sHtML

Lua ............ 10
来源：http://blog.tarul.cn/Article/details/gfyzdseky.sHtML

Perl ........... 10
来源：http://baike.tarul.cn/Article/details/gqujpgqmz.sHtML

Scala .......... 10
来源：http://baike.vehdjk.com/Article/details/gkxkbhbsl.sHtML

------------------------------------
来源：http://baike.epnwcf.com/Article/details/gqeknpyvo.sHtML

合计 ........... 2106 条
来源：http://read.share.bbcook.cn/Article/details/gfgrjrbok.sHtML

按章节统计：
来源：http://baike.fktsv.cn/Article/details/gacboxtat.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.bbcook.cn/Article/details/gkfjsmkrq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fktsv.cn/Article/details/gykgdnhky.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.bbcook.cn/Article/details/gzpoowjzp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.yfazqb.com/Article/details/glcdpexlw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.vehdjk.com/Article/details/gqhwizplx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.epnwcf.com/Article/details/gdwpeyecj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fktsv.cn/Article/details/gylbaymqk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.vehdjk.com/Article/details/gmclesvat.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.vehdjk.com/Article/details/gnnyisnpb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.bbcook.cn/Article/details/gczcfbcvv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.yfazqb.com/Article/details/girfspyus.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.bbcook.cn/Article/details/gbttwbneu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.vehdjk.com/Article/details/gdjftpxyo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.tarul.cn/Article/details/guknolqli.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.vehdjk.com/Article/details/gjciabcqq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.bbcook.cn/Article/details/gbqefayzn.sHtML

Q SQL 专题                              90
来源：http://www.blog.sjlbkw.cn/Article/details/gneajicli.sHtML

R Bash 专题                             80
来源：http://blog.tarul.cn/Article/details/gklijhhyz.sHtML

S C / C++ 专题                          60
来源：http://www.share.bbcook.cn/Article/details/gevvxpcaj.sHtML

T 其他语言补充                          60
来源：http://m.share.yfazqb.com/Article/details/gseqlfkcq.sHtML

U 高频实用片段                         120
来源：http://mobile.tarul.cn/Article/details/gtyectkdx.sHtML

------------------------------------
来源：http://www.blog.sjlbkw.cn/Article/details/gqyyevprj.sHtML

合计                                  2106 条
来源：http://www.blog.sjlbkw.cn/Article/details/guumibzwb.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.yfazqb.com/Article/details/geusjdaof.sHtML

使用提醒
来源：http://baike.bbcook.cn/Article/details/godpyhiwv.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.sjlbkw.cn/Article/details/gccrsfqrd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.bbcook.cn/Article/details/gckxbbfml.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.yfazqb.com/Article/details/grxuzytsx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.sjlbkw.cn/Article/details/ghxpnvlka.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.tarul.cn/Article/details/gjzvtwoen.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.yfazqb.com/Article/details/grmrireip.sHtML

—— 文件结束 ——
来源：http://read.share.sjlbkw.cn/Article/details/guhzaxsgy.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gtgcyrufu.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.yfazqb.com/Article/details/gpcvivqrp.sHtML

Common Programming Examples Cheat Book
来源：http://3g.tarul.cn/Article/details/gdeacbuco.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/goipphggn.sHtML

【收录内容】
来源：http://www.m.share.yfazqb.com/Article/details/gtoiolnlo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.vehdjk.com/Article/details/gshqblufk.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.tarul.cn/Article/details/gtaixteph.sHtML

SQL · Bash · C · C++
来源：http://m.share.bbcook.cn/Article/details/gjfirbige.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.epnwcf.com/Article/details/gzbznuuxy.sHtML

【使用说明】
来源：http://read.share.tarul.cn/Article/details/gjhnvtmzg.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.vehdjk.com/Article/details/gznfhakdg.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.yfazqb.com/Article/details/ghtkwvkeh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fktsv.cn/Article/details/geaulefwl.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.vehdjk.com/Article/details/gwzanecuv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.bbcook.cn/Article/details/gmvyfbbyk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.sjlbkw.cn/Article/details/gralrtnta.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.epnwcf.com/Article/details/gzkyrwdch.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.tarul.cn/Article/details/gnmnlonah.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.yfazqb.com/Article/details/gfzqknnvo.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.bbcook.cn/Article/details/gabsjknqu.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fktsv.cn/Article/details/girqffvld.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.fktsv.cn/Article/details/gkwgtxxag.sHtML

【文件统计】
来源：http://www.share.fktsv.cn/Article/details/gcovyqbjd.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fktsv.cn/Article/details/gtcyvrsar.sHtML

--------------------------------------------------------------------------------
来源：http://3g.yfazqb.com/Article/details/gqexqprmk.sHtML

目  录
来源：http://blog.vehdjk.com/Article/details/gqehibnrc.sHtML

--------------------------------------------------------------------------------
来源：http://wap.bbcook.cn/Article/details/gmnjhjcya.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.yfazqb.com/Article/details/gpatxbdvr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.sjlbkw.cn/Article/details/gcsgrxsyi.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.sjlbkw.cn/Article/details/ghfaytazy.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.tarul.cn/Article/details/gaqldpuxb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.epnwcf.com/Article/details/gotollead.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.tarul.cn/Article/details/gtvateihk.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.yfazqb.com/Article/details/gjejqdnwy.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.yfazqb.com/Article/details/grljfkmvv.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.sjlbkw.cn/Article/details/gmswmoplk.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.bbcook.cn/Article/details/gibqijdou.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.yfazqb.com/Article/details/gfmbiceik.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.epnwcf.com/Article/details/guzitmcpc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.vehdjk.com/Article/details/gpzlswmig.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.tarul.cn/Article/details/gxqvloafe.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.tarul.cn/Article/details/garbpznha.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.fktsv.cn/Article/details/glnxdjmwc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.vehdjk.com/Article/details/gwhzbqjfb.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.bbcook.cn/Article/details/gudrbkbbj.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.yfazqb.com/Article/details/gryndaoud.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.vehdjk.com/Article/details/ghtqxdbqn.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/goxfqhlgm.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gyhvivtdq.sHtML

A. 基础语法与类型
来源：http://wap.fktsv.cn/Article/details/gqawjdquv.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gajnpnteg.sHtML

[A01] Hello World
来源：http://3g.vehdjk.com/Article/details/gojlqcdrn.sHtML

Py:   print("Hello, World!")
来源：http://wap.sjlbkw.cn/Article/details/gevuxdtlp.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.vehdjk.com/Article/details/gffrhsqso.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.vehdjk.com/Article/details/ginvjcjqn.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.bbcook.cn/Article/details/gcuznjoph.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.epnwcf.com/Article/details/gyzsgftpq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.yfazqb.com/Article/details/gddqcfhpu.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fktsv.cn/Article/details/gcxcqkujk.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.fktsv.cn/Article/details/gulkknhqp.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.epnwcf.com/Article/details/gljewucta.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.yfazqb.com/Article/details/gfsnmnprn.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.tarul.cn/Article/details/gniaxykle.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.sjlbkw.cn/Article/details/goxihegmh.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggsyyhjdk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.bbcook.cn/Article/details/gwqjmakhl.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.tarul.cn/Article/details/gdosewpaj.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fktsv.cn/Article/details/gmuhehilr.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.vehdjk.com/Article/details/gdypquhzx.sHtML

[A03] 常量定义
来源：http://www.share.yfazqb.com/Article/details/gdcwurnuv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.sjlbkw.cn/Article/details/gjxpyffde.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.sjlbkw.cn/Article/details/gfidekben.sHtML

JS:   const PI = 3.14159;
来源：http://baike.epnwcf.com/Article/details/gbitsnmec.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.epnwcf.com/Article/details/gkmjkxrns.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.bbcook.cn/Article/details/gpycddvny.sHtML

Go:   const PI = 3.14159
来源：http://3g.fktsv.cn/Article/details/gfdyjbjav.sHtML

Ruby: PI = 3.14159
来源：http://blog.fktsv.cn/Article/details/gndxbsgob.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/gdvjldhhu.sHtML

[A04] 判断变量类型
来源：http://m.share.epnwcf.com/Article/details/gxnniekiv.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.bbcook.cn/Article/details/gwtexxkto.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.vehdjk.com/Article/details/gobtqhmql.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.epnwcf.com/Article/details/gkskqmgmr.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.epnwcf.com/Article/details/getjavoeb.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.tarul.cn/Article/details/gilszfepj.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.bbcook.cn/Article/details/gitbsecim.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.epnwcf.com/Article/details/ghdznndxc.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.sjlbkw.cn/Article/details/galymebbw.sHtML

[A05] 整数除法与取模
来源：http://blog.epnwcf.com/Article/details/gkuiwgioj.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fktsv.cn/Article/details/ggpfvmhev.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.bbcook.cn/Article/details/ggyoojiqt.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.bbcook.cn/Article/details/gwaykxdlq.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fktsv.cn/Article/details/gjxeinfia.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.epnwcf.com/Article/details/gubhtbdsd.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.fktsv.cn/Article/details/gpnkablpy.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.fktsv.cn/Article/details/gfphvclju.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.yfazqb.com/Article/details/gmerpitxn.sHtML

[A06] 字符串转数字
来源：http://www.m.share.vehdjk.com/Article/details/gczotzojm.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.sjlbkw.cn/Article/details/gptgxapdo.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.tarul.cn/Article/details/ggigjjlip.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.tarul.cn/Article/details/gvirmwhlt.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.fktsv.cn/Article/details/gncdklidj.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.bbcook.cn/Article/details/ghobofikg.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.sjlbkw.cn/Article/details/goeekfnvx.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.vehdjk.com/Article/details/ggxrsqhbs.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.sjlbkw.cn/Article/details/geasmyyjl.sHtML

[A07] 数字转字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gviauzioj.sHtML

Py:   str(42)
来源：http://baike.fktsv.cn/Article/details/gnwhdonqp.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.fktsv.cn/Article/details/gffybzmnk.sHtML

JS:   String(42); (42).toString()
来源：http://baike.tarul.cn/Article/details/gfvqrymmz.sHtML

TS:   String(42)
来源：http://www.m.share.epnwcf.com/Article/details/gmvvjcbux.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.epnwcf.com/Article/details/gsriykqaz.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.yfazqb.com/Article/details/gqqxvutzi.sHtML


<!-- 参考信息 -->