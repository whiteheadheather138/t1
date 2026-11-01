代发 wailian999

[U53] PHP：空合并运算符
来源：http://read.share.sjlbkw.cn/Article/details/geecvrotk.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.tarul.cn/Article/details/gunhyfnif.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fktsv.cn/Article/details/gjoklkrjm.sHtML

$obj?->method()
来源：http://blog.bbcook.cn/Article/details/gorieaahb.sHtML

[U55] PHP：match 表达式
来源：http://www.share.bbcook.cn/Article/details/gxuerferc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.yfazqb.com/Article/details/gxclftozd.sHtML

[U56] PHP：命名参数
来源：http://blog.sjlbkw.cn/Article/details/gsrtkzpey.sHtML

f(a: 1, b: 2)
来源：http://3g.yfazqb.com/Article/details/gzkfzsypu.sHtML

[U57] PHP：字符串插值
来源：http://read.share.sjlbkw.cn/Article/details/gqjqrfroy.sHtML

"值: {$a}"
来源：http://baike.tarul.cn/Article/details/gitwpqxlt.sHtML

[U58] PHP：数组三件套
来源：http://read.share.yfazqb.com/Article/details/gvbofgesz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.epnwcf.com/Article/details/gtyjuiogc.sHtML

[U59] PHP：自定义排序
来源：http://m.share.bbcook.cn/Article/details/gganotkdm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.epnwcf.com/Article/details/gxoyokfrh.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fktsv.cn/Article/details/geqwrvuaz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.sjlbkw.cn/Article/details/gwmzktwxg.sHtML

[U61] PHP：正则
来源：http://www.share.vehdjk.com/Article/details/gkqixjivm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.bbcook.cn/Article/details/gmiubzzfj.sHtML

[U62] PHP：日期对象
来源：http://read.share.yfazqb.com/Article/details/gidqbpogz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fktsv.cn/Article/details/gyianwjzr.sHtML

[U63] PHP：文件读写
来源：http://3g.bbcook.cn/Article/details/gegrjgwjz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.yfazqb.com/Article/details/gkqlfnahs.sHtML

[U64] PHP：目录遍历
来源：http://read.share.epnwcf.com/Article/details/gfwugomxx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.vehdjk.com/Article/details/gytvoayii.sHtML

[U65] PHP：会话
来源：http://mobile.vehdjk.com/Article/details/gmdfstbvb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.vehdjk.com/Article/details/gvqfwoest.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fktsv.cn/Article/details/gbaravfws.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.vehdjk.com/Article/details/gehohlhad.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.vehdjk.com/Article/details/gnlpxgugw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fktsv.cn/Article/details/gvotljkgp.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.vehdjk.com/Article/details/ggkethkmo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.bbcook.cn/Article/details/gptowzcfz.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.epnwcf.com/Article/details/grtwmkbfv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fktsv.cn/Article/details/gqybedidk.sHtML

[U70] PHP：PDO 事务
来源：http://3g.yfazqb.com/Article/details/gwthglyvj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.sjlbkw.cn/Article/details/gohrljdiz.sHtML

[U71] PHP：抛出异常
来源：http://mobile.tarul.cn/Article/details/getxiuayy.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.yfazqb.com/Article/details/gvdyrljsn.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.yfazqb.com/Article/details/gvsisohea.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.epnwcf.com/Article/details/gkapmvxwj.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.sjlbkw.cn/Article/details/goolhrvqw.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.bbcook.cn/Article/details/gvpzveppg.sHtML

[U74] PHP：读取环境变量
来源：http://blog.epnwcf.com/Article/details/gwoeruycs.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.epnwcf.com/Article/details/gzfjnnjpr.sHtML

[U75] PHP：依赖注入
来源：http://baike.bbcook.cn/Article/details/givgeysue.sHtML

composer require psr/container
来源：http://3g.fktsv.cn/Article/details/gresjpqca.sHtML

[U76] PHP：简单路由
来源：http://read.share.sjlbkw.cn/Article/details/ghqstxbga.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fktsv.cn/Article/details/gwfqtvobz.sHtML

[U77] PHP：模板渲染
来源：http://read.share.bbcook.cn/Article/details/gdqwmbwlh.sHtML

composer require twig/twig
来源：http://mobile.bbcook.cn/Article/details/gnnawsnfn.sHtML

[U78] PHP：单元测试
来源：http://baike.fktsv.cn/Article/details/gciiqyxio.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.sjlbkw.cn/Article/details/gpidpwxbr.sHtML

[U79] PHP：静态分析
来源：http://read.share.yfazqb.com/Article/details/gamnteckg.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.tarul.cn/Article/details/gkpusbxlu.sHtML

[U80] PHP：代码规范修复
来源：http://3g.tarul.cn/Article/details/gpvbfvyfj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.vehdjk.com/Article/details/gfkocbkss.sHtML

[U81] JS：初始化项目
来源：http://www.share.bbcook.cn/Article/details/giuwixxsa.sHtML

npm init -y;  npm i express
来源：http://www.blog.tarul.cn/Article/details/gdkyvsias.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.vehdjk.com/Article/details/gjhqxsulb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.bbcook.cn/Article/details/ghtqplivv.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fktsv.cn/Article/details/georcqlmm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.bbcook.cn/Article/details/gsechfked.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fktsv.cn/Article/details/gtfincxki.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fktsv.cn/Article/details/grivxjyeh.sHtML

[U85] JS：可选链
来源：http://3g.tarul.cn/Article/details/gxvntiofr.sHtML

a?.b?.c
来源：http://mobile.bbcook.cn/Article/details/gqdpeunpi.sHtML

[U86] JS：空值合并
来源：http://blog.bbcook.cn/Article/details/gblsrzymk.sHtML

a ?? b
来源：http://mobile.yfazqb.com/Article/details/gujyuscnd.sHtML

[U87] JS：解构默认值
来源：http://3g.bbcook.cn/Article/details/gysrqxotd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.sjlbkw.cn/Article/details/gskfftbez.sHtML

[U88] JS：对象展开合并
来源：http://blog.tarul.cn/Article/details/gcokwcecf.sHtML

{ ...a, ...b }
来源：http://www.m.share.yfazqb.com/Article/details/gmrmtnpfj.sHtML

[U89] JS：数组去重
来源：http://read.share.fktsv.cn/Article/details/gitnvfvjk.sHtML

[...new Set(arr)]
来源：http://baike.epnwcf.com/Article/details/gxsugdpkf.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.vehdjk.com/Article/details/gvvprsbkf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.yfazqb.com/Article/details/grukuzyff.sHtML

[U91] JS：对象键值遍历
来源：http://3g.sjlbkw.cn/Article/details/gikwvmorm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fktsv.cn/Article/details/gejxlmjxt.sHtML

[U92] JS：深拷贝
来源：http://baike.tarul.cn/Article/details/ggvrejedk.sHtML

structuredClone(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gfngphabm.sHtML

[U93] JS：模板字符串
来源：http://www.blog.yfazqb.com/Article/details/geabnxecj.sHtML

`共 ${n} 条`
来源：http://www.share.yfazqb.com/Article/details/gtlgpqxif.sHtML

[U94] JS：箭头函数
来源：http://mobile.fktsv.cn/Article/details/gwtqvjpgl.sHtML

const double = x => x * 2;
来源：http://baike.fktsv.cn/Article/details/gtdzczxqb.sHtML

[U95] JS：Promise 包装
来源：http://read.share.epnwcf.com/Article/details/gigarbcqt.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fktsv.cn/Article/details/gmhtsqgrl.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.sjlbkw.cn/Article/details/gcxspbohx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.epnwcf.com/Article/details/gncbnhkjl.sHtML

[U97] JS：并发请求
来源：http://www.blog.yfazqb.com/Article/details/gjinumwfj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.bbcook.cn/Article/details/gxfyjrqlt.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.bbcook.cn/Article/details/gioakzhmi.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.tarul.cn/Article/details/gnmcdqhlz.sHtML

[U99] JS：事件监听
来源：http://wap.vehdjk.com/Article/details/gahjxatxi.sHtML

el.addEventListener("click", e => {})
来源：http://blog.vehdjk.com/Article/details/gfdlfiowf.sHtML

[U100] JS：DOM 查询
来源：http://read.share.epnwcf.com/Article/details/grcvfosdc.sHtML

document.querySelector(".item")
来源：http://baike.fktsv.cn/Article/details/gzrxqomqa.sHtML

[U101] JS：classList 操作
来源：http://www.blog.yfazqb.com/Article/details/gkzsktref.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fktsv.cn/Article/details/golijqxuq.sHtML

[U102] JS：本地存储
来源：http://baike.bbcook.cn/Article/details/gpoqkppmv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.bbcook.cn/Article/details/gbjqkfvkq.sHtML

[U103] JS：定时器
来源：http://m.share.fktsv.cn/Article/details/gasmyeqph.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.epnwcf.com/Article/details/gynbmfltq.sHtML

[U104] JS：防抖
来源：http://baike.bbcook.cn/Article/details/gslzvjjgh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.vehdjk.com/Article/details/gfinhkwzh.sHtML

[U105] JS：节流
来源：http://wap.epnwcf.com/Article/details/gbupstckp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.vehdjk.com/Article/details/gdgvadgqc.sHtML

[U106] JS：日期格式化
来源：http://mobile.fktsv.cn/Article/details/gqmyurpom.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fktsv.cn/Article/details/gykmwoewd.sHtML

[U107] JS：数字千分位
来源：http://m.share.fktsv.cn/Article/details/gpsjpbfdp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.bbcook.cn/Article/details/gyeetwkmf.sHtML

[U108] JS：随机整数
来源：http://www.share.yfazqb.com/Article/details/gbelvblgo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.yfazqb.com/Article/details/giahfczhv.sHtML

[U109] JS：数组分组
来源：http://www.blog.epnwcf.com/Article/details/guvldfmog.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.tarul.cn/Article/details/gasnhdjnz.sHtML

[U110] JS：数组分块
来源：http://blog.sjlbkw.cn/Article/details/ggalrvzse.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.epnwcf.com/Article/details/ghqsurxbg.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fktsv.cn/Article/details/gfnqyticc.sHtML

new Map(Object.entries(obj))
来源：http://wap.epnwcf.com/Article/details/gbjmnnymh.sHtML

[U112] JS：字符串补位
来源：http://mobile.vehdjk.com/Article/details/gyhgjvbyy.sHtML

"7".padStart(3, "0")
来源：http://blog.fktsv.cn/Article/details/grubmtdid.sHtML

[U113] JS：正则替换全部
来源：http://mobile.sjlbkw.cn/Article/details/gawmassvh.sHtML

s.replaceAll("a", "b")
来源：http://www.share.tarul.cn/Article/details/gtgfgfsww.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.bbcook.cn/Article/details/gxoutpket.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.tarul.cn/Article/details/gvgyhchzm.sHtML

[U115] JS：生成 UUID
来源：http://blog.yfazqb.com/Article/details/gmppomdpm.sHtML

crypto.randomUUID()
来源：http://www.blog.epnwcf.com/Article/details/gboxrcjob.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fktsv.cn/Article/details/gapxzfnjz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.vehdjk.com/Article/details/gblhndaaz.sHtML

[U117] JS：单元测试
来源：http://www.m.share.vehdjk.com/Article/details/gocjakqvq.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.epnwcf.com/Article/details/gjvmtghrs.sHtML

[U118] JS：开发服务器
来源：http://mobile.bbcook.cn/Article/details/gftxuvpca.sHtML

npm i -D vite;  npx vite
来源：http://read.share.yfazqb.com/Article/details/gufygruha.sHtML

[U119] JS：生产构建
来源：http://3g.fktsv.cn/Article/details/gztgunnsg.sHtML

npx vite build
来源：http://read.share.yfazqb.com/Article/details/gsjerirmt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.epnwcf.com/Article/details/gkriqseih.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.tarul.cn/Article/details/gclevehah.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gciguhkbt.sHtML

统计汇总
来源：http://3g.epnwcf.com/Article/details/gohenkwlh.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gqxhufxkm.sHtML

按语言统计（条）：
来源：http://3g.yfazqb.com/Article/details/gjfenbkrj.sHtML

Python ......... 252
来源：http://read.share.sjlbkw.cn/Article/details/gfdcwmgef.sHtML

PHP ............ 252
来源：http://www.share.tarul.cn/Article/details/gdexbeshk.sHtML

JavaScript ..... 252
来源：http://mobile.sjlbkw.cn/Article/details/glqvmlajr.sHtML

TypeScript ..... 212
来源：http://www.share.vehdjk.com/Article/details/gwoatierk.sHtML

Java ........... 212
来源：http://www.blog.bbcook.cn/Article/details/gbexzbzyz.sHtML

Go ............. 212
来源：http://www.m.share.vehdjk.com/Article/details/gjklopmyy.sHtML

Ruby ........... 212
来源：http://mobile.sjlbkw.cn/Article/details/gegrfnmai.sHtML

C# ............. 212
来源：http://mobile.tarul.cn/Article/details/gurchqexu.sHtML

C .............. 30
来源：http://www.blog.tarul.cn/Article/details/gyljzyikq.sHtML

C++ ............ 30
来源：http://baike.vehdjk.com/Article/details/gfuzzdjoc.sHtML

SQL ............ 90
来源：http://wap.yfazqb.com/Article/details/gytubphia.sHtML

Bash ........... 80
来源：http://read.share.epnwcf.com/Article/details/gpyuedvtn.sHtML

Kotlin ......... 15
来源：http://www.share.fktsv.cn/Article/details/gkxauipeg.sHtML

Swift .......... 15
来源：http://wap.vehdjk.com/Article/details/ggsxjmupm.sHtML

Lua ............ 10
来源：http://mobile.tarul.cn/Article/details/gjwznbclo.sHtML

Perl ........... 10
来源：http://wap.yfazqb.com/Article/details/gyngqvqsx.sHtML

Scala .......... 10
来源：http://blog.tarul.cn/Article/details/gqvzwfeaf.sHtML

------------------------------------
来源：http://wap.sjlbkw.cn/Article/details/gkpjxlckw.sHtML

合计 ........... 2106 条
来源：http://www.blog.yfazqb.com/Article/details/gwxgewtdn.sHtML

按章节统计：
来源：http://wap.fktsv.cn/Article/details/gynjtdluu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.epnwcf.com/Article/details/genvfnlip.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.sjlbkw.cn/Article/details/gfkavcgcf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.vehdjk.com/Article/details/gifhyktnl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.yfazqb.com/Article/details/ggfydwwgo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fktsv.cn/Article/details/gueggxcfo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.sjlbkw.cn/Article/details/gtheiiovy.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.sjlbkw.cn/Article/details/gpueoubip.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.vehdjk.com/Article/details/gtovxgbdj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.tarul.cn/Article/details/gdhewvbou.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.yfazqb.com/Article/details/gzseiiaam.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/gzztxndew.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.yfazqb.com/Article/details/gekwbgeuj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.sjlbkw.cn/Article/details/goqjmqbts.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.epnwcf.com/Article/details/gmgpqxylc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.tarul.cn/Article/details/gbotuvjvv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fktsv.cn/Article/details/gkccrwnxw.sHtML

Q SQL 专题                              90
来源：http://baike.tarul.cn/Article/details/glagheyji.sHtML

R Bash 专题                             80
来源：http://www.blog.vehdjk.com/Article/details/gsvcwqyzd.sHtML

S C / C++ 专题                          60
来源：http://wap.yfazqb.com/Article/details/gzyffsede.sHtML

T 其他语言补充                          60
来源：http://3g.sjlbkw.cn/Article/details/gkhhjljym.sHtML

U 高频实用片段                         120
来源：http://baike.yfazqb.com/Article/details/gozhsrebx.sHtML

------------------------------------
来源：http://blog.yfazqb.com/Article/details/gxiwiadjx.sHtML

合计                                  2106 条
来源：http://wap.vehdjk.com/Article/details/glacgrtat.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.bbcook.cn/Article/details/gmtupyezu.sHtML

使用提醒
来源：http://www.m.share.sjlbkw.cn/Article/details/gtobxsnvy.sHtML

--------------------------------------------------------------------------------
来源：http://3g.epnwcf.com/Article/details/gncnwpbgz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.yfazqb.com/Article/details/grritwxqc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.yfazqb.com/Article/details/gculaqjgh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.bbcook.cn/Article/details/gqtnvmati.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.epnwcf.com/Article/details/ggritmpmp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fktsv.cn/Article/details/gcaqdbizj.sHtML

—— 文件结束 ——
来源：http://blog.epnwcf.com/Article/details/godybdnlp.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/ggrccgivf.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.sjlbkw.cn/Article/details/gkzzfvaqf.sHtML

Common Programming Examples Cheat Book
来源：http://3g.bbcook.cn/Article/details/gyjkitnsv.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gpvasgnvn.sHtML

【收录内容】
来源：http://www.share.tarul.cn/Article/details/gsquxdtse.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.vehdjk.com/Article/details/gghtfcsbc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.bbcook.cn/Article/details/gtcfhaypu.sHtML

SQL · Bash · C · C++
来源：http://m.share.sjlbkw.cn/Article/details/ghdgxwwfs.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.epnwcf.com/Article/details/gkpygesnr.sHtML

【使用说明】
来源：http://m.share.sjlbkw.cn/Article/details/glykvsfnl.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.bbcook.cn/Article/details/gtrpatcge.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.epnwcf.com/Article/details/gmhiiunfx.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.yfazqb.com/Article/details/gjoqoiikw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fktsv.cn/Article/details/gdyglnxgf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.epnwcf.com/Article/details/gngrakuwn.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.vehdjk.com/Article/details/gnrecypfl.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fktsv.cn/Article/details/gllsalxsi.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fktsv.cn/Article/details/gqftrdppe.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fktsv.cn/Article/details/gebgdqnte.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.yfazqb.com/Article/details/gdsrmwuta.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.yfazqb.com/Article/details/gmrgcmwtu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.epnwcf.com/Article/details/gfmksuhdh.sHtML

【文件统计】
来源：http://baike.bbcook.cn/Article/details/gbvnabfmr.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.fktsv.cn/Article/details/gbbttyenq.sHtML

--------------------------------------------------------------------------------
来源：http://wap.vehdjk.com/Article/details/gjgqsmayw.sHtML

目  录
来源：http://baike.vehdjk.com/Article/details/ghdbkivsq.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fktsv.cn/Article/details/gvfxaqnbf.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.sjlbkw.cn/Article/details/glknqoqau.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fktsv.cn/Article/details/gjqsiirfo.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.tarul.cn/Article/details/gjtrmfyoz.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.yfazqb.com/Article/details/gnigucxob.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.epnwcf.com/Article/details/ghcxyjfyx.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.yfazqb.com/Article/details/gvonajqbo.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.yfazqb.com/Article/details/grqcelahr.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.tarul.cn/Article/details/gyozzelhz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.tarul.cn/Article/details/gmkcljgln.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.tarul.cn/Article/details/gsaxapdwh.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.tarul.cn/Article/details/gaszivsnu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.bbcook.cn/Article/details/gucitkuvg.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.bbcook.cn/Article/details/gvzxakwdx.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.bbcook.cn/Article/details/gggyhgciu.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.epnwcf.com/Article/details/gahjndvsg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.tarul.cn/Article/details/gwxqjbcvc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.yfazqb.com/Article/details/gqqmnuudc.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/grjlyeqid.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.bbcook.cn/Article/details/gobyvqfse.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fktsv.cn/Article/details/gfzcfjkkq.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.epnwcf.com/Article/details/gjqordxdj.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gcjhgxnmw.sHtML

A. 基础语法与类型
来源：http://blog.yfazqb.com/Article/details/ginbhazbg.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gwtgpdoqx.sHtML

[A01] Hello World
来源：http://baike.yfazqb.com/Article/details/gmbyznbpo.sHtML

Py:   print("Hello, World!")
来源：http://m.share.fktsv.cn/Article/details/gcyjkeyeh.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.bbcook.cn/Article/details/gysquvwxk.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.fktsv.cn/Article/details/gniddtbip.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.sjlbkw.cn/Article/details/gbhhbngfm.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.tarul.cn/Article/details/gifdhaoza.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.tarul.cn/Article/details/gznghavxr.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.epnwcf.com/Article/details/ghqpuflmr.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.vehdjk.com/Article/details/gnlnlohme.sHtML

[A02] 变量声明与赋值
来源：http://www.share.epnwcf.com/Article/details/ggsbkflaf.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.vehdjk.com/Article/details/gwwlwzkvk.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.sjlbkw.cn/Article/details/grbluckpr.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.epnwcf.com/Article/details/gjfmlyaqh.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.yfazqb.com/Article/details/guaxorhua.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.fktsv.cn/Article/details/gjkgfeqht.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.vehdjk.com/Article/details/glubknocr.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.sjlbkw.cn/Article/details/gdfjcuurs.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.fktsv.cn/Article/details/gufkbgovx.sHtML

[A03] 常量定义
来源：http://www.blog.tarul.cn/Article/details/guhybhgia.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.tarul.cn/Article/details/gqngulqdk.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/gammsjghc.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.fktsv.cn/Article/details/gwjaskxby.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/gosvezxdy.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.fktsv.cn/Article/details/gjphtmnmd.sHtML

Go:   const PI = 3.14159
来源：http://wap.vehdjk.com/Article/details/ggrxbzkam.sHtML

Ruby: PI = 3.14159
来源：http://blog.bbcook.cn/Article/details/gwleuxgur.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.bbcook.cn/Article/details/glrbmiyuj.sHtML

[A04] 判断变量类型
来源：http://www.m.share.yfazqb.com/Article/details/gkluodisb.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.epnwcf.com/Article/details/ggsdtqhof.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.bbcook.cn/Article/details/gyrwqcfqu.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.bbcook.cn/Article/details/gcwnnwwkn.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.bbcook.cn/Article/details/gtrivglts.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.yfazqb.com/Article/details/gwmakacgm.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.tarul.cn/Article/details/gmelzvxxv.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.sjlbkw.cn/Article/details/gpqlxisfp.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.sjlbkw.cn/Article/details/glmzlqsbb.sHtML

[A05] 整数除法与取模
来源：http://wap.epnwcf.com/Article/details/gazbetukh.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.fktsv.cn/Article/details/gnmjhhvoc.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.vehdjk.com/Article/details/gfvvsnubn.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.tarul.cn/Article/details/gzcrjeejh.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.epnwcf.com/Article/details/gjexhoscw.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.fktsv.cn/Article/details/gpnlortci.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.epnwcf.com/Article/details/gngrumaac.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.bbcook.cn/Article/details/gqxamlvaq.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.bbcook.cn/Article/details/gojpnphpg.sHtML

[A06] 字符串转数字
来源：http://blog.sjlbkw.cn/Article/details/gdftojfcj.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.vehdjk.com/Article/details/gtqatmsoz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.vehdjk.com/Article/details/gunfjcifu.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.bbcook.cn/Article/details/gojjhjgud.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.epnwcf.com/Article/details/ggzwaaztw.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.epnwcf.com/Article/details/gvxnqvrnj.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.yfazqb.com/Article/details/gdlzovcgv.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.yfazqb.com/Article/details/gzabwxebp.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.epnwcf.com/Article/details/gkgwensib.sHtML

[A07] 数字转字符串
来源：http://wap.epnwcf.com/Article/details/ggqrguwkr.sHtML

Py:   str(42)
来源：http://www.share.epnwcf.com/Article/details/goevnjdgk.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.yfazqb.com/Article/details/gufbfiwqp.sHtML


<!-- 参考信息 -->