代发 wailian999

[U51] PHP：数组解构
来源：http://tgt.nanxuanxn.top

[$a, $b] = $arr;
来源：http://wke.sysykeji.top

[U52] PHP：箭头函数
来源：http://lcl.hnqzz.top

$double = fn($x) => $x * 2;
来源：http://klk.xuanzx.com

[U53] PHP：空合并运算符
来源：http://hsv.jinqigfzy.top

$v = $a ?? $b ?? "default";
来源：http://psk.fzhhl.top

[U54] PHP：空安全调用
来源：http://fhc.tian-w.cn

$obj?->method()
来源：http://ads.zhengqikj.top

[U55] PHP：match 表达式
来源：http://yxy.jinyuanbaomall.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pfp.aibaodan.cn

[U56] PHP：命名参数
来源：http://dyi.chenzaomai.com

f(a: 1, b: 2)
来源：http://eam.zhaomingkeji.xyz

[U57] PHP：字符串插值
来源：http://odn.0kj1m.cn

"值: {$a}"
来源：http://ztg.nwbrower.top

[U58] PHP：数组三件套
来源：http://jlc.gotoacloud.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rxz.meibo888.top

[U59] PHP：自定义排序
来源：http://lfu.yj202588.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zjz.0kj1m.cn

[U60] PHP：JSON 编解码
来源：http://ppm.shangyingyoupin.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mbi.yongpay.top

[U61] PHP：正则
来源：http://msf.jqgfzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gac.jqgufenzy.top

[U62] PHP：日期对象
来源：http://jxj.gotoacloud.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ixj.haohaochexian.top

[U63] PHP：文件读写
来源：http://ouk.tanke756.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ckj.smart0.xyz

[U64] PHP：目录遍历
来源：http://pcu.shangyingyoupin.top

glob("dir/*.php");  scandir("dir");
来源：http://hnd.sysykeji.top

[U65] PHP：会话
来源：http://hpe.kuanghao11.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://lqa.aizwys.cn

[U66] PHP：设置 Cookie
来源：http://evm.hongshengwenyu.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fsq.sysykeji.top

[U67] PHP：处理文件上传
来源：http://vub.jinyuanbaomall.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lqa.pycfn.com

[U68] PHP：PDO 连接
来源：http://cah.bjfxy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wfn.tarul.cn

[U69] PHP：PDO 预处理
来源：http://qfv.yanxiufei.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://oal.tianlin.xyz

[U70] PHP：PDO 事务
来源：http://pqz.jiagoushi.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xfo.0kj1m.cn

[U71] PHP：抛出异常
来源：http://dsn.aibaodan.cn

throw new RuntimeException("失败", 500);
来源：http://stp.hywenlv.cn

[U72] PHP：写错误日志
来源：http://ndz.wangdashe.top

error_log("失败: " . $e->getMessage());
来源：http://dlo.yangfankeji.com

[U73] PHP：读取 ini 配置
来源：http://kbx.snrcjt.cn

parse_ini_file("config.ini", true)
来源：http://gph.fanxiaobao.xyz

[U74] PHP：读取环境变量
来源：http://yrn.wangdashe.top

getenv("APP_ENV") ?: "production"
来源：http://lix.shanyushiyangtech.top

[U75] PHP：依赖注入
来源：http://poj.fanxiaobao.xyz

composer require psr/container
来源：http://xzc.fktsv.cn

[U76] PHP：简单路由
来源：http://ley.jqgufenzy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qqe.fktsv.cn

[U77] PHP：模板渲染
来源：http://wxc.daxiang520.top

composer require twig/twig
来源：http://ppk.mhx1999.top

[U78] PHP：单元测试
来源：http://hkz.9152youxi.cn

composer require --dev phpunit/phpunit
来源：http://xuf.shuidangran.top

[U79] PHP：静态分析
来源：http://pqj.haohaochexian.top

composer require --dev phpstan/phpstan
来源：http://bzy.xinyue.icu

[U80] PHP：代码规范修复
来源：http://rxx.zhijiandao.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://rhb.vqdsnc.cn

[U81] JS：初始化项目
来源：http://jgn.tanke756.top

npm init -y;  npm i express
来源：http://etp.jyoumei.cn

[U82] JS：package.json 脚本
来源：http://hxk.zhijiandao.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dvg.hesvh.cn

[U83] JS：ES Module 导入导出
来源：http://cnh.zhaomingkeji.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://mja.daxiang520.top

[U84] JS：CommonJS 写法
来源：http://efb.xylfe.cn

module.exports = { a };  const { a } = require("./m");
来源：http://jxk.aizwys.cn

[U85] JS：可选链
来源：http://aue.zhaomingkeji.xyz

a?.b?.c
来源：http://xjc.xziqi.cn

[U86] JS：空值合并
来源：http://pgk.jlsjyb.cn

a ?? b
来源：http://emq.yongpay.top

[U87] JS：解构默认值
来源：http://hkz.pengpengdd.cyou

const { a = 1, b = 2 } = obj;
来源：http://nnz.0kj1m.cn

[U88] JS：对象展开合并
来源：http://afd.snrcjt.cn

{ ...a, ...b }
来源：http://jsa.ivvv.top

[U89] JS：数组去重
来源：http://nmz.guowangkeji.top

[...new Set(arr)]
来源：http://yqh.vehdjk.com

[U90] JS：数字数组排序
来源：http://wrz.xziqi.cn

[...arr].sort((a, b) => a - b)
来源：http://muk.hesvh.cn

[U91] JS：对象键值遍历
来源：http://pog.jinyuanbaomall.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kmn.xinyue.icu

[U92] JS：深拷贝
来源：http://hzm.xuetiantiany.cn

structuredClone(obj)
来源：http://nxq.nanxuanxn.top

[U93] JS：模板字符串
来源：http://cqv.cdnleiting.top

`共 ${n} 条`
来源：http://ahn.tarul.cn

[U94] JS：箭头函数
来源：http://ybz.uphjek.com

const double = x => x * 2;
来源：http://clt.ehwqpu.com

[U95] JS：Promise 包装
来源：http://hhi.fengsongda.top

new Promise((resolve, reject) => {})
来源：http://mvr.gaohongyu789.top

[U96] JS：async/await 与异常
来源：http://elv.snrcjt.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://joq.daxiang520.top

[U97] JS：并发请求
来源：http://sbe.wangshuangyany.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://emy.hammf.cn

[U98] JS：fetch 带 JSON
来源：http://drj.dashuyun.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://oew.jqgufenzy.top

[U99] JS：事件监听
来源：http://fwg.ehwqpu.com

el.addEventListener("click", e => {})
来源：http://tyn.ivvv.top

[U100] JS：DOM 查询
来源：http://eot.hammf.cn

document.querySelector(".item")
来源：http://lem.sweek.top

[U101] JS：classList 操作
来源：http://jox.cashguo.top

el.classList.toggle("active")
来源：http://oqu.nwbrower.top

[U102] JS：本地存储
来源：http://qzn.feifeiyinyue.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://xxn.jqgufenzy.top

[U103] JS：定时器
来源：http://crc.zycfv.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tvt.jlsjyb.cn

[U104] JS：防抖
来源：http://mpd.mhx1999.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bsg.jinyuanbaomall.cn

[U105] JS：节流
来源：http://dmo.yonumen.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vvw.yonumen.top

[U106] JS：日期格式化
来源：http://ere.xuetiantiany.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://knt.ydjk.org.cn

[U107] JS：数字千分位
来源：http://ybr.ppjwa.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qhi.chenjidiqi.icu

[U108] JS：随机整数
来源：http://ahp.yanxiufei.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://agd.jinghuilouyu.cn

[U109] JS：数组分组
来源：http://zeb.jqgfzy.top

Object.groupBy(arr, x => x.type)
来源：http://uxj.guowangkeji.top

[U110] JS：数组分块
来源：http://ath.nanxinkj.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ygd.ywan-chungtsiang.top

[U111] JS：对象转 Map
来源：http://xms.jianghu66.top

new Map(Object.entries(obj))
来源：http://zcq.52xcode.cn

[U112] JS：字符串补位
来源：http://ofd.uphjek.com

"7".padStart(3, "0")
来源：http://xtu.ctjpmb.com

[U113] JS：正则替换全部
来源：http://pnr.hongshengwenyu.top

s.replaceAll("a", "b")
来源：http://wyn.dashuyun.cn

[U114] JS：JSON 深比较
来源：http://xcg.yj20258888.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://zjy.dashuyun.cn

[U115] JS：生成 UUID
来源：http://ojk.hongshengwenyu.top

crypto.randomUUID()
来源：http://nmo.kuanghao11.cn

[U116] JS：类型检查（JSDoc）
来源：http://dxg.vqdsnc.cn

/** @param {string} name */ function f(name) {}
来源：http://enj.vehdjk.com

[U117] JS：单元测试
来源：http://xjv.tian-w.cn

npm i -D vitest;  npx vitest
来源：http://fzr.nanxinkj.top

[U118] JS：开发服务器
来源：http://ypm.nanxuanxn.top

npm i -D vite;  npx vite
来源：http://ayy.cashguo.top

[U119] JS：生产构建
来源：http://aun.jqgfzy.top

npx vite build
来源：http://ixg.vehdjk.com

[U120] JS：读取环境变量（Vite）
来源：http://xzf.hammf.cn

import.meta.env.VITE_API_URL
来源：http://och.chenzaomai.com

================================================================================
来源：http://aso.yuxming.cn

统计汇总
来源：http://qns.gotoacloud.top

================================================================================
来源：http://uga.nanxuanxn.top

按语言统计（条）：
来源：http://ovc.mhx1999.top

Python ......... 252
来源：http://obu.yonumen.top

PHP ............ 252
来源：http://kli.ehwqpu.com

JavaScript ..... 252
来源：http://djx.pycfn.com

TypeScript ..... 212
来源：http://rjq.meibo888.top

Java ........... 212
来源：http://dmq.gotoacloud.top

Go ............. 212
来源：http://lwk.hnqzz.top

Ruby ........... 212
来源：http://pva.sxryk.cn

C# ............. 212
来源：http://inm.ivvv.top

C .............. 30
来源：http://bkr.guannengcc.top

C++ ............ 30
来源：http://rza.ywan-chungtsiang.top

SQL ............ 90
来源：http://oxe.sjlbkw.cn

Bash ........... 80
来源：http://pgn.ivvv.top

Kotlin ......... 15
来源：http://vxg.meibo888.top

Swift .......... 15
来源：http://arg.iojbl.cn

Lua ............ 10
来源：http://vfd.daxiang520.top

Perl ........... 10
来源：http://ccl.cheryme.top

Scala .......... 10
来源：http://zam.havefunace.top

------------------------------------
来源：http://hkt.zhengqikj.top

合计 ........... 2106 条
来源：http://twr.daxiang520.top

按章节统计：
来源：http://ztc.guowangkeji.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zxs.ybcxt.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mez.tarul.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bwq.fktsv.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rfw.xuetiantiany.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nfe.jlsjyb.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://toy.yongpay.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jno.quarkkingdee.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cyl.jqgufenzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uxs.svipenyu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jel.epnwcf.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ust.yongpay.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jyj.smart0.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nvy.nanxuanxn.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://whx.cqqwz.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fqe.birdmap.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bgm.mhx1999.top

Q SQL 专题                              90
来源：http://tqo.birdmap.top

R Bash 专题                             80
来源：http://ull.haohaochexian.top

S C / C++ 专题                          60
来源：http://dbk.9152youxi.cn

T 其他语言补充                          60
来源：http://fnt.uphjek.com

U 高频实用片段                         120
来源：http://dxi.cucudq.cn

------------------------------------
来源：http://bho.daxiang520.top

合计                                  2106 条
来源：http://fjg.iojbl.cn

--------------------------------------------------------------------------------
来源：http://sbi.fzhhl.top

使用提醒
来源：http://dli.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://dgk.redwolf501.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rip.gogol.net.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gjs.gzhubu.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qig.52xcode.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://tkv.tian-w.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ukv.c1oappe.top

—— 文件结束 ——
来源：http://yns.chenzaomai.com

================================================================================
来源：http://unc.iojbl.cn

程序语言常见例子速查手册（2024 版）
来源：http://tdn.hesvh.cn

Common Programming Examples Cheat Book
来源：http://qis.hywenlv.cn

================================================================================
来源：http://try.birdmap.top

【收录内容】
来源：http://pza.chenlongwang.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://sfe.birdmap.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fri.bbcook.cn

SQL · Bash · C · C++
来源：http://txb.tarul.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://eup.jinghuilouyu.cn

【使用说明】
来源：http://pnj.xziqi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://riq.jlsjyb.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://slt.sufxvd.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://yhh.yonumen.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fgl.zhaomingkeji.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://efx.ydjk.org.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ftm.gotoacloud.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qud.xuanzx.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://tww.guowangkeji.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xss.haohaochexian.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://esy.cashguo.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pnh.chenzaomai.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bts.wangdashe.top

【文件统计】
来源：http://ncw.havefunace.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qjm.shangyingyoupin.top

--------------------------------------------------------------------------------
来源：http://vvl.feifeiyinyue.top

目  录
来源：http://efi.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://nhx.hnqzz.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ful.zdbjq.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://muq.guannengcc.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://otd.xuetiantiany.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ghk.epnwcf.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://pdh.zdbjq.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ymz.sjlbkw.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kvz.cashguo.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://guy.chenzaomai.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mdu.quarkkingdee.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qsm.smart0.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hkc.gotoacloud.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://tln.0kj1m.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qvt.zhiwuduotai.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pwa.yuxming.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cda.ywan-chungtsiang.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qot.chenjidiqi.icu

Q. SQL 专题                    （第 17 节，90 条）
来源：http://djp.andypj.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://rsv.meibo888.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ikk.iojbl.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bwq.zhaomingkeji.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://tjk.yangfankeji.com

================================================================================
来源：http://eny.snrcjt.cn

A. 基础语法与类型
来源：http://qqr.tian-w.cn

================================================================================
来源：http://wgm.sweek.top

[A01] Hello World
来源：http://pjs.jyoumei.cn

Py:   print("Hello, World!")
来源：http://kpv.nwbrower.top

PHP:  echo "Hello, World!";
来源：http://lxl.fanxiaobao.xyz

JS:   console.log("Hello, World!");
来源：http://abn.zhongyouzk.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ugw.shuidangran.top

Java: System.out.println("Hello, World!");
来源：http://ryz.xziqi.cn

Go:   fmt.Println("Hello, World!")
来源：http://eai.xuanzx.com

Ruby: puts "Hello, World!"
来源：http://gyt.hesvh.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://cdg.nanxuanxn.top

[A02] 变量声明与赋值
来源：http://jow.feifeiyinyue.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wcd.haohaochexian.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ohh.gzhubu.top

JS:   let name = "Alex"; const age = 20;
来源：http://ids.epnwcf.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jhs.zhaomingkeji.xyz

Java: String name = "Alex"; int age = 20;
来源：http://ahg.guowangkeji.top

Go:   name := "Alex"; age := 20
来源：http://kbm.nwbrower.top

Ruby: name = "Alex"; age = 20
来源：http://lhh.xuanzx.com

C#:   string name = "Alex"; int age = 20;
来源：http://yhm.jinghuilouyu.cn

[A03] 常量定义
来源：http://avk.daria6918.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zye.hysaishi.cn

PHP:  const PI = 3.14159;
来源：http://wcv.xingfuxueyuan.xyz

JS:   const PI = 3.14159;
来源：http://aft.jlsjyb.cn

TS:   const PI: number = 3.14159;
来源：http://mba.sysykeji.top

Java: static final double PI = 3.14159;
来源：http://ach.gaohongyu789.top

Go:   const PI = 3.14159
来源：http://xur.jinqigufen.top

Ruby: PI = 3.14159
来源：http://gbn.jianghu66.top

C#:   const double PI = 3.14159;
来源：http://qqb.yangfankeji.com

[A04] 判断变量类型
来源：http://fae.fktsv.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://hdk.gzhubu.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://pxh.fanxiaobao.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://egg.epnwcf.com

TS:   typeof x; x instanceof Date
来源：http://vuy.ctjpmb.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://opj.gogol.net.cn

Go:   reflect.TypeOf(x).Name()
来源：http://xgi.haohaochexian.top

Ruby: x.class; x.is_a?(Integer)
来源：http://sbw.pengpengdd.cyou

C#:   x.GetType().Name; x is int
来源：http://gxl.hcnkem.com

[A05] 整数除法与取模
来源：http://djs.ybcxt.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ctr.wangdashe.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://vkl.c1oappe.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://haj.yanxiufei.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ijr.xingfuxueyuan.xyz

Java: 7 / 2; 7 % 2
来源：http://jsv.shanyushiyangkeji.top

Go:   7 / 2; 7 % 2
来源：http://vzq.nwbrower.top

Ruby: 7 / 2; 7 % 2
来源：http://geo.shangyingyoupin.top

C#:   7 / 2; 7 % 2
来源：http://hnn.andypj.xyz

[A06] 字符串转数字
来源：http://lyh.jqgufenzy.top

Py:   int("42"); float("3.14")
来源：http://eqi.sxryk.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://sef.hongshengwenyu.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://kts.cdnleiting.top

TS:   parseInt("42", 10); Number("42")
来源：http://gcu.hcnkem.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://sse.jianghu66.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://puh.andypj.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://iee.wangdashe.top


<!-- 参考信息 -->