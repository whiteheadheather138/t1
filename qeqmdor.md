代发 wailian999

[U57] PHP：字符串插值
来源：http://mobile.sjlbkw.cn/Article/details/gnguvgjxv.sHtML

"值: {$a}"
来源：http://m.share.bbcook.cn/Article/details/gypwjchyf.sHtML

[U58] PHP：数组三件套
来源：http://baike.fktsv.cn/Article/details/gcesdjhzl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.bbcook.cn/Article/details/ghduiurpp.sHtML

[U59] PHP：自定义排序
来源：http://3g.tarul.cn/Article/details/gjycpnnci.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fktsv.cn/Article/details/gwhatfuko.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.sjlbkw.cn/Article/details/gwqktyatx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.epnwcf.com/Article/details/gfrrxauni.sHtML

[U61] PHP：正则
来源：http://3g.tarul.cn/Article/details/gcnnqbrre.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fktsv.cn/Article/details/gykbohzkh.sHtML

[U62] PHP：日期对象
来源：http://blog.tarul.cn/Article/details/gbsssppar.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.tarul.cn/Article/details/gzfxftggc.sHtML

[U63] PHP：文件读写
来源：http://www.share.sjlbkw.cn/Article/details/gpuyghdml.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fktsv.cn/Article/details/gkrtgqjga.sHtML

[U64] PHP：目录遍历
来源：http://wap.yfazqb.com/Article/details/ghwzdssxo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.vehdjk.com/Article/details/gcrwcthfd.sHtML

[U65] PHP：会话
来源：http://www.blog.bbcook.cn/Article/details/gggyjzkew.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.vehdjk.com/Article/details/gktuqvxdj.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.vehdjk.com/Article/details/gdtrwukvh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.tarul.cn/Article/details/gmhipxdpa.sHtML

[U67] PHP：处理文件上传
来源：http://blog.bbcook.cn/Article/details/gilgsfklj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.tarul.cn/Article/details/gkghmfcxp.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.bbcook.cn/Article/details/gfupmtjky.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.epnwcf.com/Article/details/gxjpjgdpb.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.epnwcf.com/Article/details/gjsgjrjqr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.bbcook.cn/Article/details/ghrdillka.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.epnwcf.com/Article/details/guqbwdagu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.sjlbkw.cn/Article/details/gscutizfk.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.vehdjk.com/Article/details/glmgiukhm.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.bbcook.cn/Article/details/ggbpfrjel.sHtML

[U72] PHP：写错误日志
来源：http://blog.fktsv.cn/Article/details/gnkapfphe.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.sjlbkw.cn/Article/details/gkxwkjizj.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.yfazqb.com/Article/details/gsjqahopi.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.vehdjk.com/Article/details/gjhqomurj.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.yfazqb.com/Article/details/gmhomlsaw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.epnwcf.com/Article/details/gkptodhgm.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fktsv.cn/Article/details/gkyqldbyh.sHtML

composer require psr/container
来源：http://baike.yfazqb.com/Article/details/grsvcuyte.sHtML

[U76] PHP：简单路由
来源：http://3g.epnwcf.com/Article/details/ghikdrsxx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.epnwcf.com/Article/details/gzvajrnco.sHtML

[U77] PHP：模板渲染
来源：http://mobile.epnwcf.com/Article/details/gkftssqri.sHtML

composer require twig/twig
来源：http://www.share.tarul.cn/Article/details/gxtjronfq.sHtML

[U78] PHP：单元测试
来源：http://read.share.sjlbkw.cn/Article/details/grlsmvxoo.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.epnwcf.com/Article/details/gfkzfjgal.sHtML

[U79] PHP：静态分析
来源：http://m.share.yfazqb.com/Article/details/ghmciimru.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.bbcook.cn/Article/details/ghplshvis.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.vehdjk.com/Article/details/geewxbtwy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.sjlbkw.cn/Article/details/gfqrdrxgo.sHtML

[U81] JS：初始化项目
来源：http://read.share.fktsv.cn/Article/details/gwnzqhimr.sHtML

npm init -y;  npm i express
来源：http://wap.sjlbkw.cn/Article/details/gzqkzjpan.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fktsv.cn/Article/details/gweonovjk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.bbcook.cn/Article/details/guniarxtl.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fktsv.cn/Article/details/gykotmrug.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.yfazqb.com/Article/details/grfimdfgx.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.vehdjk.com/Article/details/gmjimsidm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.bbcook.cn/Article/details/gzwmxstod.sHtML

[U85] JS：可选链
来源：http://3g.fktsv.cn/Article/details/gzbnejjto.sHtML

a?.b?.c
来源：http://read.share.tarul.cn/Article/details/gybxeqogm.sHtML

[U86] JS：空值合并
来源：http://www.share.vehdjk.com/Article/details/glpsfgwrf.sHtML

a ?? b
来源：http://mobile.yfazqb.com/Article/details/glqbtlfzg.sHtML

[U87] JS：解构默认值
来源：http://blog.yfazqb.com/Article/details/goqjwynwz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.epnwcf.com/Article/details/gjboombtu.sHtML

[U88] JS：对象展开合并
来源：http://blog.vehdjk.com/Article/details/gxvoizxxd.sHtML

{ ...a, ...b }
来源：http://m.share.bbcook.cn/Article/details/ggaaxoeav.sHtML

[U89] JS：数组去重
来源：http://www.share.bbcook.cn/Article/details/gygklolfc.sHtML

[...new Set(arr)]
来源：http://mobile.vehdjk.com/Article/details/glkcayctj.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.bbcook.cn/Article/details/gsoiflhik.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.sjlbkw.cn/Article/details/giecxkpny.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.epnwcf.com/Article/details/geatbteql.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.yfazqb.com/Article/details/godmokmuh.sHtML

[U92] JS：深拷贝
来源：http://blog.tarul.cn/Article/details/gvuxjrlcx.sHtML

structuredClone(obj)
来源：http://www.blog.yfazqb.com/Article/details/gutykypkv.sHtML

[U93] JS：模板字符串
来源：http://mobile.vehdjk.com/Article/details/gisbiguzi.sHtML

`共 ${n} 条`
来源：http://blog.sjlbkw.cn/Article/details/glphcrtmm.sHtML

[U94] JS：箭头函数
来源：http://www.blog.bbcook.cn/Article/details/gnzbmiqto.sHtML

const double = x => x * 2;
来源：http://baike.bbcook.cn/Article/details/gvockpoiu.sHtML

[U95] JS：Promise 包装
来源：http://blog.vehdjk.com/Article/details/gjehlorra.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.vehdjk.com/Article/details/gkdvibpve.sHtML

[U96] JS：async/await 与异常
来源：http://baike.bbcook.cn/Article/details/glvcqlrjd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.epnwcf.com/Article/details/geetdnecu.sHtML

[U97] JS：并发请求
来源：http://www.m.share.yfazqb.com/Article/details/gjomvhezo.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.yfazqb.com/Article/details/gszoprbad.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.vehdjk.com/Article/details/geljrtloq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.epnwcf.com/Article/details/gmyejzkol.sHtML

[U99] JS：事件监听
来源：http://mobile.tarul.cn/Article/details/gflpprtdt.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.tarul.cn/Article/details/gzqlowaqu.sHtML

[U100] JS：DOM 查询
来源：http://blog.fktsv.cn/Article/details/gaplivnwv.sHtML

document.querySelector(".item")
来源：http://www.blog.yfazqb.com/Article/details/gepkrljxn.sHtML

[U101] JS：classList 操作
来源：http://wap.fktsv.cn/Article/details/gvfcuhntk.sHtML

el.classList.toggle("active")
来源：http://www.share.sjlbkw.cn/Article/details/giedgtccu.sHtML

[U102] JS：本地存储
来源：http://3g.sjlbkw.cn/Article/details/gzjankmmv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.yfazqb.com/Article/details/ggvxlpawc.sHtML

[U103] JS：定时器
来源：http://m.share.yfazqb.com/Article/details/gxvwzvabv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.bbcook.cn/Article/details/gkaexprau.sHtML

[U104] JS：防抖
来源：http://m.share.vehdjk.com/Article/details/gcezxbmzt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fktsv.cn/Article/details/gibhjibcy.sHtML

[U105] JS：节流
来源：http://www.m.share.epnwcf.com/Article/details/galeiqacz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.epnwcf.com/Article/details/grwerdsvv.sHtML

[U106] JS：日期格式化
来源：http://www.share.yfazqb.com/Article/details/gqpdjoyoi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fktsv.cn/Article/details/ghxobkxol.sHtML

[U107] JS：数字千分位
来源：http://m.share.yfazqb.com/Article/details/gvxdurfkm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.yfazqb.com/Article/details/gandcjcsk.sHtML

[U108] JS：随机整数
来源：http://www.share.yfazqb.com/Article/details/gskpczeov.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.tarul.cn/Article/details/gmizzqhpf.sHtML

[U109] JS：数组分组
来源：http://mobile.epnwcf.com/Article/details/gosfknnqz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.bbcook.cn/Article/details/gcknsrtgl.sHtML

[U110] JS：数组分块
来源：http://mobile.bbcook.cn/Article/details/gyvudjycn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.tarul.cn/Article/details/gigpzywas.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fktsv.cn/Article/details/ghhqlvfli.sHtML

new Map(Object.entries(obj))
来源：http://mobile.epnwcf.com/Article/details/ggcnnedbi.sHtML

[U112] JS：字符串补位
来源：http://3g.tarul.cn/Article/details/gvixduvgx.sHtML

"7".padStart(3, "0")
来源：http://www.share.tarul.cn/Article/details/gbdlxcvrx.sHtML

[U113] JS：正则替换全部
来源：http://wap.sjlbkw.cn/Article/details/goewwdlbl.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gqhwylxjo.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fktsv.cn/Article/details/gvrpnfykz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.yfazqb.com/Article/details/grfjzmtsi.sHtML

[U115] JS：生成 UUID
来源：http://www.share.yfazqb.com/Article/details/gixbjojfu.sHtML

crypto.randomUUID()
来源：http://m.share.tarul.cn/Article/details/glvuobgth.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.sjlbkw.cn/Article/details/gazqtyjtz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.vehdjk.com/Article/details/gajxymacw.sHtML

[U117] JS：单元测试
来源：http://www.m.share.epnwcf.com/Article/details/gzhuxbilb.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.sjlbkw.cn/Article/details/gqxkmvbgp.sHtML

[U118] JS：开发服务器
来源：http://mobile.bbcook.cn/Article/details/ggyjmsbfb.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.epnwcf.com/Article/details/gjoacivjj.sHtML

[U119] JS：生产构建
来源：http://wap.tarul.cn/Article/details/godlhntbf.sHtML

npx vite build
来源：http://baike.tarul.cn/Article/details/gwvynbebm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.yfazqb.com/Article/details/gvnssfhls.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.epnwcf.com/Article/details/gioagtlkv.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gcsadbcen.sHtML

统计汇总
来源：http://read.share.sjlbkw.cn/Article/details/ggcreqfqk.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/grolukhos.sHtML

按语言统计（条）：
来源：http://www.m.share.yfazqb.com/Article/details/gweyjqtas.sHtML

Python ......... 252
来源：http://3g.epnwcf.com/Article/details/gacqarrnx.sHtML

PHP ............ 252
来源：http://www.blog.sjlbkw.cn/Article/details/gwyuucanx.sHtML

JavaScript ..... 252
来源：http://blog.sjlbkw.cn/Article/details/gsocenzjp.sHtML

TypeScript ..... 212
来源：http://wap.sjlbkw.cn/Article/details/gumlvohxb.sHtML

Java ........... 212
来源：http://m.share.fktsv.cn/Article/details/gmmjcuhem.sHtML

Go ............. 212
来源：http://www.share.sjlbkw.cn/Article/details/gkumkhhtb.sHtML

Ruby ........... 212
来源：http://blog.tarul.cn/Article/details/gndplxydj.sHtML

C# ............. 212
来源：http://wap.fktsv.cn/Article/details/gxxcwrxoy.sHtML

C .............. 30
来源：http://mobile.tarul.cn/Article/details/gdjbmidyr.sHtML

C++ ............ 30
来源：http://www.m.share.yfazqb.com/Article/details/gvljapxqv.sHtML

SQL ............ 90
来源：http://wap.fktsv.cn/Article/details/gbucmxsxt.sHtML

Bash ........... 80
来源：http://read.share.tarul.cn/Article/details/gmomhudwx.sHtML

Kotlin ......... 15
来源：http://wap.tarul.cn/Article/details/gsoqfcntj.sHtML

Swift .......... 15
来源：http://www.share.bbcook.cn/Article/details/gvhumwnfe.sHtML

Lua ............ 10
来源：http://www.m.share.yfazqb.com/Article/details/gowtumokr.sHtML

Perl ........... 10
来源：http://baike.tarul.cn/Article/details/gswyfqycl.sHtML

Scala .......... 10
来源：http://read.share.vehdjk.com/Article/details/gztlhnobf.sHtML

------------------------------------
来源：http://blog.epnwcf.com/Article/details/glqdskwwg.sHtML

合计 ........... 2106 条
来源：http://blog.bbcook.cn/Article/details/gpoyyhfys.sHtML

按章节统计：
来源：http://www.share.yfazqb.com/Article/details/gfwygcsmm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.bbcook.cn/Article/details/grgojtiye.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.bbcook.cn/Article/details/goruttwcu.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.epnwcf.com/Article/details/gzahlmpzz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.vehdjk.com/Article/details/gnapsvajz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.epnwcf.com/Article/details/gdiwwgrpv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.vehdjk.com/Article/details/gsajivwvj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.tarul.cn/Article/details/gxahrhatb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.yfazqb.com/Article/details/gyupbikiy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.bbcook.cn/Article/details/gkhnemffb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.epnwcf.com/Article/details/gwkbpgpqv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.bbcook.cn/Article/details/gvorqtqzm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.tarul.cn/Article/details/gglvlsfpj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.yfazqb.com/Article/details/gbwwcljpe.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.sjlbkw.cn/Article/details/gzzfdlkih.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.tarul.cn/Article/details/gpllcqnfl.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.vehdjk.com/Article/details/gygoopwow.sHtML

Q SQL 专题                              90
来源：http://m.share.bbcook.cn/Article/details/grmcmfwru.sHtML

R Bash 专题                             80
来源：http://www.m.share.epnwcf.com/Article/details/gzdihwvqf.sHtML

S C / C++ 专题                          60
来源：http://m.share.sjlbkw.cn/Article/details/gbpivvyut.sHtML

T 其他语言补充                          60
来源：http://www.blog.epnwcf.com/Article/details/gbelkbcrt.sHtML

U 高频实用片段                         120
来源：http://mobile.fktsv.cn/Article/details/guglhkger.sHtML

------------------------------------
来源：http://www.blog.yfazqb.com/Article/details/gssvhdvnn.sHtML

合计                                  2106 条
来源：http://mobile.yfazqb.com/Article/details/guubvslkb.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.sjlbkw.cn/Article/details/gxxuvbsim.sHtML

使用提醒
来源：http://wap.bbcook.cn/Article/details/gatdvifoa.sHtML

--------------------------------------------------------------------------------
来源：http://baike.sjlbkw.cn/Article/details/guengwbuc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.epnwcf.com/Article/details/gzhnlmstq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.vehdjk.com/Article/details/gtxoxlrtz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.epnwcf.com/Article/details/gptucsmld.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fktsv.cn/Article/details/grbweclia.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.sjlbkw.cn/Article/details/gdjiocpdh.sHtML

—— 文件结束 ——
来源：http://baike.epnwcf.com/Article/details/gygshczeo.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gmfnicgof.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.bbcook.cn/Article/details/gxdxnphdk.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.epnwcf.com/Article/details/gbqhmcnjm.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gqruqegzo.sHtML

【收录内容】
来源：http://m.share.bbcook.cn/Article/details/gwnxclqiv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.sjlbkw.cn/Article/details/gdfozoyao.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.bbcook.cn/Article/details/gtwnzikoq.sHtML

SQL · Bash · C · C++
来源：http://wap.sjlbkw.cn/Article/details/gqfsodzbo.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.tarul.cn/Article/details/gfuffbavz.sHtML

【使用说明】
来源：http://baike.yfazqb.com/Article/details/givudckkp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.bbcook.cn/Article/details/gdwlwcemq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.bbcook.cn/Article/details/gpkzsootc.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.vehdjk.com/Article/details/gyhpwwkno.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.epnwcf.com/Article/details/gcdsklvqx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.tarul.cn/Article/details/gvynapvgv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.yfazqb.com/Article/details/gpnylynif.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.vehdjk.com/Article/details/grresvcob.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.yfazqb.com/Article/details/gsusmuxwp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.epnwcf.com/Article/details/gwcvdejyg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.tarul.cn/Article/details/gdwhgtisj.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fktsv.cn/Article/details/gjczpzhqo.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.yfazqb.com/Article/details/goxrrfzda.sHtML

【文件统计】
来源：http://blog.epnwcf.com/Article/details/glyvozxec.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.sjlbkw.cn/Article/details/ggrzhrumh.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.vehdjk.com/Article/details/gphlewagd.sHtML

目  录
来源：http://baike.bbcook.cn/Article/details/gmbciqnrj.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.bbcook.cn/Article/details/gxjwvrawu.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.bbcook.cn/Article/details/guxwoouvb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.tarul.cn/Article/details/gaetnqgpn.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fktsv.cn/Article/details/gpywqlnfl.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.epnwcf.com/Article/details/gyvmgubam.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.epnwcf.com/Article/details/gvdryippc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.sjlbkw.cn/Article/details/gusqtytsg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.sjlbkw.cn/Article/details/gheuaddxb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.tarul.cn/Article/details/gadbuoeug.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.epnwcf.com/Article/details/gzymiutvd.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gugtbgwug.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.bbcook.cn/Article/details/grejtyipe.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.bbcook.cn/Article/details/gbkskghss.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.epnwcf.com/Article/details/gxxmgjuid.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.epnwcf.com/Article/details/ghrxhphjl.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.tarul.cn/Article/details/gidtjmndi.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.bbcook.cn/Article/details/gunpjiiqp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.yfazqb.com/Article/details/gbbxbdjes.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.tarul.cn/Article/details/gwkcvxeku.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fktsv.cn/Article/details/gtttbjufv.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.yfazqb.com/Article/details/gsejhygip.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.tarul.cn/Article/details/gnbvtpsys.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gpmldgzeh.sHtML

A. 基础语法与类型
来源：http://www.m.share.bbcook.cn/Article/details/gqkzpbubt.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gvmfbqrqq.sHtML

[A01] Hello World
来源：http://m.share.fktsv.cn/Article/details/ghjbutrmr.sHtML

Py:   print("Hello, World!")
来源：http://www.share.fktsv.cn/Article/details/gyjeanolz.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.vehdjk.com/Article/details/glvntsrwg.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.sjlbkw.cn/Article/details/gidxdwnwb.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.bbcook.cn/Article/details/gkigskncx.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.yfazqb.com/Article/details/ghvejzbgm.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.bbcook.cn/Article/details/glcvjjsls.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.tarul.cn/Article/details/ggxbgzufh.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.tarul.cn/Article/details/gwugukxmk.sHtML

[A02] 变量声明与赋值
来源：http://www.share.sjlbkw.cn/Article/details/godtewtab.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.yfazqb.com/Article/details/ggyerfial.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.bbcook.cn/Article/details/gxxewiaum.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.epnwcf.com/Article/details/groadfkfn.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.fktsv.cn/Article/details/gtrpmnfly.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.yfazqb.com/Article/details/ggscymhxq.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.yfazqb.com/Article/details/ggddynbgk.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.sjlbkw.cn/Article/details/guwepgdzf.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.tarul.cn/Article/details/gdhlqyzcn.sHtML

[A03] 常量定义
来源：http://www.blog.yfazqb.com/Article/details/glyumaevy.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.sjlbkw.cn/Article/details/gjgnzpvfc.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.sjlbkw.cn/Article/details/gmbotpexz.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.fktsv.cn/Article/details/gpkoitmck.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/glormymoz.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.tarul.cn/Article/details/gogeinijo.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.sjlbkw.cn/Article/details/gopjkdkyh.sHtML

Ruby: PI = 3.14159
来源：http://m.share.sjlbkw.cn/Article/details/gxidqhoei.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.epnwcf.com/Article/details/gncnehjqz.sHtML

[A04] 判断变量类型
来源：http://www.blog.bbcook.cn/Article/details/gkdfwcmdc.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.fktsv.cn/Article/details/gqmvwbkce.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.sjlbkw.cn/Article/details/gpmjyawhe.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.bbcook.cn/Article/details/gtlnwrtgv.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.sjlbkw.cn/Article/details/gakjdwyhv.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.yfazqb.com/Article/details/goocpepbb.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.sjlbkw.cn/Article/details/gvbydjfgt.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.fktsv.cn/Article/details/gyjdnxrcp.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.yfazqb.com/Article/details/gjxirukzb.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.vehdjk.com/Article/details/gqqnvcjph.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.fktsv.cn/Article/details/giejvjtpb.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.sjlbkw.cn/Article/details/gwjitmxkf.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.yfazqb.com/Article/details/ghhwpimjm.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.vehdjk.com/Article/details/gebhsalon.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.yfazqb.com/Article/details/gywofxkzy.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.tarul.cn/Article/details/ggjsyeoef.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.fktsv.cn/Article/details/gihxllisu.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.vehdjk.com/Article/details/ghvfgvlmv.sHtML

[A06] 字符串转数字
来源：http://wap.epnwcf.com/Article/details/gdalduffl.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.yfazqb.com/Article/details/gtrqnlqeg.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.epnwcf.com/Article/details/glahosecx.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.tarul.cn/Article/details/ggebeyach.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.yfazqb.com/Article/details/gfobtjoor.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.sjlbkw.cn/Article/details/geosmculy.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.bbcook.cn/Article/details/gwxcsvbxg.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.vehdjk.com/Article/details/glgtcbotk.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.sjlbkw.cn/Article/details/gqkhcknrw.sHtML

[A07] 数字转字符串
来源：http://www.share.fktsv.cn/Article/details/gzaqgyptg.sHtML

Py:   str(42)
来源：http://wap.sjlbkw.cn/Article/details/gwsvrnivm.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.epnwcf.com/Article/details/grfehhmsp.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.epnwcf.com/Article/details/gzwiqflna.sHtML

TS:   String(42)
来源：http://blog.tarul.cn/Article/details/gfjglqrql.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.sjlbkw.cn/Article/details/gfzdmxnev.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.tarul.cn/Article/details/gjvnptcgv.sHtML

Ruby: 42.to_s
来源：http://3g.epnwcf.com/Article/details/gdkhvmzfc.sHtML

C#:   42.ToString()
来源：http://blog.epnwcf.com/Article/details/glsjlysll.sHtML

[A08] 取整与四舍五入
来源：http://baike.sjlbkw.cn/Article/details/glwlzoiup.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.epnwcf.com/Article/details/gzvgjdhcr.sHtML


<!-- 参考信息 -->