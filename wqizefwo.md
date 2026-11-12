代发 wailian999

[U57] PHP：字符串插值
来源：http://dmi.chenlongwang.top

"值: {$a}"
来源：http://mgn.hammf.cn

[U58] PHP：数组三件套
来源：http://sqh.haohaochexian.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hrp.xziqi.cn

[U59] PHP：自定义排序
来源：http://whx.fktsv.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pkw.vqdsnc.cn

[U60] PHP：JSON 编解码
来源：http://obz.jinghuilouyu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xdt.c1oappe.top

[U61] PHP：正则
来源：http://kyz.wangshuangyany.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jcg.hnqzz.top

[U62] PHP：日期对象
来源：http://avb.daria6918.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://djo.gogol.net.cn

[U63] PHP：文件读写
来源：http://xkk.wangdashe.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lik.ivvv.top

[U64] PHP：目录遍历
来源：http://ayy.yj20258888.top

glob("dir/*.php");  scandir("dir");
来源：http://viy.iojbl.cn

[U65] PHP：会话
来源：http://obv.wangdashe.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ink.gogol.net.cn

[U66] PHP：设置 Cookie
来源：http://hul.pycfn.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rne.wangshuangyany.cn

[U67] PHP：处理文件上传
来源：http://lxf.bjfxy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xms.tanke756.top

[U68] PHP：PDO 连接
来源：http://dzr.52xcode.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vkb.cucudq.cn

[U69] PHP：PDO 预处理
来源：http://tmq.jinghuilouyu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://atc.dianchejie.cn

[U70] PHP：PDO 事务
来源：http://sgm.jqgufenzy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ext.pengpengdd.cyou

[U71] PHP：抛出异常
来源：http://jnx.guowangkeji.top

throw new RuntimeException("失败", 500);
来源：http://qli.snrcjt.cn

[U72] PHP：写错误日志
来源：http://miq.hnqzz.top

error_log("失败: " . $e->getMessage());
来源：http://pwh.pycfn.com

[U73] PHP：读取 ini 配置
来源：http://kxx.redwolf501.top

parse_ini_file("config.ini", true)
来源：http://ayw.zhiwuduotai.top

[U74] PHP：读取环境变量
来源：http://ziw.xuanzx.com

getenv("APP_ENV") ?: "production"
来源：http://kum.ivvv.top

[U75] PHP：依赖注入
来源：http://klz.yangfankeji.com

composer require psr/container
来源：http://jgb.jlsjyb.cn

[U76] PHP：简单路由
来源：http://uui.yanxiufei.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://thm.hesvh.cn

[U77] PHP：模板渲染
来源：http://rqr.tian-w.cn

composer require twig/twig
来源：http://gly.sjlbkw.cn

[U78] PHP：单元测试
来源：http://uyy.yfazqb.com

composer require --dev phpunit/phpunit
来源：http://cov.vqdsnc.cn

[U79] PHP：静态分析
来源：http://fxo.zhengqikj.top

composer require --dev phpstan/phpstan
来源：http://pzh.shanyushiyangkeji.top

[U80] PHP：代码规范修复
来源：http://cgr.jyoumei.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://vja.yueranfly.top

[U81] JS：初始化项目
来源：http://xwz.zhixingplan.top

npm init -y;  npm i express
来源：http://uoz.c1oappe.top

[U82] JS：package.json 脚本
来源：http://rns.daria6918.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zba.chenlongwang.top

[U83] JS：ES Module 导入导出
来源：http://avp.shangyingyoupin.top

export const a = 1;  import { a } from "./m.js";
来源：http://mnk.fzhhl.top

[U84] JS：CommonJS 写法
来源：http://uju.jyoumei.cn

module.exports = { a };  const { a } = require("./m");
来源：http://glw.yj202588.top

[U85] JS：可选链
来源：http://vll.hnqzz.top

a?.b?.c
来源：http://zys.hnxiangtu.top

[U86] JS：空值合并
来源：http://mwa.yueranfly.top

a ?? b
来源：http://mch.9152youxi.cn

[U87] JS：解构默认值
来源：http://urd.jqgfzy.top

const { a = 1, b = 2 } = obj;
来源：http://osj.xinyue.icu

[U88] JS：对象展开合并
来源：http://iza.fehbvm.com

{ ...a, ...b }
来源：http://qlj.iojbl.cn

[U89] JS：数组去重
来源：http://sld.shuidangran.top

[...new Set(arr)]
来源：http://ydy.zhiwuduotai.top

[U90] JS：数字数组排序
来源：http://msg.xylfe.cn

[...arr].sort((a, b) => a - b)
来源：http://hvm.aizwys.cn

[U91] JS：对象键值遍历
来源：http://let.9152youxi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ldi.zdqjudy.top

[U92] JS：深拷贝
来源：http://xks.chenzaomai.com

structuredClone(obj)
来源：http://drk.bjfxy.top

[U93] JS：模板字符串
来源：http://ifv.hcnkem.com

`共 ${n} 条`
来源：http://suo.zycfv.cn

[U94] JS：箭头函数
来源：http://sqx.yongpay.top

const double = x => x * 2;
来源：http://jnd.yuxming.cn

[U95] JS：Promise 包装
来源：http://ovt.yongpay.top

new Promise((resolve, reject) => {})
来源：http://ctq.gaohongyu789.top

[U96] JS：async/await 与异常
来源：http://tfh.9152youxi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uzv.yj20258.top

[U97] JS：并发请求
来源：http://rso.ivvv.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://nbo.guannengcc.top

[U98] JS：fetch 带 JSON
来源：http://xdz.jqgfzy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ymr.kuanghao11.cn

[U99] JS：事件监听
来源：http://csl.yj20258888.top

el.addEventListener("click", e => {})
来源：http://med.daxiang520.top

[U100] JS：DOM 查询
来源：http://qst.jinghuilouyu.cn

document.querySelector(".item")
来源：http://icb.jiagoushi.top

[U101] JS：classList 操作
来源：http://gpl.xingfuxueyuan.xyz

el.classList.toggle("active")
来源：http://vrt.chenlongwang.top

[U102] JS：本地存储
来源：http://gws.fanxiaobao.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://gmt.xinyue.icu

[U103] JS：定时器
来源：http://ihb.ydjk.org.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ktw.yuanzhike.top

[U104] JS：防抖
来源：http://goy.yongpay.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ygi.fzhhl.top

[U105] JS：节流
来源：http://dve.hywenlv.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ekc.shzxlz.cn

[U106] JS：日期格式化
来源：http://eoo.jyoumei.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pqs.yj202588.top

[U107] JS：数字千分位
来源：http://mto.hfpthk.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://udw.meibo888.top

[U108] JS：随机整数
来源：http://vle.hysaishi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hyg.shanyushiyangkeji.top

[U109] JS：数组分组
来源：http://cdf.zdbjq.cn

Object.groupBy(arr, x => x.type)
来源：http://cik.mhx1999.top

[U110] JS：数组分块
来源：http://div.iojbl.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://itg.316326.xyz

[U111] JS：对象转 Map
来源：http://zyq.hywenlv.cn

new Map(Object.entries(obj))
来源：http://ofw.jlsjyb.cn

[U112] JS：字符串补位
来源：http://rzc.jqgufenzy.top

"7".padStart(3, "0")
来源：http://uki.chenjidiqi.icu

[U113] JS：正则替换全部
来源：http://xqj.fehbvm.com

s.replaceAll("a", "b")
来源：http://vyj.jiagoushi.top

[U114] JS：JSON 深比较
来源：http://amv.cqqwz.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://bxe.gaohongyu789.top

[U115] JS：生成 UUID
来源：http://srb.bjfxy.top

crypto.randomUUID()
来源：http://rfv.hesvh.cn

[U116] JS：类型检查（JSDoc）
来源：http://qto.zhiwuduotai.top

/** @param {string} name */ function f(name) {}
来源：http://ztn.hongshengwenyu.top

[U117] JS：单元测试
来源：http://fbu.xuetiantiany.cn

npm i -D vitest;  npx vitest
来源：http://qsh.shangyingyoupin.top

[U118] JS：开发服务器
来源：http://eqh.snrcjt.cn

npm i -D vite;  npx vite
来源：http://jza.pycfn.com

[U119] JS：生产构建
来源：http://ulg.wangdashe.top

npx vite build
来源：http://wdx.chenlongwang.top

[U120] JS：读取环境变量（Vite）
来源：http://ypx.pycfn.com

import.meta.env.VITE_API_URL
来源：http://tkw.tanke756.top

================================================================================
来源：http://iiy.shanyushiyangkeji.top

统计汇总
来源：http://nlq.zdbjq.cn

================================================================================
来源：http://bcu.xuanzx.com

按语言统计（条）：
来源：http://ilg.hesvh.cn

Python ......... 252
来源：http://irh.jinqigufen.top

PHP ............ 252
来源：http://lcu.tarul.cn

JavaScript ..... 252
来源：http://fok.tanke756.top

TypeScript ..... 212
来源：http://sez.nanxinkj.top

Java ........... 212
来源：http://tgr.kuanghao11.cn

Go ............. 212
来源：http://zkh.aibaodan.cn

Ruby ........... 212
来源：http://tgr.gotoacloud.top

C# ............. 212
来源：http://hrz.wangshuangyany.cn

C .............. 30
来源：http://ime.ydjk.org.cn

C++ ............ 30
来源：http://afp.tian-w.cn

SQL ............ 90
来源：http://xfy.tarul.cn

Bash ........... 80
来源：http://lhn.fzhhl.top

Kotlin ......... 15
来源：http://muf.feifeiyinyue.top

Swift .......... 15
来源：http://ahr.zhiwuduotai.top

Lua ............ 10
来源：http://riy.redwolf501.top

Perl ........... 10
来源：http://zjz.pengpengdd.cyou

Scala .......... 10
来源：http://ngh.shanyushiyangtech.top

------------------------------------
来源：http://aao.fehbvm.com

合计 ........... 2106 条
来源：http://jid.fanxiaobao.xyz

按章节统计：
来源：http://umy.zycfv.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://coc.iojbl.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://uuf.hesvh.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://umu.xziqi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://feq.gaohongyu789.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ngn.shuidangran.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xqt.ctjpmb.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://afd.dashuyun.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vaz.fanxiaobao.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ddk.hysaishi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dih.pengpengdd.cyou

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pag.xziqi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cdn.mhx1999.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://axk.quarkkingdee.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pbq.shangyingyoupin.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gma.shzxlz.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zxy.hcnkem.com

Q SQL 专题                              90
来源：http://wii.yongpay.top

R Bash 专题                             80
来源：http://uio.bjfxy.top

S C / C++ 专题                          60
来源：http://sfv.hammf.cn

T 其他语言补充                          60
来源：http://anf.guowangkeji.top

U 高频实用片段                         120
来源：http://dci.zhoulong.xyz

------------------------------------
来源：http://dgv.hywenlv.cn

合计                                  2106 条
来源：http://euv.ctjpmb.com

--------------------------------------------------------------------------------
来源：http://qch.jqgfzy.top

使用提醒
来源：http://exv.yanxiufei.cn

--------------------------------------------------------------------------------
来源：http://tua.ppjwa.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ogo.tanke756.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zzg.epnwcf.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dfc.pycfn.com

在旧版本上使用前请先确认语法支持情况。
来源：http://svi.ppjwa.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yxd.hnxiangtu.top

—— 文件结束 ——
来源：http://qok.tian-w.cn

================================================================================
来源：http://tbr.cqqwz.cn

程序语言常见例子速查手册（2024 版）
来源：http://zsf.svipenyu.cn

Common Programming Examples Cheat Book
来源：http://qqq.redwolf501.top

================================================================================
来源：http://abg.shzxlz.cn

【收录内容】
来源：http://asp.chenzaomai.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://igp.ydjk.org.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mei.316326.xyz

SQL · Bash · C · C++
来源：http://hss.ybcxt.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://uae.hammf.cn

【使用说明】
来源：http://kst.svipenyu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qlm.shanyushiyangkeji.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://whu.gotoacloud.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ali.quarkkingdee.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://efi.hysaishi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://nkm.tian-w.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wzk.ctjpmb.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tdj.jlsjyb.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fui.ctjpmb.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ylw.guowangkeji.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://bnp.yueranfly.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dlv.jinghuilouyu.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vzx.yj202588.top

【文件统计】
来源：http://iqf.yongpay.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://kil.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://eze.ivvv.top

目  录
来源：http://ogm.0kj1m.cn

--------------------------------------------------------------------------------
来源：http://bhz.316326.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://weh.shangyingyoupin.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qvy.xylfe.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kfk.aibaodan.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tql.uphjek.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://php.tianlin.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xwd.pycfn.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://tkm.jqgfzy.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bxi.cqqwz.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://cka.daxiang520.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://waj.guannengcc.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://tsw.sweek.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dsp.yfazqb.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wwa.dashuyun.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ufy.c1oappe.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://oem.shuidangran.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vyt.redwolf501.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lvd.tian-w.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://hnw.vqdsnc.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rch.vqdsnc.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kto.xziqi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cpi.yfazqb.com

================================================================================
来源：http://jmu.quarkkingdee.top

A. 基础语法与类型
来源：http://qqy.ivvv.top

================================================================================
来源：http://kza.jianghu66.top

[A01] Hello World
来源：http://vhw.sysykeji.top

Py:   print("Hello, World!")
来源：http://ppf.hywenlv.cn

PHP:  echo "Hello, World!";
来源：http://vay.gzhubu.top

JS:   console.log("Hello, World!");
来源：http://sws.shanyushiyangtech.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://utq.fanxiaobao.xyz

Java: System.out.println("Hello, World!");
来源：http://eko.yvedp.cn

Go:   fmt.Println("Hello, World!")
来源：http://srt.uphjek.com

Ruby: puts "Hello, World!"
来源：http://ppz.jqgfzy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://wfj.52xcode.cn

[A02] 变量声明与赋值
来源：http://zhu.gotoacloud.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fgc.shanyushiyangkeji.top

PHP:  $name = "Alex"; $age = 20;
来源：http://xpc.jinqigufen.top

JS:   let name = "Alex"; const age = 20;
来源：http://gsw.gaohongyu789.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rxt.yongpay.top

Java: String name = "Alex"; int age = 20;
来源：http://hgz.jqgufenzy.top

Go:   name := "Alex"; age := 20
来源：http://epp.tarul.cn

Ruby: name = "Alex"; age = 20
来源：http://ugd.zhiwuduotai.top

C#:   string name = "Alex"; int age = 20;
来源：http://xsb.zhaomingkeji.xyz

[A03] 常量定义
来源：http://nvk.jqgufenzy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://puw.yueranfly.top

PHP:  const PI = 3.14159;
来源：http://roc.bjfxy.top

JS:   const PI = 3.14159;
来源：http://dab.9152youxi.cn

TS:   const PI: number = 3.14159;
来源：http://ggy.52xcode.cn

Java: static final double PI = 3.14159;
来源：http://qzx.ehwqpu.com

Go:   const PI = 3.14159
来源：http://uxf.gotoacloud.top

Ruby: PI = 3.14159
来源：http://btg.chenzaomai.com

C#:   const double PI = 3.14159;
来源：http://qbl.vqdsnc.cn

[A04] 判断变量类型
来源：http://uvq.chenzaomai.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://tlh.snrcjt.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ftb.yanxiufei.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lxv.chenlongwang.top

TS:   typeof x; x instanceof Date
来源：http://slk.cheryme.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kie.gogol.net.cn

Go:   reflect.TypeOf(x).Name()
来源：http://uyk.c1oappe.top

Ruby: x.class; x.is_a?(Integer)
来源：http://kqp.ctjpmb.com

C#:   x.GetType().Name; x is int
来源：http://env.zdbjq.cn

[A05] 整数除法与取模
来源：http://alc.hnqzz.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hes.jinqigfzy.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ugb.jlsjyb.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hqf.jinyuanbaomall.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gnf.mhx1999.top

Java: 7 / 2; 7 % 2
来源：http://ast.vqdsnc.cn

Go:   7 / 2; 7 % 2
来源：http://eyp.cheryme.top

Ruby: 7 / 2; 7 % 2
来源：http://bgk.hcnkem.com

C#:   7 / 2; 7 % 2
来源：http://coz.tianlin.xyz

[A06] 字符串转数字
来源：http://ygk.9152youxi.cn

Py:   int("42"); float("3.14")
来源：http://ibz.cheryme.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ndn.havefunace.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baf.ehwqpu.com

TS:   parseInt("42", 10); Number("42")
来源：http://bjq.chenjidiqi.icu

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://nqz.uphjek.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://uef.shangyingyoupin.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ubv.zhongyouzk.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://anv.nwbrower.top

[A07] 数字转字符串
来源：http://aqx.yuanzhike.top

Py:   str(42)
来源：http://crn.ppjwa.cn

PHP:  (string) 42; strval(42)
来源：http://mcr.9152youxi.cn

JS:   String(42); (42).toString()
来源：http://ckg.sysykeji.top

TS:   String(42)
来源：http://kgv.jianghu66.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ewj.zdqjudy.top

Go:   strconv.Itoa(42)
来源：http://bzq.dianchejie.cn

Ruby: 42.to_s
来源：http://nza.hongshengwenyu.top

C#:   42.ToString()
来源：http://gvq.fzhhl.top

[A08] 取整与四舍五入
来源：http://epn.chenzaomai.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dbe.zdbjq.cn


<!-- 参考信息 -->