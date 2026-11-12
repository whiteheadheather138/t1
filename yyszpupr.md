代发 wailian999

[U75] PHP：依赖注入
来源：http://ymd.cucudq.cn

composer require psr/container
来源：http://stw.havefunace.top

[U76] PHP：简单路由
来源：http://wmz.zhaomingkeji.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yao.gzhubu.top

[U77] PHP：模板渲染
来源：http://lrs.jqgfzy.top

composer require twig/twig
来源：http://svl.meibo888.top

[U78] PHP：单元测试
来源：http://iom.yonumen.top

composer require --dev phpunit/phpunit
来源：http://ozw.cheryme.top

[U79] PHP：静态分析
来源：http://xut.birdmap.top

composer require --dev phpstan/phpstan
来源：http://cee.gotoacloud.top

[U80] PHP：代码规范修复
来源：http://keu.zhengqikj.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://bde.cashguo.top

[U81] JS：初始化项目
来源：http://tpt.guowangkeji.top

npm init -y;  npm i express
来源：http://klq.hesvh.cn

[U82] JS：package.json 脚本
来源：http://cdc.xuanzx.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gtu.hammf.cn

[U83] JS：ES Module 导入导出
来源：http://mio.jianghu66.top

export const a = 1;  import { a } from "./m.js";
来源：http://xhx.jinyuanbaomall.cn

[U84] JS：CommonJS 写法
来源：http://msv.cashguo.top

module.exports = { a };  const { a } = require("./m");
来源：http://tmc.9152youxi.cn

[U85] JS：可选链
来源：http://amr.sweek.top

a?.b?.c
来源：http://ffj.tarul.cn

[U86] JS：空值合并
来源：http://rhb.guannengcc.top

a ?? b
来源：http://oog.daxiang520.top

[U87] JS：解构默认值
来源：http://nok.cdnleiting.top

const { a = 1, b = 2 } = obj;
来源：http://gtx.cqqwz.cn

[U88] JS：对象展开合并
来源：http://qvr.iojbl.cn

{ ...a, ...b }
来源：http://wfz.yonumen.top

[U89] JS：数组去重
来源：http://iqi.zdbjq.cn

[...new Set(arr)]
来源：http://dgv.gaohongyu789.top

[U90] JS：数字数组排序
来源：http://dua.sufxvd.cn

[...arr].sort((a, b) => a - b)
来源：http://vej.pengpengdd.cyou

[U91] JS：对象键值遍历
来源：http://ckw.uphjek.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://uip.zdqjudy.top

[U92] JS：深拷贝
来源：http://qwm.yj20258888.top

structuredClone(obj)
来源：http://jzn.zhiwuduotai.top

[U93] JS：模板字符串
来源：http://avp.cheryme.top

`共 ${n} 条`
来源：http://pim.jqgfzy.top

[U94] JS：箭头函数
来源：http://xku.ivvv.top

const double = x => x * 2;
来源：http://omo.yonumen.top

[U95] JS：Promise 包装
来源：http://yde.yvedp.cn

new Promise((resolve, reject) => {})
来源：http://mpe.sysykeji.top

[U96] JS：async/await 与异常
来源：http://ptj.hnqzz.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lcw.sweek.top

[U97] JS：并发请求
来源：http://dkf.hysaishi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rid.hysaishi.cn

[U98] JS：fetch 带 JSON
来源：http://sal.ywan-chungtsiang.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ikv.tanke756.top

[U99] JS：事件监听
来源：http://tcz.iojbl.cn

el.addEventListener("click", e => {})
来源：http://dkh.jinghuilouyu.cn

[U100] JS：DOM 查询
来源：http://npo.uphjek.com

document.querySelector(".item")
来源：http://yis.yangfankeji.com

[U101] JS：classList 操作
来源：http://mfk.smart0.xyz

el.classList.toggle("active")
来源：http://efw.nwbrower.top

[U102] JS：本地存储
来源：http://ewr.hywenlv.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dnr.hammf.cn

[U103] JS：定时器
来源：http://zyd.snrcjt.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cwf.jinyuanbaomall.cn

[U104] JS：防抖
来源：http://ndn.wangdashe.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tjd.dianchejie.cn

[U105] JS：节流
来源：http://avf.sjlbkw.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ohm.fehbvm.com

[U106] JS：日期格式化
来源：http://vwa.yj202588.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fzh.guannengcc.top

[U107] JS：数字千分位
来源：http://jse.jianghu66.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rez.zdbjq.cn

[U108] JS：随机整数
来源：http://hij.sufxvd.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dem.jinghuilouyu.cn

[U109] JS：数组分组
来源：http://kfu.shanyushiyangtech.top

Object.groupBy(arr, x => x.type)
来源：http://ptl.haohaochexian.top

[U110] JS：数组分块
来源：http://xqx.zhoulong.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://inj.xinyue.icu

[U111] JS：对象转 Map
来源：http://ozj.hnxiangtu.top

new Map(Object.entries(obj))
来源：http://zwy.shzxlz.cn

[U112] JS：字符串补位
来源：http://fak.zhongyouzk.top

"7".padStart(3, "0")
来源：http://tmz.52xcode.cn

[U113] JS：正则替换全部
来源：http://jol.ppjwa.cn

s.replaceAll("a", "b")
来源：http://qsh.iojbl.cn

[U114] JS：JSON 深比较
来源：http://lka.chenjidiqi.icu

JSON.stringify(a) === JSON.stringify(b)
来源：http://qkz.nanxinkj.top

[U115] JS：生成 UUID
来源：http://ehy.ehwqpu.com

crypto.randomUUID()
来源：http://jhe.sufxvd.cn

[U116] JS：类型检查（JSDoc）
来源：http://iti.zhixingplan.top

/** @param {string} name */ function f(name) {}
来源：http://csp.zhijiandao.cn

[U117] JS：单元测试
来源：http://eqn.hesvh.cn

npm i -D vitest;  npx vitest
来源：http://zer.ywan-chungtsiang.top

[U118] JS：开发服务器
来源：http://akd.aizwys.cn

npm i -D vite;  npx vite
来源：http://ovh.vehdjk.com

[U119] JS：生产构建
来源：http://ifn.gzhubu.top

npx vite build
来源：http://eoy.yuxming.cn

[U120] JS：读取环境变量（Vite）
来源：http://roq.hysaishi.cn

import.meta.env.VITE_API_URL
来源：http://knc.gaohongyu789.top

================================================================================
来源：http://agi.jinyuanbaomall.cn

统计汇总
来源：http://acl.sufxvd.cn

================================================================================
来源：http://kyj.nanxuanxn.top

按语言统计（条）：
来源：http://wvm.zdqjudy.top

Python ......... 252
来源：http://hhs.fzhhl.top

PHP ............ 252
来源：http://yeg.zdqjudy.top

JavaScript ..... 252
来源：http://bpd.dianchejie.cn

TypeScript ..... 212
来源：http://sad.snrcjt.cn

Java ........... 212
来源：http://ctc.chenzaomai.com

Go ............. 212
来源：http://cev.yj20258.top

Ruby ........... 212
来源：http://aes.yuanzhike.top

C# ............. 212
来源：http://llz.hesvh.cn

C .............. 30
来源：http://jcw.mhx1999.top

C++ ............ 30
来源：http://lvz.yanxiufei.cn

SQL ............ 90
来源：http://gqf.fehbvm.com

Bash ........... 80
来源：http://fwo.zdqjudy.top

Kotlin ......... 15
来源：http://qrj.wangshuangyany.cn

Swift .......... 15
来源：http://cfw.aizwys.cn

Lua ............ 10
来源：http://uoe.fanxiaobao.xyz

Perl ........... 10
来源：http://ach.hesvh.cn

Scala .......... 10
来源：http://ncm.chenzaomai.com

------------------------------------
来源：http://tjq.0kj1m.cn

合计 ........... 2106 条
来源：http://bmd.quarkkingdee.top

按章节统计：
来源：http://sjl.daxiang520.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pbn.tanke756.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://eqh.wangdashe.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://twm.hfpthk.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tty.xuanzx.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://agl.cashguo.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hoy.nwbrower.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jxi.yfazqb.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zox.shuidangran.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://szk.ivvv.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zjg.guowangkeji.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fel.uphjek.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zei.jianghu66.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://eqp.gotoacloud.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://axr.yanxiufei.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pxi.9152youxi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dia.hysaishi.cn

Q SQL 专题                              90
来源：http://scv.yuxming.cn

R Bash 专题                             80
来源：http://hhb.jqgfzy.top

S C / C++ 专题                          60
来源：http://edj.hywenlv.cn

T 其他语言补充                          60
来源：http://ftn.xingfuxueyuan.xyz

U 高频实用片段                         120
来源：http://tiu.0kj1m.cn

------------------------------------
来源：http://swx.smart0.xyz

合计                                  2106 条
来源：http://ezv.jyoumei.cn

--------------------------------------------------------------------------------
来源：http://tyz.hnqzz.top

使用提醒
来源：http://cpe.jinqigufen.top

--------------------------------------------------------------------------------
来源：http://odc.jiagoushi.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://roe.zhijiandao.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kpr.havefunace.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xsm.zhongyouzk.top

在旧版本上使用前请先确认语法支持情况。
来源：http://smo.nwbrower.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bwv.fktsv.cn

—— 文件结束 ——
来源：http://spq.hesvh.cn

================================================================================
来源：http://doy.yanxiufei.cn

程序语言常见例子速查手册（2024 版）
来源：http://isi.hongshengwenyu.top

Common Programming Examples Cheat Book
来源：http://izc.birdmap.top

================================================================================
来源：http://esm.ctjpmb.com

【收录内容】
来源：http://xfu.shzxlz.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://pia.xylfe.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://brs.nanxuanxn.top

SQL · Bash · C · C++
来源：http://ycz.tanke756.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://clh.cheryme.top

【使用说明】
来源：http://bad.yuanzhike.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://edw.hammf.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cjt.chenjidiqi.icu

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://uqi.yj202588.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zdq.dianchejie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://qyu.svipenyu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://job.dianchejie.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://dje.birdmap.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zpl.zdbjq.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ewu.tianlin.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fxx.daxiang520.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mnh.shangyingyoupin.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qcb.gzhubu.top

【文件统计】
来源：http://sci.0kj1m.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://uxy.hysaishi.cn

--------------------------------------------------------------------------------
来源：http://rbj.iojbl.cn

目  录
来源：http://prv.svipenyu.cn

--------------------------------------------------------------------------------
来源：http://cri.cdnleiting.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pdb.jyoumei.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://asn.zhoulong.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vps.daria6918.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://sjb.cheryme.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fti.daria6918.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kfg.0kj1m.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://cyt.shanyushiyangkeji.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://srn.hesvh.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xds.guowangkeji.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://oct.hnxiangtu.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://drk.cheryme.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fpo.jianghu66.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://sdi.xinyue.icu

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ybw.hammf.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bmj.0kj1m.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bgb.tanke756.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tmw.hnqzz.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ebd.hcnkem.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qwr.hfpthk.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://oow.zhaomingkeji.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://erm.yj202588.top

================================================================================
来源：http://jte.haohaochexian.top

A. 基础语法与类型
来源：http://yww.pengpengdd.cyou

================================================================================
来源：http://pqf.fanxiaobao.xyz

[A01] Hello World
来源：http://ofz.andypj.xyz

Py:   print("Hello, World!")
来源：http://kyo.nanxinkj.top

PHP:  echo "Hello, World!";
来源：http://nqn.chenlongwang.top

JS:   console.log("Hello, World!");
来源：http://rzi.xingfuxueyuan.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jxl.uphjek.com

Java: System.out.println("Hello, World!");
来源：http://iac.shuidangran.top

Go:   fmt.Println("Hello, World!")
来源：http://btc.pycfn.com

Ruby: puts "Hello, World!"
来源：http://pid.shanyushiyangtech.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ykp.bjfxy.top

[A02] 变量声明与赋值
来源：http://iqp.jinghuilouyu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jam.quarkkingdee.top

PHP:  $name = "Alex"; $age = 20;
来源：http://nxt.dianchejie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://gmf.jqgufenzy.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fci.zhixingplan.top

Java: String name = "Alex"; int age = 20;
来源：http://dbs.yongpay.top

Go:   name := "Alex"; age := 20
来源：http://txe.hcnkem.com

Ruby: name = "Alex"; age = 20
来源：http://rws.havefunace.top

C#:   string name = "Alex"; int age = 20;
来源：http://lvb.gaohongyu789.top

[A03] 常量定义
来源：http://sro.hysaishi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qjw.nwbrower.top

PHP:  const PI = 3.14159;
来源：http://ygm.zhijiandao.cn

JS:   const PI = 3.14159;
来源：http://ypq.aibaodan.cn

TS:   const PI: number = 3.14159;
来源：http://dbm.aizwys.cn

Java: static final double PI = 3.14159;
来源：http://ezd.zycfv.cn

Go:   const PI = 3.14159
来源：http://dwg.xuanzx.com

Ruby: PI = 3.14159
来源：http://qdg.tianlin.xyz

C#:   const double PI = 3.14159;
来源：http://hcg.ctjpmb.com

[A04] 判断变量类型
来源：http://hmm.yuanzhike.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://osv.xingfuxueyuan.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zyk.nwbrower.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mxu.mhx1999.top

TS:   typeof x; x instanceof Date
来源：http://bkl.hesvh.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://nqe.jinyuanbaomall.cn

Go:   reflect.TypeOf(x).Name()
来源：http://bxu.shanyushiyangkeji.top

Ruby: x.class; x.is_a?(Integer)
来源：http://azh.fehbvm.com

C#:   x.GetType().Name; x is int
来源：http://mgn.sysykeji.top

[A05] 整数除法与取模
来源：http://fsg.nwbrower.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lsp.vehdjk.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://znk.hnxiangtu.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bfd.xuanzx.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://foa.sjlbkw.cn

Java: 7 / 2; 7 % 2
来源：http://met.cqqwz.cn

Go:   7 / 2; 7 % 2
来源：http://eed.shuidangran.top

Ruby: 7 / 2; 7 % 2
来源：http://kcr.gotoacloud.top

C#:   7 / 2; 7 % 2
来源：http://qgq.zdqjudy.top

[A06] 字符串转数字
来源：http://euh.yueranfly.top

Py:   int("42"); float("3.14")
来源：http://mem.birdmap.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://paf.hammf.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xqo.yvedp.cn

TS:   parseInt("42", 10); Number("42")
来源：http://tzs.gzhubu.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gkf.jinghuilouyu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xvo.jinghuilouyu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://zwj.9152youxi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jrj.daria6918.cn

[A07] 数字转字符串
来源：http://knp.nanxuanxn.top

Py:   str(42)
来源：http://fbo.gotoacloud.top

PHP:  (string) 42; strval(42)
来源：http://gqn.xuetiantiany.cn

JS:   String(42); (42).toString()
来源：http://dre.hesvh.cn

TS:   String(42)
来源：http://qlf.jinghuilouyu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://gon.zhiwuduotai.top

Go:   strconv.Itoa(42)
来源：http://jth.shangyingyoupin.top

Ruby: 42.to_s
来源：http://ejh.316326.xyz

C#:   42.ToString()
来源：http://ter.chenzaomai.com

[A08] 取整与四舍五入
来源：http://oon.yj20258.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://eod.feifeiyinyue.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qwz.ydjk.org.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://krh.yanxiufei.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wtt.gzhubu.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nml.zhixingplan.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gby.yonumen.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://hnx.316326.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lvw.mhx1999.top

[A09] 绝对值与最大最小值
来源：http://bgy.hywenlv.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xvi.jyoumei.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://fks.gzhubu.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://axa.zhongyouzk.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://sua.shzxlz.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xbe.havefunace.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xbr.jlsjyb.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lsg.nanxuanxn.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://omm.52xcode.cn

[A10] 生成随机数
来源：http://lkf.jinyuanbaomall.cn

Py:   import random; random.randint(1, 100)
来源：http://lqc.dashuyun.cn

PHP:  random_int(1, 100);
来源：http://yta.hfpthk.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lcv.nanxuanxn.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qvr.bbcook.cn

Java: new Random().nextInt(100) + 1
来源：http://lrj.ybcxt.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://nwr.zhiwuduotai.top

Ruby: rand(1..100)
来源：http://mkf.xylfe.cn

C#:   new Random().Next(1, 101)
来源：http://knw.daria6918.cn

[A11] 条件表达式（三元）
来源：http://oxc.0kj1m.cn

Py:   "yes" if x > 0 else "no"
来源：http://ays.zhoulong.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://bkq.shzxlz.cn

JS:   x > 0 ? "yes" : "no"
来源：http://sgw.fanxiaobao.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://uxl.zdqjudy.top

Java: x > 0 ? "yes" : "no"
来源：http://zfm.316326.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://vde.ctjpmb.com

Ruby: x > 0 ? "yes" : "no"
来源：http://hmk.jqgufenzy.top

C#:   x > 0 ? "yes" : "no"
来源：http://ape.zdqjudy.top

[A12] 字符串插值 / 格式化
来源：http://hvm.zdqjudy.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bot.hywenlv.cn


<!-- 参考信息 -->