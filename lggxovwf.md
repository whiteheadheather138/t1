代发 wailian999

[U55] PHP：match 表达式
来源：http://oqp.yonumen.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kgm.sxryk.cn

[U56] PHP：命名参数
来源：http://wpr.guannengcc.top

f(a: 1, b: 2)
来源：http://sen.yj202588.top

[U57] PHP：字符串插值
来源：http://eqf.wangshuangyany.cn

"值: {$a}"
来源：http://trw.tarul.cn

[U58] PHP：数组三件套
来源：http://jls.meibo888.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://onl.jiagoushi.top

[U59] PHP：自定义排序
来源：http://zsq.wangdashe.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nrh.havefunace.top

[U60] PHP：JSON 编解码
来源：http://jsj.zhiwuduotai.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mec.52xcode.cn

[U61] PHP：正则
来源：http://kle.sysykeji.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kym.yj20258888.top

[U62] PHP：日期对象
来源：http://gwz.ivvv.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gxl.ivvv.top

[U63] PHP：文件读写
来源：http://fyw.hnqzz.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lfz.uphjek.com

[U64] PHP：目录遍历
来源：http://rrp.ppjwa.cn

glob("dir/*.php");  scandir("dir");
来源：http://ywq.cqqwz.cn

[U65] PHP：会话
来源：http://bxn.kuanghao11.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bns.feifeiyinyue.top

[U66] PHP：设置 Cookie
来源：http://oau.smart0.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ful.mhx1999.top

[U67] PHP：处理文件上传
来源：http://iea.smart0.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zxv.aibaodan.cn

[U68] PHP：PDO 连接
来源：http://mzb.fktsv.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vqf.wangdashe.top

[U69] PHP：PDO 预处理
来源：http://hsn.sysykeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rzl.kuanghao11.cn

[U70] PHP：PDO 事务
来源：http://dco.cqqwz.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hvi.316326.xyz

[U71] PHP：抛出异常
来源：http://uru.iojbl.cn

throw new RuntimeException("失败", 500);
来源：http://waf.hammf.cn

[U72] PHP：写错误日志
来源：http://ctj.sysykeji.top

error_log("失败: " . $e->getMessage());
来源：http://uyi.316326.xyz

[U73] PHP：读取 ini 配置
来源：http://ooz.jqgfzy.top

parse_ini_file("config.ini", true)
来源：http://mrg.guannengcc.top

[U74] PHP：读取环境变量
来源：http://olq.tarul.cn

getenv("APP_ENV") ?: "production"
来源：http://bke.hywenlv.cn

[U75] PHP：依赖注入
来源：http://jii.zhiwuduotai.top

composer require psr/container
来源：http://tcp.yvedp.cn

[U76] PHP：简单路由
来源：http://bqc.daxiang520.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yrp.hysaishi.cn

[U77] PHP：模板渲染
来源：http://wgv.zhijiandao.cn

composer require twig/twig
来源：http://bbp.iojbl.cn

[U78] PHP：单元测试
来源：http://btd.fanxiaobao.xyz

composer require --dev phpunit/phpunit
来源：http://qki.chenzaomai.com

[U79] PHP：静态分析
来源：http://ymn.zhoulong.xyz

composer require --dev phpstan/phpstan
来源：http://hbr.zdbjq.cn

[U80] PHP：代码规范修复
来源：http://zfu.aibaodan.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mys.52xcode.cn

[U81] JS：初始化项目
来源：http://rdy.zhoulong.xyz

npm init -y;  npm i express
来源：http://rdc.meibo888.top

[U82] JS：package.json 脚本
来源：http://xxo.feifeiyinyue.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://svu.guannengcc.top

[U83] JS：ES Module 导入导出
来源：http://pxr.xuetiantiany.cn

export const a = 1;  import { a } from "./m.js";
来源：http://wyk.jinqigfzy.top

[U84] JS：CommonJS 写法
来源：http://hfn.zdbjq.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pkd.jqgufenzy.top

[U85] JS：可选链
来源：http://vsk.daria6918.cn

a?.b?.c
来源：http://dvk.jianghu66.top

[U86] JS：空值合并
来源：http://nwm.ehwqpu.com

a ?? b
来源：http://oah.ivvv.top

[U87] JS：解构默认值
来源：http://qhe.wangdashe.top

const { a = 1, b = 2 } = obj;
来源：http://tlq.nanxuanxn.top

[U88] JS：对象展开合并
来源：http://vgo.zhiwuduotai.top

{ ...a, ...b }
来源：http://pyw.zhixingplan.top

[U89] JS：数组去重
来源：http://bqm.shanyushiyangtech.top

[...new Set(arr)]
来源：http://nfu.9152youxi.cn

[U90] JS：数字数组排序
来源：http://mkr.aibaodan.cn

[...arr].sort((a, b) => a - b)
来源：http://ggw.hnxiangtu.top

[U91] JS：对象键值遍历
来源：http://jcp.c1oappe.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://elw.cqqwz.cn

[U92] JS：深拷贝
来源：http://ihs.yangfankeji.com

structuredClone(obj)
来源：http://ikw.zhoulong.xyz

[U93] JS：模板字符串
来源：http://env.zdbjq.cn

`共 ${n} 条`
来源：http://jvb.havefunace.top

[U94] JS：箭头函数
来源：http://sor.chenlongwang.top

const double = x => x * 2;
来源：http://dun.kuanghao11.cn

[U95] JS：Promise 包装
来源：http://aqn.sxryk.cn

new Promise((resolve, reject) => {})
来源：http://gob.hnqzz.top

[U96] JS：async/await 与异常
来源：http://xee.jqgfzy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nid.yangfankeji.com

[U97] JS：并发请求
来源：http://rso.jinqigfzy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://evu.dianchejie.cn

[U98] JS：fetch 带 JSON
来源：http://oan.hysaishi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://oxm.uphjek.com

[U99] JS：事件监听
来源：http://prm.9152youxi.cn

el.addEventListener("click", e => {})
来源：http://pnp.zdqjudy.top

[U100] JS：DOM 查询
来源：http://tky.tian-w.cn

document.querySelector(".item")
来源：http://vog.yuxming.cn

[U101] JS：classList 操作
来源：http://xfz.hesvh.cn

el.classList.toggle("active")
来源：http://ddn.hesvh.cn

[U102] JS：本地存储
来源：http://vtv.ppjwa.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://swo.pycfn.com

[U103] JS：定时器
来源：http://wkf.hysaishi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dwu.dianchejie.cn

[U104] JS：防抖
来源：http://ohm.yj202588.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pun.meibo888.top

[U105] JS：节流
来源：http://dph.cucudq.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tqd.gotoacloud.top

[U106] JS：日期格式化
来源：http://aeq.redwolf501.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qoj.sysykeji.top

[U107] JS：数字千分位
来源：http://ium.haohaochexian.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cha.gaohongyu789.top

[U108] JS：随机整数
来源：http://czp.tian-w.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kqo.haohaochexian.top

[U109] JS：数组分组
来源：http://slu.zhiwuduotai.top

Object.groupBy(arr, x => x.type)
来源：http://vms.chenjidiqi.icu

[U110] JS：数组分块
来源：http://pud.yanxiufei.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tla.snrcjt.cn

[U111] JS：对象转 Map
来源：http://rta.xuetiantiany.cn

new Map(Object.entries(obj))
来源：http://yyc.fengsongda.top

[U112] JS：字符串补位
来源：http://oip.cucudq.cn

"7".padStart(3, "0")
来源：http://yeg.meibo888.top

[U113] JS：正则替换全部
来源：http://won.mhx1999.top

s.replaceAll("a", "b")
来源：http://bwh.shzxlz.cn

[U114] JS：JSON 深比较
来源：http://ybl.hongshengwenyu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://gej.cheryme.top

[U115] JS：生成 UUID
来源：http://jjj.yonumen.top

crypto.randomUUID()
来源：http://bgz.iojbl.cn

[U116] JS：类型检查（JSDoc）
来源：http://vmd.ehwqpu.com

/** @param {string} name */ function f(name) {}
来源：http://crm.yangfankeji.com

[U117] JS：单元测试
来源：http://fct.yuxming.cn

npm i -D vitest;  npx vitest
来源：http://vlh.vqdsnc.cn

[U118] JS：开发服务器
来源：http://toj.zhijiandao.cn

npm i -D vite;  npx vite
来源：http://net.jianghu66.top

[U119] JS：生产构建
来源：http://gir.vehdjk.com

npx vite build
来源：http://ggp.zhixingplan.top

[U120] JS：读取环境变量（Vite）
来源：http://mun.cucudq.cn

import.meta.env.VITE_API_URL
来源：http://vqz.redwolf501.top

================================================================================
来源：http://ysd.meibo888.top

统计汇总
来源：http://mbq.bjfxy.top

================================================================================
来源：http://mwl.andypj.xyz

按语言统计（条）：
来源：http://hon.zhixingplan.top

Python ......... 252
来源：http://swf.ppjwa.cn

PHP ............ 252
来源：http://gdx.wangshuangyany.cn

JavaScript ..... 252
来源：http://ssm.pengpengdd.cyou

TypeScript ..... 212
来源：http://ukv.yongpay.top

Java ........... 212
来源：http://arm.gogol.net.cn

Go ............. 212
来源：http://csz.smart0.xyz

Ruby ........... 212
来源：http://jky.redwolf501.top

C# ............. 212
来源：http://pkc.ybcxt.top

C .............. 30
来源：http://wvy.nanxinkj.top

C++ ............ 30
来源：http://ish.bbcook.cn

SQL ............ 90
来源：http://ihk.jinqigfzy.top

Bash ........... 80
来源：http://loz.dashuyun.cn

Kotlin ......... 15
来源：http://tvr.yangfankeji.com

Swift .......... 15
来源：http://atd.jyoumei.cn

Lua ............ 10
来源：http://qwa.cdnleiting.top

Perl ........... 10
来源：http://yyi.dianchejie.cn

Scala .......... 10
来源：http://lev.guannengcc.top

------------------------------------
来源：http://fid.pycfn.com

合计 ........... 2106 条
来源：http://dks.birdmap.top

按章节统计：
来源：http://but.chenjidiqi.icu

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kih.zhoulong.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tgz.shzxlz.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jgq.xziqi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fto.ctjpmb.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kms.tarul.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rqd.zhengqikj.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://enx.haohaochexian.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dvr.guannengcc.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dzm.jiagoushi.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://uxn.dashuyun.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://grc.sjlbkw.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gcy.xylfe.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bhx.jiagoushi.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://uiv.fktsv.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ume.vehdjk.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://aui.meibo888.top

Q SQL 专题                              90
来源：http://zhs.jianghu66.top

R Bash 专题                             80
来源：http://drd.ywan-chungtsiang.top

S C / C++ 专题                          60
来源：http://zoj.jqgufenzy.top

T 其他语言补充                          60
来源：http://xqo.yvedp.cn

U 高频实用片段                         120
来源：http://xfb.uphjek.com

------------------------------------
来源：http://vvh.nanxuanxn.top

合计                                  2106 条
来源：http://ezv.xuanzx.com

--------------------------------------------------------------------------------
来源：http://dal.meibo888.top

使用提醒
来源：http://qhm.shanyushiyangkeji.top

--------------------------------------------------------------------------------
来源：http://rxy.9152youxi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://eec.yvedp.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bvw.gotoacloud.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jnb.c1oappe.top

在旧版本上使用前请先确认语法支持情况。
来源：http://rfl.vqdsnc.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dam.zhixingplan.top

—— 文件结束 ——
来源：http://aqa.guowangkeji.top

================================================================================
来源：http://ala.zhiwuduotai.top

程序语言常见例子速查手册（2024 版）
来源：http://xyr.zdbjq.cn

Common Programming Examples Cheat Book
来源：http://ace.ydjk.org.cn

================================================================================
来源：http://hyn.hnxiangtu.top

【收录内容】
来源：http://ryy.tian-w.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ocp.hammf.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yat.yonumen.top

SQL · Bash · C · C++
来源：http://bye.wangshuangyany.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wyt.tanke756.top

【使用说明】
来源：http://esv.yvedp.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bpl.cashguo.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nkx.aibaodan.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bcm.shanyushiyangtech.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hbl.wangdashe.top

Bash:  Shell         C:     C             C++:   C++
来源：http://rts.sjlbkw.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lam.gzhubu.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://dbw.bbcook.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://geb.jyoumei.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jek.gotoacloud.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ruh.guannengcc.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bbu.andypj.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tlu.aizwys.cn

【文件统计】
来源：http://qpj.yj202588.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cuv.vqdsnc.cn

--------------------------------------------------------------------------------
来源：http://sri.yueranfly.top

目  录
来源：http://uca.vqdsnc.cn

--------------------------------------------------------------------------------
来源：http://hoc.cdnleiting.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://nuj.vqdsnc.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://whg.bbcook.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hbx.sysykeji.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://prl.zhaomingkeji.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mtc.316326.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xrq.pycfn.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nym.fzhhl.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ohb.xylfe.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://svq.fehbvm.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ebm.gotoacloud.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://kxh.jinqigufen.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zpx.yangfankeji.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vwr.shanyushiyangkeji.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://npf.9152youxi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://eod.zhongyouzk.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zpa.havefunace.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://plt.aizwys.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://qno.jinghuilouyu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://caw.zhixingplan.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://noy.zdbjq.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qxa.hnxiangtu.top

================================================================================
来源：http://xrf.ywan-chungtsiang.top

A. 基础语法与类型
来源：http://jfd.hongshengwenyu.top

================================================================================
来源：http://qvq.ivvv.top

[A01] Hello World
来源：http://edd.c1oappe.top

Py:   print("Hello, World!")
来源：http://wre.ydzc1.top

PHP:  echo "Hello, World!";
来源：http://hpu.guowangkeji.top

JS:   console.log("Hello, World!");
来源：http://kfq.sxryk.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rtu.zhengqikj.top

Java: System.out.println("Hello, World!");
来源：http://uan.gaohongyu789.top

Go:   fmt.Println("Hello, World!")
来源：http://jvk.pengpengdd.cyou

Ruby: puts "Hello, World!"
来源：http://qnh.nwbrower.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ago.aibaodan.cn

[A02] 变量声明与赋值
来源：http://ycp.epnwcf.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zfn.fanxiaobao.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://amh.jlsjyb.cn

JS:   let name = "Alex"; const age = 20;
来源：http://poe.xinyue.icu

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://itg.jinyuanbaomall.cn

Java: String name = "Alex"; int age = 20;
来源：http://zjt.sjlbkw.cn

Go:   name := "Alex"; age := 20
来源：http://fad.shzxlz.cn

Ruby: name = "Alex"; age = 20
来源：http://yhw.gaohongyu789.top

C#:   string name = "Alex"; int age = 20;
来源：http://iin.shzxlz.cn

[A03] 常量定义
来源：http://yab.havefunace.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jka.bjfxy.top

PHP:  const PI = 3.14159;
来源：http://tcv.hnxiangtu.top

JS:   const PI = 3.14159;
来源：http://elc.yj202588.top

TS:   const PI: number = 3.14159;
来源：http://tva.bjfxy.top

Java: static final double PI = 3.14159;
来源：http://nsk.hysaishi.cn

Go:   const PI = 3.14159
来源：http://twg.fehbvm.com

Ruby: PI = 3.14159
来源：http://vqq.svipenyu.cn

C#:   const double PI = 3.14159;
来源：http://lhz.jyoumei.cn

[A04] 判断变量类型
来源：http://kcp.sjlbkw.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://nha.cheryme.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hhr.cqqwz.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gve.zhiwuduotai.top

TS:   typeof x; x instanceof Date
来源：http://yuq.fzhhl.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xdu.gzhubu.top

Go:   reflect.TypeOf(x).Name()
来源：http://fgq.hesvh.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://fvu.redwolf501.top

C#:   x.GetType().Name; x is int
来源：http://egq.xuanzx.com

[A05] 整数除法与取模
来源：http://zct.zhongyouzk.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gko.daria6918.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://yns.gogol.net.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cyi.kuanghao11.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://sni.sufxvd.cn

Java: 7 / 2; 7 % 2
来源：http://yee.cqqwz.cn

Go:   7 / 2; 7 % 2
来源：http://zzc.ydjk.org.cn

Ruby: 7 / 2; 7 % 2
来源：http://fra.guannengcc.top

C#:   7 / 2; 7 % 2
来源：http://dpt.birdmap.top

[A06] 字符串转数字
来源：http://hsc.nanxuanxn.top

Py:   int("42"); float("3.14")
来源：http://fwu.chenzaomai.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mrv.tarul.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://sim.chenlongwang.top

TS:   parseInt("42", 10); Number("42")
来源：http://gud.vehdjk.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://caq.c1oappe.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://doa.yanxiufei.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://lii.ppjwa.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fmt.pengpengdd.cyou

[A07] 数字转字符串
来源：http://arp.pengpengdd.cyou

Py:   str(42)
来源：http://sre.bbcook.cn

PHP:  (string) 42; strval(42)
来源：http://ojc.epnwcf.com

JS:   String(42); (42).toString()
来源：http://qjb.zhongyouzk.top

TS:   String(42)
来源：http://vge.fzhhl.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://iqj.aizwys.cn

Go:   strconv.Itoa(42)
来源：http://ezg.zhaomingkeji.xyz


<!-- 参考信息 -->