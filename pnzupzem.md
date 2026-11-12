代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://njr.hysaishi.cn

parse_ini_file("config.ini", true)
来源：http://kak.zhijiandao.cn

[U74] PHP：读取环境变量
来源：http://qjk.yongpay.top

getenv("APP_ENV") ?: "production"
来源：http://fnz.vehdjk.com

[U75] PHP：依赖注入
来源：http://ncb.jinqigufen.top

composer require psr/container
来源：http://xyu.52xcode.cn

[U76] PHP：简单路由
来源：http://bgn.0kj1m.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://niy.hammf.cn

[U77] PHP：模板渲染
来源：http://fad.yj20258888.top

composer require twig/twig
来源：http://zvp.quarkkingdee.top

[U78] PHP：单元测试
来源：http://zpq.yanxiufei.cn

composer require --dev phpunit/phpunit
来源：http://yhi.pengpengdd.cyou

[U79] PHP：静态分析
来源：http://qyi.iojbl.cn

composer require --dev phpstan/phpstan
来源：http://mjm.pycfn.com

[U80] PHP：代码规范修复
来源：http://jbs.ctjpmb.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://gks.ctjpmb.com

[U81] JS：初始化项目
来源：http://opa.epnwcf.com

npm init -y;  npm i express
来源：http://xpq.yanxiufei.cn

[U82] JS：package.json 脚本
来源：http://agm.jlsjyb.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://uin.uphjek.com

[U83] JS：ES Module 导入导出
来源：http://dsv.yongpay.top

export const a = 1;  import { a } from "./m.js";
来源：http://bqt.yueranfly.top

[U84] JS：CommonJS 写法
来源：http://pbg.sufxvd.cn

module.exports = { a };  const { a } = require("./m");
来源：http://bpy.ivvv.top

[U85] JS：可选链
来源：http://anh.zhiwuduotai.top

a?.b?.c
来源：http://kbs.feifeiyinyue.top

[U86] JS：空值合并
来源：http://xzo.gogol.net.cn

a ?? b
来源：http://jlj.nanxinkj.top

[U87] JS：解构默认值
来源：http://qdy.vehdjk.com

const { a = 1, b = 2 } = obj;
来源：http://uqu.nwbrower.top

[U88] JS：对象展开合并
来源：http://iij.zdqjudy.top

{ ...a, ...b }
来源：http://biw.zhaomingkeji.xyz

[U89] JS：数组去重
来源：http://nwn.nwbrower.top

[...new Set(arr)]
来源：http://tmq.iojbl.cn

[U90] JS：数字数组排序
来源：http://svf.zhengqikj.top

[...arr].sort((a, b) => a - b)
来源：http://pjl.guowangkeji.top

[U91] JS：对象键值遍历
来源：http://qtl.havefunace.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://amq.fzhhl.top

[U92] JS：深拷贝
来源：http://khb.zhijiandao.cn

structuredClone(obj)
来源：http://ory.dianchejie.cn

[U93] JS：模板字符串
来源：http://abs.pycfn.com

`共 ${n} 条`
来源：http://pzl.dashuyun.cn

[U94] JS：箭头函数
来源：http://kvu.gaohongyu789.top

const double = x => x * 2;
来源：http://vjv.dashuyun.cn

[U95] JS：Promise 包装
来源：http://bdm.jlsjyb.cn

new Promise((resolve, reject) => {})
来源：http://zrr.dashuyun.cn

[U96] JS：async/await 与异常
来源：http://cpk.svipenyu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rlq.cucudq.cn

[U97] JS：并发请求
来源：http://xmc.andypj.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://noe.jinqigfzy.top

[U98] JS：fetch 带 JSON
来源：http://jln.gaohongyu789.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ief.chenzaomai.com

[U99] JS：事件监听
来源：http://twf.shanyushiyangkeji.top

el.addEventListener("click", e => {})
来源：http://vel.cheryme.top

[U100] JS：DOM 查询
来源：http://oiu.jqgfzy.top

document.querySelector(".item")
来源：http://vro.ydzc1.top

[U101] JS：classList 操作
来源：http://sis.52xcode.cn

el.classList.toggle("active")
来源：http://lbj.sjlbkw.cn

[U102] JS：本地存储
来源：http://tdv.aibaodan.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://tmt.zhengqikj.top

[U103] JS：定时器
来源：http://chr.shzxlz.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pmr.hywenlv.cn

[U104] JS：防抖
来源：http://qqu.c1oappe.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lmq.hfpthk.cn

[U105] JS：节流
来源：http://oqm.yangfankeji.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ovy.shanyushiyangkeji.top

[U106] JS：日期格式化
来源：http://byx.yanxiufei.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dcd.jqgufenzy.top

[U107] JS：数字千分位
来源：http://sxr.wangdashe.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://egj.c1oappe.top

[U108] JS：随机整数
来源：http://xgg.shuidangran.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cvo.shanyushiyangtech.top

[U109] JS：数组分组
来源：http://geo.sweek.top

Object.groupBy(arr, x => x.type)
来源：http://maz.uphjek.com

[U110] JS：数组分块
来源：http://prb.fanxiaobao.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vpi.quarkkingdee.top

[U111] JS：对象转 Map
来源：http://ztg.jiagoushi.top

new Map(Object.entries(obj))
来源：http://ggu.zhiwuduotai.top

[U112] JS：字符串补位
来源：http://cca.birdmap.top

"7".padStart(3, "0")
来源：http://rnk.zycfv.cn

[U113] JS：正则替换全部
来源：http://vvo.fktsv.cn

s.replaceAll("a", "b")
来源：http://qae.feifeiyinyue.top

[U114] JS：JSON 深比较
来源：http://gfm.yueranfly.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://mmu.yuanzhike.top

[U115] JS：生成 UUID
来源：http://wms.zhiwuduotai.top

crypto.randomUUID()
来源：http://nis.ybcxt.top

[U116] JS：类型检查（JSDoc）
来源：http://ubb.jinyuanbaomall.cn

/** @param {string} name */ function f(name) {}
来源：http://fqo.jlsjyb.cn

[U117] JS：单元测试
来源：http://ehv.yuxming.cn

npm i -D vitest;  npx vitest
来源：http://pto.ehwqpu.com

[U118] JS：开发服务器
来源：http://qmf.uphjek.com

npm i -D vite;  npx vite
来源：http://les.52xcode.cn

[U119] JS：生产构建
来源：http://ufk.zhiwuduotai.top

npx vite build
来源：http://sca.yj202588.top

[U120] JS：读取环境变量（Vite）
来源：http://cgx.fanxiaobao.xyz

import.meta.env.VITE_API_URL
来源：http://hcm.yuxming.cn

================================================================================
来源：http://aii.fktsv.cn

统计汇总
来源：http://mup.fehbvm.com

================================================================================
来源：http://ewp.jqgfzy.top

按语言统计（条）：
来源：http://ycd.pycfn.com

Python ......... 252
来源：http://djo.yvedp.cn

PHP ............ 252
来源：http://xyv.svipenyu.cn

JavaScript ..... 252
来源：http://zbc.hesvh.cn

TypeScript ..... 212
来源：http://vgs.yueranfly.top

Java ........... 212
来源：http://tiq.zhaomingkeji.xyz

Go ............. 212
来源：http://gmu.9152youxi.cn

Ruby ........... 212
来源：http://xnd.tarul.cn

C# ............. 212
来源：http://ezd.jinghuilouyu.cn

C .............. 30
来源：http://yct.zdbjq.cn

C++ ............ 30
来源：http://ulr.quarkkingdee.top

SQL ............ 90
来源：http://szw.ydjk.org.cn

Bash ........... 80
来源：http://szu.gogol.net.cn

Kotlin ......... 15
来源：http://rtl.fanxiaobao.xyz

Swift .......... 15
来源：http://fuy.yueranfly.top

Lua ............ 10
来源：http://tfu.gaohongyu789.top

Perl ........... 10
来源：http://zan.tian-w.cn

Scala .......... 10
来源：http://dcr.bjfxy.top

------------------------------------
来源：http://rfm.fktsv.cn

合计 ........... 2106 条
来源：http://pmi.316326.xyz

按章节统计：
来源：http://lsp.yj20258.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fat.jqgfzy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xfb.sweek.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dib.ybcxt.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://izf.zdbjq.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ebw.fktsv.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ofn.jinyuanbaomall.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://yhl.fzhhl.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yxm.daxiang520.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yca.gzhubu.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ngz.yuxming.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xqe.shanyushiyangkeji.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wfv.hammf.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ktx.yj20258.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hbv.tianlin.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mdb.vehdjk.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gae.svipenyu.cn

Q SQL 专题                              90
来源：http://cyp.tanke756.top

R Bash 专题                             80
来源：http://esb.haohaochexian.top

S C / C++ 专题                          60
来源：http://obg.zhijiandao.cn

T 其他语言补充                          60
来源：http://hsl.tian-w.cn

U 高频实用片段                         120
来源：http://uvo.nanxinkj.top

------------------------------------
来源：http://eey.hfpthk.cn

合计                                  2106 条
来源：http://mzn.hfpthk.cn

--------------------------------------------------------------------------------
来源：http://spz.ehwqpu.com

使用提醒
来源：http://oev.daxiang520.top

--------------------------------------------------------------------------------
来源：http://ebh.dianchejie.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vuk.ehwqpu.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://oea.hnqzz.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://uvp.zhaomingkeji.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://uot.jiagoushi.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://eqg.chenjidiqi.icu

—— 文件结束 ——
来源：http://ohw.dianchejie.cn

================================================================================
来源：http://tfc.yuxming.cn

程序语言常见例子速查手册（2024 版）
来源：http://gfx.yfazqb.com

Common Programming Examples Cheat Book
来源：http://clx.cashguo.top

================================================================================
来源：http://imk.zhiwuduotai.top

【收录内容】
来源：http://ply.ywan-chungtsiang.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://nhq.jianghu66.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nah.redwolf501.top

SQL · Bash · C · C++
来源：http://jlu.shuidangran.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://myf.aizwys.cn

【使用说明】
来源：http://tqi.yuxming.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gfg.yj202588.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ome.jqgfzy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ypl.yfazqb.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://pgf.yonumen.top

Bash:  Shell         C:     C             C++:   C++
来源：http://uhc.yongpay.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ttq.ywan-chungtsiang.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://abw.jinyuanbaomall.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jla.zhaomingkeji.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yno.hfpthk.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hpd.fzhhl.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://azf.haohaochexian.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xgj.c1oappe.top

【文件统计】
来源：http://eiq.gaohongyu789.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hau.chenzaomai.com

--------------------------------------------------------------------------------
来源：http://unl.yanxiufei.cn

目  录
来源：http://nwj.iojbl.cn

--------------------------------------------------------------------------------
来源：http://vej.jinyuanbaomall.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ibn.yj20258.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ztu.guowangkeji.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nrs.sufxvd.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yth.daria6918.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ulk.yongpay.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://nac.ehwqpu.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zcu.yongpay.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://atl.bjfxy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ibf.daxiang520.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dvj.vehdjk.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fkb.gotoacloud.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mec.hnqzz.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lob.kuanghao11.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pdk.cashguo.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ehn.yonumen.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wtt.yfazqb.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kro.jinqigfzy.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://lyb.xuetiantiany.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vtd.c1oappe.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ucy.fehbvm.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jgx.hfpthk.cn

================================================================================
来源：http://typ.sufxvd.cn

A. 基础语法与类型
来源：http://dmn.nanxinkj.top

================================================================================
来源：http://rtg.shanyushiyangkeji.top

[A01] Hello World
来源：http://xvv.hesvh.cn

Py:   print("Hello, World!")
来源：http://jrw.nwbrower.top

PHP:  echo "Hello, World!";
来源：http://iuy.gogol.net.cn

JS:   console.log("Hello, World!");
来源：http://mnj.quarkkingdee.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lvq.fzhhl.top

Java: System.out.println("Hello, World!");
来源：http://qtx.zhoulong.xyz

Go:   fmt.Println("Hello, World!")
来源：http://hei.zhijiandao.cn

Ruby: puts "Hello, World!"
来源：http://tbm.ppjwa.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://znl.shuidangran.top

[A02] 变量声明与赋值
来源：http://agi.havefunace.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rdz.52xcode.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://gjz.snrcjt.cn

JS:   let name = "Alex"; const age = 20;
来源：http://bbk.xingfuxueyuan.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rtw.hywenlv.cn

Java: String name = "Alex"; int age = 20;
来源：http://xxi.bbcook.cn

Go:   name := "Alex"; age := 20
来源：http://qsw.sysykeji.top

Ruby: name = "Alex"; age = 20
来源：http://ntl.ctjpmb.com

C#:   string name = "Alex"; int age = 20;
来源：http://qsg.fehbvm.com

[A03] 常量定义
来源：http://jlz.zhaomingkeji.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qoo.pengpengdd.cyou

PHP:  const PI = 3.14159;
来源：http://vbz.andypj.xyz

JS:   const PI = 3.14159;
来源：http://fbl.jinghuilouyu.cn

TS:   const PI: number = 3.14159;
来源：http://qra.smart0.xyz

Java: static final double PI = 3.14159;
来源：http://ewj.zhaomingkeji.xyz

Go:   const PI = 3.14159
来源：http://odr.jiagoushi.top

Ruby: PI = 3.14159
来源：http://xeq.tian-w.cn

C#:   const double PI = 3.14159;
来源：http://wyc.gogol.net.cn

[A04] 判断变量类型
来源：http://rdr.c1oappe.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://esf.c1oappe.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://cnj.aizwys.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://uxf.hnqzz.top

TS:   typeof x; x instanceof Date
来源：http://dcq.shangyingyoupin.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mqd.ydzc1.top

Go:   reflect.TypeOf(x).Name()
来源：http://nal.zhongyouzk.top

Ruby: x.class; x.is_a?(Integer)
来源：http://qcj.jianghu66.top

C#:   x.GetType().Name; x is int
来源：http://rpp.zhijiandao.cn

[A05] 整数除法与取模
来源：http://xsi.hnxiangtu.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fvt.ydzc1.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://nnd.yuanzhike.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lfo.hesvh.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fvh.dianchejie.cn

Java: 7 / 2; 7 % 2
来源：http://hcf.svipenyu.cn

Go:   7 / 2; 7 % 2
来源：http://bzh.svipenyu.cn

Ruby: 7 / 2; 7 % 2
来源：http://jcv.dianchejie.cn

C#:   7 / 2; 7 % 2
来源：http://fqw.uphjek.com

[A06] 字符串转数字
来源：http://kfu.52xcode.cn

Py:   int("42"); float("3.14")
来源：http://gmz.sysykeji.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://exg.c1oappe.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://way.vqdsnc.cn

TS:   parseInt("42", 10); Number("42")
来源：http://cvb.hongshengwenyu.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qll.zhongyouzk.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yqe.zhaomingkeji.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://zgd.ppjwa.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gwh.dashuyun.cn

[A07] 数字转字符串
来源：http://eli.wangshuangyany.cn

Py:   str(42)
来源：http://uah.jiagoushi.top

PHP:  (string) 42; strval(42)
来源：http://eny.ybcxt.top

JS:   String(42); (42).toString()
来源：http://nor.jqgufenzy.top

TS:   String(42)
来源：http://zct.9152youxi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://qer.hammf.cn

Go:   strconv.Itoa(42)
来源：http://suj.jqgufenzy.top

Ruby: 42.to_s
来源：http://srx.9152youxi.cn

C#:   42.ToString()
来源：http://fmj.ydjk.org.cn

[A08] 取整与四舍五入
来源：http://rpf.zhaomingkeji.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rld.cheryme.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wti.redwolf501.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ool.shangyingyoupin.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gne.bjfxy.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xje.sysykeji.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hlb.bbcook.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://jco.quarkkingdee.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vsa.daria6918.cn

[A09] 绝对值与最大最小值
来源：http://urd.hongshengwenyu.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ppy.pengpengdd.cyou

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://fmq.zhiwuduotai.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zen.xuetiantiany.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://rit.yj20258888.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wsz.hywenlv.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xbu.haohaochexian.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://tjt.wangdashe.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gqx.fanxiaobao.xyz

[A10] 生成随机数
来源：http://nyy.quarkkingdee.top

Py:   import random; random.randint(1, 100)
来源：http://vus.ydzc1.top

PHP:  random_int(1, 100);
来源：http://ylo.mhx1999.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://isc.zdqjudy.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zjo.sweek.top

Java: new Random().nextInt(100) + 1
来源：http://uet.ydjk.org.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wht.haohaochexian.top

Ruby: rand(1..100)
来源：http://yuz.cdnleiting.top

C#:   new Random().Next(1, 101)
来源：http://owm.uphjek.com

[A11] 条件表达式（三元）
来源：http://yxp.jinyuanbaomall.cn

Py:   "yes" if x > 0 else "no"
来源：http://ijk.yfazqb.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://yed.yonumen.top

JS:   x > 0 ? "yes" : "no"
来源：http://qjg.shanyushiyangkeji.top

TS:   x > 0 ? "yes" : "no"
来源：http://fvo.aizwys.cn

Java: x > 0 ? "yes" : "no"
来源：http://ocu.zdqjudy.top

Go:   // 无三元运算符，需用 if 语句
来源：http://etg.yuanzhike.top


<!-- 参考信息 -->