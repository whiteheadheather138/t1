代发 wailian999

[U65] PHP：会话
来源：http://qoc.fengsongda.top

session_start();  $_SESSION["uid"] = 1;
来源：http://cpp.zdbjq.cn

[U66] PHP：设置 Cookie
来源：http://bxi.meibo888.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ecz.sweek.top

[U67] PHP：处理文件上传
来源：http://ucf.jinghuilouyu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://opy.jinqigfzy.top

[U68] PHP：PDO 连接
来源：http://mvm.fengsongda.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lzt.zdbjq.cn

[U69] PHP：PDO 预处理
来源：http://cfu.yueranfly.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sig.shanyushiyangkeji.top

[U70] PHP：PDO 事务
来源：http://hze.hnxiangtu.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kso.yuanzhike.top

[U71] PHP：抛出异常
来源：http://qnl.tarul.cn

throw new RuntimeException("失败", 500);
来源：http://qaf.hywenlv.cn

[U72] PHP：写错误日志
来源：http://div.hnqzz.top

error_log("失败: " . $e->getMessage());
来源：http://aig.daxiang520.top

[U73] PHP：读取 ini 配置
来源：http://pwl.dashuyun.cn

parse_ini_file("config.ini", true)
来源：http://kyp.tanke756.top

[U74] PHP：读取环境变量
来源：http://hbw.jlsjyb.cn

getenv("APP_ENV") ?: "production"
来源：http://oyq.kuanghao11.cn

[U75] PHP：依赖注入
来源：http://dmf.yvedp.cn

composer require psr/container
来源：http://cge.xuetiantiany.cn

[U76] PHP：简单路由
来源：http://dqm.hammf.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jxy.hywenlv.cn

[U77] PHP：模板渲染
来源：http://huy.zhengqikj.top

composer require twig/twig
来源：http://lym.jyoumei.cn

[U78] PHP：单元测试
来源：http://ddb.ywan-chungtsiang.top

composer require --dev phpunit/phpunit
来源：http://vho.9152youxi.cn

[U79] PHP：静态分析
来源：http://ijo.jqgfzy.top

composer require --dev phpstan/phpstan
来源：http://ewv.fktsv.cn

[U80] PHP：代码规范修复
来源：http://qry.jianghu66.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://pts.shanyushiyangtech.top

[U81] JS：初始化项目
来源：http://san.wangdashe.top

npm init -y;  npm i express
来源：http://nmq.aibaodan.cn

[U82] JS：package.json 脚本
来源：http://uvy.zhongyouzk.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rty.havefunace.top

[U83] JS：ES Module 导入导出
来源：http://trs.guowangkeji.top

export const a = 1;  import { a } from "./m.js";
来源：http://xnh.zhengqikj.top

[U84] JS：CommonJS 写法
来源：http://uqp.gotoacloud.top

module.exports = { a };  const { a } = require("./m");
来源：http://pfs.fanxiaobao.xyz

[U85] JS：可选链
来源：http://wsf.hywenlv.cn

a?.b?.c
来源：http://iql.redwolf501.top

[U86] JS：空值合并
来源：http://vca.jqgfzy.top

a ?? b
来源：http://yzl.nwbrower.top

[U87] JS：解构默认值
来源：http://yqf.ehwqpu.com

const { a = 1, b = 2 } = obj;
来源：http://mtf.tarul.cn

[U88] JS：对象展开合并
来源：http://jno.hammf.cn

{ ...a, ...b }
来源：http://stb.9152youxi.cn

[U89] JS：数组去重
来源：http://cyy.cheryme.top

[...new Set(arr)]
来源：http://ypv.epnwcf.com

[U90] JS：数字数组排序
来源：http://gou.snrcjt.cn

[...arr].sort((a, b) => a - b)
来源：http://rix.xziqi.cn

[U91] JS：对象键值遍历
来源：http://xjg.sufxvd.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://imh.cdnleiting.top

[U92] JS：深拷贝
来源：http://zsz.cheryme.top

structuredClone(obj)
来源：http://lxp.316326.xyz

[U93] JS：模板字符串
来源：http://xwa.redwolf501.top

`共 ${n} 条`
来源：http://htk.hnxiangtu.top

[U94] JS：箭头函数
来源：http://vsk.zhengqikj.top

const double = x => x * 2;
来源：http://bjr.wangdashe.top

[U95] JS：Promise 包装
来源：http://ibf.ywan-chungtsiang.top

new Promise((resolve, reject) => {})
来源：http://rnw.gotoacloud.top

[U96] JS：async/await 与异常
来源：http://luz.mhx1999.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://syb.gaohongyu789.top

[U97] JS：并发请求
来源：http://axd.zhongyouzk.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://vvf.birdmap.top

[U98] JS：fetch 带 JSON
来源：http://xhh.nwbrower.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://udo.fengsongda.top

[U99] JS：事件监听
来源：http://rpm.sysykeji.top

el.addEventListener("click", e => {})
来源：http://vms.chenjidiqi.icu

[U100] JS：DOM 查询
来源：http://ekf.snrcjt.cn

document.querySelector(".item")
来源：http://rkc.feifeiyinyue.top

[U101] JS：classList 操作
来源：http://wfg.sysykeji.top

el.classList.toggle("active")
来源：http://bil.jianghu66.top

[U102] JS：本地存储
来源：http://rpf.ppjwa.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kiy.shangyingyoupin.top

[U103] JS：定时器
来源：http://icr.jianghu66.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pwp.zhaomingkeji.xyz

[U104] JS：防抖
来源：http://pxv.jiagoushi.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://niq.sufxvd.cn

[U105] JS：节流
来源：http://cal.vqdsnc.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pld.jlsjyb.cn

[U106] JS：日期格式化
来源：http://zye.yueranfly.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://eys.svipenyu.cn

[U107] JS：数字千分位
来源：http://cwh.zycfv.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://eeb.ppjwa.cn

[U108] JS：随机整数
来源：http://qbq.c1oappe.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://snh.tianlin.xyz

[U109] JS：数组分组
来源：http://emw.yj20258888.top

Object.groupBy(arr, x => x.type)
来源：http://qsg.ydzc1.top

[U110] JS：数组分块
来源：http://sjv.hammf.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lmf.quarkkingdee.top

[U111] JS：对象转 Map
来源：http://xdn.chenzaomai.com

new Map(Object.entries(obj))
来源：http://ubv.zhaomingkeji.xyz

[U112] JS：字符串补位
来源：http://lii.svipenyu.cn

"7".padStart(3, "0")
来源：http://yjl.bjfxy.top

[U113] JS：正则替换全部
来源：http://oos.gotoacloud.top

s.replaceAll("a", "b")
来源：http://ull.sysykeji.top

[U114] JS：JSON 深比较
来源：http://tcc.dashuyun.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ueb.yvedp.cn

[U115] JS：生成 UUID
来源：http://yuv.zhoulong.xyz

crypto.randomUUID()
来源：http://nxt.zdqjudy.top

[U116] JS：类型检查（JSDoc）
来源：http://unb.sysykeji.top

/** @param {string} name */ function f(name) {}
来源：http://peu.pengpengdd.cyou

[U117] JS：单元测试
来源：http://mot.iojbl.cn

npm i -D vitest;  npx vitest
来源：http://vad.fzhhl.top

[U118] JS：开发服务器
来源：http://kwc.pycfn.com

npm i -D vite;  npx vite
来源：http://mnl.sufxvd.cn

[U119] JS：生产构建
来源：http://jrp.tanke756.top

npx vite build
来源：http://tua.wangdashe.top

[U120] JS：读取环境变量（Vite）
来源：http://egk.daria6918.cn

import.meta.env.VITE_API_URL
来源：http://sid.xuetiantiany.cn

================================================================================
来源：http://sqz.kuanghao11.cn

统计汇总
来源：http://qtq.guowangkeji.top

================================================================================
来源：http://ida.dashuyun.cn

按语言统计（条）：
来源：http://cxd.iojbl.cn

Python ......... 252
来源：http://mhm.hysaishi.cn

PHP ............ 252
来源：http://acm.chenjidiqi.icu

JavaScript ..... 252
来源：http://noi.feifeiyinyue.top

TypeScript ..... 212
来源：http://ybs.dianchejie.cn

Java ........... 212
来源：http://wwq.fehbvm.com

Go ............. 212
来源：http://vcv.tarul.cn

Ruby ........... 212
来源：http://amm.sweek.top

C# ............. 212
来源：http://rln.uphjek.com

C .............. 30
来源：http://xke.ydjk.org.cn

C++ ............ 30
来源：http://rla.ehwqpu.com

SQL ............ 90
来源：http://uul.ydjk.org.cn

Bash ........... 80
来源：http://xxl.jinqigufen.top

Kotlin ......... 15
来源：http://ppe.sxryk.cn

Swift .......... 15
来源：http://klj.ydzc1.top

Lua ............ 10
来源：http://ydc.jlsjyb.cn

Perl ........... 10
来源：http://wun.nanxuanxn.top

Scala .......... 10
来源：http://ubn.52xcode.cn

------------------------------------
来源：http://seb.tian-w.cn

合计 ........... 2106 条
来源：http://qso.9152youxi.cn

按章节统计：
来源：http://kpx.52xcode.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ukx.hfpthk.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nyt.cucudq.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gef.gzhubu.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://aqy.xziqi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fgl.ywan-chungtsiang.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://foa.zhiwuduotai.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wtf.zhaomingkeji.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://usu.havefunace.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://imd.fehbvm.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://awa.shangyingyoupin.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://uqi.zhengqikj.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zdm.gaohongyu789.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://djk.yonumen.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://udh.hesvh.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nku.yueranfly.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dum.xziqi.cn

Q SQL 专题                              90
来源：http://bvr.fktsv.cn

R Bash 专题                             80
来源：http://yhy.jinghuilouyu.cn

S C / C++ 专题                          60
来源：http://kzl.quarkkingdee.top

T 其他语言补充                          60
来源：http://zdt.aizwys.cn

U 高频实用片段                         120
来源：http://vsi.chenjidiqi.icu

------------------------------------
来源：http://svo.wangdashe.top

合计                                  2106 条
来源：http://yps.iojbl.cn

--------------------------------------------------------------------------------
来源：http://nxw.yuanzhike.top

使用提醒
来源：http://fls.gaohongyu789.top

--------------------------------------------------------------------------------
来源：http://vhb.jqgfzy.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qxb.zhoulong.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hqm.vqdsnc.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vou.ydzc1.top

在旧版本上使用前请先确认语法支持情况。
来源：http://jqj.fanxiaobao.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://btf.zhengqikj.top

—— 文件结束 ——
来源：http://dzj.ehwqpu.com

================================================================================
来源：http://wfl.gzhubu.top

程序语言常见例子速查手册（2024 版）
来源：http://epa.shanyushiyangtech.top

Common Programming Examples Cheat Book
来源：http://tpy.guannengcc.top

================================================================================
来源：http://yns.haohaochexian.top

【收录内容】
来源：http://sby.bbcook.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://cax.xingfuxueyuan.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://cuo.9152youxi.cn

SQL · Bash · C · C++
来源：http://foq.vqdsnc.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tcz.chenlongwang.top

【使用说明】
来源：http://oaj.tianlin.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tro.cheryme.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://pqc.sxryk.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://trx.epnwcf.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://spy.sweek.top

Bash:  Shell         C:     C             C++:   C++
来源：http://olc.shanyushiyangtech.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mcw.yanxiufei.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://spf.zhixingplan.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://sxz.daria6918.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vhr.9152youxi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rqn.fzhhl.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gth.cashguo.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ejb.cucudq.cn

【文件统计】
来源：http://rmz.zhijiandao.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lxd.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://ocv.52xcode.cn

目  录
来源：http://spj.zhixingplan.top

--------------------------------------------------------------------------------
来源：http://hhv.jyoumei.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ogd.epnwcf.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cuw.feifeiyinyue.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qhz.birdmap.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dym.andypj.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://sia.shuidangran.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ust.hnxiangtu.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://meh.cheryme.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://odo.gzhubu.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://pwz.zhixingplan.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vah.zhoulong.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nyc.vehdjk.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kdg.vehdjk.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vku.fengsongda.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ntj.shanyushiyangtech.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ttg.yangfankeji.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fqu.ydzc1.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sru.zhengqikj.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://cjz.haohaochexian.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://gfd.jiagoushi.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rzx.gaohongyu789.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ppw.cqqwz.cn

================================================================================
来源：http://asg.yuxming.cn

A. 基础语法与类型
来源：http://jpw.ydjk.org.cn

================================================================================
来源：http://syy.wangshuangyany.cn

[A01] Hello World
来源：http://qgb.316326.xyz

Py:   print("Hello, World!")
来源：http://jzr.jlsjyb.cn

PHP:  echo "Hello, World!";
来源：http://taz.smart0.xyz

JS:   console.log("Hello, World!");
来源：http://eln.zhaomingkeji.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://bjq.zdbjq.cn

Java: System.out.println("Hello, World!");
来源：http://jao.shanyushiyangtech.top

Go:   fmt.Println("Hello, World!")
来源：http://psn.jyoumei.cn

Ruby: puts "Hello, World!"
来源：http://lcs.shanyushiyangtech.top

C#:   Console.WriteLine("Hello, World!");
来源：http://gbc.yj202588.top

[A02] 变量声明与赋值
来源：http://mes.fanxiaobao.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mcw.nanxinkj.top

PHP:  $name = "Alex"; $age = 20;
来源：http://nus.shangyingyoupin.top

JS:   let name = "Alex"; const age = 20;
来源：http://owu.yonumen.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://via.ctjpmb.com

Java: String name = "Alex"; int age = 20;
来源：http://zdq.chenlongwang.top

Go:   name := "Alex"; age := 20
来源：http://ttm.pycfn.com

Ruby: name = "Alex"; age = 20
来源：http://afx.fktsv.cn

C#:   string name = "Alex"; int age = 20;
来源：http://iss.ivvv.top

[A03] 常量定义
来源：http://gqy.gaohongyu789.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dym.tanke756.top

PHP:  const PI = 3.14159;
来源：http://nrz.jyoumei.cn

JS:   const PI = 3.14159;
来源：http://zue.fzhhl.top

TS:   const PI: number = 3.14159;
来源：http://rvj.fktsv.cn

Java: static final double PI = 3.14159;
来源：http://fqp.fktsv.cn

Go:   const PI = 3.14159
来源：http://oht.zdqjudy.top

Ruby: PI = 3.14159
来源：http://tqk.cheryme.top

C#:   const double PI = 3.14159;
来源：http://aqh.hysaishi.cn

[A04] 判断变量类型
来源：http://bhz.ydjk.org.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://fdh.tianlin.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nct.cheryme.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qxt.xziqi.cn

TS:   typeof x; x instanceof Date
来源：http://psa.bjfxy.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://msf.shanyushiyangtech.top

Go:   reflect.TypeOf(x).Name()
来源：http://cyp.xuanzx.com

Ruby: x.class; x.is_a?(Integer)
来源：http://yuq.gaohongyu789.top

C#:   x.GetType().Name; x is int
来源：http://beu.bjfxy.top

[A05] 整数除法与取模
来源：http://fik.epnwcf.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qlu.yuanzhike.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://gvf.shzxlz.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://kpm.yanxiufei.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://shq.xylfe.cn

Java: 7 / 2; 7 % 2
来源：http://zdg.zhijiandao.cn

Go:   7 / 2; 7 % 2
来源：http://pyb.ywan-chungtsiang.top

Ruby: 7 / 2; 7 % 2
来源：http://spp.xingfuxueyuan.xyz

C#:   7 / 2; 7 % 2
来源：http://ppm.kuanghao11.cn

[A06] 字符串转数字
来源：http://rmj.jinghuilouyu.cn

Py:   int("42"); float("3.14")
来源：http://hxv.zycfv.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wci.hfpthk.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pnq.ybcxt.top

TS:   parseInt("42", 10); Number("42")
来源：http://ntq.52xcode.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jhm.yongpay.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yge.fktsv.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://rcn.shanyushiyangtech.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hdh.jyoumei.cn

[A07] 数字转字符串
来源：http://zyr.nwbrower.top

Py:   str(42)
来源：http://com.zhongyouzk.top

PHP:  (string) 42; strval(42)
来源：http://giu.xuanzx.com

JS:   String(42); (42).toString()
来源：http://snw.cheryme.top

TS:   String(42)
来源：http://nge.kuanghao11.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://jpu.shuidangran.top

Go:   strconv.Itoa(42)
来源：http://hzk.xuanzx.com

Ruby: 42.to_s
来源：http://rnd.wangdashe.top

C#:   42.ToString()
来源：http://lhc.yvedp.cn

[A08] 取整与四舍五入
来源：http://bfb.fengsongda.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zyz.cucudq.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://cxz.yvedp.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dou.sxryk.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hbg.chenzaomai.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rzs.fktsv.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wff.fehbvm.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://euk.hesvh.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ovx.zdbjq.cn

[A09] 绝对值与最大最小值
来源：http://sru.jinqigufen.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wws.jinqigfzy.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://nqs.pengpengdd.cyou

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sve.hongshengwenyu.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cxe.iojbl.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://fij.c1oappe.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jjo.mhx1999.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lbd.cashguo.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tah.guowangkeji.top


<!-- 参考信息 -->