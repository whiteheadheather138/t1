代发 wailian999

[U55] PHP：match 表达式
来源：http://wle.fzhhl.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lds.zdbjq.cn

[U56] PHP：命名参数
来源：http://chk.jinghuilouyu.cn

f(a: 1, b: 2)
来源：http://pal.shanyushiyangkeji.top

[U57] PHP：字符串插值
来源：http://hqu.wangdashe.top

"值: {$a}"
来源：http://sba.ybcxt.top

[U58] PHP：数组三件套
来源：http://wsy.bjfxy.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sxi.meibo888.top

[U59] PHP：自定义排序
来源：http://ykr.jinyuanbaomall.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qnf.sjlbkw.cn

[U60] PHP：JSON 编解码
来源：http://sfb.birdmap.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xsm.bjfxy.top

[U61] PHP：正则
来源：http://bqr.hammf.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nfw.daxiang520.top

[U62] PHP：日期对象
来源：http://lfq.fktsv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rrj.fengsongda.top

[U63] PHP：文件读写
来源：http://blx.sysykeji.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yhz.zhengqikj.top

[U64] PHP：目录遍历
来源：http://tcn.xziqi.cn

glob("dir/*.php");  scandir("dir");
来源：http://czr.haohaochexian.top

[U65] PHP：会话
来源：http://wuz.jyoumei.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://mhh.gaohongyu789.top

[U66] PHP：设置 Cookie
来源：http://ket.gaohongyu789.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://toq.yueranfly.top

[U67] PHP：处理文件上传
来源：http://hlw.zhiwuduotai.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gwo.snrcjt.cn

[U68] PHP：PDO 连接
来源：http://lqk.0kj1m.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hkh.tian-w.cn

[U69] PHP：PDO 预处理
来源：http://qgu.yuxming.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hhp.tanke756.top

[U70] PHP：PDO 事务
来源：http://qpc.shangyingyoupin.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://daf.shuidangran.top

[U71] PHP：抛出异常
来源：http://eka.wangshuangyany.cn

throw new RuntimeException("失败", 500);
来源：http://mek.zhaomingkeji.xyz

[U72] PHP：写错误日志
来源：http://rqj.ybcxt.top

error_log("失败: " . $e->getMessage());
来源：http://zom.wangdashe.top

[U73] PHP：读取 ini 配置
来源：http://alm.ehwqpu.com

parse_ini_file("config.ini", true)
来源：http://jbm.chenjidiqi.icu

[U74] PHP：读取环境变量
来源：http://sta.daxiang520.top

getenv("APP_ENV") ?: "production"
来源：http://rlw.jqgfzy.top

[U75] PHP：依赖注入
来源：http://pxv.hywenlv.cn

composer require psr/container
来源：http://eju.jlsjyb.cn

[U76] PHP：简单路由
来源：http://cbu.jinqigufen.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://opc.jinyuanbaomall.cn

[U77] PHP：模板渲染
来源：http://aua.chenzaomai.com

composer require twig/twig
来源：http://sua.shuidangran.top

[U78] PHP：单元测试
来源：http://qyp.cheryme.top

composer require --dev phpunit/phpunit
来源：http://wwh.dashuyun.cn

[U79] PHP：静态分析
来源：http://lnl.gotoacloud.top

composer require --dev phpstan/phpstan
来源：http://beg.jinyuanbaomall.cn

[U80] PHP：代码规范修复
来源：http://tst.9152youxi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://voj.tian-w.cn

[U81] JS：初始化项目
来源：http://epq.jinyuanbaomall.cn

npm init -y;  npm i express
来源：http://pdf.nwbrower.top

[U82] JS：package.json 脚本
来源：http://trs.fengsongda.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xzb.cdnleiting.top

[U83] JS：ES Module 导入导出
来源：http://ivf.xuetiantiany.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ngd.vehdjk.com

[U84] JS：CommonJS 写法
来源：http://alu.ppjwa.cn

module.exports = { a };  const { a } = require("./m");
来源：http://vpv.birdmap.top

[U85] JS：可选链
来源：http://zfb.chenjidiqi.icu

a?.b?.c
来源：http://eqj.shuidangran.top

[U86] JS：空值合并
来源：http://hur.havefunace.top

a ?? b
来源：http://sin.haohaochexian.top

[U87] JS：解构默认值
来源：http://orb.vehdjk.com

const { a = 1, b = 2 } = obj;
来源：http://pwn.sufxvd.cn

[U88] JS：对象展开合并
来源：http://imm.shangyingyoupin.top

{ ...a, ...b }
来源：http://ddx.sufxvd.cn

[U89] JS：数组去重
来源：http://ehm.yj20258888.top

[...new Set(arr)]
来源：http://lyz.52xcode.cn

[U90] JS：数字数组排序
来源：http://rby.shangyingyoupin.top

[...arr].sort((a, b) => a - b)
来源：http://kpf.ywan-chungtsiang.top

[U91] JS：对象键值遍历
来源：http://fit.andypj.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fvc.hfpthk.cn

[U92] JS：深拷贝
来源：http://wns.jqgufenzy.top

structuredClone(obj)
来源：http://hwe.havefunace.top

[U93] JS：模板字符串
来源：http://zvu.redwolf501.top

`共 ${n} 条`
来源：http://swu.jlsjyb.cn

[U94] JS：箭头函数
来源：http://oqj.kuanghao11.cn

const double = x => x * 2;
来源：http://rcp.9152youxi.cn

[U95] JS：Promise 包装
来源：http://svf.zhijiandao.cn

new Promise((resolve, reject) => {})
来源：http://chn.hammf.cn

[U96] JS：async/await 与异常
来源：http://tvk.shanyushiyangtech.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ayj.yj202588.top

[U97] JS：并发请求
来源：http://lxn.shanyushiyangtech.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://pjt.fzhhl.top

[U98] JS：fetch 带 JSON
来源：http://ten.fengsongda.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jbw.hcnkem.com

[U99] JS：事件监听
来源：http://hcu.sxryk.cn

el.addEventListener("click", e => {})
来源：http://pzp.shuidangran.top

[U100] JS：DOM 查询
来源：http://ltd.zdbjq.cn

document.querySelector(".item")
来源：http://sgi.nanxinkj.top

[U101] JS：classList 操作
来源：http://iuv.hongshengwenyu.top

el.classList.toggle("active")
来源：http://vwe.zycfv.cn

[U102] JS：本地存储
来源：http://yal.yj20258888.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ihx.0kj1m.cn

[U103] JS：定时器
来源：http://qgu.zdbjq.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://eli.fengsongda.top

[U104] JS：防抖
来源：http://bae.yj20258888.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ieu.sufxvd.cn

[U105] JS：节流
来源：http://bbz.haohaochexian.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tse.vehdjk.com

[U106] JS：日期格式化
来源：http://rno.yj20258.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pke.cdnleiting.top

[U107] JS：数字千分位
来源：http://ppl.dashuyun.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xqv.yj202588.top

[U108] JS：随机整数
来源：http://spf.kuanghao11.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://iuu.xinyue.icu

[U109] JS：数组分组
来源：http://jvj.nanxuanxn.top

Object.groupBy(arr, x => x.type)
来源：http://xek.jinyuanbaomall.cn

[U110] JS：数组分块
来源：http://lbv.sufxvd.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jfg.tarul.cn

[U111] JS：对象转 Map
来源：http://ebc.yuxming.cn

new Map(Object.entries(obj))
来源：http://rfk.tian-w.cn

[U112] JS：字符串补位
来源：http://jcc.fengsongda.top

"7".padStart(3, "0")
来源：http://ugk.nwbrower.top

[U113] JS：正则替换全部
来源：http://tdx.tarul.cn

s.replaceAll("a", "b")
来源：http://clo.jianghu66.top

[U114] JS：JSON 深比较
来源：http://gwl.sysykeji.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://bwc.52xcode.cn

[U115] JS：生成 UUID
来源：http://tqq.fzhhl.top

crypto.randomUUID()
来源：http://jba.yonumen.top

[U116] JS：类型检查（JSDoc）
来源：http://txh.yvedp.cn

/** @param {string} name */ function f(name) {}
来源：http://nqa.cqqwz.cn

[U117] JS：单元测试
来源：http://tdl.aizwys.cn

npm i -D vitest;  npx vitest
来源：http://yju.sysykeji.top

[U118] JS：开发服务器
来源：http://all.meibo888.top

npm i -D vite;  npx vite
来源：http://rfn.tian-w.cn

[U119] JS：生产构建
来源：http://dwi.jinqigfzy.top

npx vite build
来源：http://hza.0kj1m.cn

[U120] JS：读取环境变量（Vite）
来源：http://zfn.cdnleiting.top

import.meta.env.VITE_API_URL
来源：http://gxp.daria6918.cn

================================================================================
来源：http://cnk.cqqwz.cn

统计汇总
来源：http://euh.gotoacloud.top

================================================================================
来源：http://rry.hysaishi.cn

按语言统计（条）：
来源：http://bhk.hnxiangtu.top

Python ......... 252
来源：http://his.xziqi.cn

PHP ............ 252
来源：http://fjc.jqgfzy.top

JavaScript ..... 252
来源：http://zlm.cheryme.top

TypeScript ..... 212
来源：http://pkk.shanyushiyangtech.top

Java ........... 212
来源：http://jki.hammf.cn

Go ............. 212
来源：http://kpz.hnxiangtu.top

Ruby ........... 212
来源：http://pjm.cashguo.top

C# ............. 212
来源：http://etz.zdbjq.cn

C .............. 30
来源：http://fhg.iojbl.cn

C++ ............ 30
来源：http://zhe.fzhhl.top

SQL ............ 90
来源：http://agw.hesvh.cn

Bash ........... 80
来源：http://njt.xuetiantiany.cn

Kotlin ......... 15
来源：http://zbu.yuanzhike.top

Swift .......... 15
来源：http://fla.xingfuxueyuan.xyz

Lua ............ 10
来源：http://ugl.fanxiaobao.xyz

Perl ........... 10
来源：http://gvu.chenlongwang.top

Scala .......... 10
来源：http://mek.hesvh.cn

------------------------------------
来源：http://oce.meibo888.top

合计 ........... 2106 条
来源：http://veq.shzxlz.cn

按章节统计：
来源：http://xxl.ywan-chungtsiang.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cnx.hammf.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bmx.hongshengwenyu.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://snh.ppjwa.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sji.gzhubu.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tqr.jinqigfzy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mkz.yfazqb.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ytb.tian-w.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xxr.tarul.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://egw.yongpay.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vlx.xziqi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zle.wangdashe.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://omi.nanxinkj.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lmx.epnwcf.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wsq.jiagoushi.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blq.ydjk.org.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://myl.zhengqikj.top

Q SQL 专题                              90
来源：http://zaj.cucudq.cn

R Bash 专题                             80
来源：http://jva.guowangkeji.top

S C / C++ 专题                          60
来源：http://evk.bjfxy.top

T 其他语言补充                          60
来源：http://znf.wangshuangyany.cn

U 高频实用片段                         120
来源：http://dfx.fktsv.cn

------------------------------------
来源：http://dmw.quarkkingdee.top

合计                                  2106 条
来源：http://nhg.yueranfly.top

--------------------------------------------------------------------------------
来源：http://rpi.jlsjyb.cn

使用提醒
来源：http://ysz.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://pxr.zhengqikj.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://evn.wangshuangyany.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://sqh.pycfn.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tus.cucudq.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://rsy.smart0.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mwe.xuetiantiany.cn

—— 文件结束 ——
来源：http://kuy.ybcxt.top

================================================================================
来源：http://ghf.dashuyun.cn

程序语言常见例子速查手册（2024 版）
来源：http://cnc.cheryme.top

Common Programming Examples Cheat Book
来源：http://hco.chenlongwang.top

================================================================================
来源：http://fyz.havefunace.top

【收录内容】
来源：http://hhd.feifeiyinyue.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://vlq.gzhubu.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mos.cdnleiting.top

SQL · Bash · C · C++
来源：http://uoe.shanyushiyangkeji.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lwh.ehwqpu.com

【使用说明】
来源：http://itf.fktsv.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gog.jqgufenzy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hcm.shanyushiyangkeji.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://iwa.zhijiandao.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jtt.vehdjk.com

Bash:  Shell         C:     C             C++:   C++
来源：http://whh.316326.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://spq.yuxming.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gmd.cqqwz.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://efk.zhijiandao.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gym.hesvh.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lbl.sysykeji.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kge.zhijiandao.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ilf.hcnkem.com

【文件统计】
来源：http://asu.chenjidiqi.icu

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://aca.jqgfzy.top

--------------------------------------------------------------------------------
来源：http://qpx.dashuyun.cn

目  录
来源：http://afq.yj20258888.top

--------------------------------------------------------------------------------
来源：http://hdt.xylfe.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qxk.nanxuanxn.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cfp.sjlbkw.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://upq.shangyingyoupin.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ssy.zhixingplan.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ufl.jqgfzy.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://sqo.guannengcc.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jlv.yj202588.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pxw.nanxinkj.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rdf.zycfv.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vcg.dianchejie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jsu.jqgufenzy.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dug.daxiang520.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xqw.gaohongyu789.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cbd.jlsjyb.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ttm.fzhhl.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://seg.vehdjk.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ktx.haohaochexian.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://mlp.andypj.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rgt.cqqwz.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://avt.yj20258.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zuh.tian-w.cn

================================================================================
来源：http://qkc.xingfuxueyuan.xyz

A. 基础语法与类型
来源：http://pph.zhengqikj.top

================================================================================
来源：http://mcg.mhx1999.top

[A01] Hello World
来源：http://hev.xziqi.cn

Py:   print("Hello, World!")
来源：http://lvw.cdnleiting.top

PHP:  echo "Hello, World!";
来源：http://uic.sufxvd.cn

JS:   console.log("Hello, World!");
来源：http://usb.mhx1999.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://oka.andypj.xyz

Java: System.out.println("Hello, World!");
来源：http://cpn.nanxinkj.top

Go:   fmt.Println("Hello, World!")
来源：http://nen.hcnkem.com

Ruby: puts "Hello, World!"
来源：http://sle.ctjpmb.com

C#:   Console.WriteLine("Hello, World!");
来源：http://fli.jlsjyb.cn

[A02] 变量声明与赋值
来源：http://lrn.316326.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://foj.shuidangran.top

PHP:  $name = "Alex"; $age = 20;
来源：http://awt.cashguo.top

JS:   let name = "Alex"; const age = 20;
来源：http://lee.ybcxt.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vgk.fehbvm.com

Java: String name = "Alex"; int age = 20;
来源：http://joq.cheryme.top

Go:   name := "Alex"; age := 20
来源：http://bxr.fzhhl.top

Ruby: name = "Alex"; age = 20
来源：http://ucd.dianchejie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://myi.bjfxy.top

[A03] 常量定义
来源：http://qpd.yuanzhike.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kuu.bjfxy.top

PHP:  const PI = 3.14159;
来源：http://fnu.aibaodan.cn

JS:   const PI = 3.14159;
来源：http://iqj.yj20258888.top

TS:   const PI: number = 3.14159;
来源：http://ivz.9152youxi.cn

Java: static final double PI = 3.14159;
来源：http://byn.fanxiaobao.xyz

Go:   const PI = 3.14159
来源：http://rxx.sjlbkw.cn

Ruby: PI = 3.14159
来源：http://qcc.yanxiufei.cn

C#:   const double PI = 3.14159;
来源：http://xhr.feifeiyinyue.top

[A04] 判断变量类型
来源：http://syg.jiagoushi.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://olx.shanyushiyangtech.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ycu.dashuyun.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qpj.nanxinkj.top

TS:   typeof x; x instanceof Date
来源：http://vuv.zhoulong.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fou.fengsongda.top

Go:   reflect.TypeOf(x).Name()
来源：http://wou.ivvv.top

Ruby: x.class; x.is_a?(Integer)
来源：http://bgm.sweek.top

C#:   x.GetType().Name; x is int
来源：http://gnz.birdmap.top

[A05] 整数除法与取模
来源：http://jyz.guowangkeji.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lyh.cashguo.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://uqv.jinqigfzy.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://rui.bjfxy.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://noi.shzxlz.cn

Java: 7 / 2; 7 % 2
来源：http://uih.pycfn.com

Go:   7 / 2; 7 % 2
来源：http://mup.hfpthk.cn

Ruby: 7 / 2; 7 % 2
来源：http://tqg.sxryk.cn

C#:   7 / 2; 7 % 2
来源：http://lzy.c1oappe.top

[A06] 字符串转数字
来源：http://bdj.zdbjq.cn

Py:   int("42"); float("3.14")
来源：http://tzx.jinyuanbaomall.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://azy.wangdashe.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qzv.hnqzz.top

TS:   parseInt("42", 10); Number("42")
来源：http://env.cheryme.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vvx.yongpay.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tet.zdbjq.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://faw.kuanghao11.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qlf.aibaodan.cn

[A07] 数字转字符串
来源：http://pqm.fengsongda.top

Py:   str(42)
来源：http://vbv.yuxming.cn

PHP:  (string) 42; strval(42)
来源：http://kbo.c1oappe.top

JS:   String(42); (42).toString()
来源：http://glb.pengpengdd.cyou

TS:   String(42)
来源：http://ipi.jinqigfzy.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://abz.wangshuangyany.cn

Go:   strconv.Itoa(42)
来源：http://lfv.sxryk.cn


<!-- 参考信息 -->