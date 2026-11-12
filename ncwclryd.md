代发 wailian999

[U53] PHP：空合并运算符
来源：http://zkt.ydjk.org.cn

$v = $a ?? $b ?? "default";
来源：http://twi.yonumen.top

[U54] PHP：空安全调用
来源：http://zju.birdmap.top

$obj?->method()
来源：http://mdm.hammf.cn

[U55] PHP：match 表达式
来源：http://lry.yanxiufei.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cqx.c1oappe.top

[U56] PHP：命名参数
来源：http://wwo.redwolf501.top

f(a: 1, b: 2)
来源：http://nti.kuanghao11.cn

[U57] PHP：字符串插值
来源：http://vat.jqgufenzy.top

"值: {$a}"
来源：http://ipu.vqdsnc.cn

[U58] PHP：数组三件套
来源：http://akp.yvedp.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sel.jinqigfzy.top

[U59] PHP：自定义排序
来源：http://gjq.bjfxy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tcm.xinyue.icu

[U60] PHP：JSON 编解码
来源：http://eyl.zdbjq.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ifq.chenjidiqi.icu

[U61] PHP：正则
来源：http://tqe.dianchejie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lrx.tanke756.top

[U62] PHP：日期对象
来源：http://jng.c1oappe.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ehl.wangdashe.top

[U63] PHP：文件读写
来源：http://xiz.ydjk.org.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://glq.hnqzz.top

[U64] PHP：目录遍历
来源：http://zhy.hnqzz.top

glob("dir/*.php");  scandir("dir");
来源：http://ylk.aibaodan.cn

[U65] PHP：会话
来源：http://vav.nwbrower.top

session_start();  $_SESSION["uid"] = 1;
来源：http://oce.hesvh.cn

[U66] PHP：设置 Cookie
来源：http://ibe.ywan-chungtsiang.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hwy.jqgfzy.top

[U67] PHP：处理文件上传
来源：http://fpo.vqdsnc.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://plc.birdmap.top

[U68] PHP：PDO 连接
来源：http://xfa.vqdsnc.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ykb.ehwqpu.com

[U69] PHP：PDO 预处理
来源：http://joa.xylfe.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rub.jqgfzy.top

[U70] PHP：PDO 事务
来源：http://aga.guowangkeji.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kaq.redwolf501.top

[U71] PHP：抛出异常
来源：http://gox.ybcxt.top

throw new RuntimeException("失败", 500);
来源：http://jdt.aibaodan.cn

[U72] PHP：写错误日志
来源：http://wkr.nwbrower.top

error_log("失败: " . $e->getMessage());
来源：http://spq.fengsongda.top

[U73] PHP：读取 ini 配置
来源：http://csc.sufxvd.cn

parse_ini_file("config.ini", true)
来源：http://vcb.ppjwa.cn

[U74] PHP：读取环境变量
来源：http://hur.jinyuanbaomall.cn

getenv("APP_ENV") ?: "production"
来源：http://fen.cucudq.cn

[U75] PHP：依赖注入
来源：http://dgt.jinqigfzy.top

composer require psr/container
来源：http://ykf.bjfxy.top

[U76] PHP：简单路由
来源：http://srw.c1oappe.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uti.quarkkingdee.top

[U77] PHP：模板渲染
来源：http://hgn.52xcode.cn

composer require twig/twig
来源：http://hzf.ehwqpu.com

[U78] PHP：单元测试
来源：http://czw.birdmap.top

composer require --dev phpunit/phpunit
来源：http://wvf.sxryk.cn

[U79] PHP：静态分析
来源：http://mlv.aibaodan.cn

composer require --dev phpstan/phpstan
来源：http://uzd.shzxlz.cn

[U80] PHP：代码规范修复
来源：http://czj.zhiwuduotai.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://gyu.pengpengdd.cyou

[U81] JS：初始化项目
来源：http://bah.pengpengdd.cyou

npm init -y;  npm i express
来源：http://hpg.316326.xyz

[U82] JS：package.json 脚本
来源：http://fuc.zhoulong.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yxu.yj20258888.top

[U83] JS：ES Module 导入导出
来源：http://lby.cdnleiting.top

export const a = 1;  import { a } from "./m.js";
来源：http://zrq.ctjpmb.com

[U84] JS：CommonJS 写法
来源：http://kjy.c1oappe.top

module.exports = { a };  const { a } = require("./m");
来源：http://hlv.chenjidiqi.icu

[U85] JS：可选链
来源：http://idj.cucudq.cn

a?.b?.c
来源：http://ike.xuetiantiany.cn

[U86] JS：空值合并
来源：http://zue.gzhubu.top

a ?? b
来源：http://xom.ydzc1.top

[U87] JS：解构默认值
来源：http://bqx.iojbl.cn

const { a = 1, b = 2 } = obj;
来源：http://ctq.hcnkem.com

[U88] JS：对象展开合并
来源：http://mxk.xingfuxueyuan.xyz

{ ...a, ...b }
来源：http://jhp.c1oappe.top

[U89] JS：数组去重
来源：http://trl.ydjk.org.cn

[...new Set(arr)]
来源：http://qiw.52xcode.cn

[U90] JS：数字数组排序
来源：http://xag.zhiwuduotai.top

[...arr].sort((a, b) => a - b)
来源：http://qmq.aibaodan.cn

[U91] JS：对象键值遍历
来源：http://orm.vqdsnc.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lql.daria6918.cn

[U92] JS：深拷贝
来源：http://kmi.nanxuanxn.top

structuredClone(obj)
来源：http://cva.hnxiangtu.top

[U93] JS：模板字符串
来源：http://mxk.jinqigfzy.top

`共 ${n} 条`
来源：http://juj.haohaochexian.top

[U94] JS：箭头函数
来源：http://ggs.ywan-chungtsiang.top

const double = x => x * 2;
来源：http://bsm.sysykeji.top

[U95] JS：Promise 包装
来源：http://nlo.svipenyu.cn

new Promise((resolve, reject) => {})
来源：http://tha.hfpthk.cn

[U96] JS：async/await 与异常
来源：http://eih.hnqzz.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gzo.hcnkem.com

[U97] JS：并发请求
来源：http://ela.zhiwuduotai.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://czo.uphjek.com

[U98] JS：fetch 带 JSON
来源：http://abu.zhijiandao.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vnp.sufxvd.cn

[U99] JS：事件监听
来源：http://kwk.zhaomingkeji.xyz

el.addEventListener("click", e => {})
来源：http://uzi.316326.xyz

[U100] JS：DOM 查询
来源：http://lwp.andypj.xyz

document.querySelector(".item")
来源：http://yui.yj20258.top

[U101] JS：classList 操作
来源：http://ipl.9152youxi.cn

el.classList.toggle("active")
来源：http://bvy.mhx1999.top

[U102] JS：本地存储
来源：http://uii.316326.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://pfk.xingfuxueyuan.xyz

[U103] JS：定时器
来源：http://mnh.iojbl.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fhz.ivvv.top

[U104] JS：防抖
来源：http://nzl.yongpay.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uzi.tanke756.top

[U105] JS：节流
来源：http://pvg.cheryme.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ieo.zhijiandao.cn

[U106] JS：日期格式化
来源：http://buo.guowangkeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://noh.fehbvm.com

[U107] JS：数字千分位
来源：http://ykk.pengpengdd.cyou

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fiy.xziqi.cn

[U108] JS：随机整数
来源：http://xrk.ehwqpu.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rii.vehdjk.com

[U109] JS：数组分组
来源：http://xtd.yangfankeji.com

Object.groupBy(arr, x => x.type)
来源：http://hjr.c1oappe.top

[U110] JS：数组分块
来源：http://ivv.hammf.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qdr.yvedp.cn

[U111] JS：对象转 Map
来源：http://uft.yangfankeji.com

new Map(Object.entries(obj))
来源：http://vhy.guowangkeji.top

[U112] JS：字符串补位
来源：http://dcq.jiagoushi.top

"7".padStart(3, "0")
来源：http://uur.hywenlv.cn

[U113] JS：正则替换全部
来源：http://twd.jqgfzy.top

s.replaceAll("a", "b")
来源：http://ysr.ctjpmb.com

[U114] JS：JSON 深比较
来源：http://pqy.jinqigfzy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://lpf.fehbvm.com

[U115] JS：生成 UUID
来源：http://kjs.wangdashe.top

crypto.randomUUID()
来源：http://niz.xingfuxueyuan.xyz

[U116] JS：类型检查（JSDoc）
来源：http://qgc.svipenyu.cn

/** @param {string} name */ function f(name) {}
来源：http://yji.9152youxi.cn

[U117] JS：单元测试
来源：http://urn.zhijiandao.cn

npm i -D vitest;  npx vitest
来源：http://kzz.jyoumei.cn

[U118] JS：开发服务器
来源：http://wpp.jinghuilouyu.cn

npm i -D vite;  npx vite
来源：http://dck.sweek.top

[U119] JS：生产构建
来源：http://lcu.zhengqikj.top

npx vite build
来源：http://fay.ydjk.org.cn

[U120] JS：读取环境变量（Vite）
来源：http://goc.smart0.xyz

import.meta.env.VITE_API_URL
来源：http://mvc.fanxiaobao.xyz

================================================================================
来源：http://rmk.xinyue.icu

统计汇总
来源：http://kbf.birdmap.top

================================================================================
来源：http://vks.yangfankeji.com

按语言统计（条）：
来源：http://kfl.sjlbkw.cn

Python ......... 252
来源：http://qex.daxiang520.top

PHP ............ 252
来源：http://akk.feifeiyinyue.top

JavaScript ..... 252
来源：http://isw.zhijiandao.cn

TypeScript ..... 212
来源：http://ezy.hywenlv.cn

Java ........... 212
来源：http://gfj.pycfn.com

Go ............. 212
来源：http://qlh.epnwcf.com

Ruby ........... 212
来源：http://ncf.bbcook.cn

C# ............. 212
来源：http://uaf.cheryme.top

C .............. 30
来源：http://ezo.wangshuangyany.cn

C++ ............ 30
来源：http://ies.tanke756.top

SQL ............ 90
来源：http://alt.fzhhl.top

Bash ........... 80
来源：http://qte.meibo888.top

Kotlin ......... 15
来源：http://feu.jianghu66.top

Swift .......... 15
来源：http://neg.smart0.xyz

Lua ............ 10
来源：http://egm.dianchejie.cn

Perl ........... 10
来源：http://lnk.hammf.cn

Scala .......... 10
来源：http://upb.tarul.cn

------------------------------------
来源：http://ddj.fehbvm.com

合计 ........... 2106 条
来源：http://wxq.cashguo.top

按章节统计：
来源：http://ggf.wangdashe.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pae.hongshengwenyu.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hzt.gaohongyu789.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://msv.pycfn.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://khm.cucudq.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mes.shanyushiyangtech.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vok.0kj1m.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bfh.vehdjk.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fuj.guannengcc.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vft.cucudq.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ext.guowangkeji.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vfe.tarul.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://oly.ybcxt.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://frg.ivvv.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rkl.shanyushiyangtech.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gtf.bbcook.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xzv.yangfankeji.com

Q SQL 专题                              90
来源：http://pzu.ehwqpu.com

R Bash 专题                             80
来源：http://zvs.sjlbkw.cn

S C / C++ 专题                          60
来源：http://oll.zhijiandao.cn

T 其他语言补充                          60
来源：http://qqe.zhoulong.xyz

U 高频实用片段                         120
来源：http://uqu.fehbvm.com

------------------------------------
来源：http://jua.zhijiandao.cn

合计                                  2106 条
来源：http://zsv.hammf.cn

--------------------------------------------------------------------------------
来源：http://qnj.aizwys.cn

使用提醒
来源：http://vuu.jqgufenzy.top

--------------------------------------------------------------------------------
来源：http://hkw.ppjwa.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zal.ctjpmb.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qnl.jinyuanbaomall.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mxi.hfpthk.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://usk.jlsjyb.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://thm.hnqzz.top

—— 文件结束 ——
来源：http://lyv.cqqwz.cn

================================================================================
来源：http://tmy.sufxvd.cn

程序语言常见例子速查手册（2024 版）
来源：http://kun.aibaodan.cn

Common Programming Examples Cheat Book
来源：http://ygg.quarkkingdee.top

================================================================================
来源：http://cnc.yj202588.top

【收录内容】
来源：http://luj.dianchejie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://mkd.ppjwa.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jss.cheryme.top

SQL · Bash · C · C++
来源：http://rep.chenlongwang.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pch.ydjk.org.cn

【使用说明】
来源：http://zfl.zhijiandao.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jhf.vehdjk.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jwb.xylfe.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mov.zhoulong.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ykz.zhoulong.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://kew.hysaishi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://uom.jinghuilouyu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://oeu.yfazqb.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yae.fktsv.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vvs.xinyue.icu

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://liq.zhijiandao.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dgw.nanxuanxn.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://lkb.zhaomingkeji.xyz

【文件统计】
来源：http://zcr.hnqzz.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fpg.nanxuanxn.top

--------------------------------------------------------------------------------
来源：http://uka.feifeiyinyue.top

目  录
来源：http://zpj.uphjek.com

--------------------------------------------------------------------------------
来源：http://rcx.pycfn.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rrg.shzxlz.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://uob.zhixingplan.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wfz.gotoacloud.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xfe.hysaishi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://cdz.yonumen.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kvz.yj202588.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://iyq.cdnleiting.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fmf.yanxiufei.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lsl.zhoulong.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jph.nwbrower.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://kvu.meibo888.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lbx.fanxiaobao.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://iyz.jiagoushi.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gpa.yuanzhike.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mvk.ppjwa.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://sra.hywenlv.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bnw.hywenlv.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://anh.jyoumei.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://nmx.xinyue.icu

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pfu.cheryme.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pti.jinghuilouyu.cn

================================================================================
来源：http://isp.chenzaomai.com

A. 基础语法与类型
来源：http://wfr.epnwcf.com

================================================================================
来源：http://eyj.yj20258.top

[A01] Hello World
来源：http://ntz.cucudq.cn

Py:   print("Hello, World!")
来源：http://nib.wangshuangyany.cn

PHP:  echo "Hello, World!";
来源：http://sgc.quarkkingdee.top

JS:   console.log("Hello, World!");
来源：http://mha.gzhubu.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://sui.9152youxi.cn

Java: System.out.println("Hello, World!");
来源：http://una.tanke756.top

Go:   fmt.Println("Hello, World!")
来源：http://fns.jlsjyb.cn

Ruby: puts "Hello, World!"
来源：http://qmr.zhiwuduotai.top

C#:   Console.WriteLine("Hello, World!");
来源：http://naa.havefunace.top

[A02] 变量声明与赋值
来源：http://yyz.feifeiyinyue.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://stx.havefunace.top

PHP:  $name = "Alex"; $age = 20;
来源：http://yzp.guowangkeji.top

JS:   let name = "Alex"; const age = 20;
来源：http://blo.birdmap.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jna.gotoacloud.top

Java: String name = "Alex"; int age = 20;
来源：http://cut.xziqi.cn

Go:   name := "Alex"; age := 20
来源：http://fao.bjfxy.top

Ruby: name = "Alex"; age = 20
来源：http://xnf.52xcode.cn

C#:   string name = "Alex"; int age = 20;
来源：http://aow.aizwys.cn

[A03] 常量定义
来源：http://ujx.tarul.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hnf.birdmap.top

PHP:  const PI = 3.14159;
来源：http://elz.hysaishi.cn

JS:   const PI = 3.14159;
来源：http://cva.ehwqpu.com

TS:   const PI: number = 3.14159;
来源：http://int.snrcjt.cn

Java: static final double PI = 3.14159;
来源：http://jeg.epnwcf.com

Go:   const PI = 3.14159
来源：http://blq.hongshengwenyu.top

Ruby: PI = 3.14159
来源：http://ajy.9152youxi.cn

C#:   const double PI = 3.14159;
来源：http://hrw.dianchejie.cn

[A04] 判断变量类型
来源：http://wxj.zhaomingkeji.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://tjq.yongpay.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bhw.yongpay.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ifv.xuanzx.com

TS:   typeof x; x instanceof Date
来源：http://uzi.ydjk.org.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kvk.jinqigufen.top

Go:   reflect.TypeOf(x).Name()
来源：http://vbs.sjlbkw.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://kbx.jinqigfzy.top

C#:   x.GetType().Name; x is int
来源：http://oln.mhx1999.top

[A05] 整数除法与取模
来源：http://ukn.iojbl.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://epf.vqdsnc.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://drh.havefunace.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tra.zhijiandao.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jed.ydzc1.top

Java: 7 / 2; 7 % 2
来源：http://caf.yuanzhike.top

Go:   7 / 2; 7 % 2
来源：http://azo.dashuyun.cn

Ruby: 7 / 2; 7 % 2
来源：http://apq.zhengqikj.top

C#:   7 / 2; 7 % 2
来源：http://vul.guannengcc.top

[A06] 字符串转数字
来源：http://gph.9152youxi.cn

Py:   int("42"); float("3.14")
来源：http://twf.wangshuangyany.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://iib.yueranfly.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jav.pengpengdd.cyou

TS:   parseInt("42", 10); Number("42")
来源：http://fsk.ehwqpu.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://enx.yonumen.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qmj.hfpthk.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://mjc.nanxinkj.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zce.daxiang520.top

[A07] 数字转字符串
来源：http://ruu.xuanzx.com

Py:   str(42)
来源：http://msw.birdmap.top

PHP:  (string) 42; strval(42)
来源：http://fsr.yj202588.top


<!-- 参考信息 -->