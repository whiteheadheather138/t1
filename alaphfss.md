代发 wailian999

[U67] PHP：处理文件上传
来源：http://sck.hysaishi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lax.zhaomingkeji.xyz

[U68] PHP：PDO 连接
来源：http://fdu.hammf.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rlz.sjlbkw.cn

[U69] PHP：PDO 预处理
来源：http://mmq.yvedp.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://idx.xziqi.cn

[U70] PHP：PDO 事务
来源：http://wum.ybcxt.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dmq.zdbjq.cn

[U71] PHP：抛出异常
来源：http://gnn.yuanzhike.top

throw new RuntimeException("失败", 500);
来源：http://vms.hesvh.cn

[U72] PHP：写错误日志
来源：http://arv.0kj1m.cn

error_log("失败: " . $e->getMessage());
来源：http://smd.epnwcf.com

[U73] PHP：读取 ini 配置
来源：http://vot.xylfe.cn

parse_ini_file("config.ini", true)
来源：http://pcz.jiagoushi.top

[U74] PHP：读取环境变量
来源：http://bfc.iojbl.cn

getenv("APP_ENV") ?: "production"
来源：http://cmy.yonumen.top

[U75] PHP：依赖注入
来源：http://scz.vqdsnc.cn

composer require psr/container
来源：http://azm.zdqjudy.top

[U76] PHP：简单路由
来源：http://tdh.fanxiaobao.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cxh.chenlongwang.top

[U77] PHP：模板渲染
来源：http://nwk.jianghu66.top

composer require twig/twig
来源：http://vrk.jlsjyb.cn

[U78] PHP：单元测试
来源：http://vka.hammf.cn

composer require --dev phpunit/phpunit
来源：http://uog.guannengcc.top

[U79] PHP：静态分析
来源：http://xpc.fktsv.cn

composer require --dev phpstan/phpstan
来源：http://pje.uphjek.com

[U80] PHP：代码规范修复
来源：http://zob.tianlin.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://ryb.zhaomingkeji.xyz

[U81] JS：初始化项目
来源：http://fdn.fengsongda.top

npm init -y;  npm i express
来源：http://sfu.yanxiufei.cn

[U82] JS：package.json 脚本
来源：http://fww.bbcook.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://phl.yonumen.top

[U83] JS：ES Module 导入导出
来源：http://keh.xuanzx.com

export const a = 1;  import { a } from "./m.js";
来源：http://eux.sjlbkw.cn

[U84] JS：CommonJS 写法
来源：http://ytt.cdnleiting.top

module.exports = { a };  const { a } = require("./m");
来源：http://jqh.snrcjt.cn

[U85] JS：可选链
来源：http://wvl.hammf.cn

a?.b?.c
来源：http://kel.yj202588.top

[U86] JS：空值合并
来源：http://cqh.zdqjudy.top

a ?? b
来源：http://fuh.nwbrower.top

[U87] JS：解构默认值
来源：http://jiw.fzhhl.top

const { a = 1, b = 2 } = obj;
来源：http://xhl.ivvv.top

[U88] JS：对象展开合并
来源：http://whm.jinyuanbaomall.cn

{ ...a, ...b }
来源：http://iqr.cucudq.cn

[U89] JS：数组去重
来源：http://zwj.cqqwz.cn

[...new Set(arr)]
来源：http://ygt.chenzaomai.com

[U90] JS：数字数组排序
来源：http://uuy.pycfn.com

[...arr].sort((a, b) => a - b)
来源：http://mtn.hywenlv.cn

[U91] JS：对象键值遍历
来源：http://fdt.shanyushiyangkeji.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://olr.yongpay.top

[U92] JS：深拷贝
来源：http://xuv.birdmap.top

structuredClone(obj)
来源：http://jtb.havefunace.top

[U93] JS：模板字符串
来源：http://rej.yongpay.top

`共 ${n} 条`
来源：http://yim.smart0.xyz

[U94] JS：箭头函数
来源：http://svv.dianchejie.cn

const double = x => x * 2;
来源：http://opk.iojbl.cn

[U95] JS：Promise 包装
来源：http://ncm.xuetiantiany.cn

new Promise((resolve, reject) => {})
来源：http://dvo.chenjidiqi.icu

[U96] JS：async/await 与异常
来源：http://gjs.yj20258.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wsd.zhoulong.xyz

[U97] JS：并发请求
来源：http://gow.ivvv.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://heb.ivvv.top

[U98] JS：fetch 带 JSON
来源：http://fzi.pycfn.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ans.jlsjyb.cn

[U99] JS：事件监听
来源：http://uqx.daxiang520.top

el.addEventListener("click", e => {})
来源：http://chu.hysaishi.cn

[U100] JS：DOM 查询
来源：http://wyz.redwolf501.top

document.querySelector(".item")
来源：http://zvy.zhengqikj.top

[U101] JS：classList 操作
来源：http://umu.bjfxy.top

el.classList.toggle("active")
来源：http://gmy.fehbvm.com

[U102] JS：本地存储
来源：http://jri.zhaomingkeji.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://bvb.guannengcc.top

[U103] JS：定时器
来源：http://wcj.cdnleiting.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lvp.smart0.xyz

[U104] JS：防抖
来源：http://kvc.yj202588.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tje.tianlin.xyz

[U105] JS：节流
来源：http://lpo.yfazqb.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uyi.xylfe.cn

[U106] JS：日期格式化
来源：http://lbv.bbcook.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qqz.iojbl.cn

[U107] JS：数字千分位
来源：http://nbc.aizwys.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uwr.jlsjyb.cn

[U108] JS：随机整数
来源：http://ghz.yuxming.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ube.xuanzx.com

[U109] JS：数组分组
来源：http://xon.yanxiufei.cn

Object.groupBy(arr, x => x.type)
来源：http://cgq.vehdjk.com

[U110] JS：数组分块
来源：http://oke.sweek.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rmn.jqgfzy.top

[U111] JS：对象转 Map
来源：http://wkm.yj202588.top

new Map(Object.entries(obj))
来源：http://kbd.cdnleiting.top

[U112] JS：字符串补位
来源：http://chj.hnxiangtu.top

"7".padStart(3, "0")
来源：http://wlu.guannengcc.top

[U113] JS：正则替换全部
来源：http://hkr.xinyue.icu

s.replaceAll("a", "b")
来源：http://ero.feifeiyinyue.top

[U114] JS：JSON 深比较
来源：http://rrr.tian-w.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hxk.wangshuangyany.cn

[U115] JS：生成 UUID
来源：http://tzl.hnqzz.top

crypto.randomUUID()
来源：http://gjj.aizwys.cn

[U116] JS：类型检查（JSDoc）
来源：http://dmp.wangshuangyany.cn

/** @param {string} name */ function f(name) {}
来源：http://oil.wangdashe.top

[U117] JS：单元测试
来源：http://ynh.ybcxt.top

npm i -D vitest;  npx vitest
来源：http://tgh.uphjek.com

[U118] JS：开发服务器
来源：http://rbt.hywenlv.cn

npm i -D vite;  npx vite
来源：http://oii.zdbjq.cn

[U119] JS：生产构建
来源：http://fct.shzxlz.cn

npx vite build
来源：http://voe.tanke756.top

[U120] JS：读取环境变量（Vite）
来源：http://wcp.iojbl.cn

import.meta.env.VITE_API_URL
来源：http://upv.cheryme.top

================================================================================
来源：http://zro.fzhhl.top

统计汇总
来源：http://gcf.zhiwuduotai.top

================================================================================
来源：http://wvx.ppjwa.cn

按语言统计（条）：
来源：http://sck.xinyue.icu

Python ......... 252
来源：http://hwo.jinqigfzy.top

PHP ............ 252
来源：http://lyi.hongshengwenyu.top

JavaScript ..... 252
来源：http://oco.pengpengdd.cyou

TypeScript ..... 212
来源：http://wgy.jinqigufen.top

Java ........... 212
来源：http://gxm.daria6918.cn

Go ............. 212
来源：http://pss.hywenlv.cn

Ruby ........... 212
来源：http://ees.gotoacloud.top

C# ............. 212
来源：http://ayq.daxiang520.top

C .............. 30
来源：http://vob.yanxiufei.cn

C++ ............ 30
来源：http://iuf.yvedp.cn

SQL ............ 90
来源：http://pnm.vehdjk.com

Bash ........... 80
来源：http://idk.yangfankeji.com

Kotlin ......... 15
来源：http://nyp.nanxinkj.top

Swift .......... 15
来源：http://nbj.jyoumei.cn

Lua ............ 10
来源：http://xrp.hnqzz.top

Perl ........... 10
来源：http://oyt.52xcode.cn

Scala .......... 10
来源：http://lbu.jinghuilouyu.cn

------------------------------------
来源：http://pmt.guowangkeji.top

合计 ........... 2106 条
来源：http://yrd.jiagoushi.top

按章节统计：
来源：http://zes.zhiwuduotai.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ahp.tian-w.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lxk.redwolf501.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fyr.kuanghao11.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zmt.guowangkeji.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jgn.fktsv.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://own.hcnkem.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://oia.wangdashe.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://aga.yangfankeji.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://con.aizwys.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xmc.chenzaomai.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zwv.yj20258.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gvg.gzhubu.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://swt.hywenlv.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ucg.dashuyun.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ppe.fanxiaobao.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ouu.hcnkem.com

Q SQL 专题                              90
来源：http://qre.zhijiandao.cn

R Bash 专题                             80
来源：http://gpo.316326.xyz

S C / C++ 专题                          60
来源：http://rdw.daria6918.cn

T 其他语言补充                          60
来源：http://wms.iojbl.cn

U 高频实用片段                         120
来源：http://bgf.chenjidiqi.icu

------------------------------------
来源：http://prz.mhx1999.top

合计                                  2106 条
来源：http://rax.zhiwuduotai.top

--------------------------------------------------------------------------------
来源：http://qmx.epnwcf.com

使用提醒
来源：http://hif.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://feq.sxryk.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://iks.mhx1999.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tag.epnwcf.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://sqq.yonumen.top

在旧版本上使用前请先确认语法支持情况。
来源：http://rxs.bbcook.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lzq.epnwcf.com

—— 文件结束 ——
来源：http://vgy.zhiwuduotai.top

================================================================================
来源：http://hlr.jinqigufen.top

程序语言常见例子速查手册（2024 版）
来源：http://okt.daria6918.cn

Common Programming Examples Cheat Book
来源：http://lgk.daria6918.cn

================================================================================
来源：http://xua.redwolf501.top

【收录内容】
来源：http://bio.ivvv.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://gkp.jiagoushi.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fqh.shuidangran.top

SQL · Bash · C · C++
来源：http://ijl.nwbrower.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zrs.yj202588.top

【使用说明】
来源：http://ubf.kuanghao11.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://dar.ybcxt.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jzh.tian-w.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gcy.shzxlz.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://noz.daria6918.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://hgd.pycfn.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jqo.hcnkem.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://msz.chenlongwang.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ydl.svipenyu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gsc.sweek.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ndp.zhongyouzk.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://nao.daria6918.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://npy.zdqjudy.top

【文件统计】
来源：http://rof.shzxlz.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hhx.shzxlz.cn

--------------------------------------------------------------------------------
来源：http://asx.snrcjt.cn

目  录
来源：http://yvw.hammf.cn

--------------------------------------------------------------------------------
来源：http://jue.dashuyun.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ozw.nanxinkj.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tyt.zhongyouzk.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://uua.sxryk.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vvb.gotoacloud.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://csg.jqgufenzy.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cdr.jianghu66.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wpv.yanxiufei.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xsp.dashuyun.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rgo.ydjk.org.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fub.fanxiaobao.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wcq.daria6918.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ttc.tarul.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://btg.pycfn.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ook.xuanzx.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://tlg.havefunace.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://esp.jlsjyb.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xhq.zhaomingkeji.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://wnu.yj20258.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vgc.ydzc1.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qlb.zhaomingkeji.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pal.gaohongyu789.top

================================================================================
来源：http://qla.jlsjyb.cn

A. 基础语法与类型
来源：http://pqo.xylfe.cn

================================================================================
来源：http://bql.yfazqb.com

[A01] Hello World
来源：http://pnu.fzhhl.top

Py:   print("Hello, World!")
来源：http://pks.wangshuangyany.cn

PHP:  echo "Hello, World!";
来源：http://ufm.xziqi.cn

JS:   console.log("Hello, World!");
来源：http://nsx.xingfuxueyuan.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ytx.ydzc1.top

Java: System.out.println("Hello, World!");
来源：http://bvu.chenzaomai.com

Go:   fmt.Println("Hello, World!")
来源：http://csm.316326.xyz

Ruby: puts "Hello, World!"
来源：http://ppi.feifeiyinyue.top

C#:   Console.WriteLine("Hello, World!");
来源：http://gij.shuidangran.top

[A02] 变量声明与赋值
来源：http://ypp.daxiang520.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://cza.ydzc1.top

PHP:  $name = "Alex"; $age = 20;
来源：http://zaz.hfpthk.cn

JS:   let name = "Alex"; const age = 20;
来源：http://buk.feifeiyinyue.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://uvv.yj20258.top

Java: String name = "Alex"; int age = 20;
来源：http://wob.daxiang520.top

Go:   name := "Alex"; age := 20
来源：http://xai.ctjpmb.com

Ruby: name = "Alex"; age = 20
来源：http://imi.shzxlz.cn

C#:   string name = "Alex"; int age = 20;
来源：http://wfk.hywenlv.cn

[A03] 常量定义
来源：http://cui.zdbjq.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://cww.andypj.xyz

PHP:  const PI = 3.14159;
来源：http://oea.chenlongwang.top

JS:   const PI = 3.14159;
来源：http://bcq.yueranfly.top

TS:   const PI: number = 3.14159;
来源：http://lyv.quarkkingdee.top

Java: static final double PI = 3.14159;
来源：http://upo.hammf.cn

Go:   const PI = 3.14159
来源：http://per.chenzaomai.com

Ruby: PI = 3.14159
来源：http://mxo.xuetiantiany.cn

C#:   const double PI = 3.14159;
来源：http://kof.ppjwa.cn

[A04] 判断变量类型
来源：http://fuu.shanyushiyangkeji.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://alz.vehdjk.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wuc.sysykeji.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rbz.fanxiaobao.xyz

TS:   typeof x; x instanceof Date
来源：http://qrd.hysaishi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rid.zhijiandao.cn

Go:   reflect.TypeOf(x).Name()
来源：http://emk.gogol.net.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://vuq.hnqzz.top

C#:   x.GetType().Name; x is int
来源：http://grm.jqgufenzy.top

[A05] 整数除法与取模
来源：http://avq.gogol.net.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://elz.zhixingplan.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://uoe.jianghu66.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tog.yj20258.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ewl.cqqwz.cn

Java: 7 / 2; 7 % 2
来源：http://sal.cucudq.cn

Go:   7 / 2; 7 % 2
来源：http://saf.9152youxi.cn

Ruby: 7 / 2; 7 % 2
来源：http://vdi.gaohongyu789.top

C#:   7 / 2; 7 % 2
来源：http://qjg.cheryme.top

[A06] 字符串转数字
来源：http://tnn.chenjidiqi.icu

Py:   int("42"); float("3.14")
来源：http://ptw.hnxiangtu.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tzm.ctjpmb.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://plo.zhongyouzk.top

TS:   parseInt("42", 10); Number("42")
来源：http://rjt.ppjwa.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://uoj.jlsjyb.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ywa.guannengcc.top

Ruby: "42".to_i; "3.14".to_f
来源：http://nea.ydzc1.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rar.hongshengwenyu.top

[A07] 数字转字符串
来源：http://okg.shanyushiyangtech.top

Py:   str(42)
来源：http://tpq.pengpengdd.cyou

PHP:  (string) 42; strval(42)
来源：http://gef.sxryk.cn

JS:   String(42); (42).toString()
来源：http://cxf.zdqjudy.top

TS:   String(42)
来源：http://ziz.wangshuangyany.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://miv.hfpthk.cn

Go:   strconv.Itoa(42)
来源：http://ikz.jqgufenzy.top

Ruby: 42.to_s
来源：http://xgd.wangshuangyany.cn

C#:   42.ToString()
来源：http://yak.fehbvm.com

[A08] 取整与四舍五入
来源：http://udg.tianlin.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gyw.fzhhl.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://enh.yangfankeji.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gcw.52xcode.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://lsb.zhixingplan.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gmt.hesvh.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://roq.fktsv.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://gwt.daxiang520.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fbj.hammf.cn

[A09] 绝对值与最大最小值
来源：http://xyw.shzxlz.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rqa.chenlongwang.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://pft.ppjwa.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mbb.guowangkeji.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://euq.shangyingyoupin.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lfg.jqgufenzy.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rvf.yuxming.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nkj.gzhubu.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mvy.hcnkem.com

[A10] 生成随机数
来源：http://ycf.yvedp.cn

Py:   import random; random.randint(1, 100)
来源：http://nvj.shanyushiyangkeji.top

PHP:  random_int(1, 100);
来源：http://dwy.shanyushiyangtech.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vyu.iojbl.cn


<!-- 参考信息 -->