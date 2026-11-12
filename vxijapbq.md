代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://auu.shuidangran.top

parse_ini_file("config.ini", true)
来源：http://ptu.yfazqb.com

[U74] PHP：读取环境变量
来源：http://kve.daxiang520.top

getenv("APP_ENV") ?: "production"
来源：http://anm.zycfv.cn

[U75] PHP：依赖注入
来源：http://rko.yonumen.top

composer require psr/container
来源：http://xcr.9152youxi.cn

[U76] PHP：简单路由
来源：http://cmt.gaohongyu789.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bbp.hesvh.cn

[U77] PHP：模板渲染
来源：http://cdk.cucudq.cn

composer require twig/twig
来源：http://ipp.zycfv.cn

[U78] PHP：单元测试
来源：http://rtd.chenlongwang.top

composer require --dev phpunit/phpunit
来源：http://cxy.tanke756.top

[U79] PHP：静态分析
来源：http://igk.snrcjt.cn

composer require --dev phpstan/phpstan
来源：http://msv.zhongyouzk.top

[U80] PHP：代码规范修复
来源：http://zrg.jiagoushi.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://res.aibaodan.cn

[U81] JS：初始化项目
来源：http://kyq.52xcode.cn

npm init -y;  npm i express
来源：http://dgb.chenjidiqi.icu

[U82] JS：package.json 脚本
来源：http://jrq.quarkkingdee.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sen.bjfxy.top

[U83] JS：ES Module 导入导出
来源：http://mgv.yuxming.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zhl.yongpay.top

[U84] JS：CommonJS 写法
来源：http://bed.gaohongyu789.top

module.exports = { a };  const { a } = require("./m");
来源：http://nex.gogol.net.cn

[U85] JS：可选链
来源：http://zfg.jqgufenzy.top

a?.b?.c
来源：http://mly.yj20258888.top

[U86] JS：空值合并
来源：http://fwy.cucudq.cn

a ?? b
来源：http://alb.cqqwz.cn

[U87] JS：解构默认值
来源：http://tsu.epnwcf.com

const { a = 1, b = 2 } = obj;
来源：http://dwy.xziqi.cn

[U88] JS：对象展开合并
来源：http://gqb.ybcxt.top

{ ...a, ...b }
来源：http://tje.yj20258.top

[U89] JS：数组去重
来源：http://xyi.hcnkem.com

[...new Set(arr)]
来源：http://lzs.hysaishi.cn

[U90] JS：数字数组排序
来源：http://jtu.cashguo.top

[...arr].sort((a, b) => a - b)
来源：http://zlm.yonumen.top

[U91] JS：对象键值遍历
来源：http://sqc.hnxiangtu.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ikj.ywan-chungtsiang.top

[U92] JS：深拷贝
来源：http://zbg.svipenyu.cn

structuredClone(obj)
来源：http://lek.fehbvm.com

[U93] JS：模板字符串
来源：http://eja.cucudq.cn

`共 ${n} 条`
来源：http://lov.mhx1999.top

[U94] JS：箭头函数
来源：http://bef.zhijiandao.cn

const double = x => x * 2;
来源：http://bvq.iojbl.cn

[U95] JS：Promise 包装
来源：http://acw.sufxvd.cn

new Promise((resolve, reject) => {})
来源：http://fpt.fengsongda.top

[U96] JS：async/await 与异常
来源：http://thn.hammf.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jho.birdmap.top

[U97] JS：并发请求
来源：http://gvr.9152youxi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://dmt.redwolf501.top

[U98] JS：fetch 带 JSON
来源：http://eis.bbcook.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://myw.pengpengdd.cyou

[U99] JS：事件监听
来源：http://wsm.zhongyouzk.top

el.addEventListener("click", e => {})
来源：http://gyu.jinqigufen.top

[U100] JS：DOM 查询
来源：http://sla.zhixingplan.top

document.querySelector(".item")
来源：http://dme.bbcook.cn

[U101] JS：classList 操作
来源：http://isq.yongpay.top

el.classList.toggle("active")
来源：http://xlr.9152youxi.cn

[U102] JS：本地存储
来源：http://ujr.guowangkeji.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ifp.hammf.cn

[U103] JS：定时器
来源：http://lzm.yanxiufei.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nho.havefunace.top

[U104] JS：防抖
来源：http://xrx.ctjpmb.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pzl.zhengqikj.top

[U105] JS：节流
来源：http://hky.ydzc1.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sjt.ydjk.org.cn

[U106] JS：日期格式化
来源：http://thy.yuxming.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ept.jianghu66.top

[U107] JS：数字千分位
来源：http://tnn.sxryk.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ils.nanxinkj.top

[U108] JS：随机整数
来源：http://das.316326.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jfl.jinqigfzy.top

[U109] JS：数组分组
来源：http://div.jlsjyb.cn

Object.groupBy(arr, x => x.type)
来源：http://ftx.xziqi.cn

[U110] JS：数组分块
来源：http://evc.haohaochexian.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yql.xziqi.cn

[U111] JS：对象转 Map
来源：http://qeu.xuanzx.com

new Map(Object.entries(obj))
来源：http://twg.shuidangran.top

[U112] JS：字符串补位
来源：http://omu.fktsv.cn

"7".padStart(3, "0")
来源：http://rgw.shzxlz.cn

[U113] JS：正则替换全部
来源：http://lqk.fanxiaobao.xyz

s.replaceAll("a", "b")
来源：http://sle.tian-w.cn

[U114] JS：JSON 深比较
来源：http://vlj.0kj1m.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qqj.guannengcc.top

[U115] JS：生成 UUID
来源：http://nrd.52xcode.cn

crypto.randomUUID()
来源：http://mpn.zdbjq.cn

[U116] JS：类型检查（JSDoc）
来源：http://fbt.sufxvd.cn

/** @param {string} name */ function f(name) {}
来源：http://vtg.xuanzx.com

[U117] JS：单元测试
来源：http://txr.havefunace.top

npm i -D vitest;  npx vitest
来源：http://wdc.fktsv.cn

[U118] JS：开发服务器
来源：http://onv.yangfankeji.com

npm i -D vite;  npx vite
来源：http://sso.hongshengwenyu.top

[U119] JS：生产构建
来源：http://zmz.sysykeji.top

npx vite build
来源：http://ccp.tanke756.top

[U120] JS：读取环境变量（Vite）
来源：http://sdb.cdnleiting.top

import.meta.env.VITE_API_URL
来源：http://hvk.cdnleiting.top

================================================================================
来源：http://cfg.cdnleiting.top

统计汇总
来源：http://jgf.meibo888.top

================================================================================
来源：http://olh.chenlongwang.top

按语言统计（条）：
来源：http://qns.jinqigufen.top

Python ......... 252
来源：http://whr.yj20258.top

PHP ............ 252
来源：http://uaa.fengsongda.top

JavaScript ..... 252
来源：http://kre.sxryk.cn

TypeScript ..... 212
来源：http://gia.yongpay.top

Java ........... 212
来源：http://jjw.feifeiyinyue.top

Go ............. 212
来源：http://akd.xziqi.cn

Ruby ........... 212
来源：http://vja.chenlongwang.top

C# ............. 212
来源：http://dyo.jyoumei.cn

C .............. 30
来源：http://gwa.havefunace.top

C++ ............ 30
来源：http://qhb.birdmap.top

SQL ............ 90
来源：http://cny.yangfankeji.com

Bash ........... 80
来源：http://dqq.fzhhl.top

Kotlin ......... 15
来源：http://fdc.bjfxy.top

Swift .......... 15
来源：http://lug.zhoulong.xyz

Lua ............ 10
来源：http://dju.meibo888.top

Perl ........... 10
来源：http://yyk.xingfuxueyuan.xyz

Scala .......... 10
来源：http://zxa.guowangkeji.top

------------------------------------
来源：http://caw.havefunace.top

合计 ........... 2106 条
来源：http://ytr.yfazqb.com

按章节统计：
来源：http://hpn.zhijiandao.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xqt.dianchejie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lua.sysykeji.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://spm.xuanzx.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lfq.yuxming.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dup.jianghu66.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hot.nanxuanxn.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cis.zdqjudy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mju.mhx1999.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://trc.bjfxy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yzc.zhongyouzk.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rrd.yangfankeji.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://aun.havefunace.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jgp.fehbvm.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vtj.xinyue.icu

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ayb.cheryme.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tyg.jyoumei.cn

Q SQL 专题                              90
来源：http://snz.jqgfzy.top

R Bash 专题                             80
来源：http://xtw.cdnleiting.top

S C / C++ 专题                          60
来源：http://qwg.gaohongyu789.top

T 其他语言补充                          60
来源：http://yxn.daxiang520.top

U 高频实用片段                         120
来源：http://onj.hcnkem.com

------------------------------------
来源：http://jqe.yj202588.top

合计                                  2106 条
来源：http://hgs.hysaishi.cn

--------------------------------------------------------------------------------
来源：http://buv.cucudq.cn

使用提醒
来源：http://djh.yj20258.top

--------------------------------------------------------------------------------
来源：http://srl.bbcook.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vml.hywenlv.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kfb.hesvh.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hyj.yvedp.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ffx.zhijiandao.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://tiw.redwolf501.top

—— 文件结束 ——
来源：http://rwj.andypj.xyz

================================================================================
来源：http://qeg.cashguo.top

程序语言常见例子速查手册（2024 版）
来源：http://nqk.fzhhl.top

Common Programming Examples Cheat Book
来源：http://bww.jyoumei.cn

================================================================================
来源：http://ffk.ivvv.top

【收录内容】
来源：http://hbw.yanxiufei.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://syz.kuanghao11.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qsx.chenzaomai.com

SQL · Bash · C · C++
来源：http://pxd.wangshuangyany.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vvj.tian-w.cn

【使用说明】
来源：http://lio.zhixingplan.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nhv.yfazqb.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://exi.snrcjt.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tla.sweek.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://uum.hnxiangtu.top

Bash:  Shell         C:     C             C++:   C++
来源：http://iyy.xingfuxueyuan.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://oaf.daria6918.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zsc.quarkkingdee.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://cpm.316326.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zzf.kuanghao11.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jrd.gotoacloud.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xgm.feifeiyinyue.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ahn.xuanzx.com

【文件统计】
来源：http://jrn.tianlin.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yni.jiagoushi.top

--------------------------------------------------------------------------------
来源：http://pcc.mhx1999.top

目  录
来源：http://uzm.yanxiufei.cn

--------------------------------------------------------------------------------
来源：http://dxu.epnwcf.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fft.zhaomingkeji.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qje.ydzc1.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qhc.gzhubu.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lpf.yj20258.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://plh.vehdjk.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qkl.yanxiufei.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qgg.xuetiantiany.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ecj.havefunace.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xzw.cqqwz.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gog.tianlin.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ula.0kj1m.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qym.chenlongwang.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qap.hywenlv.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://nba.tarul.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://puq.nwbrower.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bbo.fehbvm.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qix.birdmap.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://bmt.fktsv.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ams.zhongyouzk.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gxc.andypj.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://bco.xinyue.icu

================================================================================
来源：http://njp.meibo888.top

A. 基础语法与类型
来源：http://qsz.bjfxy.top

================================================================================
来源：http://npc.redwolf501.top

[A01] Hello World
来源：http://kjn.shanyushiyangkeji.top

Py:   print("Hello, World!")
来源：http://jfv.tianlin.xyz

PHP:  echo "Hello, World!";
来源：http://czq.hfpthk.cn

JS:   console.log("Hello, World!");
来源：http://asx.fzhhl.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pao.meibo888.top

Java: System.out.println("Hello, World!");
来源：http://ann.gogol.net.cn

Go:   fmt.Println("Hello, World!")
来源：http://itb.hnxiangtu.top

Ruby: puts "Hello, World!"
来源：http://yhm.chenlongwang.top

C#:   Console.WriteLine("Hello, World!");
来源：http://dhs.fehbvm.com

[A02] 变量声明与赋值
来源：http://fzz.jinghuilouyu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dnh.ehwqpu.com

PHP:  $name = "Alex"; $age = 20;
来源：http://tcv.tian-w.cn

JS:   let name = "Alex"; const age = 20;
来源：http://rzz.dashuyun.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wbu.zdbjq.cn

Java: String name = "Alex"; int age = 20;
来源：http://lfj.xuanzx.com

Go:   name := "Alex"; age := 20
来源：http://owy.sjlbkw.cn

Ruby: name = "Alex"; age = 20
来源：http://tqv.chenjidiqi.icu

C#:   string name = "Alex"; int age = 20;
来源：http://rkc.smart0.xyz

[A03] 常量定义
来源：http://qxg.cashguo.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ebm.zhongyouzk.top

PHP:  const PI = 3.14159;
来源：http://slz.zdbjq.cn

JS:   const PI = 3.14159;
来源：http://pwj.sysykeji.top

TS:   const PI: number = 3.14159;
来源：http://jyg.hywenlv.cn

Java: static final double PI = 3.14159;
来源：http://wrh.jiagoushi.top

Go:   const PI = 3.14159
来源：http://nvf.pengpengdd.cyou

Ruby: PI = 3.14159
来源：http://gsa.xuanzx.com

C#:   const double PI = 3.14159;
来源：http://pgr.shuidangran.top

[A04] 判断变量类型
来源：http://bjb.jiagoushi.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://twk.tian-w.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wtg.jyoumei.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bwn.zhoulong.xyz

TS:   typeof x; x instanceof Date
来源：http://fac.ivvv.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mgl.hcnkem.com

Go:   reflect.TypeOf(x).Name()
来源：http://ajh.gotoacloud.top

Ruby: x.class; x.is_a?(Integer)
来源：http://wit.vehdjk.com

C#:   x.GetType().Name; x is int
来源：http://arf.cdnleiting.top

[A05] 整数除法与取模
来源：http://nkv.sysykeji.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://osr.gotoacloud.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://odf.yueranfly.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://eqw.yangfankeji.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hiw.fktsv.cn

Java: 7 / 2; 7 % 2
来源：http://oyu.jinqigufen.top

Go:   7 / 2; 7 % 2
来源：http://hvy.gogol.net.cn

Ruby: 7 / 2; 7 % 2
来源：http://dem.redwolf501.top

C#:   7 / 2; 7 % 2
来源：http://oxh.yongpay.top

[A06] 字符串转数字
来源：http://uit.zhiwuduotai.top

Py:   int("42"); float("3.14")
来源：http://shm.tianlin.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wcb.zdbjq.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nxk.cashguo.top

TS:   parseInt("42", 10); Number("42")
来源：http://iqs.yvedp.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ehd.zycfv.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://uit.svipenyu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://klx.fktsv.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mww.yuanzhike.top

[A07] 数字转字符串
来源：http://fhh.xziqi.cn

Py:   str(42)
来源：http://mmo.guannengcc.top

PHP:  (string) 42; strval(42)
来源：http://qdh.nanxinkj.top

JS:   String(42); (42).toString()
来源：http://wns.tanke756.top

TS:   String(42)
来源：http://zti.daxiang520.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://wet.jinghuilouyu.cn

Go:   strconv.Itoa(42)
来源：http://tph.cashguo.top

Ruby: 42.to_s
来源：http://cho.hammf.cn

C#:   42.ToString()
来源：http://bto.xinyue.icu

[A08] 取整与四舍五入
来源：http://kod.zdqjudy.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hyl.ppjwa.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hxd.yangfankeji.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://rbi.dashuyun.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://kbs.jiagoushi.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xia.cashguo.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kgd.dianchejie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://taw.vehdjk.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lik.wangdashe.top

[A09] 绝对值与最大最小值
来源：http://nnu.shuidangran.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gob.fehbvm.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://kqx.xziqi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vkp.shanyushiyangkeji.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vsd.pycfn.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ktk.yj202588.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fjo.jyoumei.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://asf.snrcjt.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://nxy.316326.xyz

[A10] 生成随机数
来源：http://vbv.aibaodan.cn

Py:   import random; random.randint(1, 100)
来源：http://edb.sufxvd.cn

PHP:  random_int(1, 100);
来源：http://zkk.daxiang520.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mhk.zdqjudy.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://owd.bbcook.cn

Java: new Random().nextInt(100) + 1
来源：http://dok.mhx1999.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://rsc.tianlin.xyz

Ruby: rand(1..100)
来源：http://adm.shanyushiyangtech.top

C#:   new Random().Next(1, 101)
来源：http://fzp.uphjek.com

[A11] 条件表达式（三元）
来源：http://kuv.hammf.cn

Py:   "yes" if x > 0 else "no"
来源：http://tlc.cqqwz.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://lly.nwbrower.top

JS:   x > 0 ? "yes" : "no"
来源：http://zce.kuanghao11.cn

TS:   x > 0 ? "yes" : "no"
来源：http://nwb.cashguo.top

Java: x > 0 ? "yes" : "no"
来源：http://qpn.wangdashe.top

Go:   // 无三元运算符，需用 if 语句
来源：http://xeo.hywenlv.cn


<!-- 参考信息 -->