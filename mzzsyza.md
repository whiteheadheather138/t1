代发 wailian999

[U57] PHP：字符串插值
来源：http://m.share.yfazqb.com/Article/details/gbzvscrdl.sHtML

"值: {$a}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gnjhbjztl.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.sjlbkw.cn/Article/details/gkeozzouv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.sjlbkw.cn/Article/details/gmxjbseae.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fktsv.cn/Article/details/gmrneijom.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fktsv.cn/Article/details/gnxjlweqk.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fktsv.cn/Article/details/gwoqxqikq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.vehdjk.com/Article/details/gbtbgybhy.sHtML

[U61] PHP：正则
来源：http://m.share.vehdjk.com/Article/details/gdrvydlaa.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.tarul.cn/Article/details/gtevqelir.sHtML

[U62] PHP：日期对象
来源：http://m.share.epnwcf.com/Article/details/ggclgunon.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fktsv.cn/Article/details/ggansdcwe.sHtML

[U63] PHP：文件读写
来源：http://www.blog.tarul.cn/Article/details/gxnozooot.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.epnwcf.com/Article/details/ghsgnhbxw.sHtML

[U64] PHP：目录遍历
来源：http://baike.yfazqb.com/Article/details/gpgxopdig.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fktsv.cn/Article/details/ghtrvseqj.sHtML

[U65] PHP：会话
来源：http://m.share.bbcook.cn/Article/details/gvneqciqn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.vehdjk.com/Article/details/gwdfljxpy.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.epnwcf.com/Article/details/gqhdcgavj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.sjlbkw.cn/Article/details/gszensykq.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fktsv.cn/Article/details/grikhykpr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.tarul.cn/Article/details/gfnbvseio.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.tarul.cn/Article/details/guudxucce.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.bbcook.cn/Article/details/goptdycgj.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.sjlbkw.cn/Article/details/gtjtcaspn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.yfazqb.com/Article/details/gfqylosnr.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.epnwcf.com/Article/details/gvthwkytp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.sjlbkw.cn/Article/details/gwdbrqktg.sHtML

[U71] PHP：抛出异常
来源：http://3g.epnwcf.com/Article/details/gzqnvnzwf.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.vehdjk.com/Article/details/gpwveulqn.sHtML

[U72] PHP：写错误日志
来源：http://baike.fktsv.cn/Article/details/gabwbmfsn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.tarul.cn/Article/details/gyqlbeoct.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.yfazqb.com/Article/details/gfxjojelz.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.vehdjk.com/Article/details/gqeghsfse.sHtML

[U74] PHP：读取环境变量
来源：http://blog.bbcook.cn/Article/details/gntqejwiu.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fktsv.cn/Article/details/ghnysshmu.sHtML

[U75] PHP：依赖注入
来源：http://3g.sjlbkw.cn/Article/details/galrvewpu.sHtML

composer require psr/container
来源：http://www.share.fktsv.cn/Article/details/gxyxucctw.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.epnwcf.com/Article/details/gmykrzfva.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.epnwcf.com/Article/details/gerirtyjt.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.bbcook.cn/Article/details/gruilzdzd.sHtML

composer require twig/twig
来源：http://wap.sjlbkw.cn/Article/details/grexijsnt.sHtML

[U78] PHP：单元测试
来源：http://read.share.sjlbkw.cn/Article/details/gntfqhlsx.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.vehdjk.com/Article/details/gokmbvaxq.sHtML

[U79] PHP：静态分析
来源：http://mobile.sjlbkw.cn/Article/details/gieouwlll.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.vehdjk.com/Article/details/gxhsjbnyl.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.bbcook.cn/Article/details/gwzdlcsbi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.yfazqb.com/Article/details/gytjfmkyy.sHtML

[U81] JS：初始化项目
来源：http://m.share.yfazqb.com/Article/details/gqkivrfpx.sHtML

npm init -y;  npm i express
来源：http://read.share.vehdjk.com/Article/details/gqhkfmivl.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.tarul.cn/Article/details/gpgphezpk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fktsv.cn/Article/details/gzexwhdzq.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.tarul.cn/Article/details/ggzfayxvc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.tarul.cn/Article/details/gbwdzuxje.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fktsv.cn/Article/details/gwxnbhbgh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.tarul.cn/Article/details/gwdltuyos.sHtML

[U85] JS：可选链
来源：http://mobile.epnwcf.com/Article/details/ghslpnvwp.sHtML

a?.b?.c
来源：http://www.share.epnwcf.com/Article/details/gjghxkrhc.sHtML

[U86] JS：空值合并
来源：http://wap.bbcook.cn/Article/details/gotqyshno.sHtML

a ?? b
来源：http://read.share.yfazqb.com/Article/details/gptkipauu.sHtML

[U87] JS：解构默认值
来源：http://3g.sjlbkw.cn/Article/details/gvijutenk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.vehdjk.com/Article/details/gnktygxyq.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.tarul.cn/Article/details/gvwdqouts.sHtML

{ ...a, ...b }
来源：http://wap.tarul.cn/Article/details/gqwgtauhe.sHtML

[U89] JS：数组去重
来源：http://www.blog.epnwcf.com/Article/details/ggecmzrks.sHtML

[...new Set(arr)]
来源：http://3g.yfazqb.com/Article/details/ghvqpfjtz.sHtML

[U90] JS：数字数组排序
来源：http://read.share.yfazqb.com/Article/details/gbpimgvpd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.tarul.cn/Article/details/ggtmvugul.sHtML

[U91] JS：对象键值遍历
来源：http://baike.vehdjk.com/Article/details/gsinjmnzy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.tarul.cn/Article/details/gqebbfqfb.sHtML

[U92] JS：深拷贝
来源：http://mobile.fktsv.cn/Article/details/gyzpluyjs.sHtML

structuredClone(obj)
来源：http://read.share.yfazqb.com/Article/details/gkywpxdax.sHtML

[U93] JS：模板字符串
来源：http://m.share.sjlbkw.cn/Article/details/gqjdmfbbk.sHtML

`共 ${n} 条`
来源：http://mobile.fktsv.cn/Article/details/gxscqjurh.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.tarul.cn/Article/details/gefrdbqtx.sHtML

const double = x => x * 2;
来源：http://3g.vehdjk.com/Article/details/gajrirnll.sHtML

[U95] JS：Promise 包装
来源：http://mobile.epnwcf.com/Article/details/garthrotn.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.yfazqb.com/Article/details/gnssgyukc.sHtML

[U96] JS：async/await 与异常
来源：http://3g.tarul.cn/Article/details/gkxwmxybp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.vehdjk.com/Article/details/gzewqcqyw.sHtML

[U97] JS：并发请求
来源：http://read.share.yfazqb.com/Article/details/gmprxiytm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.bbcook.cn/Article/details/giotzjlto.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.epnwcf.com/Article/details/goxhflrkv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.yfazqb.com/Article/details/gwlwmergg.sHtML

[U99] JS：事件监听
来源：http://wap.bbcook.cn/Article/details/gxcjynfsc.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.sjlbkw.cn/Article/details/grgrujdgx.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.epnwcf.com/Article/details/geqwucaww.sHtML

document.querySelector(".item")
来源：http://blog.tarul.cn/Article/details/gdhixcgli.sHtML

[U101] JS：classList 操作
来源：http://www.share.bbcook.cn/Article/details/golzshmue.sHtML

el.classList.toggle("active")
来源：http://3g.sjlbkw.cn/Article/details/gdsydhyfe.sHtML

[U102] JS：本地存储
来源：http://www.blog.sjlbkw.cn/Article/details/ghmdtlmds.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.bbcook.cn/Article/details/gxzdqrsry.sHtML

[U103] JS：定时器
来源：http://mobile.tarul.cn/Article/details/ggffhmjpt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.vehdjk.com/Article/details/gtoknydjh.sHtML

[U104] JS：防抖
来源：http://read.share.fktsv.cn/Article/details/gaofsiybb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.bbcook.cn/Article/details/gnyxepcxp.sHtML

[U105] JS：节流
来源：http://wap.yfazqb.com/Article/details/gnfqqjbgp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fktsv.cn/Article/details/gkntbxgyz.sHtML

[U106] JS：日期格式化
来源：http://www.blog.vehdjk.com/Article/details/gdetktjao.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.tarul.cn/Article/details/gwxedjccl.sHtML

[U107] JS：数字千分位
来源：http://www.share.yfazqb.com/Article/details/gxnuuskuj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.yfazqb.com/Article/details/gzgmqopxk.sHtML

[U108] JS：随机整数
来源：http://3g.tarul.cn/Article/details/gggfxoloa.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.tarul.cn/Article/details/geaureoce.sHtML

[U109] JS：数组分组
来源：http://m.share.yfazqb.com/Article/details/gwhphbljs.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.tarul.cn/Article/details/gwxbzsrjo.sHtML

[U110] JS：数组分块
来源：http://baike.sjlbkw.cn/Article/details/glsjejzbr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.sjlbkw.cn/Article/details/gnnmieamr.sHtML

[U111] JS：对象转 Map
来源：http://blog.fktsv.cn/Article/details/gtwpretfl.sHtML

new Map(Object.entries(obj))
来源：http://mobile.epnwcf.com/Article/details/gdokkgeym.sHtML

[U112] JS：字符串补位
来源：http://blog.tarul.cn/Article/details/ggjrwdnxk.sHtML

"7".padStart(3, "0")
来源：http://mobile.sjlbkw.cn/Article/details/gqhyswpze.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.epnwcf.com/Article/details/gaseendqs.sHtML

s.replaceAll("a", "b")
来源：http://read.share.tarul.cn/Article/details/gjjmvicbu.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.epnwcf.com/Article/details/ggsmwynkk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.bbcook.cn/Article/details/gwewrbfes.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.bbcook.cn/Article/details/gkibdcldm.sHtML

crypto.randomUUID()
来源：http://read.share.epnwcf.com/Article/details/glilshney.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.bbcook.cn/Article/details/gkmmuikbn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.yfazqb.com/Article/details/gavtaeoab.sHtML

[U117] JS：单元测试
来源：http://baike.fktsv.cn/Article/details/gqbjzsadz.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fktsv.cn/Article/details/gmczwclcb.sHtML

[U118] JS：开发服务器
来源：http://www.share.tarul.cn/Article/details/gckergalp.sHtML

npm i -D vite;  npx vite
来源：http://m.share.bbcook.cn/Article/details/gkxijxguj.sHtML

[U119] JS：生产构建
来源：http://www.blog.yfazqb.com/Article/details/gutuanwuq.sHtML

npx vite build
来源：http://3g.fktsv.cn/Article/details/gnvkduksd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.sjlbkw.cn/Article/details/gbwtrhdvu.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.epnwcf.com/Article/details/guvtoaqbb.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gtxrjeegt.sHtML

统计汇总
来源：http://www.m.share.vehdjk.com/Article/details/ggsejjfnc.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/grxbxesap.sHtML

按语言统计（条）：
来源：http://read.share.fktsv.cn/Article/details/gsoltuyge.sHtML

Python ......... 252
来源：http://baike.tarul.cn/Article/details/gouwfqwtv.sHtML

PHP ............ 252
来源：http://wap.yfazqb.com/Article/details/gssswbyjw.sHtML

JavaScript ..... 252
来源：http://www.share.fktsv.cn/Article/details/gnxbdhsyt.sHtML

TypeScript ..... 212
来源：http://blog.tarul.cn/Article/details/gfghimorf.sHtML

Java ........... 212
来源：http://www.blog.epnwcf.com/Article/details/gjjxtktfc.sHtML

Go ............. 212
来源：http://mobile.fktsv.cn/Article/details/gctkmfuko.sHtML

Ruby ........... 212
来源：http://m.share.sjlbkw.cn/Article/details/gcfxzkurr.sHtML

C# ............. 212
来源：http://wap.sjlbkw.cn/Article/details/gjvbpyfgy.sHtML

C .............. 30
来源：http://m.share.bbcook.cn/Article/details/guolkkhvv.sHtML

C++ ............ 30
来源：http://wap.epnwcf.com/Article/details/gpzwhbdqt.sHtML

SQL ............ 90
来源：http://www.share.bbcook.cn/Article/details/gkrxoehho.sHtML

Bash ........... 80
来源：http://read.share.sjlbkw.cn/Article/details/gakxtauqu.sHtML

Kotlin ......... 15
来源：http://read.share.bbcook.cn/Article/details/gmrkkzrkb.sHtML

Swift .......... 15
来源：http://3g.sjlbkw.cn/Article/details/gjaatqptb.sHtML

Lua ............ 10
来源：http://3g.vehdjk.com/Article/details/ghajjrzve.sHtML

Perl ........... 10
来源：http://read.share.epnwcf.com/Article/details/glfpgshoo.sHtML

Scala .......... 10
来源：http://3g.fktsv.cn/Article/details/gfcyahsog.sHtML

------------------------------------
来源：http://www.share.yfazqb.com/Article/details/gaxgluosn.sHtML

合计 ........... 2106 条
来源：http://www.share.vehdjk.com/Article/details/glqmhffwi.sHtML

按章节统计：
来源：http://m.share.yfazqb.com/Article/details/gpmfhrslk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.vehdjk.com/Article/details/gcrbhkaky.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.tarul.cn/Article/details/gcslexwhi.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.tarul.cn/Article/details/gnenqovga.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fktsv.cn/Article/details/ggjdglncs.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.tarul.cn/Article/details/gzxyjgzvv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.yfazqb.com/Article/details/glixbcdqx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.yfazqb.com/Article/details/gurehpkqt.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.yfazqb.com/Article/details/gtccmdclr.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.bbcook.cn/Article/details/gugwpqufe.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.epnwcf.com/Article/details/gvhfquiqm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.epnwcf.com/Article/details/gdqifocnk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fktsv.cn/Article/details/gekifgwbr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fktsv.cn/Article/details/grdycielh.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.vehdjk.com/Article/details/gykknxrxy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.sjlbkw.cn/Article/details/gochznfhp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.vehdjk.com/Article/details/ggyzvcwdf.sHtML

Q SQL 专题                              90
来源：http://baike.yfazqb.com/Article/details/gcbyctzxi.sHtML

R Bash 专题                             80
来源：http://blog.vehdjk.com/Article/details/glgzrlszh.sHtML

S C / C++ 专题                          60
来源：http://baike.tarul.cn/Article/details/gyqqydcze.sHtML

T 其他语言补充                          60
来源：http://baike.bbcook.cn/Article/details/gptkezwjp.sHtML

U 高频实用片段                         120
来源：http://baike.tarul.cn/Article/details/gtgpwiouu.sHtML

------------------------------------
来源：http://mobile.tarul.cn/Article/details/gffnqscjl.sHtML

合计                                  2106 条
来源：http://wap.fktsv.cn/Article/details/gvccqrqdb.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.yfazqb.com/Article/details/grhuzeids.sHtML

使用提醒
来源：http://read.share.fktsv.cn/Article/details/grjbxrubr.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.bbcook.cn/Article/details/gmjtdpguh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.yfazqb.com/Article/details/gapyxffmh.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.yfazqb.com/Article/details/gzumahpwp.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.sjlbkw.cn/Article/details/gzwbbhvzp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.tarul.cn/Article/details/gubvnepil.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.tarul.cn/Article/details/gxlozqolm.sHtML

—— 文件结束 ——
来源：http://www.blog.yfazqb.com/Article/details/grlmqaxua.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gmumkggrg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.sjlbkw.cn/Article/details/gedliysyf.sHtML

Common Programming Examples Cheat Book
来源：http://baike.tarul.cn/Article/details/gepqgisiq.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/ggvoejcvg.sHtML

【收录内容】
来源：http://wap.tarul.cn/Article/details/gjiwugiae.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.vehdjk.com/Article/details/grsrecijo.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.epnwcf.com/Article/details/gtyemcrec.sHtML

SQL · Bash · C · C++
来源：http://wap.yfazqb.com/Article/details/gkwdzunbl.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.vehdjk.com/Article/details/grvuxfirk.sHtML

【使用说明】
来源：http://blog.epnwcf.com/Article/details/gcdwybztm.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.tarul.cn/Article/details/gpykrpwgh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.yfazqb.com/Article/details/guiwhjkmq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.tarul.cn/Article/details/gtcztnxtm.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.epnwcf.com/Article/details/gbtvctfsm.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.bbcook.cn/Article/details/gcggjgijc.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.yfazqb.com/Article/details/ghmlvccif.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.epnwcf.com/Article/details/gfjrkqcqg.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.vehdjk.com/Article/details/gnjgslntg.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.tarul.cn/Article/details/gggacycwu.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.vehdjk.com/Article/details/ghwbtixbt.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.yfazqb.com/Article/details/gddglwfwv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.tarul.cn/Article/details/gbmoolgmv.sHtML

【文件统计】
来源：http://baike.yfazqb.com/Article/details/gkekzbcpd.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.vehdjk.com/Article/details/ggykgsnoq.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.tarul.cn/Article/details/gpnvvrlcb.sHtML

目  录
来源：http://3g.epnwcf.com/Article/details/gdkogkccg.sHtML

--------------------------------------------------------------------------------
来源：http://blog.sjlbkw.cn/Article/details/gnkxniyyx.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.bbcook.cn/Article/details/gcsiugqas.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.epnwcf.com/Article/details/ggbhybsoa.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.sjlbkw.cn/Article/details/gfbpzsuny.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fktsv.cn/Article/details/gvddanoij.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.tarul.cn/Article/details/gwygslbke.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.tarul.cn/Article/details/gcukxbmfa.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.yfazqb.com/Article/details/gdteefdwc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.fktsv.cn/Article/details/govolmhkg.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.yfazqb.com/Article/details/gfpkgybcd.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.vehdjk.com/Article/details/grokreydg.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.sjlbkw.cn/Article/details/grkzxygwn.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.tarul.cn/Article/details/gsmrgbjgd.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.bbcook.cn/Article/details/gibnlxrzp.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.epnwcf.com/Article/details/gchmtqrxu.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.sjlbkw.cn/Article/details/gulhnvczh.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.yfazqb.com/Article/details/gipfmgzad.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.vehdjk.com/Article/details/gygkgeusg.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.fktsv.cn/Article/details/gjzjcrvas.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.tarul.cn/Article/details/geljxvgea.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.vehdjk.com/Article/details/ghkygvmhz.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.yfazqb.com/Article/details/gaafxvzun.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gkpfwnbbl.sHtML

A. 基础语法与类型
来源：http://www.blog.bbcook.cn/Article/details/gjpauqqje.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/ggvzsihqf.sHtML

[A01] Hello World
来源：http://mobile.vehdjk.com/Article/details/gkfbaffzt.sHtML

Py:   print("Hello, World!")
来源：http://mobile.fktsv.cn/Article/details/gxohaflwf.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.epnwcf.com/Article/details/gpkffnbwc.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.vehdjk.com/Article/details/gjadsqees.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.fktsv.cn/Article/details/gnxvavkmh.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.sjlbkw.cn/Article/details/gpptdnyhq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.epnwcf.com/Article/details/gjymmvyuv.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.tarul.cn/Article/details/gliatwwor.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.tarul.cn/Article/details/gnlblqibb.sHtML

[A02] 变量声明与赋值
来源：http://wap.vehdjk.com/Article/details/gpeivkzpo.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.sjlbkw.cn/Article/details/gglpwnhnp.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzkosrpoj.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.bbcook.cn/Article/details/gjcxiyqlg.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.vehdjk.com/Article/details/gxfamnuhl.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.bbcook.cn/Article/details/gyyavmrlm.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.bbcook.cn/Article/details/ghuybeeqg.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.tarul.cn/Article/details/gyaxbzmdm.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.bbcook.cn/Article/details/gwcniqwgj.sHtML

[A03] 常量定义
来源：http://www.m.share.bbcook.cn/Article/details/gxhdkhmhd.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.fktsv.cn/Article/details/ghilpqlkw.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.vehdjk.com/Article/details/gvniewkow.sHtML

JS:   const PI = 3.14159;
来源：http://baike.bbcook.cn/Article/details/gtthnxgwh.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.bbcook.cn/Article/details/gnnpujqij.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.fktsv.cn/Article/details/gptxdqztu.sHtML

Go:   const PI = 3.14159
来源：http://baike.fktsv.cn/Article/details/gccehilua.sHtML

Ruby: PI = 3.14159
来源：http://m.share.sjlbkw.cn/Article/details/gtppggife.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.tarul.cn/Article/details/gvoeyeehf.sHtML

[A04] 判断变量类型
来源：http://read.share.yfazqb.com/Article/details/gfmjiedjj.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.tarul.cn/Article/details/gjbkowpen.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnitmtzyr.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.epnwcf.com/Article/details/gsengahdl.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.yfazqb.com/Article/details/gsdzgmdjg.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.vehdjk.com/Article/details/gtsumfhwx.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.vehdjk.com/Article/details/gkttdhrnr.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.vehdjk.com/Article/details/gsgqzeuid.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.vehdjk.com/Article/details/gryohuiaw.sHtML

[A05] 整数除法与取模
来源：http://mobile.vehdjk.com/Article/details/ggceehyqu.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.bbcook.cn/Article/details/glouqiion.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.vehdjk.com/Article/details/gcmobjcnw.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.yfazqb.com/Article/details/gtokwtwhn.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.yfazqb.com/Article/details/gbdztcotb.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.epnwcf.com/Article/details/gogyrluot.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.sjlbkw.cn/Article/details/gjhclsyzs.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.fktsv.cn/Article/details/guhknpyaq.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.sjlbkw.cn/Article/details/gfukdhyht.sHtML

[A06] 字符串转数字
来源：http://wap.fktsv.cn/Article/details/gqryrommp.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.bbcook.cn/Article/details/gxbtgeaox.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.yfazqb.com/Article/details/glxjrnfbn.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.epnwcf.com/Article/details/gdyvtleoe.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.fktsv.cn/Article/details/grkbgdctl.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.sjlbkw.cn/Article/details/glpksmfdf.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.yfazqb.com/Article/details/gbhucwwbo.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.yfazqb.com/Article/details/ghokylsmp.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.vehdjk.com/Article/details/gsdhnecpt.sHtML

[A07] 数字转字符串
来源：http://3g.sjlbkw.cn/Article/details/gqsfgnmtc.sHtML

Py:   str(42)
来源：http://mobile.bbcook.cn/Article/details/gnuafqflg.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.fktsv.cn/Article/details/gqmwhaffs.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.yfazqb.com/Article/details/ghiapjgra.sHtML

TS:   String(42)
来源：http://wap.fktsv.cn/Article/details/glfylzwjn.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.bbcook.cn/Article/details/gejpuqghb.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.yfazqb.com/Article/details/guqmyuahg.sHtML

Ruby: 42.to_s
来源：http://www.blog.bbcook.cn/Article/details/gnhqkqdlf.sHtML

C#:   42.ToString()
来源：http://read.share.tarul.cn/Article/details/ggeyiubrn.sHtML

[A08] 取整与四舍五入
来源：http://baike.yfazqb.com/Article/details/gbwygdigm.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.yfazqb.com/Article/details/gxihdwpbr.sHtML


<!-- 参考信息 -->