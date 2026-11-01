代发 wailian999

[U55] PHP：match 表达式
来源：http://blog.sjlbkw.cn/Article/details/gumxgaebd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.epnwcf.com/Article/details/gcxlxalld.sHtML

[U56] PHP：命名参数
来源：http://blog.sjlbkw.cn/Article/details/gbbhtbwod.sHtML

f(a: 1, b: 2)
来源：http://read.share.tarul.cn/Article/details/gjxvgmoav.sHtML

[U57] PHP：字符串插值
来源：http://www.share.tarul.cn/Article/details/ggkrfthzs.sHtML

"值: {$a}"
来源：http://www.m.share.vehdjk.com/Article/details/gjwbohmew.sHtML

[U58] PHP：数组三件套
来源：http://m.share.sjlbkw.cn/Article/details/gzgjuhuxp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.tarul.cn/Article/details/gbsbektbp.sHtML

[U59] PHP：自定义排序
来源：http://wap.tarul.cn/Article/details/gaqbbazjl.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.epnwcf.com/Article/details/gokrynsjc.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.sjlbkw.cn/Article/details/gprnkeoby.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.yfazqb.com/Article/details/ghqyrgcax.sHtML

[U61] PHP：正则
来源：http://mobile.fktsv.cn/Article/details/gbkjritoe.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.vehdjk.com/Article/details/gdjonypvj.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fktsv.cn/Article/details/ghbfzuwci.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.vehdjk.com/Article/details/gsksligxt.sHtML

[U63] PHP：文件读写
来源：http://read.share.epnwcf.com/Article/details/gqxgrtqid.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.epnwcf.com/Article/details/gyyxyjbip.sHtML

[U64] PHP：目录遍历
来源：http://blog.bbcook.cn/Article/details/gpmvizdtj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.sjlbkw.cn/Article/details/gnivkxaml.sHtML

[U65] PHP：会话
来源：http://mobile.vehdjk.com/Article/details/gznpbtorx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fktsv.cn/Article/details/gcyvzyjit.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.epnwcf.com/Article/details/gzsrsswac.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.sjlbkw.cn/Article/details/gtunzirir.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fktsv.cn/Article/details/goiqzzshw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fktsv.cn/Article/details/gktksunwe.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fktsv.cn/Article/details/gkezukfwc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.sjlbkw.cn/Article/details/gsvodnbtg.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.bbcook.cn/Article/details/gryjglhmk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.yfazqb.com/Article/details/gmvnxgxld.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.tarul.cn/Article/details/gtsbahsou.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.tarul.cn/Article/details/gyzahotis.sHtML

[U71] PHP：抛出异常
来源：http://wap.yfazqb.com/Article/details/grauutidb.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.sjlbkw.cn/Article/details/gexcchhfo.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.vehdjk.com/Article/details/gnfdeidkf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fktsv.cn/Article/details/glkyzqjed.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.epnwcf.com/Article/details/gsjdmnogf.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.vehdjk.com/Article/details/gzqqpvqqp.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fktsv.cn/Article/details/glmbkkezm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.sjlbkw.cn/Article/details/gjwueciuz.sHtML

[U75] PHP：依赖注入
来源：http://www.share.vehdjk.com/Article/details/gjruadfhf.sHtML

composer require psr/container
来源：http://blog.vehdjk.com/Article/details/gqtuynkvg.sHtML

[U76] PHP：简单路由
来源：http://mobile.epnwcf.com/Article/details/guxkuurav.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fktsv.cn/Article/details/gmqusdpmj.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.epnwcf.com/Article/details/gsjugcuag.sHtML

composer require twig/twig
来源：http://www.blog.tarul.cn/Article/details/grqkdgdyu.sHtML

[U78] PHP：单元测试
来源：http://blog.bbcook.cn/Article/details/gbqrtqwfk.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.vehdjk.com/Article/details/gfagflijn.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fktsv.cn/Article/details/gdeackqah.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.vehdjk.com/Article/details/gtwmbhwcg.sHtML

[U80] PHP：代码规范修复
来源：http://wap.vehdjk.com/Article/details/gnlnqvspu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fktsv.cn/Article/details/gdhyhndul.sHtML

[U81] JS：初始化项目
来源：http://m.share.vehdjk.com/Article/details/gqiovfzqs.sHtML

npm init -y;  npm i express
来源：http://read.share.epnwcf.com/Article/details/gpoupgyoo.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.yfazqb.com/Article/details/gpwdibope.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.sjlbkw.cn/Article/details/gyrbuewbb.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.sjlbkw.cn/Article/details/geiepxkbl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.vehdjk.com/Article/details/gqmfkzzww.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.epnwcf.com/Article/details/guwcyfsog.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fktsv.cn/Article/details/gcrgrifok.sHtML

[U85] JS：可选链
来源：http://www.m.share.fktsv.cn/Article/details/gzoadjadr.sHtML

a?.b?.c
来源：http://wap.epnwcf.com/Article/details/gpndrzdjn.sHtML

[U86] JS：空值合并
来源：http://3g.tarul.cn/Article/details/gilhwgpai.sHtML

a ?? b
来源：http://wap.yfazqb.com/Article/details/gjevgzxxi.sHtML

[U87] JS：解构默认值
来源：http://wap.fktsv.cn/Article/details/gyfhyzhpm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.yfazqb.com/Article/details/gwluldxin.sHtML

[U88] JS：对象展开合并
来源：http://m.share.tarul.cn/Article/details/gyssdfksy.sHtML

{ ...a, ...b }
来源：http://www.share.fktsv.cn/Article/details/gxhcdwgcq.sHtML

[U89] JS：数组去重
来源：http://www.m.share.tarul.cn/Article/details/gtazyzhhm.sHtML

[...new Set(arr)]
来源：http://3g.fktsv.cn/Article/details/gvjelcncl.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.bbcook.cn/Article/details/ggprccfyi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.epnwcf.com/Article/details/ggsxqkugf.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fktsv.cn/Article/details/gvjbqacig.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.sjlbkw.cn/Article/details/grnavfigg.sHtML

[U92] JS：深拷贝
来源：http://blog.yfazqb.com/Article/details/giesnxpqu.sHtML

structuredClone(obj)
来源：http://m.share.tarul.cn/Article/details/gvkbivpfb.sHtML

[U93] JS：模板字符串
来源：http://mobile.sjlbkw.cn/Article/details/ggijugvqf.sHtML

`共 ${n} 条`
来源：http://blog.yfazqb.com/Article/details/gijchspzr.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fktsv.cn/Article/details/gyndysivc.sHtML

const double = x => x * 2;
来源：http://3g.fktsv.cn/Article/details/gwstclzey.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.sjlbkw.cn/Article/details/grasrfmto.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.tarul.cn/Article/details/glefjfsdu.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.bbcook.cn/Article/details/gljpiscyc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.epnwcf.com/Article/details/gmjhgswfp.sHtML

[U97] JS：并发请求
来源：http://www.blog.yfazqb.com/Article/details/gzpqrawzn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.epnwcf.com/Article/details/gnrxncvne.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.bbcook.cn/Article/details/ghzfcvkwn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.bbcook.cn/Article/details/geyoxjtiy.sHtML

[U99] JS：事件监听
来源：http://www.m.share.epnwcf.com/Article/details/gdodngrlv.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.vehdjk.com/Article/details/gxlyedgar.sHtML

[U100] JS：DOM 查询
来源：http://wap.fktsv.cn/Article/details/gtfuqirwu.sHtML

document.querySelector(".item")
来源：http://blog.sjlbkw.cn/Article/details/gvnkxqyuy.sHtML

[U101] JS：classList 操作
来源：http://wap.vehdjk.com/Article/details/gjchvobek.sHtML

el.classList.toggle("active")
来源：http://blog.tarul.cn/Article/details/gjpafxydb.sHtML

[U102] JS：本地存储
来源：http://mobile.sjlbkw.cn/Article/details/ghynienyt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.vehdjk.com/Article/details/gosbydymw.sHtML

[U103] JS：定时器
来源：http://mobile.sjlbkw.cn/Article/details/gbjfzjkkd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.tarul.cn/Article/details/glapbtfqu.sHtML

[U104] JS：防抖
来源：http://www.m.share.fktsv.cn/Article/details/gknwlyyvo.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.vehdjk.com/Article/details/gkkhgpfeu.sHtML

[U105] JS：节流
来源：http://read.share.fktsv.cn/Article/details/gujsvtruv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.epnwcf.com/Article/details/ganppzqrr.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.bbcook.cn/Article/details/girrxzell.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.vehdjk.com/Article/details/gntfejatx.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqpywbzl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.epnwcf.com/Article/details/ggvupnslk.sHtML

[U108] JS：随机整数
来源：http://m.share.bbcook.cn/Article/details/gvhdikfwt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.vehdjk.com/Article/details/glewynbep.sHtML

[U109] JS：数组分组
来源：http://read.share.sjlbkw.cn/Article/details/gtmhszzak.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.yfazqb.com/Article/details/gkyqsmijk.sHtML

[U110] JS：数组分块
来源：http://mobile.yfazqb.com/Article/details/gmlwsybjs.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.vehdjk.com/Article/details/gkevlkabt.sHtML

[U111] JS：对象转 Map
来源：http://blog.yfazqb.com/Article/details/gfwdaermu.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fktsv.cn/Article/details/gwtpjgvzj.sHtML

[U112] JS：字符串补位
来源：http://wap.tarul.cn/Article/details/grjpunamg.sHtML

"7".padStart(3, "0")
来源：http://wap.bbcook.cn/Article/details/grhfqnvgr.sHtML

[U113] JS：正则替换全部
来源：http://read.share.epnwcf.com/Article/details/gyawmspce.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/grlliqdim.sHtML

[U114] JS：JSON 深比较
来源：http://blog.yfazqb.com/Article/details/gecusymmh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.yfazqb.com/Article/details/gtcjecrxw.sHtML

[U115] JS：生成 UUID
来源：http://www.share.vehdjk.com/Article/details/gciumqblm.sHtML

crypto.randomUUID()
来源：http://www.m.share.yfazqb.com/Article/details/ggljfnxyv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.vehdjk.com/Article/details/ghznvxszb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.tarul.cn/Article/details/gkbhcnstr.sHtML

[U117] JS：单元测试
来源：http://www.m.share.epnwcf.com/Article/details/gfcwmowka.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.tarul.cn/Article/details/gmrouraxn.sHtML

[U118] JS：开发服务器
来源：http://3g.fktsv.cn/Article/details/gzpwozcnp.sHtML

npm i -D vite;  npx vite
来源：http://www.share.sjlbkw.cn/Article/details/gzsuhacyu.sHtML

[U119] JS：生产构建
来源：http://wap.bbcook.cn/Article/details/glzrnvcpa.sHtML

npx vite build
来源：http://baike.sjlbkw.cn/Article/details/gpvgvnojy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.sjlbkw.cn/Article/details/gstwpyzcf.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.sjlbkw.cn/Article/details/ghreeadsb.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gczpmpkcl.sHtML

统计汇总
来源：http://www.share.fktsv.cn/Article/details/gpagjqfvh.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/glhozdveh.sHtML

按语言统计（条）：
来源：http://read.share.bbcook.cn/Article/details/glyzfdvhy.sHtML

Python ......... 252
来源：http://m.share.vehdjk.com/Article/details/gyzdnddts.sHtML

PHP ............ 252
来源：http://m.share.tarul.cn/Article/details/gxdlywhdc.sHtML

JavaScript ..... 252
来源：http://mobile.yfazqb.com/Article/details/gjivbjhuz.sHtML

TypeScript ..... 212
来源：http://www.blog.bbcook.cn/Article/details/gzzcrflgc.sHtML

Java ........... 212
来源：http://3g.yfazqb.com/Article/details/gffkahceq.sHtML

Go ............. 212
来源：http://www.m.share.bbcook.cn/Article/details/gfsombcko.sHtML

Ruby ........... 212
来源：http://wap.tarul.cn/Article/details/gzwtqqzcg.sHtML

C# ............. 212
来源：http://wap.fktsv.cn/Article/details/gyxvanzzz.sHtML

C .............. 30
来源：http://wap.epnwcf.com/Article/details/gdkzbtfex.sHtML

C++ ............ 30
来源：http://www.share.fktsv.cn/Article/details/gpownhigd.sHtML

SQL ............ 90
来源：http://m.share.sjlbkw.cn/Article/details/geeugvclw.sHtML

Bash ........... 80
来源：http://www.blog.tarul.cn/Article/details/gyvxicikq.sHtML

Kotlin ......... 15
来源：http://baike.yfazqb.com/Article/details/gxnmipdyc.sHtML

Swift .......... 15
来源：http://www.blog.sjlbkw.cn/Article/details/gyjsevyna.sHtML

Lua ............ 10
来源：http://baike.epnwcf.com/Article/details/geqeyjqmr.sHtML

Perl ........... 10
来源：http://m.share.bbcook.cn/Article/details/gbkslqeww.sHtML

Scala .......... 10
来源：http://wap.yfazqb.com/Article/details/gwvxyxlrs.sHtML

------------------------------------
来源：http://baike.epnwcf.com/Article/details/gyzntuyiu.sHtML

合计 ........... 2106 条
来源：http://3g.sjlbkw.cn/Article/details/gervtpxsx.sHtML

按章节统计：
来源：http://mobile.fktsv.cn/Article/details/gzahmilvb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.sjlbkw.cn/Article/details/gmcwzmaln.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.sjlbkw.cn/Article/details/gybkbbakh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.yfazqb.com/Article/details/gkmoleazi.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.sjlbkw.cn/Article/details/gfznyugor.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.yfazqb.com/Article/details/gyabpfcum.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.epnwcf.com/Article/details/glcapbxus.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.sjlbkw.cn/Article/details/gubqufawc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.epnwcf.com/Article/details/gumqxfbfh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.vehdjk.com/Article/details/gqnbhewsv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.yfazqb.com/Article/details/gxnhzqzhz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.epnwcf.com/Article/details/gbddbfjle.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.vehdjk.com/Article/details/gzyhfrtcf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fktsv.cn/Article/details/gvnmmpecy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.sjlbkw.cn/Article/details/gfqdbnfuu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.epnwcf.com/Article/details/gvtfkbpip.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.yfazqb.com/Article/details/guletmxim.sHtML

Q SQL 专题                              90
来源：http://www.share.vehdjk.com/Article/details/glsehljga.sHtML

R Bash 专题                             80
来源：http://mobile.bbcook.cn/Article/details/geaxvflix.sHtML

S C / C++ 专题                          60
来源：http://www.share.sjlbkw.cn/Article/details/gnrvuvmdk.sHtML

T 其他语言补充                          60
来源：http://wap.vehdjk.com/Article/details/gaevjvoqk.sHtML

U 高频实用片段                         120
来源：http://www.blog.yfazqb.com/Article/details/gpyntlaxk.sHtML

------------------------------------
来源：http://read.share.sjlbkw.cn/Article/details/gmzixwnza.sHtML

合计                                  2106 条
来源：http://www.share.fktsv.cn/Article/details/gugoautnq.sHtML

--------------------------------------------------------------------------------
来源：http://wap.epnwcf.com/Article/details/gouzphxzm.sHtML

使用提醒
来源：http://baike.tarul.cn/Article/details/grasnjhju.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.sjlbkw.cn/Article/details/gosvqwlhx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.vehdjk.com/Article/details/gyoxjzmmr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.epnwcf.com/Article/details/gnzcrxysd.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.sjlbkw.cn/Article/details/guawwumre.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.epnwcf.com/Article/details/gpcftxcvp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.sjlbkw.cn/Article/details/glugrdnkt.sHtML

—— 文件结束 ——
来源：http://wap.fktsv.cn/Article/details/gbsoieyiz.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/glyvueonr.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.vehdjk.com/Article/details/ggmckgfwa.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fktsv.cn/Article/details/grrkeyjdy.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gydplbfhr.sHtML

【收录内容】
来源：http://read.share.epnwcf.com/Article/details/gzaovzlbw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.fktsv.cn/Article/details/gmbeamjab.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.epnwcf.com/Article/details/geyrprkwb.sHtML

SQL · Bash · C · C++
来源：http://blog.sjlbkw.cn/Article/details/gkpuoohon.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.bbcook.cn/Article/details/gmeybghpc.sHtML

【使用说明】
来源：http://3g.vehdjk.com/Article/details/gqycwmchx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.yfazqb.com/Article/details/gwtdgwruu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.sjlbkw.cn/Article/details/gfomvsnuf.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.bbcook.cn/Article/details/gywdjjpmz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.fktsv.cn/Article/details/gtpwcwuzf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.sjlbkw.cn/Article/details/gvcvhnwed.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.epnwcf.com/Article/details/ggwnvyeyz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.epnwcf.com/Article/details/gefzuasgr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fktsv.cn/Article/details/gaxkthltj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.yfazqb.com/Article/details/gietddnpj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.tarul.cn/Article/details/gdpybpbou.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.sjlbkw.cn/Article/details/gnsuvnuot.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.tarul.cn/Article/details/gpdhltkji.sHtML

【文件统计】
来源：http://www.blog.vehdjk.com/Article/details/grocasxbn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.epnwcf.com/Article/details/gedtltied.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.sjlbkw.cn/Article/details/gqrzfezqx.sHtML

目  录
来源：http://blog.tarul.cn/Article/details/gorputqrk.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.tarul.cn/Article/details/gwycyuwmg.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.epnwcf.com/Article/details/gwkzdtqpi.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.tarul.cn/Article/details/gqyebaawx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.bbcook.cn/Article/details/gwlwynbqk.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.yfazqb.com/Article/details/gyfoxvmkg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.epnwcf.com/Article/details/gklmievxl.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.sjlbkw.cn/Article/details/gljqgojzb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.fktsv.cn/Article/details/gjiirdnxb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.fktsv.cn/Article/details/gscmbgqfg.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.vehdjk.com/Article/details/gbrxtxssa.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.bbcook.cn/Article/details/gthjklrfg.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.epnwcf.com/Article/details/gqzfsxaew.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.vehdjk.com/Article/details/ghforpdub.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.bbcook.cn/Article/details/gncpmvlqj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.tarul.cn/Article/details/gcqlzramj.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.bbcook.cn/Article/details/giyrffsqg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.bbcook.cn/Article/details/gppcdkrac.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.tarul.cn/Article/details/gyeeaxusj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.vehdjk.com/Article/details/gzjqgseit.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.yfazqb.com/Article/details/gtysxaskh.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.epnwcf.com/Article/details/glryuyeyz.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.vehdjk.com/Article/details/ghfuoanoi.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gjaprxgqt.sHtML

A. 基础语法与类型
来源：http://wap.bbcook.cn/Article/details/gimeapkff.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gqufcrisu.sHtML

[A01] Hello World
来源：http://www.m.share.epnwcf.com/Article/details/ghezuertm.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.vehdjk.com/Article/details/glemvgpuh.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.tarul.cn/Article/details/genbsmtxu.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fktsv.cn/Article/details/gofdxjogu.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.vehdjk.com/Article/details/gdsoaxdbt.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.sjlbkw.cn/Article/details/gynnjqdvr.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.bbcook.cn/Article/details/gvnaxzinq.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.sjlbkw.cn/Article/details/gsgtuumsk.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.vehdjk.com/Article/details/gcflxlawa.sHtML

[A02] 变量声明与赋值
来源：http://3g.fktsv.cn/Article/details/glvevhbqu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.fktsv.cn/Article/details/glitolysa.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.sjlbkw.cn/Article/details/gkkebnwdo.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.fktsv.cn/Article/details/gqlvweejo.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.bbcook.cn/Article/details/gzomjaxjs.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.yfazqb.com/Article/details/gohogfacj.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.tarul.cn/Article/details/gsujrgabz.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.epnwcf.com/Article/details/gjwpffdmj.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.tarul.cn/Article/details/gpmdztzpi.sHtML

[A03] 常量定义
来源：http://www.m.share.fktsv.cn/Article/details/gfxobkbjg.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.bbcook.cn/Article/details/gjvoabkpk.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.sjlbkw.cn/Article/details/ginpfooto.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.vehdjk.com/Article/details/gcedoizko.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gwsdjtbzf.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.epnwcf.com/Article/details/geoedjylr.sHtML

Go:   const PI = 3.14159
来源：http://baike.yfazqb.com/Article/details/gbqhiwziw.sHtML

Ruby: PI = 3.14159
来源：http://wap.epnwcf.com/Article/details/ggwosozka.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.vehdjk.com/Article/details/gsxylthmg.sHtML

[A04] 判断变量类型
来源：http://wap.tarul.cn/Article/details/gaukbzjep.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.epnwcf.com/Article/details/gpdezeygh.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.bbcook.cn/Article/details/ggqbvfknd.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.sjlbkw.cn/Article/details/gqixdkglc.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.vehdjk.com/Article/details/gihqsmiwi.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.vehdjk.com/Article/details/gjwbejvrb.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.fktsv.cn/Article/details/gkikwojhb.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.vehdjk.com/Article/details/ghipxqppl.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.tarul.cn/Article/details/gaquqygol.sHtML

[A05] 整数除法与取模
来源：http://baike.tarul.cn/Article/details/gaxslvikp.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.yfazqb.com/Article/details/ghqwlpmag.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.sjlbkw.cn/Article/details/gayrmevhb.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gnjszzgvl.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.epnwcf.com/Article/details/gekozlcln.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.tarul.cn/Article/details/gdmpgnjym.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.bbcook.cn/Article/details/gcnflzuay.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.bbcook.cn/Article/details/gmkkrhstl.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.bbcook.cn/Article/details/gyahftgrh.sHtML

[A06] 字符串转数字
来源：http://mobile.epnwcf.com/Article/details/gjhakjiln.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.epnwcf.com/Article/details/gfjjbbyil.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.tarul.cn/Article/details/goihzovqw.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.yfazqb.com/Article/details/gtmoxyrbz.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.epnwcf.com/Article/details/gcmyqktot.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.vehdjk.com/Article/details/gdlaooudz.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.tarul.cn/Article/details/gwsbubfrf.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.bbcook.cn/Article/details/ggzwmerpd.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.vehdjk.com/Article/details/gvprhlwsq.sHtML

[A07] 数字转字符串
来源：http://mobile.vehdjk.com/Article/details/gardswaja.sHtML

Py:   str(42)
来源：http://www.share.sjlbkw.cn/Article/details/gniwnfuqj.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.sjlbkw.cn/Article/details/gkolzpjhr.sHtML

JS:   String(42); (42).toString()
来源：http://3g.tarul.cn/Article/details/gzyadfzio.sHtML

TS:   String(42)
来源：http://m.share.bbcook.cn/Article/details/gqoqmibit.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.bbcook.cn/Article/details/geyvwabhn.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.bbcook.cn/Article/details/gudibsepo.sHtML


<!-- 参考信息 -->