代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://ekh.cashguo.top

parse_ini_file("config.ini", true)
来源：http://rwv.xylfe.cn

[U74] PHP：读取环境变量
来源：http://equ.9152youxi.cn

getenv("APP_ENV") ?: "production"
来源：http://bhw.feifeiyinyue.top

[U75] PHP：依赖注入
来源：http://xfw.0kj1m.cn

composer require psr/container
来源：http://rss.nwbrower.top

[U76] PHP：简单路由
来源：http://vha.andypj.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://abc.sjlbkw.cn

[U77] PHP：模板渲染
来源：http://vxg.hesvh.cn

composer require twig/twig
来源：http://aiz.smart0.xyz

[U78] PHP：单元测试
来源：http://ela.yongpay.top

composer require --dev phpunit/phpunit
来源：http://yml.ybcxt.top

[U79] PHP：静态分析
来源：http://hyo.zhongyouzk.top

composer require --dev phpstan/phpstan
来源：http://zqy.0kj1m.cn

[U80] PHP：代码规范修复
来源：http://eit.hywenlv.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://fjd.aibaodan.cn

[U81] JS：初始化项目
来源：http://wyb.chenlongwang.top

npm init -y;  npm i express
来源：http://nvo.yfazqb.com

[U82] JS：package.json 脚本
来源：http://psz.xuanzx.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gvd.shangyingyoupin.top

[U83] JS：ES Module 导入导出
来源：http://cjp.shanyushiyangkeji.top

export const a = 1;  import { a } from "./m.js";
来源：http://gjl.hfpthk.cn

[U84] JS：CommonJS 写法
来源：http://ssu.jianghu66.top

module.exports = { a };  const { a } = require("./m");
来源：http://mgu.jlsjyb.cn

[U85] JS：可选链
来源：http://ilo.yangfankeji.com

a?.b?.c
来源：http://mqv.hywenlv.cn

[U86] JS：空值合并
来源：http://dmz.hywenlv.cn

a ?? b
来源：http://lng.yj20258.top

[U87] JS：解构默认值
来源：http://tps.ehwqpu.com

const { a = 1, b = 2 } = obj;
来源：http://dow.sweek.top

[U88] JS：对象展开合并
来源：http://opa.chenjidiqi.icu

{ ...a, ...b }
来源：http://esk.ivvv.top

[U89] JS：数组去重
来源：http://tfy.c1oappe.top

[...new Set(arr)]
来源：http://tuk.uphjek.com

[U90] JS：数字数组排序
来源：http://xwf.ehwqpu.com

[...arr].sort((a, b) => a - b)
来源：http://hmn.sweek.top

[U91] JS：对象键值遍历
来源：http://abm.fktsv.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bek.cashguo.top

[U92] JS：深拷贝
来源：http://wzj.yonumen.top

structuredClone(obj)
来源：http://bkg.yongpay.top

[U93] JS：模板字符串
来源：http://sym.wangdashe.top

`共 ${n} 条`
来源：http://hzq.ydzc1.top

[U94] JS：箭头函数
来源：http://acd.52xcode.cn

const double = x => x * 2;
来源：http://hzw.kuanghao11.cn

[U95] JS：Promise 包装
来源：http://whi.ybcxt.top

new Promise((resolve, reject) => {})
来源：http://czz.yvedp.cn

[U96] JS：async/await 与异常
来源：http://xgt.guowangkeji.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ekk.daxiang520.top

[U97] JS：并发请求
来源：http://wmu.xuanzx.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://kfp.mhx1999.top

[U98] JS：fetch 带 JSON
来源：http://bww.yongpay.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nnb.cheryme.top

[U99] JS：事件监听
来源：http://prp.andypj.xyz

el.addEventListener("click", e => {})
来源：http://kql.tian-w.cn

[U100] JS：DOM 查询
来源：http://czi.jqgfzy.top

document.querySelector(".item")
来源：http://eyh.shanyushiyangkeji.top

[U101] JS：classList 操作
来源：http://zfb.cdnleiting.top

el.classList.toggle("active")
来源：http://dvs.vqdsnc.cn

[U102] JS：本地存储
来源：http://ztc.haohaochexian.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://zgv.316326.xyz

[U103] JS：定时器
来源：http://edl.fehbvm.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uba.hnxiangtu.top

[U104] JS：防抖
来源：http://dyl.pengpengdd.cyou

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ocv.fanxiaobao.xyz

[U105] JS：节流
来源：http://gvg.nanxuanxn.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://afj.tarul.cn

[U106] JS：日期格式化
来源：http://bjj.vehdjk.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://oby.zhengqikj.top

[U107] JS：数字千分位
来源：http://rcz.zhijiandao.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jgp.xinyue.icu

[U108] JS：随机整数
来源：http://fsr.ehwqpu.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nnq.nwbrower.top

[U109] JS：数组分组
来源：http://nhj.pengpengdd.cyou

Object.groupBy(arr, x => x.type)
来源：http://lrx.jinqigufen.top

[U110] JS：数组分块
来源：http://zeo.ydjk.org.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ilq.tanke756.top

[U111] JS：对象转 Map
来源：http://apg.zhijiandao.cn

new Map(Object.entries(obj))
来源：http://mmd.nanxinkj.top

[U112] JS：字符串补位
来源：http://cgx.vqdsnc.cn

"7".padStart(3, "0")
来源：http://paf.fengsongda.top

[U113] JS：正则替换全部
来源：http://coy.zhoulong.xyz

s.replaceAll("a", "b")
来源：http://byz.daria6918.cn

[U114] JS：JSON 深比较
来源：http://bla.yangfankeji.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://luc.tian-w.cn

[U115] JS：生成 UUID
来源：http://vqf.zhijiandao.cn

crypto.randomUUID()
来源：http://zrf.wangshuangyany.cn

[U116] JS：类型检查（JSDoc）
来源：http://aua.tian-w.cn

/** @param {string} name */ function f(name) {}
来源：http://dkf.yj20258888.top

[U117] JS：单元测试
来源：http://sph.bjfxy.top

npm i -D vitest;  npx vitest
来源：http://mlb.tarul.cn

[U118] JS：开发服务器
来源：http://tqd.gzhubu.top

npm i -D vite;  npx vite
来源：http://zop.shangyingyoupin.top

[U119] JS：生产构建
来源：http://vlv.zhijiandao.cn

npx vite build
来源：http://nvp.zhaomingkeji.xyz

[U120] JS：读取环境变量（Vite）
来源：http://gdq.yuxming.cn

import.meta.env.VITE_API_URL
来源：http://hvc.hesvh.cn

================================================================================
来源：http://wge.tarul.cn

统计汇总
来源：http://dyc.zhaomingkeji.xyz

================================================================================
来源：http://tao.yangfankeji.com

按语言统计（条）：
来源：http://wvx.fktsv.cn

Python ......... 252
来源：http://bes.gogol.net.cn

PHP ............ 252
来源：http://kir.yvedp.cn

JavaScript ..... 252
来源：http://rdk.tianlin.xyz

TypeScript ..... 212
来源：http://yxh.yueranfly.top

Java ........... 212
来源：http://ryd.daxiang520.top

Go ............. 212
来源：http://hje.ydzc1.top

Ruby ........... 212
来源：http://ard.xuetiantiany.cn

C# ............. 212
来源：http://vii.pengpengdd.cyou

C .............. 30
来源：http://ebd.shuidangran.top

C++ ............ 30
来源：http://poq.zdqjudy.top

SQL ............ 90
来源：http://efu.bjfxy.top

Bash ........... 80
来源：http://xgh.bbcook.cn

Kotlin ......... 15
来源：http://lxr.shzxlz.cn

Swift .......... 15
来源：http://edr.cheryme.top

Lua ............ 10
来源：http://xqu.bbcook.cn

Perl ........... 10
来源：http://vvg.dashuyun.cn

Scala .......... 10
来源：http://osp.tanke756.top

------------------------------------
来源：http://wrt.bbcook.cn

合计 ........... 2106 条
来源：http://emh.yonumen.top

按章节统计：
来源：http://ldt.xuetiantiany.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://axq.shzxlz.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xdl.0kj1m.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tco.zdbjq.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yga.mhx1999.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ftm.redwolf501.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nmw.havefunace.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dim.316326.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kjb.wangshuangyany.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nso.zhengqikj.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kdq.tianlin.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://huu.fehbvm.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xhd.xinyue.icu

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ifd.dianchejie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cog.hesvh.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qhw.jianghu66.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xmk.uphjek.com

Q SQL 专题                              90
来源：http://ljj.xylfe.cn

R Bash 专题                             80
来源：http://wzs.0kj1m.cn

S C / C++ 专题                          60
来源：http://srz.jyoumei.cn

T 其他语言补充                          60
来源：http://aet.jinqigufen.top

U 高频实用片段                         120
来源：http://bcx.cucudq.cn

------------------------------------
来源：http://hga.shzxlz.cn

合计                                  2106 条
来源：http://qzu.ehwqpu.com

--------------------------------------------------------------------------------
来源：http://ldx.yvedp.cn

使用提醒
来源：http://krb.jinghuilouyu.cn

--------------------------------------------------------------------------------
来源：http://ijr.xinyue.icu

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ami.kuanghao11.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://sfw.fengsongda.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://uzb.xingfuxueyuan.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://sss.ydjk.org.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lmv.andypj.xyz

—— 文件结束 ——
来源：http://cqc.cheryme.top

================================================================================
来源：http://owl.jianghu66.top

程序语言常见例子速查手册（2024 版）
来源：http://kwk.sxryk.cn

Common Programming Examples Cheat Book
来源：http://mqt.zhixingplan.top

================================================================================
来源：http://ysf.cdnleiting.top

【收录内容】
来源：http://iid.chenjidiqi.icu

覆盖 12 种语言 / 语法与常见 API：
来源：http://rul.fzhhl.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://thh.uphjek.com

SQL · Bash · C · C++
来源：http://wmq.jqgufenzy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://isd.zycfv.cn

【使用说明】
来源：http://wec.fanxiaobao.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cof.fanxiaobao.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://biv.zhixingplan.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jqq.smart0.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fpg.yongpay.top

Bash:  Shell         C:     C             C++:   C++
来源：http://gsz.0kj1m.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hom.tanke756.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vvm.bjfxy.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pwq.iojbl.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gzh.ctjpmb.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vcs.zhiwuduotai.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vjg.yanxiufei.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nep.uphjek.com

【文件统计】
来源：http://yjx.jqgfzy.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lah.yvedp.cn

--------------------------------------------------------------------------------
来源：http://svq.zhengqikj.top

目  录
来源：http://sft.uphjek.com

--------------------------------------------------------------------------------
来源：http://xzq.haohaochexian.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://uwv.hammf.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://iyr.yuanzhike.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xni.smart0.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://guc.dianchejie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ifb.fktsv.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://noa.vehdjk.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ftj.cashguo.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rsz.guowangkeji.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://scc.yanxiufei.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://kqh.zdqjudy.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xnc.bbcook.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rdz.xuanzx.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ray.fehbvm.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ojp.sxryk.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lut.ivvv.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ktx.ehwqpu.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://muj.yj20258888.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://gbm.yj20258.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hrh.shanyushiyangtech.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mbf.zhixingplan.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ymo.havefunace.top

================================================================================
来源：http://awj.epnwcf.com

A. 基础语法与类型
来源：http://wsq.jiagoushi.top

================================================================================
来源：http://lzu.52xcode.cn

[A01] Hello World
来源：http://nse.316326.xyz

Py:   print("Hello, World!")
来源：http://cte.chenlongwang.top

PHP:  echo "Hello, World!";
来源：http://odx.sxryk.cn

JS:   console.log("Hello, World!");
来源：http://bnl.chenzaomai.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zdt.chenlongwang.top

Java: System.out.println("Hello, World!");
来源：http://aep.c1oappe.top

Go:   fmt.Println("Hello, World!")
来源：http://vet.ivvv.top

Ruby: puts "Hello, World!"
来源：http://pck.dianchejie.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://oqd.tianlin.xyz

[A02] 变量声明与赋值
来源：http://rsd.sufxvd.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tej.hysaishi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ezd.jiagoushi.top

JS:   let name = "Alex"; const age = 20;
来源：http://pvb.jinghuilouyu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ltp.wangdashe.top

Java: String name = "Alex"; int age = 20;
来源：http://gpu.xylfe.cn

Go:   name := "Alex"; age := 20
来源：http://ptp.fengsongda.top

Ruby: name = "Alex"; age = 20
来源：http://fzy.zdqjudy.top

C#:   string name = "Alex"; int age = 20;
来源：http://uuc.yj20258888.top

[A03] 常量定义
来源：http://uyf.xziqi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ohg.vehdjk.com

PHP:  const PI = 3.14159;
来源：http://kmp.zdbjq.cn

JS:   const PI = 3.14159;
来源：http://itg.zdqjudy.top

TS:   const PI: number = 3.14159;
来源：http://emh.mhx1999.top

Java: static final double PI = 3.14159;
来源：http://tgp.zhengqikj.top

Go:   const PI = 3.14159
来源：http://etf.jyoumei.cn

Ruby: PI = 3.14159
来源：http://int.shanyushiyangtech.top

C#:   const double PI = 3.14159;
来源：http://yqq.hfpthk.cn

[A04] 判断变量类型
来源：http://jle.jyoumei.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://cfa.jqgfzy.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://oaw.aibaodan.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://txv.ydjk.org.cn

TS:   typeof x; x instanceof Date
来源：http://cqb.sxryk.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tzq.ppjwa.cn

Go:   reflect.TypeOf(x).Name()
来源：http://bcw.xinyue.icu

Ruby: x.class; x.is_a?(Integer)
来源：http://nvg.cheryme.top

C#:   x.GetType().Name; x is int
来源：http://srv.gotoacloud.top

[A05] 整数除法与取模
来源：http://kue.hnqzz.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://duq.ehwqpu.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://uiw.pengpengdd.cyou

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cqb.zhaomingkeji.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vjr.gotoacloud.top

Java: 7 / 2; 7 % 2
来源：http://avo.yvedp.cn

Go:   7 / 2; 7 % 2
来源：http://ewv.xingfuxueyuan.xyz

Ruby: 7 / 2; 7 % 2
来源：http://ymk.feifeiyinyue.top

C#:   7 / 2; 7 % 2
来源：http://acp.gzhubu.top

[A06] 字符串转数字
来源：http://nox.guowangkeji.top

Py:   int("42"); float("3.14")
来源：http://ejr.hcnkem.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hzh.cheryme.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wvx.yonumen.top

TS:   parseInt("42", 10); Number("42")
来源：http://vzo.hongshengwenyu.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://djd.hammf.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rzo.yj20258.top

Ruby: "42".to_i; "3.14".to_f
来源：http://otj.havefunace.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xqf.gaohongyu789.top

[A07] 数字转字符串
来源：http://ode.zhijiandao.cn

Py:   str(42)
来源：http://qzl.nwbrower.top

PHP:  (string) 42; strval(42)
来源：http://ykv.guannengcc.top

JS:   String(42); (42).toString()
来源：http://lgv.shuidangran.top

TS:   String(42)
来源：http://veb.epnwcf.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://tfz.mhx1999.top

Go:   strconv.Itoa(42)
来源：http://uep.hfpthk.cn

Ruby: 42.to_s
来源：http://jig.316326.xyz

C#:   42.ToString()
来源：http://pfq.ppjwa.cn

[A08] 取整与四舍五入
来源：http://soa.dashuyun.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://csw.epnwcf.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://plc.sweek.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://iqe.feifeiyinyue.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mkw.tianlin.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://seu.c1oappe.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tgc.tanke756.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://epq.haohaochexian.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fhb.hysaishi.cn

[A09] 绝对值与最大最小值
来源：http://dbm.kuanghao11.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lra.snrcjt.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rxg.svipenyu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://byd.mhx1999.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://eub.xziqi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://qxt.daria6918.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://syp.ppjwa.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gub.iojbl.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://atp.haohaochexian.top

[A10] 生成随机数
来源：http://emt.jinqigfzy.top

Py:   import random; random.randint(1, 100)
来源：http://xmi.jinghuilouyu.cn

PHP:  random_int(1, 100);
来源：http://lgj.cashguo.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://tto.fktsv.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ale.tian-w.cn

Java: new Random().nextInt(100) + 1
来源：http://hzz.cucudq.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dye.yongpay.top

Ruby: rand(1..100)
来源：http://pam.jlsjyb.cn

C#:   new Random().Next(1, 101)
来源：http://vhd.chenjidiqi.icu

[A11] 条件表达式（三元）
来源：http://owo.yonumen.top

Py:   "yes" if x > 0 else "no"
来源：http://ojt.gzhubu.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://qen.yuanzhike.top

JS:   x > 0 ? "yes" : "no"
来源：http://qqv.fengsongda.top

TS:   x > 0 ? "yes" : "no"
来源：http://cal.hnqzz.top

Java: x > 0 ? "yes" : "no"
来源：http://qut.sweek.top

Go:   // 无三元运算符，需用 if 语句
来源：http://vhe.jianghu66.top


<!-- 参考信息 -->