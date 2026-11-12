代发 wailian999

[U57] PHP：字符串插值
来源：http://uao.hywenlv.cn

"值: {$a}"
来源：http://wgu.tianlin.xyz

[U58] PHP：数组三件套
来源：http://wrp.xylfe.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hee.sysykeji.top

[U59] PHP：自定义排序
来源：http://luk.sysykeji.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pbh.vehdjk.com

[U60] PHP：JSON 编解码
来源：http://lcy.jqgfzy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nrh.gzhubu.top

[U61] PHP：正则
来源：http://ijd.hfpthk.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nks.cucudq.cn

[U62] PHP：日期对象
来源：http://jvd.shangyingyoupin.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ozz.yanxiufei.cn

[U63] PHP：文件读写
来源：http://zdc.yfazqb.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tnz.tanke756.top

[U64] PHP：目录遍历
来源：http://tyf.jinghuilouyu.cn

glob("dir/*.php");  scandir("dir");
来源：http://rez.chenjidiqi.icu

[U65] PHP：会话
来源：http://jtx.hysaishi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://tpn.kuanghao11.cn

[U66] PHP：设置 Cookie
来源：http://gjz.svipenyu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ltt.ctjpmb.com

[U67] PHP：处理文件上传
来源：http://gdt.zhiwuduotai.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mqw.guannengcc.top

[U68] PHP：PDO 连接
来源：http://cqm.tanke756.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dlz.haohaochexian.top

[U69] PHP：PDO 预处理
来源：http://xnh.mhx1999.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://thk.yueranfly.top

[U70] PHP：PDO 事务
来源：http://sym.vehdjk.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qby.fehbvm.com

[U71] PHP：抛出异常
来源：http://mrn.zycfv.cn

throw new RuntimeException("失败", 500);
来源：http://lfv.zhongyouzk.top

[U72] PHP：写错误日志
来源：http://vbg.tarul.cn

error_log("失败: " . $e->getMessage());
来源：http://qoh.fehbvm.com

[U73] PHP：读取 ini 配置
来源：http://ekr.hammf.cn

parse_ini_file("config.ini", true)
来源：http://vll.kuanghao11.cn

[U74] PHP：读取环境变量
来源：http://ucw.sysykeji.top

getenv("APP_ENV") ?: "production"
来源：http://jez.zhaomingkeji.xyz

[U75] PHP：依赖注入
来源：http://egb.jinyuanbaomall.cn

composer require psr/container
来源：http://dre.0kj1m.cn

[U76] PHP：简单路由
来源：http://ivk.yangfankeji.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fwz.ydjk.org.cn

[U77] PHP：模板渲染
来源：http://skb.gaohongyu789.top

composer require twig/twig
来源：http://xmo.fktsv.cn

[U78] PHP：单元测试
来源：http://zsl.vqdsnc.cn

composer require --dev phpunit/phpunit
来源：http://ntu.sufxvd.cn

[U79] PHP：静态分析
来源：http://rbq.jlsjyb.cn

composer require --dev phpstan/phpstan
来源：http://mzi.ivvv.top

[U80] PHP：代码规范修复
来源：http://bkd.bbcook.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://tvt.zhixingplan.top

[U81] JS：初始化项目
来源：http://siz.nanxinkj.top

npm init -y;  npm i express
来源：http://vqo.daria6918.cn

[U82] JS：package.json 脚本
来源：http://izd.jinghuilouyu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pwt.ydjk.org.cn

[U83] JS：ES Module 导入导出
来源：http://qmi.kuanghao11.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xgl.chenlongwang.top

[U84] JS：CommonJS 写法
来源：http://vek.nwbrower.top

module.exports = { a };  const { a } = require("./m");
来源：http://spv.yvedp.cn

[U85] JS：可选链
来源：http://dje.pengpengdd.cyou

a?.b?.c
来源：http://diw.dianchejie.cn

[U86] JS：空值合并
来源：http://qmj.yueranfly.top

a ?? b
来源：http://kfs.svipenyu.cn

[U87] JS：解构默认值
来源：http://huh.birdmap.top

const { a = 1, b = 2 } = obj;
来源：http://ntm.aizwys.cn

[U88] JS：对象展开合并
来源：http://pbd.ybcxt.top

{ ...a, ...b }
来源：http://ybn.zdbjq.cn

[U89] JS：数组去重
来源：http://rxw.hongshengwenyu.top

[...new Set(arr)]
来源：http://ipt.yvedp.cn

[U90] JS：数字数组排序
来源：http://kdk.xziqi.cn

[...arr].sort((a, b) => a - b)
来源：http://xbv.guannengcc.top

[U91] JS：对象键值遍历
来源：http://rrl.ydzc1.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://sjv.dianchejie.cn

[U92] JS：深拷贝
来源：http://htk.zhengqikj.top

structuredClone(obj)
来源：http://swn.9152youxi.cn

[U93] JS：模板字符串
来源：http://haa.ctjpmb.com

`共 ${n} 条`
来源：http://jos.jinyuanbaomall.cn

[U94] JS：箭头函数
来源：http://dwt.uphjek.com

const double = x => x * 2;
来源：http://tgf.guannengcc.top

[U95] JS：Promise 包装
来源：http://fam.hcnkem.com

new Promise((resolve, reject) => {})
来源：http://jgh.yfazqb.com

[U96] JS：async/await 与异常
来源：http://zzm.xziqi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qqu.tianlin.xyz

[U97] JS：并发请求
来源：http://nts.daria6918.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://gsf.wangdashe.top

[U98] JS：fetch 带 JSON
来源：http://knh.tianlin.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wnq.yongpay.top

[U99] JS：事件监听
来源：http://dnn.tian-w.cn

el.addEventListener("click", e => {})
来源：http://rtq.0kj1m.cn

[U100] JS：DOM 查询
来源：http://bmu.tarul.cn

document.querySelector(".item")
来源：http://vvu.52xcode.cn

[U101] JS：classList 操作
来源：http://bwy.yanxiufei.cn

el.classList.toggle("active")
来源：http://qih.cqqwz.cn

[U102] JS：本地存储
来源：http://kpf.xingfuxueyuan.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://fdv.xuanzx.com

[U103] JS：定时器
来源：http://olx.ivvv.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dmx.gaohongyu789.top

[U104] JS：防抖
来源：http://qly.jianghu66.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kpk.cdnleiting.top

[U105] JS：节流
来源：http://nuk.sysykeji.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://evq.zhengqikj.top

[U106] JS：日期格式化
来源：http://qlj.ctjpmb.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wex.jinqigfzy.top

[U107] JS：数字千分位
来源：http://awh.jinyuanbaomall.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ndx.havefunace.top

[U108] JS：随机整数
来源：http://akw.fanxiaobao.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ftj.xuetiantiany.cn

[U109] JS：数组分组
来源：http://mwk.shanyushiyangtech.top

Object.groupBy(arr, x => x.type)
来源：http://bgr.xziqi.cn

[U110] JS：数组分块
来源：http://qvt.hysaishi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ukl.chenlongwang.top

[U111] JS：对象转 Map
来源：http://zdf.zycfv.cn

new Map(Object.entries(obj))
来源：http://lcb.ydjk.org.cn

[U112] JS：字符串补位
来源：http://pvh.bjfxy.top

"7".padStart(3, "0")
来源：http://voi.zhiwuduotai.top

[U113] JS：正则替换全部
来源：http://hsg.yj20258888.top

s.replaceAll("a", "b")
来源：http://vez.zhongyouzk.top

[U114] JS：JSON 深比较
来源：http://wja.fehbvm.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://eif.fktsv.cn

[U115] JS：生成 UUID
来源：http://zpc.iojbl.cn

crypto.randomUUID()
来源：http://zni.pycfn.com

[U116] JS：类型检查（JSDoc）
来源：http://umg.bbcook.cn

/** @param {string} name */ function f(name) {}
来源：http://rzn.iojbl.cn

[U117] JS：单元测试
来源：http://xdw.yuanzhike.top

npm i -D vitest;  npx vitest
来源：http://rdk.aizwys.cn

[U118] JS：开发服务器
来源：http://exh.hesvh.cn

npm i -D vite;  npx vite
来源：http://grn.hcnkem.com

[U119] JS：生产构建
来源：http://ide.smart0.xyz

npx vite build
来源：http://lhj.sweek.top

[U120] JS：读取环境变量（Vite）
来源：http://lwv.aibaodan.cn

import.meta.env.VITE_API_URL
来源：http://ose.yueranfly.top

================================================================================
来源：http://dew.yj20258888.top

统计汇总
来源：http://wjb.cucudq.cn

================================================================================
来源：http://ezq.gogol.net.cn

按语言统计（条）：
来源：http://pdv.316326.xyz

Python ......... 252
来源：http://frq.redwolf501.top

PHP ............ 252
来源：http://ktu.fktsv.cn

JavaScript ..... 252
来源：http://ste.cdnleiting.top

TypeScript ..... 212
来源：http://rll.hongshengwenyu.top

Java ........... 212
来源：http://fud.hysaishi.cn

Go ............. 212
来源：http://ukk.yuxming.cn

Ruby ........... 212
来源：http://ztn.meibo888.top

C# ............. 212
来源：http://ylj.yuanzhike.top

C .............. 30
来源：http://hrm.redwolf501.top

C++ ............ 30
来源：http://yyi.nwbrower.top

SQL ............ 90
来源：http://zwp.jlsjyb.cn

Bash ........... 80
来源：http://ooq.shuidangran.top

Kotlin ......... 15
来源：http://pub.9152youxi.cn

Swift .......... 15
来源：http://keq.ehwqpu.com

Lua ............ 10
来源：http://kgb.quarkkingdee.top

Perl ........... 10
来源：http://lgo.tianlin.xyz

Scala .......... 10
来源：http://gjy.ivvv.top

------------------------------------
来源：http://fkl.feifeiyinyue.top

合计 ........... 2106 条
来源：http://vdm.tarul.cn

按章节统计：
来源：http://wdi.hcnkem.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dnx.jinghuilouyu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nqs.yj202588.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lic.aibaodan.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hjs.jinqigfzy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tvj.guannengcc.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mbf.zdbjq.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hxn.vehdjk.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nrk.cashguo.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qfx.bbcook.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fbr.jinqigfzy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://epa.ppjwa.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rmx.nanxinkj.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fdm.zdqjudy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xiq.hysaishi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ipl.meibo888.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nlx.0kj1m.cn

Q SQL 专题                              90
来源：http://adw.hcnkem.com

R Bash 专题                             80
来源：http://nzx.yuanzhike.top

S C / C++ 专题                          60
来源：http://kgc.hcnkem.com

T 其他语言补充                          60
来源：http://pdb.hysaishi.cn

U 高频实用片段                         120
来源：http://iik.jqgufenzy.top

------------------------------------
来源：http://esr.jqgufenzy.top

合计                                  2106 条
来源：http://oes.shanyushiyangtech.top

--------------------------------------------------------------------------------
来源：http://hyt.ehwqpu.com

使用提醒
来源：http://dcc.sufxvd.cn

--------------------------------------------------------------------------------
来源：http://qsw.tianlin.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ttb.jqgfzy.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tgc.zhaomingkeji.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ygq.pycfn.com

在旧版本上使用前请先确认语法支持情况。
来源：http://ras.ivvv.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://utr.vqdsnc.cn

—— 文件结束 ——
来源：http://ifh.sweek.top

================================================================================
来源：http://neb.yuanzhike.top

程序语言常见例子速查手册（2024 版）
来源：http://rya.nanxinkj.top

Common Programming Examples Cheat Book
来源：http://lwn.jinqigfzy.top

================================================================================
来源：http://pmj.jinyuanbaomall.cn

【收录内容】
来源：http://yos.52xcode.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://tsp.xuetiantiany.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xrj.cucudq.cn

SQL · Bash · C · C++
来源：http://dgi.hesvh.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ffs.yj202588.top

【使用说明】
来源：http://wpu.xuanzx.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://dsu.yj20258888.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xpw.yanxiufei.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://omd.hfpthk.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://euu.birdmap.top

Bash:  Shell         C:     C             C++:   C++
来源：http://gth.xylfe.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hrm.gogol.net.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vdw.zhixingplan.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mei.ppjwa.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vpm.hesvh.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vid.xziqi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qcz.kuanghao11.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://cjg.ivvv.top

【文件统计】
来源：http://cfi.zhiwuduotai.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fsm.feifeiyinyue.top

--------------------------------------------------------------------------------
来源：http://mlb.sysykeji.top

目  录
来源：http://dto.epnwcf.com

--------------------------------------------------------------------------------
来源：http://kre.52xcode.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qlu.jqgfzy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://fdn.sjlbkw.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://osw.yongpay.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://gbn.wangshuangyany.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rsq.quarkkingdee.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bgd.ivvv.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jlc.yangfankeji.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pbb.dianchejie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hyw.jinqigufen.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nnq.hysaishi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zrf.iojbl.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://shy.316326.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qva.cqqwz.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yze.cdnleiting.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fpc.gotoacloud.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jtm.gogol.net.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dnt.xziqi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://eyp.kuanghao11.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://dvr.gotoacloud.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ipa.dashuyun.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cmg.hnxiangtu.top

================================================================================
来源：http://dfa.zdqjudy.top

A. 基础语法与类型
来源：http://pdf.shangyingyoupin.top

================================================================================
来源：http://zqc.ehwqpu.com

[A01] Hello World
来源：http://mqm.shzxlz.cn

Py:   print("Hello, World!")
来源：http://hmp.hesvh.cn

PHP:  echo "Hello, World!";
来源：http://miy.guowangkeji.top

JS:   console.log("Hello, World!");
来源：http://qxd.bbcook.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mnc.bjfxy.top

Java: System.out.println("Hello, World!");
来源：http://sak.aizwys.cn

Go:   fmt.Println("Hello, World!")
来源：http://qjg.wangshuangyany.cn

Ruby: puts "Hello, World!"
来源：http://hju.iojbl.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://dbt.wangshuangyany.cn

[A02] 变量声明与赋值
来源：http://fiw.316326.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://eem.0kj1m.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://tty.chenlongwang.top

JS:   let name = "Alex"; const age = 20;
来源：http://rmr.sufxvd.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://uvv.hnxiangtu.top

Java: String name = "Alex"; int age = 20;
来源：http://iuc.yfazqb.com

Go:   name := "Alex"; age := 20
来源：http://edz.zdbjq.cn

Ruby: name = "Alex"; age = 20
来源：http://mdx.uphjek.com

C#:   string name = "Alex"; int age = 20;
来源：http://die.hongshengwenyu.top

[A03] 常量定义
来源：http://pgp.redwolf501.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wsf.epnwcf.com

PHP:  const PI = 3.14159;
来源：http://bbr.xziqi.cn

JS:   const PI = 3.14159;
来源：http://ehh.fehbvm.com

TS:   const PI: number = 3.14159;
来源：http://dce.zhixingplan.top

Java: static final double PI = 3.14159;
来源：http://ioj.quarkkingdee.top

Go:   const PI = 3.14159
来源：http://vjq.wangdashe.top

Ruby: PI = 3.14159
来源：http://qlq.yonumen.top

C#:   const double PI = 3.14159;
来源：http://mki.svipenyu.cn

[A04] 判断变量类型
来源：http://skd.zhengqikj.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://osn.yuxming.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://cdt.ctjpmb.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mbs.0kj1m.cn

TS:   typeof x; x instanceof Date
来源：http://xji.ywan-chungtsiang.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://eux.shanyushiyangtech.top

Go:   reflect.TypeOf(x).Name()
来源：http://ohf.9152youxi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://wwx.dashuyun.cn

C#:   x.GetType().Name; x is int
来源：http://nsm.aibaodan.cn

[A05] 整数除法与取模
来源：http://prh.yj20258.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lmu.xuetiantiany.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ebl.redwolf501.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://taz.birdmap.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://tps.zhixingplan.top

Java: 7 / 2; 7 % 2
来源：http://rid.sxryk.cn

Go:   7 / 2; 7 % 2
来源：http://icm.hesvh.cn

Ruby: 7 / 2; 7 % 2
来源：http://dwa.yanxiufei.cn

C#:   7 / 2; 7 % 2
来源：http://evi.jqgfzy.top

[A06] 字符串转数字
来源：http://zuw.fehbvm.com

Py:   int("42"); float("3.14")
来源：http://jma.xuanzx.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kot.xuetiantiany.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hdq.cheryme.top

TS:   parseInt("42", 10); Number("42")
来源：http://pdw.jianghu66.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tqd.kuanghao11.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cmc.zhaomingkeji.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://gus.kuanghao11.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://lfp.iojbl.cn

[A07] 数字转字符串
来源：http://uuj.zhaomingkeji.xyz

Py:   str(42)
来源：http://ilp.jinghuilouyu.cn

PHP:  (string) 42; strval(42)
来源：http://yxy.hysaishi.cn

JS:   String(42); (42).toString()
来源：http://ubu.guannengcc.top

TS:   String(42)
来源：http://tvh.kuanghao11.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://bpy.yj20258888.top

Go:   strconv.Itoa(42)
来源：http://fjd.tian-w.cn

Ruby: 42.to_s
来源：http://szu.hfpthk.cn

C#:   42.ToString()
来源：http://cul.snrcjt.cn

[A08] 取整与四舍五入
来源：http://yda.c1oappe.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pbh.xylfe.cn


<!-- 参考信息 -->