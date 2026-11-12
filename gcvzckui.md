代发 wailian999

[U57] PHP：字符串插值
来源：http://his.ybcxt.top

"值: {$a}"
来源：http://rkv.jiagoushi.top

[U58] PHP：数组三件套
来源：http://oxt.ydzc1.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lij.yonumen.top

[U59] PHP：自定义排序
来源：http://rhb.jinghuilouyu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://knl.feifeiyinyue.top

[U60] PHP：JSON 编解码
来源：http://xtw.fehbvm.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://uxo.havefunace.top

[U61] PHP：正则
来源：http://bba.fzhhl.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://oqp.c1oappe.top

[U62] PHP：日期对象
来源：http://pgq.jinghuilouyu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rqc.sufxvd.cn

[U63] PHP：文件读写
来源：http://htj.dianchejie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yza.hnxiangtu.top

[U64] PHP：目录遍历
来源：http://ufz.zdqjudy.top

glob("dir/*.php");  scandir("dir");
来源：http://shu.hywenlv.cn

[U65] PHP：会话
来源：http://dhm.dashuyun.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rmw.tanke756.top

[U66] PHP：设置 Cookie
来源：http://lcy.xuetiantiany.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yvk.chenzaomai.com

[U67] PHP：处理文件上传
来源：http://xiv.nanxuanxn.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yjk.zhijiandao.cn

[U68] PHP：PDO 连接
来源：http://ijd.nwbrower.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sam.gogol.net.cn

[U69] PHP：PDO 预处理
来源：http://jen.jqgufenzy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://shs.yj20258.top

[U70] PHP：PDO 事务
来源：http://ust.chenzaomai.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qbf.jinqigufen.top

[U71] PHP：抛出异常
来源：http://sad.c1oappe.top

throw new RuntimeException("失败", 500);
来源：http://nqm.smart0.xyz

[U72] PHP：写错误日志
来源：http://lck.316326.xyz

error_log("失败: " . $e->getMessage());
来源：http://cke.yonumen.top

[U73] PHP：读取 ini 配置
来源：http://cox.gotoacloud.top

parse_ini_file("config.ini", true)
来源：http://lnb.smart0.xyz

[U74] PHP：读取环境变量
来源：http://ohg.vehdjk.com

getenv("APP_ENV") ?: "production"
来源：http://ttg.gaohongyu789.top

[U75] PHP：依赖注入
来源：http://zwb.ivvv.top

composer require psr/container
来源：http://rmf.vehdjk.com

[U76] PHP：简单路由
来源：http://pac.snrcjt.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mvf.nanxinkj.top

[U77] PHP：模板渲染
来源：http://egk.yj20258.top

composer require twig/twig
来源：http://cux.jinyuanbaomall.cn

[U78] PHP：单元测试
来源：http://rpz.shanyushiyangkeji.top

composer require --dev phpunit/phpunit
来源：http://obk.sxryk.cn

[U79] PHP：静态分析
来源：http://cjp.316326.xyz

composer require --dev phpstan/phpstan
来源：http://cbh.kuanghao11.cn

[U80] PHP：代码规范修复
来源：http://kdr.vqdsnc.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xeg.bbcook.cn

[U81] JS：初始化项目
来源：http://itm.smart0.xyz

npm init -y;  npm i express
来源：http://qpu.yj20258888.top

[U82] JS：package.json 脚本
来源：http://qmq.fzhhl.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vbg.chenlongwang.top

[U83] JS：ES Module 导入导出
来源：http://kbb.guannengcc.top

export const a = 1;  import { a } from "./m.js";
来源：http://ntc.sjlbkw.cn

[U84] JS：CommonJS 写法
来源：http://lqc.ivvv.top

module.exports = { a };  const { a } = require("./m");
来源：http://nes.c1oappe.top

[U85] JS：可选链
来源：http://otw.hcnkem.com

a?.b?.c
来源：http://qbq.zdqjudy.top

[U86] JS：空值合并
来源：http://gvk.dashuyun.cn

a ?? b
来源：http://kmb.mhx1999.top

[U87] JS：解构默认值
来源：http://dch.hongshengwenyu.top

const { a = 1, b = 2 } = obj;
来源：http://amx.nanxinkj.top

[U88] JS：对象展开合并
来源：http://kms.guowangkeji.top

{ ...a, ...b }
来源：http://iay.shanyushiyangkeji.top

[U89] JS：数组去重
来源：http://nft.quarkkingdee.top

[...new Set(arr)]
来源：http://xdt.yj20258.top

[U90] JS：数字数组排序
来源：http://wvm.smart0.xyz

[...arr].sort((a, b) => a - b)
来源：http://dal.hysaishi.cn

[U91] JS：对象键值遍历
来源：http://lrj.jianghu66.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qmp.tanke756.top

[U92] JS：深拷贝
来源：http://wos.jqgufenzy.top

structuredClone(obj)
来源：http://myj.ppjwa.cn

[U93] JS：模板字符串
来源：http://oak.sufxvd.cn

`共 ${n} 条`
来源：http://txv.yangfankeji.com

[U94] JS：箭头函数
来源：http://seo.iojbl.cn

const double = x => x * 2;
来源：http://azv.jinqigufen.top

[U95] JS：Promise 包装
来源：http://dkq.gotoacloud.top

new Promise((resolve, reject) => {})
来源：http://qye.sysykeji.top

[U96] JS：async/await 与异常
来源：http://xtd.dianchejie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mnk.jinqigufen.top

[U97] JS：并发请求
来源：http://qar.pengpengdd.cyou

await Promise.all(urls.map(u => fetch(u)))
来源：http://tja.fehbvm.com

[U98] JS：fetch 带 JSON
来源：http://cwi.cucudq.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mvl.jqgufenzy.top

[U99] JS：事件监听
来源：http://hnb.aibaodan.cn

el.addEventListener("click", e => {})
来源：http://ymb.yfazqb.com

[U100] JS：DOM 查询
来源：http://ozf.tianlin.xyz

document.querySelector(".item")
来源：http://kvr.ehwqpu.com

[U101] JS：classList 操作
来源：http://cxq.nwbrower.top

el.classList.toggle("active")
来源：http://ihd.zhixingplan.top

[U102] JS：本地存储
来源：http://qzg.zhiwuduotai.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://goz.yongpay.top

[U103] JS：定时器
来源：http://mbm.jinqigfzy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fjk.fzhhl.top

[U104] JS：防抖
来源：http://xnz.yuxming.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ugw.zhaomingkeji.xyz

[U105] JS：节流
来源：http://luy.tanke756.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mrj.xziqi.cn

[U106] JS：日期格式化
来源：http://mal.meibo888.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ijv.iojbl.cn

[U107] JS：数字千分位
来源：http://vuk.gaohongyu789.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zdq.jinyuanbaomall.cn

[U108] JS：随机整数
来源：http://iyc.xinyue.icu

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://adj.fanxiaobao.xyz

[U109] JS：数组分组
来源：http://vfl.bjfxy.top

Object.groupBy(arr, x => x.type)
来源：http://yjr.dashuyun.cn

[U110] JS：数组分块
来源：http://mlr.haohaochexian.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pln.xingfuxueyuan.xyz

[U111] JS：对象转 Map
来源：http://ivh.hysaishi.cn

new Map(Object.entries(obj))
来源：http://dcw.andypj.xyz

[U112] JS：字符串补位
来源：http://mbs.fktsv.cn

"7".padStart(3, "0")
来源：http://bmj.hcnkem.com

[U113] JS：正则替换全部
来源：http://hfx.yfazqb.com

s.replaceAll("a", "b")
来源：http://pxx.cdnleiting.top

[U114] JS：JSON 深比较
来源：http://goy.xziqi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://fww.hesvh.cn

[U115] JS：生成 UUID
来源：http://pwo.fzhhl.top

crypto.randomUUID()
来源：http://tez.jinqigufen.top

[U116] JS：类型检查（JSDoc）
来源：http://sha.zdbjq.cn

/** @param {string} name */ function f(name) {}
来源：http://clj.guowangkeji.top

[U117] JS：单元测试
来源：http://vhk.epnwcf.com

npm i -D vitest;  npx vitest
来源：http://mjh.birdmap.top

[U118] JS：开发服务器
来源：http://luz.smart0.xyz

npm i -D vite;  npx vite
来源：http://cwc.tianlin.xyz

[U119] JS：生产构建
来源：http://reg.xuanzx.com

npx vite build
来源：http://yqp.zhijiandao.cn

[U120] JS：读取环境变量（Vite）
来源：http://eql.52xcode.cn

import.meta.env.VITE_API_URL
来源：http://csh.xziqi.cn

================================================================================
来源：http://nji.hammf.cn

统计汇总
来源：http://tdg.yonumen.top

================================================================================
来源：http://dir.sysykeji.top

按语言统计（条）：
来源：http://kos.shangyingyoupin.top

Python ......... 252
来源：http://drp.fehbvm.com

PHP ............ 252
来源：http://uix.guowangkeji.top

JavaScript ..... 252
来源：http://oxo.smart0.xyz

TypeScript ..... 212
来源：http://evg.daxiang520.top

Java ........... 212
来源：http://ohg.yj20258.top

Go ............. 212
来源：http://nea.daxiang520.top

Ruby ........... 212
来源：http://dtq.0kj1m.cn

C# ............. 212
来源：http://qbx.0kj1m.cn

C .............. 30
来源：http://tli.vehdjk.com

C++ ............ 30
来源：http://uvb.hongshengwenyu.top

SQL ............ 90
来源：http://pec.guowangkeji.top

Bash ........... 80
来源：http://aml.hfpthk.cn

Kotlin ......... 15
来源：http://vzn.hywenlv.cn

Swift .......... 15
来源：http://fit.hammf.cn

Lua ............ 10
来源：http://ykt.wangdashe.top

Perl ........... 10
来源：http://vzk.meibo888.top

Scala .......... 10
来源：http://wwf.sweek.top

------------------------------------
来源：http://kuh.shuidangran.top

合计 ........... 2106 条
来源：http://ewd.hcnkem.com

按章节统计：
来源：http://vir.xuanzx.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fcz.sxryk.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ltn.nanxinkj.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dfi.c1oappe.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hqg.zhixingplan.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gjx.cheryme.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kve.birdmap.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ban.gaohongyu789.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hly.yuxming.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wgu.vehdjk.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gak.yangfankeji.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://axv.c1oappe.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yjy.jinqigufen.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lmp.shzxlz.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ttg.fktsv.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yma.yfazqb.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xtw.fengsongda.top

Q SQL 专题                              90
来源：http://mie.jinqigfzy.top

R Bash 专题                             80
来源：http://nbm.yvedp.cn

S C / C++ 专题                          60
来源：http://zxl.kuanghao11.cn

T 其他语言补充                          60
来源：http://ldj.pycfn.com

U 高频实用片段                         120
来源：http://ccu.bjfxy.top

------------------------------------
来源：http://eaj.zhijiandao.cn

合计                                  2106 条
来源：http://wdw.yuxming.cn

--------------------------------------------------------------------------------
来源：http://zte.cucudq.cn

使用提醒
来源：http://eoq.ctjpmb.com

--------------------------------------------------------------------------------
来源：http://frm.52xcode.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://css.quarkkingdee.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vsd.fktsv.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://sxq.hongshengwenyu.top

在旧版本上使用前请先确认语法支持情况。
来源：http://qia.jqgufenzy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fst.hnxiangtu.top

—— 文件结束 ——
来源：http://aen.ybcxt.top

================================================================================
来源：http://okf.dashuyun.cn

程序语言常见例子速查手册（2024 版）
来源：http://aqq.uphjek.com

Common Programming Examples Cheat Book
来源：http://rcr.nanxuanxn.top

================================================================================
来源：http://jze.jyoumei.cn

【收录内容】
来源：http://gib.gzhubu.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://oqo.gotoacloud.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://urg.epnwcf.com

SQL · Bash · C · C++
来源：http://uax.wangshuangyany.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://exu.0kj1m.cn

【使用说明】
来源：http://xzb.vehdjk.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jdb.feifeiyinyue.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jqt.sysykeji.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tmr.pengpengdd.cyou

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gsu.zdqjudy.top

Bash:  Shell         C:     C             C++:   C++
来源：http://vcb.zhongyouzk.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nfx.ydzc1.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fgs.ydjk.org.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://cgp.dashuyun.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://slb.haohaochexian.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wcj.tian-w.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dre.zhongyouzk.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://cyq.hammf.cn

【文件统计】
来源：http://wgl.jqgfzy.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jav.havefunace.top

--------------------------------------------------------------------------------
来源：http://gnj.nwbrower.top

目  录
来源：http://qan.shuidangran.top

--------------------------------------------------------------------------------
来源：http://rlc.tanke756.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ehr.cucudq.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rsf.tanke756.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zap.zhaomingkeji.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qze.jqgfzy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://eah.andypj.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vrl.cheryme.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://stn.dashuyun.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qve.shanyushiyangkeji.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jvl.nanxuanxn.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hfw.gotoacloud.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zlf.sjlbkw.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ixh.jqgfzy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rvt.hywenlv.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tdt.redwolf501.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pmk.316326.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://orx.wangshuangyany.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pwk.zhiwuduotai.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://zpw.xuanzx.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://auk.birdmap.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://skx.yanxiufei.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://frt.shanyushiyangkeji.top

================================================================================
来源：http://dhx.zhiwuduotai.top

A. 基础语法与类型
来源：http://ayt.aizwys.cn

================================================================================
来源：http://its.9152youxi.cn

[A01] Hello World
来源：http://xms.hammf.cn

Py:   print("Hello, World!")
来源：http://gul.yangfankeji.com

PHP:  echo "Hello, World!";
来源：http://gig.daxiang520.top

JS:   console.log("Hello, World!");
来源：http://shv.sysykeji.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yiw.hammf.cn

Java: System.out.println("Hello, World!");
来源：http://elp.yangfankeji.com

Go:   fmt.Println("Hello, World!")
来源：http://tct.xziqi.cn

Ruby: puts "Hello, World!"
来源：http://vjg.wangdashe.top

C#:   Console.WriteLine("Hello, World!");
来源：http://utx.zhiwuduotai.top

[A02] 变量声明与赋值
来源：http://hzl.cheryme.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://oqo.tian-w.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://htq.iojbl.cn

JS:   let name = "Alex"; const age = 20;
来源：http://nxn.daxiang520.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://urp.quarkkingdee.top

Java: String name = "Alex"; int age = 20;
来源：http://ncv.zdqjudy.top

Go:   name := "Alex"; age := 20
来源：http://kfz.tianlin.xyz

Ruby: name = "Alex"; age = 20
来源：http://apw.aizwys.cn

C#:   string name = "Alex"; int age = 20;
来源：http://yec.yj202588.top

[A03] 常量定义
来源：http://edt.sxryk.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ljo.chenlongwang.top

PHP:  const PI = 3.14159;
来源：http://mag.ehwqpu.com

JS:   const PI = 3.14159;
来源：http://jzs.gogol.net.cn

TS:   const PI: number = 3.14159;
来源：http://uyp.birdmap.top

Java: static final double PI = 3.14159;
来源：http://bfk.cdnleiting.top

Go:   const PI = 3.14159
来源：http://qvt.fzhhl.top

Ruby: PI = 3.14159
来源：http://lqy.shzxlz.cn

C#:   const double PI = 3.14159;
来源：http://apy.havefunace.top

[A04] 判断变量类型
来源：http://uvw.jinghuilouyu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://sqx.xuanzx.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://faf.cucudq.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rft.bjfxy.top

TS:   typeof x; x instanceof Date
来源：http://jhm.yfazqb.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vnh.nanxinkj.top

Go:   reflect.TypeOf(x).Name()
来源：http://qxw.daxiang520.top

Ruby: x.class; x.is_a?(Integer)
来源：http://jpm.dianchejie.cn

C#:   x.GetType().Name; x is int
来源：http://cyc.yj202588.top

[A05] 整数除法与取模
来源：http://cfv.bjfxy.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yrl.ydzc1.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://col.9152youxi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://giv.zhengqikj.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://owh.jinyuanbaomall.cn

Java: 7 / 2; 7 % 2
来源：http://kqe.cheryme.top

Go:   7 / 2; 7 % 2
来源：http://crp.shzxlz.cn

Ruby: 7 / 2; 7 % 2
来源：http://fdq.mhx1999.top

C#:   7 / 2; 7 % 2
来源：http://sga.snrcjt.cn

[A06] 字符串转数字
来源：http://lfx.jianghu66.top

Py:   int("42"); float("3.14")
来源：http://blk.shangyingyoupin.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tqx.chenlongwang.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://aqb.52xcode.cn

TS:   parseInt("42", 10); Number("42")
来源：http://vdz.gaohongyu789.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hal.daxiang520.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nox.yanxiufei.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://yrf.hnxiangtu.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://lop.redwolf501.top

[A07] 数字转字符串
来源：http://etx.9152youxi.cn

Py:   str(42)
来源：http://ngp.zhijiandao.cn

PHP:  (string) 42; strval(42)
来源：http://trm.uphjek.com

JS:   String(42); (42).toString()
来源：http://uft.birdmap.top

TS:   String(42)
来源：http://blh.yanxiufei.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://hof.hfpthk.cn

Go:   strconv.Itoa(42)
来源：http://udq.zhijiandao.cn

Ruby: 42.to_s
来源：http://vmv.jqgfzy.top

C#:   42.ToString()
来源：http://fih.vqdsnc.cn

[A08] 取整与四舍五入
来源：http://suv.sufxvd.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://prh.sjlbkw.cn


<!-- 参考信息 -->