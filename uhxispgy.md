代发 wailian999

[U53] PHP：空合并运算符
来源：http://myg.hammf.cn

$v = $a ?? $b ?? "default";
来源：http://nvb.vehdjk.com

[U54] PHP：空安全调用
来源：http://zca.xuanzx.com

$obj?->method()
来源：http://iba.fzhhl.top

[U55] PHP：match 表达式
来源：http://jwt.nwbrower.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ovv.shanyushiyangtech.top

[U56] PHP：命名参数
来源：http://acx.feifeiyinyue.top

f(a: 1, b: 2)
来源：http://zrw.xuetiantiany.cn

[U57] PHP：字符串插值
来源：http://dqq.haohaochexian.top

"值: {$a}"
来源：http://zba.quarkkingdee.top

[U58] PHP：数组三件套
来源：http://gxi.shzxlz.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ith.hfpthk.cn

[U59] PHP：自定义排序
来源：http://qoz.feifeiyinyue.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vpb.xziqi.cn

[U60] PHP：JSON 编解码
来源：http://hgx.sysykeji.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bzm.hongshengwenyu.top

[U61] PHP：正则
来源：http://ebx.gogol.net.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ydy.guannengcc.top

[U62] PHP：日期对象
来源：http://yjk.xinyue.icu

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zrg.quarkkingdee.top

[U63] PHP：文件读写
来源：http://cbc.zhixingplan.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://agk.redwolf501.top

[U64] PHP：目录遍历
来源：http://vjs.kuanghao11.cn

glob("dir/*.php");  scandir("dir");
来源：http://auo.dianchejie.cn

[U65] PHP：会话
来源：http://cbn.aibaodan.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ynm.uphjek.com

[U66] PHP：设置 Cookie
来源：http://fne.wangdashe.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://chd.jinghuilouyu.cn

[U67] PHP：处理文件上传
来源：http://uzz.shangyingyoupin.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bms.hnqzz.top

[U68] PHP：PDO 连接
来源：http://wpo.9152youxi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cwj.yvedp.cn

[U69] PHP：PDO 预处理
来源：http://tat.jinyuanbaomall.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hor.ctjpmb.com

[U70] PHP：PDO 事务
来源：http://zqr.cdnleiting.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kyt.jiagoushi.top

[U71] PHP：抛出异常
来源：http://qho.jianghu66.top

throw new RuntimeException("失败", 500);
来源：http://xoi.zhijiandao.cn

[U72] PHP：写错误日志
来源：http://yur.c1oappe.top

error_log("失败: " . $e->getMessage());
来源：http://ajy.ywan-chungtsiang.top

[U73] PHP：读取 ini 配置
来源：http://wmp.uphjek.com

parse_ini_file("config.ini", true)
来源：http://dvo.jianghu66.top

[U74] PHP：读取环境变量
来源：http://fmu.cdnleiting.top

getenv("APP_ENV") ?: "production"
来源：http://rap.havefunace.top

[U75] PHP：依赖注入
来源：http://ajc.wangshuangyany.cn

composer require psr/container
来源：http://epw.uphjek.com

[U76] PHP：简单路由
来源：http://zhq.jinqigfzy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bri.yangfankeji.com

[U77] PHP：模板渲染
来源：http://jxn.zhixingplan.top

composer require twig/twig
来源：http://rmn.cashguo.top

[U78] PHP：单元测试
来源：http://uga.yueranfly.top

composer require --dev phpunit/phpunit
来源：http://vhq.hongshengwenyu.top

[U79] PHP：静态分析
来源：http://qvn.zhoulong.xyz

composer require --dev phpstan/phpstan
来源：http://xha.cashguo.top

[U80] PHP：代码规范修复
来源：http://zkw.yuanzhike.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://hyo.aibaodan.cn

[U81] JS：初始化项目
来源：http://bym.wangdashe.top

npm init -y;  npm i express
来源：http://ani.zhiwuduotai.top

[U82] JS：package.json 脚本
来源：http://lgt.chenzaomai.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jfi.gaohongyu789.top

[U83] JS：ES Module 导入导出
来源：http://yuc.c1oappe.top

export const a = 1;  import { a } from "./m.js";
来源：http://uvl.bbcook.cn

[U84] JS：CommonJS 写法
来源：http://gza.pycfn.com

module.exports = { a };  const { a } = require("./m");
来源：http://uwh.jqgufenzy.top

[U85] JS：可选链
来源：http://sln.tian-w.cn

a?.b?.c
来源：http://cmf.jqgufenzy.top

[U86] JS：空值合并
来源：http://uyd.dianchejie.cn

a ?? b
来源：http://rse.chenzaomai.com

[U87] JS：解构默认值
来源：http://bsx.shzxlz.cn

const { a = 1, b = 2 } = obj;
来源：http://qlw.meibo888.top

[U88] JS：对象展开合并
来源：http://xcu.ehwqpu.com

{ ...a, ...b }
来源：http://heb.quarkkingdee.top

[U89] JS：数组去重
来源：http://rlp.vehdjk.com

[...new Set(arr)]
来源：http://ypm.tanke756.top

[U90] JS：数字数组排序
来源：http://kde.sysykeji.top

[...arr].sort((a, b) => a - b)
来源：http://bny.uphjek.com

[U91] JS：对象键值遍历
来源：http://ysy.ivvv.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://uhk.zhiwuduotai.top

[U92] JS：深拷贝
来源：http://znd.hnxiangtu.top

structuredClone(obj)
来源：http://vfy.cashguo.top

[U93] JS：模板字符串
来源：http://ryh.shanyushiyangkeji.top

`共 ${n} 条`
来源：http://opm.hcnkem.com

[U94] JS：箭头函数
来源：http://uhu.zycfv.cn

const double = x => x * 2;
来源：http://ccj.zhiwuduotai.top

[U95] JS：Promise 包装
来源：http://cbf.sjlbkw.cn

new Promise((resolve, reject) => {})
来源：http://slu.dashuyun.cn

[U96] JS：async/await 与异常
来源：http://mhw.dianchejie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xtg.aizwys.cn

[U97] JS：并发请求
来源：http://sst.jinyuanbaomall.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://nmj.hammf.cn

[U98] JS：fetch 带 JSON
来源：http://glq.kuanghao11.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cro.jqgufenzy.top

[U99] JS：事件监听
来源：http://zfr.epnwcf.com

el.addEventListener("click", e => {})
来源：http://tbd.hywenlv.cn

[U100] JS：DOM 查询
来源：http://ukz.hongshengwenyu.top

document.querySelector(".item")
来源：http://ftw.bjfxy.top

[U101] JS：classList 操作
来源：http://oxt.ppjwa.cn

el.classList.toggle("active")
来源：http://nmz.yonumen.top

[U102] JS：本地存储
来源：http://ern.guannengcc.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://nxv.wangdashe.top

[U103] JS：定时器
来源：http://vas.zdbjq.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://beb.jianghu66.top

[U104] JS：防抖
来源：http://flh.yangfankeji.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mlm.chenlongwang.top

[U105] JS：节流
来源：http://yye.jiagoushi.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ycs.9152youxi.cn

[U106] JS：日期格式化
来源：http://ded.birdmap.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://weg.yj20258888.top

[U107] JS：数字千分位
来源：http://heo.daria6918.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blx.yueranfly.top

[U108] JS：随机整数
来源：http://son.jlsjyb.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fbc.vehdjk.com

[U109] JS：数组分组
来源：http://nze.zhengqikj.top

Object.groupBy(arr, x => x.type)
来源：http://vfv.yueranfly.top

[U110] JS：数组分块
来源：http://nsh.chenlongwang.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gkl.nanxuanxn.top

[U111] JS：对象转 Map
来源：http://axp.nanxuanxn.top

new Map(Object.entries(obj))
来源：http://wdd.c1oappe.top

[U112] JS：字符串补位
来源：http://gam.zhengqikj.top

"7".padStart(3, "0")
来源：http://azm.jqgfzy.top

[U113] JS：正则替换全部
来源：http://uye.hesvh.cn

s.replaceAll("a", "b")
来源：http://yqe.feifeiyinyue.top

[U114] JS：JSON 深比较
来源：http://oys.vqdsnc.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://bnj.fengsongda.top

[U115] JS：生成 UUID
来源：http://wye.yj20258888.top

crypto.randomUUID()
来源：http://ram.sjlbkw.cn

[U116] JS：类型检查（JSDoc）
来源：http://axc.ehwqpu.com

/** @param {string} name */ function f(name) {}
来源：http://ytu.meibo888.top

[U117] JS：单元测试
来源：http://rpm.yangfankeji.com

npm i -D vitest;  npx vitest
来源：http://yzr.wangdashe.top

[U118] JS：开发服务器
来源：http://sgz.tianlin.xyz

npm i -D vite;  npx vite
来源：http://dua.fzhhl.top

[U119] JS：生产构建
来源：http://uzp.iojbl.cn

npx vite build
来源：http://lso.dianchejie.cn

[U120] JS：读取环境变量（Vite）
来源：http://jwg.feifeiyinyue.top

import.meta.env.VITE_API_URL
来源：http://hjl.zhijiandao.cn

================================================================================
来源：http://xiv.zdqjudy.top

统计汇总
来源：http://vgb.fengsongda.top

================================================================================
来源：http://dkv.fehbvm.com

按语言统计（条）：
来源：http://jef.jqgufenzy.top

Python ......... 252
来源：http://vlk.fktsv.cn

PHP ............ 252
来源：http://pxi.jqgufenzy.top

JavaScript ..... 252
来源：http://wzt.yanxiufei.cn

TypeScript ..... 212
来源：http://sho.shanyushiyangkeji.top

Java ........... 212
来源：http://rin.gaohongyu789.top

Go ............. 212
来源：http://ndq.cdnleiting.top

Ruby ........... 212
来源：http://rgn.sxryk.cn

C# ............. 212
来源：http://bvc.gaohongyu789.top

C .............. 30
来源：http://ppz.hongshengwenyu.top

C++ ............ 30
来源：http://arr.zhixingplan.top

SQL ............ 90
来源：http://bfp.shuidangran.top

Bash ........... 80
来源：http://ylk.tarul.cn

Kotlin ......... 15
来源：http://xlj.cashguo.top

Swift .......... 15
来源：http://fgb.yj20258.top

Lua ............ 10
来源：http://rga.ehwqpu.com

Perl ........... 10
来源：http://eoz.xziqi.cn

Scala .......... 10
来源：http://eqd.shzxlz.cn

------------------------------------
来源：http://hgv.fzhhl.top

合计 ........... 2106 条
来源：http://ete.bjfxy.top

按章节统计：
来源：http://ohh.yanxiufei.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nvs.wangdashe.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kni.quarkkingdee.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://stt.hesvh.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://meb.sjlbkw.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vbr.tianlin.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mey.zdbjq.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://puo.hesvh.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cyu.uphjek.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rng.cqqwz.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gwz.zhongyouzk.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sbg.zhixingplan.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vwj.gogol.net.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ofy.xingfuxueyuan.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://oeo.sweek.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cqg.zhixingplan.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ddg.pengpengdd.cyou

Q SQL 专题                              90
来源：http://buo.chenlongwang.top

R Bash 专题                             80
来源：http://qgw.fanxiaobao.xyz

S C / C++ 专题                          60
来源：http://stn.aibaodan.cn

T 其他语言补充                          60
来源：http://xmc.fengsongda.top

U 高频实用片段                         120
来源：http://kyc.tian-w.cn

------------------------------------
来源：http://lrj.yj202588.top

合计                                  2106 条
来源：http://exf.gogol.net.cn

--------------------------------------------------------------------------------
来源：http://fur.sufxvd.cn

使用提醒
来源：http://phi.tian-w.cn

--------------------------------------------------------------------------------
来源：http://ilu.xylfe.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hcj.gotoacloud.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xlc.cashguo.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://iki.jinqigufen.top

在旧版本上使用前请先确认语法支持情况。
来源：http://fjj.dianchejie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://oxl.xziqi.cn

—— 文件结束 ——
来源：http://xdp.shanyushiyangkeji.top

================================================================================
来源：http://pmj.zdbjq.cn

程序语言常见例子速查手册（2024 版）
来源：http://dar.jinghuilouyu.cn

Common Programming Examples Cheat Book
来源：http://roj.tanke756.top

================================================================================
来源：http://kmd.jinyuanbaomall.cn

【收录内容】
来源：http://phg.birdmap.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://zes.quarkkingdee.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fez.xziqi.cn

SQL · Bash · C · C++
来源：http://fsg.pengpengdd.cyou

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xax.hammf.cn

【使用说明】
来源：http://vui.bbcook.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qqf.zhijiandao.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wne.guannengcc.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://klo.zycfv.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ivw.0kj1m.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://uie.yonumen.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://fdk.9152youxi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rou.xuanzx.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mmj.gotoacloud.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rbt.andypj.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ldp.aizwys.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vjj.zycfv.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bqm.shanyushiyangtech.top

【文件统计】
来源：http://wdz.redwolf501.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wrg.fzhhl.top

--------------------------------------------------------------------------------
来源：http://hnz.meibo888.top

目  录
来源：http://bev.jyoumei.cn

--------------------------------------------------------------------------------
来源：http://awe.zhijiandao.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://puy.jinyuanbaomall.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://end.jlsjyb.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hdj.ehwqpu.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mbt.iojbl.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vnd.daria6918.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zex.hongshengwenyu.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://win.gotoacloud.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tmp.jianghu66.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tty.aibaodan.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xal.hysaishi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ttg.sjlbkw.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://leh.jqgfzy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dfa.gzhubu.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://nzi.0kj1m.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lto.havefunace.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ghf.havefunace.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://swj.yanxiufei.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://jvc.xziqi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://adt.guowangkeji.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ata.hysaishi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://akc.redwolf501.top

================================================================================
来源：http://wep.ehwqpu.com

A. 基础语法与类型
来源：http://ces.fktsv.cn

================================================================================
来源：http://max.sweek.top

[A01] Hello World
来源：http://gte.jinghuilouyu.cn

Py:   print("Hello, World!")
来源：http://rcw.sufxvd.cn

PHP:  echo "Hello, World!";
来源：http://xll.fzhhl.top

JS:   console.log("Hello, World!");
来源：http://yxg.meibo888.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gqy.wangshuangyany.cn

Java: System.out.println("Hello, World!");
来源：http://nkb.jqgfzy.top

Go:   fmt.Println("Hello, World!")
来源：http://nfx.shzxlz.cn

Ruby: puts "Hello, World!"
来源：http://ovo.cucudq.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://tmq.ydzc1.top

[A02] 变量声明与赋值
来源：http://uwo.tanke756.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jyb.yuanzhike.top

PHP:  $name = "Alex"; $age = 20;
来源：http://gll.xuanzx.com

JS:   let name = "Alex"; const age = 20;
来源：http://ltz.pycfn.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rfa.tanke756.top

Java: String name = "Alex"; int age = 20;
来源：http://qwf.fktsv.cn

Go:   name := "Alex"; age := 20
来源：http://vtk.fanxiaobao.xyz

Ruby: name = "Alex"; age = 20
来源：http://uvi.gogol.net.cn

C#:   string name = "Alex"; int age = 20;
来源：http://mcw.xuanzx.com

[A03] 常量定义
来源：http://yhg.xingfuxueyuan.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qow.yfazqb.com

PHP:  const PI = 3.14159;
来源：http://oxt.zhongyouzk.top

JS:   const PI = 3.14159;
来源：http://evq.zhengqikj.top

TS:   const PI: number = 3.14159;
来源：http://dmb.tian-w.cn

Java: static final double PI = 3.14159;
来源：http://hpu.ivvv.top

Go:   const PI = 3.14159
来源：http://eoc.svipenyu.cn

Ruby: PI = 3.14159
来源：http://cec.andypj.xyz

C#:   const double PI = 3.14159;
来源：http://kug.xylfe.cn

[A04] 判断变量类型
来源：http://eio.meibo888.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://kam.xinyue.icu

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hni.cucudq.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://axd.yj20258888.top

TS:   typeof x; x instanceof Date
来源：http://ppz.ctjpmb.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ibh.zdqjudy.top

Go:   reflect.TypeOf(x).Name()
来源：http://aan.quarkkingdee.top

Ruby: x.class; x.is_a?(Integer)
来源：http://fzo.pengpengdd.cyou

C#:   x.GetType().Name; x is int
来源：http://yqc.daria6918.cn

[A05] 整数除法与取模
来源：http://hgl.daxiang520.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ipk.xuanzx.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://pzb.hammf.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qpu.aizwys.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kpv.zhengqikj.top

Java: 7 / 2; 7 % 2
来源：http://fse.dianchejie.cn

Go:   7 / 2; 7 % 2
来源：http://csz.zycfv.cn

Ruby: 7 / 2; 7 % 2
来源：http://gfn.sweek.top

C#:   7 / 2; 7 % 2
来源：http://noq.zhiwuduotai.top

[A06] 字符串转数字
来源：http://nin.ivvv.top

Py:   int("42"); float("3.14")
来源：http://grt.snrcjt.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://yut.fengsongda.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xmk.fzhhl.top

TS:   parseInt("42", 10); Number("42")
来源：http://zsm.kuanghao11.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ddf.ivvv.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://doj.hesvh.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ojl.kuanghao11.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vxw.redwolf501.top

[A07] 数字转字符串
来源：http://urw.wangshuangyany.cn

Py:   str(42)
来源：http://zol.haohaochexian.top

PHP:  (string) 42; strval(42)
来源：http://hph.nwbrower.top


<!-- 参考信息 -->