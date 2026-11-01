代发 wailian999

[U51] PHP：数组解构
来源：http://baike.vehdjk.com/Article/details/glbileope.sHtML

[$a, $b] = $arr;
来源：http://wap.sjlbkw.cn/Article/details/guonpoohn.sHtML

[U52] PHP：箭头函数
来源：http://blog.vehdjk.com/Article/details/gdfygkdjz.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.vehdjk.com/Article/details/gzfvbccij.sHtML

[U53] PHP：空合并运算符
来源：http://wap.tarul.cn/Article/details/gfgyjdcvz.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.vehdjk.com/Article/details/gndslgnoz.sHtML

[U54] PHP：空安全调用
来源：http://www.share.bbcook.cn/Article/details/gkciyyljf.sHtML

$obj?->method()
来源：http://wap.vehdjk.com/Article/details/gcvfspfse.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.tarul.cn/Article/details/gfpknlujc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.yfazqb.com/Article/details/ggviaqeuk.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.epnwcf.com/Article/details/gxvevjisc.sHtML

f(a: 1, b: 2)
来源：http://read.share.bbcook.cn/Article/details/gpuposcqo.sHtML

[U57] PHP：字符串插值
来源：http://wap.tarul.cn/Article/details/gyjhoryit.sHtML

"值: {$a}"
来源：http://www.share.bbcook.cn/Article/details/gssgeezur.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fktsv.cn/Article/details/gycyvfvid.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.vehdjk.com/Article/details/ggoghviix.sHtML

[U59] PHP：自定义排序
来源：http://3g.bbcook.cn/Article/details/gvfadcxqh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.vehdjk.com/Article/details/giideppdg.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.sjlbkw.cn/Article/details/gapzkcrtz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.tarul.cn/Article/details/gwfbxmuoe.sHtML

[U61] PHP：正则
来源：http://3g.fktsv.cn/Article/details/gngccgbcx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.bbcook.cn/Article/details/ggkkbmank.sHtML

[U62] PHP：日期对象
来源：http://blog.bbcook.cn/Article/details/gxpooknqu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fktsv.cn/Article/details/gcusxxwcb.sHtML

[U63] PHP：文件读写
来源：http://blog.sjlbkw.cn/Article/details/gmtrjoena.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.sjlbkw.cn/Article/details/gwnldvgwm.sHtML

[U64] PHP：目录遍历
来源：http://3g.vehdjk.com/Article/details/gzyokmagk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.epnwcf.com/Article/details/gntjcfsok.sHtML

[U65] PHP：会话
来源：http://www.blog.tarul.cn/Article/details/gaamhhsdq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gojiwxyiw.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.yfazqb.com/Article/details/ggzcmigbf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.vehdjk.com/Article/details/gdizocmpg.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.yfazqb.com/Article/details/gopgkziwj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.tarul.cn/Article/details/gyiyatvhk.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.bbcook.cn/Article/details/gabqezcfx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.tarul.cn/Article/details/gthctocop.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.tarul.cn/Article/details/gshzkamhg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fktsv.cn/Article/details/grbzesnuj.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.tarul.cn/Article/details/glleyvbti.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fktsv.cn/Article/details/gffswknob.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.epnwcf.com/Article/details/gszqahsce.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.tarul.cn/Article/details/ghqqgddge.sHtML

[U72] PHP：写错误日志
来源：http://blog.tarul.cn/Article/details/gohahtuki.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.epnwcf.com/Article/details/gavgpkwum.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.sjlbkw.cn/Article/details/gwadwfcsk.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.vehdjk.com/Article/details/gopfjorib.sHtML

[U74] PHP：读取环境变量
来源：http://3g.bbcook.cn/Article/details/gdtetvliv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fktsv.cn/Article/details/ginqwjfrb.sHtML

[U75] PHP：依赖注入
来源：http://baike.fktsv.cn/Article/details/gorybztcr.sHtML

composer require psr/container
来源：http://blog.yfazqb.com/Article/details/gwveqcfqm.sHtML

[U76] PHP：简单路由
来源：http://baike.tarul.cn/Article/details/gucvkvopk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.tarul.cn/Article/details/gseabohdo.sHtML

[U77] PHP：模板渲染
来源：http://m.share.tarul.cn/Article/details/gxoizcnxv.sHtML

composer require twig/twig
来源：http://wap.sjlbkw.cn/Article/details/gtsxyoofc.sHtML

[U78] PHP：单元测试
来源：http://3g.fktsv.cn/Article/details/goncpsgms.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fktsv.cn/Article/details/gruwpyepb.sHtML

[U79] PHP：静态分析
来源：http://www.share.yfazqb.com/Article/details/gpobjbfzf.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fktsv.cn/Article/details/grzbxvsdj.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.sjlbkw.cn/Article/details/glqlmutaa.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fktsv.cn/Article/details/gjfgajtgl.sHtML

[U81] JS：初始化项目
来源：http://wap.fktsv.cn/Article/details/gasasocdm.sHtML

npm init -y;  npm i express
来源：http://blog.bbcook.cn/Article/details/gnwblactn.sHtML

[U82] JS：package.json 脚本
来源：http://3g.tarul.cn/Article/details/gsiiklzow.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.bbcook.cn/Article/details/gbdwcnnbs.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.yfazqb.com/Article/details/gvrsyieaj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.tarul.cn/Article/details/gkxgjerrg.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.epnwcf.com/Article/details/gjzpfcdkg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.bbcook.cn/Article/details/gjnzfjqnm.sHtML

[U85] JS：可选链
来源：http://www.share.sjlbkw.cn/Article/details/gbnrhzyai.sHtML

a?.b?.c
来源：http://baike.vehdjk.com/Article/details/gwtuzreda.sHtML

[U86] JS：空值合并
来源：http://blog.sjlbkw.cn/Article/details/gzsvkxwta.sHtML

a ?? b
来源：http://www.blog.tarul.cn/Article/details/gbynkkmfu.sHtML

[U87] JS：解构默认值
来源：http://www.blog.tarul.cn/Article/details/gwqfgsrou.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.vehdjk.com/Article/details/gnurvhbvx.sHtML

[U88] JS：对象展开合并
来源：http://blog.bbcook.cn/Article/details/gxzppzmqg.sHtML

{ ...a, ...b }
来源：http://blog.bbcook.cn/Article/details/glgnvbmpm.sHtML

[U89] JS：数组去重
来源：http://3g.yfazqb.com/Article/details/gibmwkmtq.sHtML

[...new Set(arr)]
来源：http://www.share.tarul.cn/Article/details/gfmqwzunb.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.tarul.cn/Article/details/gepuudrmq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.yfazqb.com/Article/details/gtdrideot.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fktsv.cn/Article/details/gxfnkivxh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.epnwcf.com/Article/details/gfjxkjqpz.sHtML

[U92] JS：深拷贝
来源：http://www.blog.sjlbkw.cn/Article/details/gzhygzwze.sHtML

structuredClone(obj)
来源：http://www.share.fktsv.cn/Article/details/gbgijhfhu.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.yfazqb.com/Article/details/ggudfrwnc.sHtML

`共 ${n} 条`
来源：http://m.share.sjlbkw.cn/Article/details/gvytichbq.sHtML

[U94] JS：箭头函数
来源：http://www.share.vehdjk.com/Article/details/goldescdy.sHtML

const double = x => x * 2;
来源：http://www.share.yfazqb.com/Article/details/gaxxlwhnm.sHtML

[U95] JS：Promise 包装
来源：http://wap.fktsv.cn/Article/details/gybknpavo.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.sjlbkw.cn/Article/details/gnlobqugx.sHtML

[U96] JS：async/await 与异常
来源：http://wap.yfazqb.com/Article/details/ghzfrfwae.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.epnwcf.com/Article/details/ggtvlgvnz.sHtML

[U97] JS：并发请求
来源：http://baike.vehdjk.com/Article/details/glxbzjjyf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fktsv.cn/Article/details/gykplypvz.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.yfazqb.com/Article/details/gyihvegwd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fktsv.cn/Article/details/gcmtwioue.sHtML

[U99] JS：事件监听
来源：http://3g.sjlbkw.cn/Article/details/gulvzljyf.sHtML

el.addEventListener("click", e => {})
来源：http://wap.epnwcf.com/Article/details/gmzmahrow.sHtML

[U100] JS：DOM 查询
来源：http://wap.sjlbkw.cn/Article/details/gpvbzmrvm.sHtML

document.querySelector(".item")
来源：http://wap.epnwcf.com/Article/details/grknebvvm.sHtML

[U101] JS：classList 操作
来源：http://3g.bbcook.cn/Article/details/gwpaonzfz.sHtML

el.classList.toggle("active")
来源：http://baike.vehdjk.com/Article/details/gpphhlobm.sHtML

[U102] JS：本地存储
来源：http://3g.sjlbkw.cn/Article/details/ganbkfxee.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.vehdjk.com/Article/details/gjcrtnzmv.sHtML

[U103] JS：定时器
来源：http://3g.yfazqb.com/Article/details/gtxjtbhqr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.tarul.cn/Article/details/gtueojiwi.sHtML

[U104] JS：防抖
来源：http://www.m.share.bbcook.cn/Article/details/gyyzmdgzk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.bbcook.cn/Article/details/gjgsvxtao.sHtML

[U105] JS：节流
来源：http://m.share.sjlbkw.cn/Article/details/glcxfqcbr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.tarul.cn/Article/details/glylyfogl.sHtML

[U106] JS：日期格式化
来源：http://baike.sjlbkw.cn/Article/details/gsakfwxmk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.vehdjk.com/Article/details/gnvemirzd.sHtML

[U107] JS：数字千分位
来源：http://3g.vehdjk.com/Article/details/gpefrhhwe.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.bbcook.cn/Article/details/ghuykmrjl.sHtML

[U108] JS：随机整数
来源：http://m.share.sjlbkw.cn/Article/details/guyhksjkp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fktsv.cn/Article/details/gyjdzrfyc.sHtML

[U109] JS：数组分组
来源：http://wap.bbcook.cn/Article/details/gqtigxaxp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.epnwcf.com/Article/details/gqeatefyh.sHtML

[U110] JS：数组分块
来源：http://www.blog.bbcook.cn/Article/details/gpodinnyv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fktsv.cn/Article/details/golagjfio.sHtML

[U111] JS：对象转 Map
来源：http://read.share.vehdjk.com/Article/details/gsnulceun.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.sjlbkw.cn/Article/details/goblwqiet.sHtML

[U112] JS：字符串补位
来源：http://wap.fktsv.cn/Article/details/gwhtmcain.sHtML

"7".padStart(3, "0")
来源：http://www.blog.tarul.cn/Article/details/gxxlpjymy.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.sjlbkw.cn/Article/details/gsxpewakl.sHtML

s.replaceAll("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gfmxxenqo.sHtML

[U114] JS：JSON 深比较
来源：http://baike.tarul.cn/Article/details/gyoarbfpf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.vehdjk.com/Article/details/glqlxqkwm.sHtML

[U115] JS：生成 UUID
来源：http://wap.vehdjk.com/Article/details/grzyuewsu.sHtML

crypto.randomUUID()
来源：http://3g.tarul.cn/Article/details/gnmuhyleg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.tarul.cn/Article/details/gdhproyoq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fktsv.cn/Article/details/gejsnuxst.sHtML

[U117] JS：单元测试
来源：http://read.share.bbcook.cn/Article/details/gccyrfnxl.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.bbcook.cn/Article/details/gcvlqspvf.sHtML

[U118] JS：开发服务器
来源：http://blog.sjlbkw.cn/Article/details/gbmwdiljf.sHtML

npm i -D vite;  npx vite
来源：http://blog.tarul.cn/Article/details/gjzbamgzl.sHtML

[U119] JS：生产构建
来源：http://m.share.yfazqb.com/Article/details/gcnutytpe.sHtML

npx vite build
来源：http://www.blog.fktsv.cn/Article/details/gqfpvkfte.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.bbcook.cn/Article/details/gwksdioty.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fktsv.cn/Article/details/glnildicj.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gcyijdsll.sHtML

统计汇总
来源：http://baike.tarul.cn/Article/details/gtigodntu.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gzwvuigcf.sHtML

按语言统计（条）：
来源：http://baike.epnwcf.com/Article/details/ggtmdvhxz.sHtML

Python ......... 252
来源：http://www.blog.bbcook.cn/Article/details/gvbauzppx.sHtML

PHP ............ 252
来源：http://www.share.epnwcf.com/Article/details/gavmuecpj.sHtML

JavaScript ..... 252
来源：http://www.m.share.fktsv.cn/Article/details/gxljgakal.sHtML

TypeScript ..... 212
来源：http://www.m.share.tarul.cn/Article/details/gwmqogqaw.sHtML

Java ........... 212
来源：http://baike.epnwcf.com/Article/details/gnygktsph.sHtML

Go ............. 212
来源：http://wap.fktsv.cn/Article/details/gognbyows.sHtML

Ruby ........... 212
来源：http://blog.fktsv.cn/Article/details/gcfgvsaaz.sHtML

C# ............. 212
来源：http://mobile.epnwcf.com/Article/details/ggonlqryt.sHtML

C .............. 30
来源：http://wap.tarul.cn/Article/details/gogbemzne.sHtML

C++ ............ 30
来源：http://wap.epnwcf.com/Article/details/gsdysfpmn.sHtML

SQL ............ 90
来源：http://mobile.yfazqb.com/Article/details/ghomgqyli.sHtML

Bash ........... 80
来源：http://wap.yfazqb.com/Article/details/grqyeobtn.sHtML

Kotlin ......... 15
来源：http://baike.sjlbkw.cn/Article/details/gxqvjckhk.sHtML

Swift .......... 15
来源：http://read.share.epnwcf.com/Article/details/gbolqafsi.sHtML

Lua ............ 10
来源：http://m.share.fktsv.cn/Article/details/ghvtmcuxl.sHtML

Perl ........... 10
来源：http://www.blog.bbcook.cn/Article/details/gccjcmdfh.sHtML

Scala .......... 10
来源：http://wap.sjlbkw.cn/Article/details/gdqrlbjlx.sHtML

------------------------------------
来源：http://blog.bbcook.cn/Article/details/glcsnazhg.sHtML

合计 ........... 2106 条
来源：http://www.blog.tarul.cn/Article/details/gguozansb.sHtML

按章节统计：
来源：http://baike.fktsv.cn/Article/details/ghiviluqd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.tarul.cn/Article/details/gfpxqkpnp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.tarul.cn/Article/details/gyjlpjkyk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fktsv.cn/Article/details/gwfheqgyj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fktsv.cn/Article/details/gfegttffo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.tarul.cn/Article/details/gvonlflnv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.bbcook.cn/Article/details/gckpwbnan.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.bbcook.cn/Article/details/gmvlsbllo.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fktsv.cn/Article/details/gojctwshd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.vehdjk.com/Article/details/gwpnrjwqn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.vehdjk.com/Article/details/ghbgcmtjg.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.bbcook.cn/Article/details/goexratbh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.yfazqb.com/Article/details/gxobpkpcy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.epnwcf.com/Article/details/gqzkmqdxa.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.epnwcf.com/Article/details/grevkrldw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.tarul.cn/Article/details/gjsfemvje.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.sjlbkw.cn/Article/details/gzxtqdtnb.sHtML

Q SQL 专题                              90
来源：http://www.blog.vehdjk.com/Article/details/geblrzgjw.sHtML

R Bash 专题                             80
来源：http://3g.bbcook.cn/Article/details/gkuqvkghk.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.tarul.cn/Article/details/gmfqgllzh.sHtML

T 其他语言补充                          60
来源：http://wap.epnwcf.com/Article/details/gfbmlxcsp.sHtML

U 高频实用片段                         120
来源：http://3g.epnwcf.com/Article/details/gdnrjgwkk.sHtML

------------------------------------
来源：http://www.share.vehdjk.com/Article/details/gxvvpioqv.sHtML

合计                                  2106 条
来源：http://3g.sjlbkw.cn/Article/details/gyabkqbqz.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.tarul.cn/Article/details/gbtqyghkw.sHtML

使用提醒
来源：http://www.m.share.bbcook.cn/Article/details/gieurrymi.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fktsv.cn/Article/details/gnmbtmucw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.epnwcf.com/Article/details/gcspdijkk.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.yfazqb.com/Article/details/gdewsmpkj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.sjlbkw.cn/Article/details/gvbtjcuzx.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.sjlbkw.cn/Article/details/gfuuiwdsu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.tarul.cn/Article/details/gathukwrc.sHtML

—— 文件结束 ——
来源：http://baike.epnwcf.com/Article/details/gazlmunnr.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gmovebncn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.epnwcf.com/Article/details/guszbobbx.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.vehdjk.com/Article/details/gklbuggml.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gbwykeald.sHtML

【收录内容】
来源：http://mobile.sjlbkw.cn/Article/details/gfnypvksu.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.yfazqb.com/Article/details/gokmsjqqc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.sjlbkw.cn/Article/details/gtgbdgflu.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.bbcook.cn/Article/details/gdqvtyjdj.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.epnwcf.com/Article/details/gvqgimrwu.sHtML

【使用说明】
来源：http://wap.bbcook.cn/Article/details/gpeljakxd.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.yfazqb.com/Article/details/gdtcpeqlh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.epnwcf.com/Article/details/glnuavokc.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.epnwcf.com/Article/details/ghsbzkvrh.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.sjlbkw.cn/Article/details/grbbztptj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.bbcook.cn/Article/details/gaijjqojq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.bbcook.cn/Article/details/gbfkdprkf.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.tarul.cn/Article/details/gzfnfcfxy.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.sjlbkw.cn/Article/details/gdklhqnbu.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.vehdjk.com/Article/details/gzxbzldaj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.bbcook.cn/Article/details/glciccdxw.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.epnwcf.com/Article/details/gsjoluudz.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.epnwcf.com/Article/details/gximdyzwv.sHtML

【文件统计】
来源：http://wap.sjlbkw.cn/Article/details/gulaureao.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.sjlbkw.cn/Article/details/gmojbtirc.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.tarul.cn/Article/details/gkmgmhuyb.sHtML

目  录
来源：http://m.share.bbcook.cn/Article/details/gbgdzsjag.sHtML

--------------------------------------------------------------------------------
来源：http://blog.yfazqb.com/Article/details/gavvfyobb.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.epnwcf.com/Article/details/gujwfjfms.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.tarul.cn/Article/details/geuduozrf.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.bbcook.cn/Article/details/gzidggncz.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.sjlbkw.cn/Article/details/ggnxxtfmr.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.sjlbkw.cn/Article/details/gvohyicfc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.vehdjk.com/Article/details/ggqwexmmj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.bbcook.cn/Article/details/gcvvctgcx.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.bbcook.cn/Article/details/gbsacjwrz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.sjlbkw.cn/Article/details/guyotqxdi.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.tarul.cn/Article/details/gvmexthxb.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.bbcook.cn/Article/details/gbifeazty.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.sjlbkw.cn/Article/details/gdwduixpm.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.vehdjk.com/Article/details/gcvlhzebt.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.tarul.cn/Article/details/gwxcmgbab.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.yfazqb.com/Article/details/goiqenwnn.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.yfazqb.com/Article/details/ggmwjmuhk.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.yfazqb.com/Article/details/gblzffrag.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fktsv.cn/Article/details/grognhhbi.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.fktsv.cn/Article/details/gqhosqsiq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.bbcook.cn/Article/details/gfkulmzzp.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.epnwcf.com/Article/details/gtdpkxwny.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gvbyvceke.sHtML

A. 基础语法与类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gmhidduol.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gtgrgmbbl.sHtML

[A01] Hello World
来源：http://read.share.tarul.cn/Article/details/ggffqlvlw.sHtML

Py:   print("Hello, World!")
来源：http://wap.epnwcf.com/Article/details/geanyqpoh.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.sjlbkw.cn/Article/details/geyjhhdbc.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.epnwcf.com/Article/details/gmcowygim.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.yfazqb.com/Article/details/gufzntneb.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.yfazqb.com/Article/details/gbviybxrb.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.epnwcf.com/Article/details/gvbakiuzx.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.epnwcf.com/Article/details/gmmbauyia.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.epnwcf.com/Article/details/ghklhaucr.sHtML

[A02] 变量声明与赋值
来源：http://baike.fktsv.cn/Article/details/gcnuisgxk.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.vehdjk.com/Article/details/gjalibixe.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.bbcook.cn/Article/details/gkunwlenw.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.fktsv.cn/Article/details/gkoxelunu.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.epnwcf.com/Article/details/gshzungwz.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.fktsv.cn/Article/details/gbvfoiypi.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.bbcook.cn/Article/details/gadjmyoar.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.sjlbkw.cn/Article/details/ggqrsvsyf.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.vehdjk.com/Article/details/gaoycoscv.sHtML

[A03] 常量定义
来源：http://www.share.epnwcf.com/Article/details/gctulefng.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.yfazqb.com/Article/details/gfynmdgvq.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.tarul.cn/Article/details/grgsqfrfs.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.bbcook.cn/Article/details/ggtdkrkoq.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/gzdgckxou.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.fktsv.cn/Article/details/gfvdacnya.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.vehdjk.com/Article/details/gkerkxkua.sHtML

Ruby: PI = 3.14159
来源：http://baike.tarul.cn/Article/details/gfkbwqtln.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.sjlbkw.cn/Article/details/gpmzvkwlv.sHtML

[A04] 判断变量类型
来源：http://blog.tarul.cn/Article/details/gwenljyam.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.vehdjk.com/Article/details/gswwiszsq.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.yfazqb.com/Article/details/gxjjefepd.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.bbcook.cn/Article/details/gmlndviua.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.epnwcf.com/Article/details/gbalubrli.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.epnwcf.com/Article/details/gykcxnjhm.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.epnwcf.com/Article/details/grccpieax.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.yfazqb.com/Article/details/gtnxtqkla.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.epnwcf.com/Article/details/gxrxtcrwi.sHtML

[A05] 整数除法与取模
来源：http://mobile.fktsv.cn/Article/details/giubsfzzh.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.epnwcf.com/Article/details/goywgueam.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.vehdjk.com/Article/details/gdszpamea.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.yfazqb.com/Article/details/gutxgucnj.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.sjlbkw.cn/Article/details/gxztevnsl.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.epnwcf.com/Article/details/gvpjipxgl.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.epnwcf.com/Article/details/gvmkapclo.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.yfazqb.com/Article/details/gqdqhzmno.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.sjlbkw.cn/Article/details/glkmrrzcd.sHtML

[A06] 字符串转数字
来源：http://wap.tarul.cn/Article/details/gqqcxlxse.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.yfazqb.com/Article/details/gligkopyx.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.tarul.cn/Article/details/gddgzhxpx.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.bbcook.cn/Article/details/gzqrrzdpq.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.tarul.cn/Article/details/gepihbgaf.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.fktsv.cn/Article/details/giegnemsp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.vehdjk.com/Article/details/gsuiycshi.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.tarul.cn/Article/details/grmkuzlbe.sHtML


<!-- 参考信息 -->