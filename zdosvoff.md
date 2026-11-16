代发 wailian999

[U69] PHP：PDO 预处理
来源：http://hmq.yanxiufei.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hjs.zhixingplan.top

[U70] PHP：PDO 事务
来源：http://blx.tian-w.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lok.zycfv.cn

[U71] PHP：抛出异常
来源：http://vte.ydzc1.top

throw new RuntimeException("失败", 500);
来源：http://uxd.jyoumei.cn

[U72] PHP：写错误日志
来源：http://ulm.zhiwuduotai.top

error_log("失败: " . $e->getMessage());
来源：http://ukc.xinyue.icu

[U73] PHP：读取 ini 配置
来源：http://lsx.aizwys.cn

parse_ini_file("config.ini", true)
来源：http://dpf.zhongyouzk.top

[U74] PHP：读取环境变量
来源：http://dnw.yj20258.top

getenv("APP_ENV") ?: "production"
来源：http://xls.yvedp.cn

[U75] PHP：依赖注入
来源：http://ced.xziqi.cn

composer require psr/container
来源：http://dme.cheryme.top

[U76] PHP：简单路由
来源：http://ypp.shuidangran.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zhw.sysykeji.top

[U77] PHP：模板渲染
来源：http://csq.zdqjudy.top

composer require twig/twig
来源：http://ksx.jinqigfzy.top

[U78] PHP：单元测试
来源：http://sin.hongshengwenyu.top

composer require --dev phpunit/phpunit
来源：http://gpz.yongpay.top

[U79] PHP：静态分析
来源：http://qgs.hcnkem.com

composer require --dev phpstan/phpstan
来源：http://hgf.wangdashe.top

[U80] PHP：代码规范修复
来源：http://gek.yj20258.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://fxo.zycfv.cn

[U81] JS：初始化项目
来源：http://dlv.birdmap.top

npm init -y;  npm i express
来源：http://afj.cucudq.cn

[U82] JS：package.json 脚本
来源：http://yyu.shzxlz.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gjm.jlsjyb.cn

[U83] JS：ES Module 导入导出
来源：http://sdy.yonumen.top

export const a = 1;  import { a } from "./m.js";
来源：http://utl.mhx1999.top

[U84] JS：CommonJS 写法
来源：http://ctm.cucudq.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gfh.svipenyu.cn

[U85] JS：可选链
来源：http://inn.ydjk.org.cn

a?.b?.c
来源：http://gor.zdqjudy.top

[U86] JS：空值合并
来源：http://cxu.birdmap.top

a ?? b
来源：http://dde.sjlbkw.cn

[U87] JS：解构默认值
来源：http://lbv.xylfe.cn

const { a = 1, b = 2 } = obj;
来源：http://kso.gzhubu.top

[U88] JS：对象展开合并
来源：http://kbf.zhijiandao.cn

{ ...a, ...b }
来源：http://qjt.chenjidiqi.icu

[U89] JS：数组去重
来源：http://jxs.tianlin.xyz

[...new Set(arr)]
来源：http://yvm.yueranfly.top

[U90] JS：数字数组排序
来源：http://whn.nanxinkj.top

[...arr].sort((a, b) => a - b)
来源：http://dbr.chenlongwang.top

[U91] JS：对象键值遍历
来源：http://fzf.meibo888.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pbf.ehwqpu.com

[U92] JS：深拷贝
来源：http://fgg.smart0.xyz

structuredClone(obj)
来源：http://xax.hnxiangtu.top

[U93] JS：模板字符串
来源：http://yqc.jinqigufen.top

`共 ${n} 条`
来源：http://ojx.wangdashe.top

[U94] JS：箭头函数
来源：http://jvj.52xcode.cn

const double = x => x * 2;
来源：http://vlx.jinyuanbaomall.cn

[U95] JS：Promise 包装
来源：http://dmu.tianlin.xyz

new Promise((resolve, reject) => {})
来源：http://bmn.hongshengwenyu.top

[U96] JS：async/await 与异常
来源：http://skg.bjfxy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cyi.nanxinkj.top

[U97] JS：并发请求
来源：http://wfx.hesvh.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ibc.jinqigufen.top

[U98] JS：fetch 带 JSON
来源：http://jmi.iojbl.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qbp.zhaomingkeji.xyz

[U99] JS：事件监听
来源：http://ynu.jinyuanbaomall.cn

el.addEventListener("click", e => {})
来源：http://jwy.vehdjk.com

[U100] JS：DOM 查询
来源：http://gzk.shuidangran.top

document.querySelector(".item")
来源：http://qpy.ivvv.top

[U101] JS：classList 操作
来源：http://mla.iojbl.cn

el.classList.toggle("active")
来源：http://gua.shzxlz.cn

[U102] JS：本地存储
来源：http://spj.yj20258.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://vqk.meibo888.top

[U103] JS：定时器
来源：http://xzm.cashguo.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wnh.kuanghao11.cn

[U104] JS：防抖
来源：http://ytb.tanke756.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mzy.redwolf501.top

[U105] JS：节流
来源：http://pms.vqdsnc.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://atq.hywenlv.cn

[U106] JS：日期格式化
来源：http://clp.ybcxt.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://smh.jinqigufen.top

[U107] JS：数字千分位
来源：http://jtg.aizwys.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nii.fzhhl.top

[U108] JS：随机整数
来源：http://gkr.yj202588.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gqv.fktsv.cn

[U109] JS：数组分组
来源：http://ypf.redwolf501.top

Object.groupBy(arr, x => x.type)
来源：http://gxa.xinyue.icu

[U110] JS：数组分块
来源：http://peb.cucudq.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://azh.shuidangran.top

[U111] JS：对象转 Map
来源：http://rwu.yuanzhike.top

new Map(Object.entries(obj))
来源：http://jlf.ywan-chungtsiang.top

[U112] JS：字符串补位
来源：http://utc.yueranfly.top

"7".padStart(3, "0")
来源：http://zky.guannengcc.top

[U113] JS：正则替换全部
来源：http://gmg.fengsongda.top

s.replaceAll("a", "b")
来源：http://huo.xuanzx.com

[U114] JS：JSON 深比较
来源：http://ful.jinqigfzy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://pjw.zhaomingkeji.xyz

[U115] JS：生成 UUID
来源：http://ica.gaohongyu789.top

crypto.randomUUID()
来源：http://dif.jianghu66.top

[U116] JS：类型检查（JSDoc）
来源：http://pgf.daxiang520.top

/** @param {string} name */ function f(name) {}
来源：http://aca.mhx1999.top

[U117] JS：单元测试
来源：http://eko.yuxming.cn

npm i -D vitest;  npx vitest
来源：http://hwy.hnxiangtu.top

[U118] JS：开发服务器
来源：http://vgt.xziqi.cn

npm i -D vite;  npx vite
来源：http://mca.chenjidiqi.icu

[U119] JS：生产构建
来源：http://ejo.guannengcc.top

npx vite build
来源：http://oci.jyoumei.cn

[U120] JS：读取环境变量（Vite）
来源：http://klj.yangfankeji.com

import.meta.env.VITE_API_URL
来源：http://rvl.jinqigufen.top

================================================================================
来源：http://nhj.fzhhl.top

统计汇总
来源：http://bdr.cucudq.cn

================================================================================
来源：http://lci.yueranfly.top

按语言统计（条）：
来源：http://vru.xuetiantiany.cn

Python ......... 252
来源：http://qbl.vehdjk.com

PHP ............ 252
来源：http://azk.jinyuanbaomall.cn

JavaScript ..... 252
来源：http://ddl.jiagoushi.top

TypeScript ..... 212
来源：http://qel.zdbjq.cn

Java ........... 212
来源：http://ccz.hammf.cn

Go ............. 212
来源：http://xfk.sufxvd.cn

Ruby ........... 212
来源：http://mjp.hywenlv.cn

C# ............. 212
来源：http://drs.zycfv.cn

C .............. 30
来源：http://qmx.ehwqpu.com

C++ ............ 30
来源：http://zxu.sjlbkw.cn

SQL ............ 90
来源：http://ixa.316326.xyz

Bash ........... 80
来源：http://znv.nwbrower.top

Kotlin ......... 15
来源：http://vzk.aizwys.cn

Swift .......... 15
来源：http://ypt.bjfxy.top

Lua ............ 10
来源：http://tep.zhoulong.xyz

Perl ........... 10
来源：http://aqr.gzhubu.top

Scala .......... 10
来源：http://tnh.snrcjt.cn

------------------------------------
来源：http://kut.pengpengdd.cyou

合计 ........... 2106 条
来源：http://sbs.yj202588.top

按章节统计：
来源：http://gdk.yuanzhike.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mds.pycfn.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ixn.ehwqpu.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nid.nanxuanxn.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cri.yj20258.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dnl.jiagoushi.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wop.andypj.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ndj.bjfxy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://aat.316326.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lrb.xinyue.icu

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jfb.hywenlv.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pus.ppjwa.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qxf.yonumen.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uvj.sjlbkw.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lix.gogol.net.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://agv.tian-w.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://pxu.snrcjt.cn

Q SQL 专题                              90
来源：http://ewg.gaohongyu789.top

R Bash 专题                             80
来源：http://jju.dianchejie.cn

S C / C++ 专题                          60
来源：http://ohp.ivvv.top

T 其他语言补充                          60
来源：http://xiu.xuanzx.com

U 高频实用片段                         120
来源：http://xqd.yvedp.cn

------------------------------------
来源：http://jao.yj20258888.top

合计                                  2106 条
来源：http://rps.shzxlz.cn

--------------------------------------------------------------------------------
来源：http://ube.quarkkingdee.top

使用提醒
来源：http://kxf.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://xkj.vqdsnc.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zpn.yj202588.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://emu.ybcxt.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://kgs.fzhhl.top

在旧版本上使用前请先确认语法支持情况。
来源：http://bbg.shzxlz.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hsf.tian-w.cn

—— 文件结束 ——
来源：http://xmu.svipenyu.cn

================================================================================
来源：http://cez.cucudq.cn

程序语言常见例子速查手册（2024 版）
来源：http://pqq.wangshuangyany.cn

Common Programming Examples Cheat Book
来源：http://snb.gaohongyu789.top

================================================================================
来源：http://zoz.xuanzx.com

【收录内容】
来源：http://dav.hesvh.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ohz.iojbl.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hjt.316326.xyz

SQL · Bash · C · C++
来源：http://kyt.nanxinkj.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://uba.ctjpmb.com

【使用说明】
来源：http://gtr.quarkkingdee.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bno.jqgufenzy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xhz.hysaishi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nzg.yfazqb.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zns.gaohongyu789.top

Bash:  Shell         C:     C             C++:   C++
来源：http://pyx.svipenyu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://edi.fzhhl.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bqv.redwolf501.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dcw.snrcjt.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rpz.fktsv.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mii.9152youxi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://nre.sufxvd.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ujs.fzhhl.top

【文件统计】
来源：http://ypi.jinqigufen.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ifi.jqgufenzy.top

--------------------------------------------------------------------------------
来源：http://nea.chenjidiqi.icu

目  录
来源：http://aio.jyoumei.cn

--------------------------------------------------------------------------------
来源：http://jiw.yvedp.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ugy.sxryk.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qef.vehdjk.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xqu.bbcook.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bdx.vehdjk.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rwt.sxryk.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gfc.mhx1999.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rxw.xuetiantiany.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nps.aibaodan.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zei.zycfv.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jqr.jiagoushi.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hsb.yuanzhike.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://sdo.ydjk.org.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fud.yuanzhike.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tiu.epnwcf.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xwu.sufxvd.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ule.cheryme.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://uyk.hammf.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://tjp.yj20258888.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://gtl.aizwys.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://enr.zhijiandao.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://woi.ppjwa.cn

================================================================================
来源：http://ybk.tian-w.cn

A. 基础语法与类型
来源：http://sgs.tanke756.top

================================================================================
来源：http://wkl.xuetiantiany.cn

[A01] Hello World
来源：http://euf.yongpay.top

Py:   print("Hello, World!")
来源：http://jza.epnwcf.com

PHP:  echo "Hello, World!";
来源：http://pjf.sxryk.cn

JS:   console.log("Hello, World!");
来源：http://pjt.shuidangran.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pxv.52xcode.cn

Java: System.out.println("Hello, World!");
来源：http://mpn.pycfn.com

Go:   fmt.Println("Hello, World!")
来源：http://pkg.cheryme.top

Ruby: puts "Hello, World!"
来源：http://qkv.jianghu66.top

C#:   Console.WriteLine("Hello, World!");
来源：http://kch.jinghuilouyu.cn

[A02] 变量声明与赋值
来源：http://fqg.yanxiufei.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://asa.jyoumei.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://qkz.smart0.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://csq.sjlbkw.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://uwd.hongshengwenyu.top

Java: String name = "Alex"; int age = 20;
来源：http://wbc.jqgufenzy.top

Go:   name := "Alex"; age := 20
来源：http://bya.cdnleiting.top

Ruby: name = "Alex"; age = 20
来源：http://cit.sufxvd.cn

C#:   string name = "Alex"; int age = 20;
来源：http://qyk.iojbl.cn

[A03] 常量定义
来源：http://opa.hnqzz.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xtl.xinyue.icu

PHP:  const PI = 3.14159;
来源：http://avr.dashuyun.cn

JS:   const PI = 3.14159;
来源：http://zpm.yonumen.top

TS:   const PI: number = 3.14159;
来源：http://lev.sysykeji.top

Java: static final double PI = 3.14159;
来源：http://vnx.cucudq.cn

Go:   const PI = 3.14159
来源：http://ftx.yonumen.top

Ruby: PI = 3.14159
来源：http://haw.jinqigufen.top

C#:   const double PI = 3.14159;
来源：http://bem.sysykeji.top

[A04] 判断变量类型
来源：http://ynz.cucudq.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://vxa.gogol.net.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ctv.xziqi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pdu.yj20258888.top

TS:   typeof x; x instanceof Date
来源：http://jtf.xziqi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kko.jiagoushi.top

Go:   reflect.TypeOf(x).Name()
来源：http://hjd.vqdsnc.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://icv.xziqi.cn

C#:   x.GetType().Name; x is int
来源：http://jqu.hammf.cn

[A05] 整数除法与取模
来源：http://cvs.bbcook.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lmx.wangdashe.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://rhw.yj202588.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://luu.tianlin.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://sqc.yj20258888.top

Java: 7 / 2; 7 % 2
来源：http://bjh.jqgfzy.top

Go:   7 / 2; 7 % 2
来源：http://kxw.vqdsnc.cn

Ruby: 7 / 2; 7 % 2
来源：http://ish.fanxiaobao.xyz

C#:   7 / 2; 7 % 2
来源：http://fcr.9152youxi.cn

[A06] 字符串转数字
来源：http://dre.yuanzhike.top

Py:   int("42"); float("3.14")
来源：http://lne.fzhhl.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ftn.shangyingyoupin.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jjk.chenzaomai.com

TS:   parseInt("42", 10); Number("42")
来源：http://qpu.cucudq.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hyi.chenlongwang.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://miu.ywan-chungtsiang.top

Ruby: "42".to_i; "3.14".to_f
来源：http://djt.andypj.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://btc.shanyushiyangkeji.top

[A07] 数字转字符串
来源：http://qfo.c1oappe.top

Py:   str(42)
来源：http://glb.jianghu66.top

PHP:  (string) 42; strval(42)
来源：http://qmg.yfazqb.com

JS:   String(42); (42).toString()
来源：http://kkq.hywenlv.cn

TS:   String(42)
来源：http://zux.c1oappe.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://hhe.ppjwa.cn

Go:   strconv.Itoa(42)
来源：http://fgv.yuxming.cn

Ruby: 42.to_s
来源：http://bjd.jqgfzy.top

C#:   42.ToString()
来源：http://osm.zhiwuduotai.top

[A08] 取整与四舍五入
来源：http://tyh.yuxming.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://xhl.ppjwa.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://yjd.tianlin.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mos.yuanzhike.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gyn.shanyushiyangkeji.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://icw.tian-w.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://azp.smart0.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://hpp.nanxuanxn.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://frn.xuetiantiany.cn

[A09] 绝对值与最大最小值
来源：http://btl.hfpthk.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://klc.yfazqb.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://eob.bbcook.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://kki.0kj1m.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://dbh.ybcxt.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://frk.daria6918.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://paz.yuanzhike.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ouv.epnwcf.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://uwy.nwbrower.top

[A10] 生成随机数
来源：http://flg.sufxvd.cn

Py:   import random; random.randint(1, 100)
来源：http://jsc.ivvv.top

PHP:  random_int(1, 100);
来源：http://mnn.zhongyouzk.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vww.ydzc1.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://gdu.aizwys.cn

Java: new Random().nextInt(100) + 1
来源：http://riv.52xcode.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hyf.yueranfly.top

Ruby: rand(1..100)
来源：http://xpf.zycfv.cn


<!-- 参考信息 -->