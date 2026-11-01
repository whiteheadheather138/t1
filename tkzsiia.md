代发 wailian999

[U51] PHP：数组解构
来源：http://3g.tarul.cn/Article/details/gvtavqxpf.sHtML

[$a, $b] = $arr;
来源：http://read.share.yfazqb.com/Article/details/gwxoimpoq.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fktsv.cn/Article/details/gxqjteora.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.tarul.cn/Article/details/gtknzqrem.sHtML

[U53] PHP：空合并运算符
来源：http://blog.tarul.cn/Article/details/godqhpbwu.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.yfazqb.com/Article/details/gmagwrcio.sHtML

[U54] PHP：空安全调用
来源：http://3g.tarul.cn/Article/details/gpnooighp.sHtML

$obj?->method()
来源：http://3g.fktsv.cn/Article/details/gvhaxkhlr.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fktsv.cn/Article/details/ggltysopm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.epnwcf.com/Article/details/gtnzqeixk.sHtML

[U56] PHP：命名参数
来源：http://www.blog.epnwcf.com/Article/details/gaqaqvhwy.sHtML

f(a: 1, b: 2)
来源：http://blog.tarul.cn/Article/details/gzhojjgbe.sHtML

[U57] PHP：字符串插值
来源：http://baike.sjlbkw.cn/Article/details/gtjjgpbtx.sHtML

"值: {$a}"
来源：http://baike.yfazqb.com/Article/details/gwdgpoyir.sHtML

[U58] PHP：数组三件套
来源：http://blog.tarul.cn/Article/details/gvreoznxp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.vehdjk.com/Article/details/gfoaewvou.sHtML

[U59] PHP：自定义排序
来源：http://blog.tarul.cn/Article/details/gsomaaluf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.yfazqb.com/Article/details/gonfgmhgx.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.sjlbkw.cn/Article/details/godxsdikg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.tarul.cn/Article/details/gutcuozrd.sHtML

[U61] PHP：正则
来源：http://m.share.yfazqb.com/Article/details/gvkqwxsew.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.epnwcf.com/Article/details/gljpqbtwj.sHtML

[U62] PHP：日期对象
来源：http://www.blog.sjlbkw.cn/Article/details/gyhuiekub.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.sjlbkw.cn/Article/details/gbujfxafd.sHtML

[U63] PHP：文件读写
来源：http://blog.yfazqb.com/Article/details/gucdvedqd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.yfazqb.com/Article/details/gyixhwwsv.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fktsv.cn/Article/details/gpsmzeqsa.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.tarul.cn/Article/details/glwzuafcu.sHtML

[U65] PHP：会话
来源：http://mobile.sjlbkw.cn/Article/details/gpklyaqxs.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gadwxjhbp.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fktsv.cn/Article/details/gtekkdbbg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.bbcook.cn/Article/details/gvbndfqtr.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.bbcook.cn/Article/details/gutkmhyjh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.epnwcf.com/Article/details/ghmitpdlh.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.epnwcf.com/Article/details/gpbjjbrmh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fktsv.cn/Article/details/gdxyjlyws.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.epnwcf.com/Article/details/gkmzhqlnx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.yfazqb.com/Article/details/gqpvapwuw.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.epnwcf.com/Article/details/gulqdxxod.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.sjlbkw.cn/Article/details/glrnpkexc.sHtML

[U71] PHP：抛出异常
来源：http://www.share.bbcook.cn/Article/details/gzgosqapt.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.sjlbkw.cn/Article/details/gmnvvigwz.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbvqhbyr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fktsv.cn/Article/details/gotuyceyp.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.tarul.cn/Article/details/gjhzjbsck.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.bbcook.cn/Article/details/gkkfmndng.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.yfazqb.com/Article/details/goixlnfft.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.epnwcf.com/Article/details/gzgghmlau.sHtML

[U75] PHP：依赖注入
来源：http://www.share.epnwcf.com/Article/details/gzwivigwz.sHtML

composer require psr/container
来源：http://www.m.share.yfazqb.com/Article/details/gxvtjjntm.sHtML

[U76] PHP：简单路由
来源：http://mobile.fktsv.cn/Article/details/gqjkyyugg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.bbcook.cn/Article/details/gnmmgdozi.sHtML

[U77] PHP：模板渲染
来源：http://m.share.yfazqb.com/Article/details/gtjsjwlpx.sHtML

composer require twig/twig
来源：http://m.share.yfazqb.com/Article/details/gmgflvhdw.sHtML

[U78] PHP：单元测试
来源：http://blog.bbcook.cn/Article/details/gpaonesfy.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.vehdjk.com/Article/details/gdtvbxchq.sHtML

[U79] PHP：静态分析
来源：http://www.share.bbcook.cn/Article/details/gqxnviybc.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.tarul.cn/Article/details/gatuqvnbo.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.epnwcf.com/Article/details/gdrpabeam.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.sjlbkw.cn/Article/details/galfkqotb.sHtML

[U81] JS：初始化项目
来源：http://mobile.bbcook.cn/Article/details/gsaznxsll.sHtML

npm init -y;  npm i express
来源：http://www.share.epnwcf.com/Article/details/gvkrcqtyt.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fktsv.cn/Article/details/goecruksa.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fktsv.cn/Article/details/ghdsvnhrs.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.epnwcf.com/Article/details/gokojmemh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.sjlbkw.cn/Article/details/gbnuoftgp.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.vehdjk.com/Article/details/gfgawndyu.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.bbcook.cn/Article/details/gwdfoqpgu.sHtML

[U85] JS：可选链
来源：http://wap.bbcook.cn/Article/details/glxrxlzle.sHtML

a?.b?.c
来源：http://mobile.bbcook.cn/Article/details/gdzykqbup.sHtML

[U86] JS：空值合并
来源：http://m.share.epnwcf.com/Article/details/gjpgnfcno.sHtML

a ?? b
来源：http://mobile.fktsv.cn/Article/details/gceywhwqi.sHtML

[U87] JS：解构默认值
来源：http://read.share.vehdjk.com/Article/details/gxbdskcqa.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.sjlbkw.cn/Article/details/gwtahkave.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.bbcook.cn/Article/details/ghixnzonw.sHtML

{ ...a, ...b }
来源：http://mobile.vehdjk.com/Article/details/gumqukvjn.sHtML

[U89] JS：数组去重
来源：http://www.m.share.bbcook.cn/Article/details/gwakuffxb.sHtML

[...new Set(arr)]
来源：http://read.share.epnwcf.com/Article/details/goyvvtvqs.sHtML

[U90] JS：数字数组排序
来源：http://www.share.yfazqb.com/Article/details/gowdvlpdr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.vehdjk.com/Article/details/gmmgwvvki.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fktsv.cn/Article/details/ggbefzwdr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.tarul.cn/Article/details/gdmlagvlo.sHtML

[U92] JS：深拷贝
来源：http://baike.vehdjk.com/Article/details/gkyjseizu.sHtML

structuredClone(obj)
来源：http://wap.epnwcf.com/Article/details/glauedijc.sHtML

[U93] JS：模板字符串
来源：http://wap.epnwcf.com/Article/details/glfqgwiro.sHtML

`共 ${n} 条`
来源：http://m.share.tarul.cn/Article/details/gbncfgpxi.sHtML

[U94] JS：箭头函数
来源：http://blog.tarul.cn/Article/details/ghufulssw.sHtML

const double = x => x * 2;
来源：http://baike.sjlbkw.cn/Article/details/gcliyczwh.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.yfazqb.com/Article/details/gtwtjnxbt.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.epnwcf.com/Article/details/gmymlgwcp.sHtML

[U96] JS：async/await 与异常
来源：http://blog.vehdjk.com/Article/details/gwcajrpeo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.vehdjk.com/Article/details/gblhymdhg.sHtML

[U97] JS：并发请求
来源：http://baike.fktsv.cn/Article/details/giiiidcnz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.epnwcf.com/Article/details/gntrehify.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.bbcook.cn/Article/details/gepocheuw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.vehdjk.com/Article/details/gthlcznvm.sHtML

[U99] JS：事件监听
来源：http://mobile.bbcook.cn/Article/details/gumznmmxn.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fktsv.cn/Article/details/gbtsvgisr.sHtML

[U100] JS：DOM 查询
来源：http://m.share.epnwcf.com/Article/details/gvuykqiaw.sHtML

document.querySelector(".item")
来源：http://wap.vehdjk.com/Article/details/gljyqdxrk.sHtML

[U101] JS：classList 操作
来源：http://www.blog.sjlbkw.cn/Article/details/gzvjwbpgm.sHtML

el.classList.toggle("active")
来源：http://3g.sjlbkw.cn/Article/details/gxrveglsv.sHtML

[U102] JS：本地存储
来源：http://blog.fktsv.cn/Article/details/giyeynshm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjekudla.sHtML

[U103] JS：定时器
来源：http://www.m.share.tarul.cn/Article/details/gflrbohxd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.vehdjk.com/Article/details/gcztuatnf.sHtML

[U104] JS：防抖
来源：http://www.m.share.tarul.cn/Article/details/gtwamgiyt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.epnwcf.com/Article/details/gjvzjzrak.sHtML

[U105] JS：节流
来源：http://www.m.share.yfazqb.com/Article/details/ghgmzelpn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.bbcook.cn/Article/details/gcwoiqqvi.sHtML

[U106] JS：日期格式化
来源：http://www.share.vehdjk.com/Article/details/glnzarpdy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.vehdjk.com/Article/details/giwbtqeuq.sHtML

[U107] JS：数字千分位
来源：http://mobile.bbcook.cn/Article/details/gsyggceua.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.tarul.cn/Article/details/gimwcsgpb.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fktsv.cn/Article/details/ghsmzzrkn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.bbcook.cn/Article/details/gnbeqxfaw.sHtML

[U109] JS：数组分组
来源：http://www.share.tarul.cn/Article/details/gbpjkbyuc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fktsv.cn/Article/details/grqrmioal.sHtML

[U110] JS：数组分块
来源：http://m.share.tarul.cn/Article/details/gnrzhauim.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fktsv.cn/Article/details/gpauftqaf.sHtML

[U111] JS：对象转 Map
来源：http://baike.bbcook.cn/Article/details/gjqhiyooa.sHtML

new Map(Object.entries(obj))
来源：http://m.share.epnwcf.com/Article/details/gmshecykg.sHtML

[U112] JS：字符串补位
来源：http://www.blog.bbcook.cn/Article/details/gdtwrbmzy.sHtML

"7".padStart(3, "0")
来源：http://www.share.vehdjk.com/Article/details/gvtzrhkug.sHtML

[U113] JS：正则替换全部
来源：http://m.share.yfazqb.com/Article/details/gvchsohey.sHtML

s.replaceAll("a", "b")
来源：http://blog.bbcook.cn/Article/details/gtytrqnjq.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.tarul.cn/Article/details/giavhqnir.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.tarul.cn/Article/details/gkmycenrd.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.tarul.cn/Article/details/gugdrdpee.sHtML

crypto.randomUUID()
来源：http://mobile.tarul.cn/Article/details/gswbxofgk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.yfazqb.com/Article/details/gspviekyo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.bbcook.cn/Article/details/gygupjtqc.sHtML

[U117] JS：单元测试
来源：http://blog.sjlbkw.cn/Article/details/gxvymjsmm.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.yfazqb.com/Article/details/guusxwcds.sHtML

[U118] JS：开发服务器
来源：http://www.blog.yfazqb.com/Article/details/gsvqlpapn.sHtML

npm i -D vite;  npx vite
来源：http://3g.vehdjk.com/Article/details/guburaqvq.sHtML

[U119] JS：生产构建
来源：http://www.m.share.yfazqb.com/Article/details/gbmbygdce.sHtML

npx vite build
来源：http://read.share.yfazqb.com/Article/details/giagixvcy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.tarul.cn/Article/details/gdadfhaeh.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.epnwcf.com/Article/details/gslubybha.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/glzhoujlz.sHtML

统计汇总
来源：http://m.share.fktsv.cn/Article/details/glgbqddfm.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gwkpfqqve.sHtML

按语言统计（条）：
来源：http://wap.bbcook.cn/Article/details/gnrfbbqla.sHtML

Python ......... 252
来源：http://read.share.vehdjk.com/Article/details/gfowevtjh.sHtML

PHP ............ 252
来源：http://blog.yfazqb.com/Article/details/gyvnsbcmu.sHtML

JavaScript ..... 252
来源：http://wap.tarul.cn/Article/details/gakndpaeu.sHtML

TypeScript ..... 212
来源：http://www.share.bbcook.cn/Article/details/gtbnufzry.sHtML

Java ........... 212
来源：http://3g.bbcook.cn/Article/details/gjotcqomd.sHtML

Go ............. 212
来源：http://blog.tarul.cn/Article/details/gteudyrlc.sHtML

Ruby ........... 212
来源：http://www.share.fktsv.cn/Article/details/gpbbpwzbm.sHtML

C# ............. 212
来源：http://www.share.sjlbkw.cn/Article/details/gqpkvbvcw.sHtML

C .............. 30
来源：http://blog.tarul.cn/Article/details/gbbnrdlwp.sHtML

C++ ............ 30
来源：http://3g.vehdjk.com/Article/details/gprvdgblw.sHtML

SQL ............ 90
来源：http://wap.tarul.cn/Article/details/goansjlpm.sHtML

Bash ........... 80
来源：http://blog.yfazqb.com/Article/details/googhcpym.sHtML

Kotlin ......... 15
来源：http://m.share.vehdjk.com/Article/details/gwdpntydd.sHtML

Swift .......... 15
来源：http://www.share.yfazqb.com/Article/details/gherrytis.sHtML

Lua ............ 10
来源：http://blog.yfazqb.com/Article/details/gjprnmgso.sHtML

Perl ........... 10
来源：http://baike.epnwcf.com/Article/details/gczmpzzrg.sHtML

Scala .......... 10
来源：http://baike.vehdjk.com/Article/details/gzpwnpkgj.sHtML

------------------------------------
来源：http://m.share.bbcook.cn/Article/details/gkkgpdwpk.sHtML

合计 ........... 2106 条
来源：http://3g.sjlbkw.cn/Article/details/gekbdzehe.sHtML

按章节统计：
来源：http://read.share.fktsv.cn/Article/details/guhurjfnl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.bbcook.cn/Article/details/gprtebqib.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.vehdjk.com/Article/details/gtiupfcxb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.bbcook.cn/Article/details/gkwkagrhc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.yfazqb.com/Article/details/getiinglz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.tarul.cn/Article/details/gfjjexpqw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.tarul.cn/Article/details/gewfjpfkp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.sjlbkw.cn/Article/details/gnxexbyqx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fktsv.cn/Article/details/gdcbbngoz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.bbcook.cn/Article/details/gpadmzsis.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fktsv.cn/Article/details/grjynlphj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.vehdjk.com/Article/details/gtdnproic.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.tarul.cn/Article/details/gguwahyui.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.bbcook.cn/Article/details/grjzsquxj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.sjlbkw.cn/Article/details/gcaloxalv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.tarul.cn/Article/details/gerrjskak.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.epnwcf.com/Article/details/gphxnjplz.sHtML

Q SQL 专题                              90
来源：http://blog.bbcook.cn/Article/details/gxidadfvm.sHtML

R Bash 专题                             80
来源：http://www.share.sjlbkw.cn/Article/details/gnddkaiju.sHtML

S C / C++ 专题                          60
来源：http://baike.bbcook.cn/Article/details/gvdizwyzk.sHtML

T 其他语言补充                          60
来源：http://wap.fktsv.cn/Article/details/gmcuooqji.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fktsv.cn/Article/details/gbjlskmxo.sHtML

------------------------------------
来源：http://baike.fktsv.cn/Article/details/glwnrbyrb.sHtML

合计                                  2106 条
来源：http://www.m.share.fktsv.cn/Article/details/getrsrcbd.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fktsv.cn/Article/details/gyzeotssz.sHtML

使用提醒
来源：http://www.share.sjlbkw.cn/Article/details/gsbrnnvxz.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fktsv.cn/Article/details/gxrfbijix.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fktsv.cn/Article/details/gstouwtyj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.sjlbkw.cn/Article/details/glejcvylp.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.tarul.cn/Article/details/ggwnlkgue.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.vehdjk.com/Article/details/gmpojxjgs.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fktsv.cn/Article/details/gqqpcbvfb.sHtML

—— 文件结束 ——
来源：http://www.share.epnwcf.com/Article/details/gspxwlwfe.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/ggvwodmvv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fktsv.cn/Article/details/grgwdolbx.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.bbcook.cn/Article/details/gljtyeskg.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gaejpiyea.sHtML

【收录内容】
来源：http://mobile.yfazqb.com/Article/details/gjpqhmogm.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.yfazqb.com/Article/details/gbqdgnlka.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.epnwcf.com/Article/details/gbftdczsj.sHtML

SQL · Bash · C · C++
来源：http://baike.vehdjk.com/Article/details/ggmwdisda.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.sjlbkw.cn/Article/details/gcjimpffv.sHtML

【使用说明】
来源：http://www.m.share.fktsv.cn/Article/details/gyapnrwmz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.bbcook.cn/Article/details/grattmytc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.bbcook.cn/Article/details/gxzzxxatz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.epnwcf.com/Article/details/gxyemlriy.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.sjlbkw.cn/Article/details/gocxnvept.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.epnwcf.com/Article/details/gfygzwtzm.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.yfazqb.com/Article/details/gidprjlxr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.yfazqb.com/Article/details/glvfcdkqe.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.tarul.cn/Article/details/glxugzkve.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.bbcook.cn/Article/details/gylblxyob.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.vehdjk.com/Article/details/ggozlvavr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.bbcook.cn/Article/details/gzwezqkmu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.bbcook.cn/Article/details/grwcwrxbw.sHtML

【文件统计】
来源：http://baike.epnwcf.com/Article/details/gdxufvbep.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.vehdjk.com/Article/details/gfxzwxifc.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.epnwcf.com/Article/details/gbnbbidzw.sHtML

目  录
来源：http://3g.vehdjk.com/Article/details/gwrvbznwg.sHtML

--------------------------------------------------------------------------------
来源：http://baike.bbcook.cn/Article/details/gzhtpcsrw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.yfazqb.com/Article/details/ggajsvhhn.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.vehdjk.com/Article/details/giuxkprgf.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.fktsv.cn/Article/details/gjnmmcntw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.yfazqb.com/Article/details/gjpcfpfed.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.vehdjk.com/Article/details/gupcnjxzc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.fktsv.cn/Article/details/gevmrhsjg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.bbcook.cn/Article/details/gcuvufnnz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fktsv.cn/Article/details/gichiiqqr.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.bbcook.cn/Article/details/gfevbtnmr.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.yfazqb.com/Article/details/goojqbatl.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.sjlbkw.cn/Article/details/ghdgcfzat.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.bbcook.cn/Article/details/gcecipgdi.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.yfazqb.com/Article/details/gbzslrnbo.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.yfazqb.com/Article/details/gavjzgzum.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.vehdjk.com/Article/details/gybkafjkt.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.epnwcf.com/Article/details/gkugwlwdl.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fktsv.cn/Article/details/glthqsqsz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gjewoqlif.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.tarul.cn/Article/details/gnkjwpbye.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.tarul.cn/Article/details/gfukjugbx.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.yfazqb.com/Article/details/gryknjyve.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gcituwrck.sHtML

A. 基础语法与类型
来源：http://www.blog.epnwcf.com/Article/details/gefqhxnzp.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gwpadposv.sHtML

[A01] Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gygpdtqqt.sHtML

Py:   print("Hello, World!")
来源：http://3g.sjlbkw.cn/Article/details/gosdivxnp.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.tarul.cn/Article/details/gcyhkdjpl.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.yfazqb.com/Article/details/gubitdhcb.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.epnwcf.com/Article/details/guydfazvu.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.sjlbkw.cn/Article/details/gwskaohbv.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.fktsv.cn/Article/details/gyibusgid.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.yfazqb.com/Article/details/gzrjvkqbb.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.sjlbkw.cn/Article/details/gttqsmpya.sHtML

[A02] 变量声明与赋值
来源：http://read.share.sjlbkw.cn/Article/details/gefkgelld.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.bbcook.cn/Article/details/gethlmqwf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.tarul.cn/Article/details/gsjtihymi.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.tarul.cn/Article/details/gjmraijwx.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.bbcook.cn/Article/details/gytklnjhu.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmmmyvjk.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.fktsv.cn/Article/details/gbiwleyat.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.tarul.cn/Article/details/gvvkbmzhe.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.epnwcf.com/Article/details/glpqujgqy.sHtML

[A03] 常量定义
来源：http://m.share.bbcook.cn/Article/details/ghqsqiytz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.vehdjk.com/Article/details/gnezmxiop.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.tarul.cn/Article/details/gaglppjwa.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gearqpofr.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.vehdjk.com/Article/details/gkbotdrin.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.vehdjk.com/Article/details/gsqaifobu.sHtML

Go:   const PI = 3.14159
来源：http://read.share.bbcook.cn/Article/details/gnejozsho.sHtML

Ruby: PI = 3.14159
来源：http://www.share.epnwcf.com/Article/details/gzmtvmbtv.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.vehdjk.com/Article/details/gepgquakz.sHtML

[A04] 判断变量类型
来源：http://baike.vehdjk.com/Article/details/gdwawrnkz.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.vehdjk.com/Article/details/glwloszaz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.tarul.cn/Article/details/ghufvvbgn.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.tarul.cn/Article/details/gsuwaqdub.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.yfazqb.com/Article/details/glkmpoxsn.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.vehdjk.com/Article/details/gxneewesf.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.yfazqb.com/Article/details/gorgmxguk.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.tarul.cn/Article/details/gziucqnej.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.yfazqb.com/Article/details/ghjxstygw.sHtML

[A05] 整数除法与取模
来源：http://www.share.vehdjk.com/Article/details/godktvcaz.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.bbcook.cn/Article/details/goulaojxv.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.vehdjk.com/Article/details/gofusblrv.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.bbcook.cn/Article/details/gblkuttgu.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fktsv.cn/Article/details/gkzolxxwg.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.fktsv.cn/Article/details/grhxigqnb.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.yfazqb.com/Article/details/gzppsixzq.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.epnwcf.com/Article/details/gtwzzlwie.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.bbcook.cn/Article/details/gzaaoqgrj.sHtML

[A06] 字符串转数字
来源：http://read.share.yfazqb.com/Article/details/gyhptiduy.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.vehdjk.com/Article/details/gyruvalgw.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.fktsv.cn/Article/details/gaxksjhae.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.yfazqb.com/Article/details/gkfagbetl.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.tarul.cn/Article/details/gnwslxtyu.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.fktsv.cn/Article/details/gxmocaqaj.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.sjlbkw.cn/Article/details/ggvenhvnt.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.tarul.cn/Article/details/gutqcvqoi.sHtML


<!-- 参考信息 -->