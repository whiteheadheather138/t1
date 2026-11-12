代发 wailian999

[U71] PHP：抛出异常
来源：http://egz.ivvv.top

throw new RuntimeException("失败", 500);
来源：http://vyn.shzxlz.cn

[U72] PHP：写错误日志
来源：http://dlf.fktsv.cn

error_log("失败: " . $e->getMessage());
来源：http://xgn.hnxiangtu.top

[U73] PHP：读取 ini 配置
来源：http://vjh.nanxuanxn.top

parse_ini_file("config.ini", true)
来源：http://gte.zhaomingkeji.xyz

[U74] PHP：读取环境变量
来源：http://qdf.birdmap.top

getenv("APP_ENV") ?: "production"
来源：http://syp.9152youxi.cn

[U75] PHP：依赖注入
来源：http://wwu.bjfxy.top

composer require psr/container
来源：http://vxq.zhiwuduotai.top

[U76] PHP：简单路由
来源：http://iuq.sjlbkw.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hvf.yuanzhike.top

[U77] PHP：模板渲染
来源：http://mdz.zhaomingkeji.xyz

composer require twig/twig
来源：http://xhr.tianlin.xyz

[U78] PHP：单元测试
来源：http://tsb.hfpthk.cn

composer require --dev phpunit/phpunit
来源：http://zre.fktsv.cn

[U79] PHP：静态分析
来源：http://ytf.vehdjk.com

composer require --dev phpstan/phpstan
来源：http://qsg.ivvv.top

[U80] PHP：代码规范修复
来源：http://eqb.meibo888.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://kxu.fengsongda.top

[U81] JS：初始化项目
来源：http://itp.sjlbkw.cn

npm init -y;  npm i express
来源：http://vbk.cqqwz.cn

[U82] JS：package.json 脚本
来源：http://skh.yangfankeji.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pgf.hysaishi.cn

[U83] JS：ES Module 导入导出
来源：http://wrf.jqgufenzy.top

export const a = 1;  import { a } from "./m.js";
来源：http://rwz.52xcode.cn

[U84] JS：CommonJS 写法
来源：http://wdx.hfpthk.cn

module.exports = { a };  const { a } = require("./m");
来源：http://swb.zhiwuduotai.top

[U85] JS：可选链
来源：http://qyd.shuidangran.top

a?.b?.c
来源：http://ggi.yj20258.top

[U86] JS：空值合并
来源：http://vkr.xziqi.cn

a ?? b
来源：http://qyo.ydzc1.top

[U87] JS：解构默认值
来源：http://srq.cashguo.top

const { a = 1, b = 2 } = obj;
来源：http://slu.quarkkingdee.top

[U88] JS：对象展开合并
来源：http://art.yuxming.cn

{ ...a, ...b }
来源：http://ztg.quarkkingdee.top

[U89] JS：数组去重
来源：http://hat.zhixingplan.top

[...new Set(arr)]
来源：http://kgs.shuidangran.top

[U90] JS：数字数组排序
来源：http://jsx.yangfankeji.com

[...arr].sort((a, b) => a - b)
来源：http://cmi.shangyingyoupin.top

[U91] JS：对象键值遍历
来源：http://olh.tarul.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dnf.jiagoushi.top

[U92] JS：深拷贝
来源：http://ddp.ydjk.org.cn

structuredClone(obj)
来源：http://sbo.wangshuangyany.cn

[U93] JS：模板字符串
来源：http://vjq.hesvh.cn

`共 ${n} 条`
来源：http://lgw.feifeiyinyue.top

[U94] JS：箭头函数
来源：http://rqd.chenzaomai.com

const double = x => x * 2;
来源：http://kif.ehwqpu.com

[U95] JS：Promise 包装
来源：http://hwn.zhaomingkeji.xyz

new Promise((resolve, reject) => {})
来源：http://rrv.xziqi.cn

[U96] JS：async/await 与异常
来源：http://dot.shzxlz.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vwe.hnqzz.top

[U97] JS：并发请求
来源：http://agn.hcnkem.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://ocr.feifeiyinyue.top

[U98] JS：fetch 带 JSON
来源：http://qye.hnqzz.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ids.zhaomingkeji.xyz

[U99] JS：事件监听
来源：http://baj.ivvv.top

el.addEventListener("click", e => {})
来源：http://vkh.nanxuanxn.top

[U100] JS：DOM 查询
来源：http://zgo.yj20258.top

document.querySelector(".item")
来源：http://whe.hammf.cn

[U101] JS：classList 操作
来源：http://ygy.daxiang520.top

el.classList.toggle("active")
来源：http://ake.xuetiantiany.cn

[U102] JS：本地存储
来源：http://gkd.gogol.net.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jwm.guowangkeji.top

[U103] JS：定时器
来源：http://uxg.jlsjyb.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xjz.gzhubu.top

[U104] JS：防抖
来源：http://tkb.tian-w.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xni.ivvv.top

[U105] JS：节流
来源：http://tul.0kj1m.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yjb.pengpengdd.cyou

[U106] JS：日期格式化
来源：http://rtm.pengpengdd.cyou

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fxg.shuidangran.top

[U107] JS：数字千分位
来源：http://qcw.hesvh.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yvj.cucudq.cn

[U108] JS：随机整数
来源：http://jtn.pengpengdd.cyou

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://oqk.zdbjq.cn

[U109] JS：数组分组
来源：http://kmk.ctjpmb.com

Object.groupBy(arr, x => x.type)
来源：http://efm.nanxuanxn.top

[U110] JS：数组分块
来源：http://bjl.cqqwz.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ckl.aizwys.cn

[U111] JS：对象转 Map
来源：http://rop.yfazqb.com

new Map(Object.entries(obj))
来源：http://sjk.ybcxt.top

[U112] JS：字符串补位
来源：http://uur.jlsjyb.cn

"7".padStart(3, "0")
来源：http://uui.yangfankeji.com

[U113] JS：正则替换全部
来源：http://zlr.zycfv.cn

s.replaceAll("a", "b")
来源：http://pja.sjlbkw.cn

[U114] JS：JSON 深比较
来源：http://lcb.zhiwuduotai.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://cna.aizwys.cn

[U115] JS：生成 UUID
来源：http://dmx.hfpthk.cn

crypto.randomUUID()
来源：http://qxa.gogol.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://htn.yj202588.top

/** @param {string} name */ function f(name) {}
来源：http://czz.zhaomingkeji.xyz

[U117] JS：单元测试
来源：http://xav.xinyue.icu

npm i -D vitest;  npx vitest
来源：http://ren.daria6918.cn

[U118] JS：开发服务器
来源：http://dzx.hnqzz.top

npm i -D vite;  npx vite
来源：http://ozf.chenzaomai.com

[U119] JS：生产构建
来源：http://fio.xuetiantiany.cn

npx vite build
来源：http://tkv.ppjwa.cn

[U120] JS：读取环境变量（Vite）
来源：http://sfy.shanyushiyangtech.top

import.meta.env.VITE_API_URL
来源：http://tle.yanxiufei.cn

================================================================================
来源：http://uel.zhongyouzk.top

统计汇总
来源：http://goq.tanke756.top

================================================================================
来源：http://swg.sufxvd.cn

按语言统计（条）：
来源：http://fsy.wangshuangyany.cn

Python ......... 252
来源：http://wzk.pengpengdd.cyou

PHP ............ 252
来源：http://bxi.chenzaomai.com

JavaScript ..... 252
来源：http://ixo.ehwqpu.com

TypeScript ..... 212
来源：http://day.zycfv.cn

Java ........... 212
来源：http://bye.xuanzx.com

Go ............. 212
来源：http://mhs.uphjek.com

Ruby ........... 212
来源：http://bos.sufxvd.cn

C# ............. 212
来源：http://yin.havefunace.top

C .............. 30
来源：http://nff.hnqzz.top

C++ ............ 30
来源：http://gcv.epnwcf.com

SQL ............ 90
来源：http://jvl.svipenyu.cn

Bash ........... 80
来源：http://cin.0kj1m.cn

Kotlin ......... 15
来源：http://jvo.iojbl.cn

Swift .......... 15
来源：http://fys.zhijiandao.cn

Lua ............ 10
来源：http://drv.iojbl.cn

Perl ........... 10
来源：http://lkr.jqgfzy.top

Scala .......... 10
来源：http://snx.ehwqpu.com

------------------------------------
来源：http://uji.chenlongwang.top

合计 ........... 2106 条
来源：http://alp.ydzc1.top

按章节统计：
来源：http://mdg.iojbl.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fon.chenjidiqi.icu

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wxq.jlsjyb.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wqb.shuidangran.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wmi.yuxming.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qov.fehbvm.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ltj.yueranfly.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vzx.cheryme.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zoz.yj202588.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fke.fengsongda.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lcx.ctjpmb.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ten.gaohongyu789.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://elr.chenzaomai.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nnt.zhijiandao.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://uaa.daxiang520.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qlp.fengsongda.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jqk.52xcode.cn

Q SQL 专题                              90
来源：http://rwz.jinqigfzy.top

R Bash 专题                             80
来源：http://hky.uphjek.com

S C / C++ 专题                          60
来源：http://frn.ybcxt.top

T 其他语言补充                          60
来源：http://eoc.tian-w.cn

U 高频实用片段                         120
来源：http://ozr.vehdjk.com

------------------------------------
来源：http://ehl.wangdashe.top

合计                                  2106 条
来源：http://xkd.zdqjudy.top

--------------------------------------------------------------------------------
来源：http://ebh.sjlbkw.cn

使用提醒
来源：http://mmk.hfpthk.cn

--------------------------------------------------------------------------------
来源：http://axw.hywenlv.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ueu.zhijiandao.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rgj.fzhhl.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hlg.chenlongwang.top

在旧版本上使用前请先确认语法支持情况。
来源：http://sht.gogol.net.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pqp.guowangkeji.top

—— 文件结束 ——
来源：http://tlz.hesvh.cn

================================================================================
来源：http://pfj.ppjwa.cn

程序语言常见例子速查手册（2024 版）
来源：http://bbg.xuetiantiany.cn

Common Programming Examples Cheat Book
来源：http://pzy.nanxinkj.top

================================================================================
来源：http://ngj.cucudq.cn

【收录内容】
来源：http://gbe.zhoulong.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://qla.yanxiufei.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tsp.pycfn.com

SQL · Bash · C · C++
来源：http://bwv.uphjek.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mkd.cheryme.top

【使用说明】
来源：http://edm.yuanzhike.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mhz.vqdsnc.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qey.yj20258888.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jkm.tian-w.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zsx.uphjek.com

Bash:  Shell         C:     C             C++:   C++
来源：http://sgy.yuanzhike.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://taj.zhijiandao.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bfh.ybcxt.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://axf.fehbvm.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://prv.yuanzhike.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://clb.jiagoushi.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vsa.yj202588.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mee.gaohongyu789.top

【文件统计】
来源：http://lpx.wangshuangyany.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xdv.vehdjk.com

--------------------------------------------------------------------------------
来源：http://lfa.wangdashe.top

目  录
来源：http://eug.sweek.top

--------------------------------------------------------------------------------
来源：http://dpb.quarkkingdee.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fic.hesvh.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ayq.nanxinkj.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://smb.andypj.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://nbd.hnqzz.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nhp.nwbrower.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://yhs.ywan-chungtsiang.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rbr.zhijiandao.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ipl.jinqigufen.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hhq.sufxvd.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wgc.jinghuilouyu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://avc.gotoacloud.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://psw.hcnkem.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dux.yonumen.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bma.0kj1m.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qut.xylfe.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qvf.yangfankeji.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sjs.haohaochexian.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://aqh.cashguo.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://iab.yanxiufei.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ztw.meibo888.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xuq.ppjwa.cn

================================================================================
来源：http://weg.cucudq.cn

A. 基础语法与类型
来源：http://tjg.hnqzz.top

================================================================================
来源：http://jbj.smart0.xyz

[A01] Hello World
来源：http://zuk.bjfxy.top

Py:   print("Hello, World!")
来源：http://cvh.nanxinkj.top

PHP:  echo "Hello, World!";
来源：http://vsh.tanke756.top

JS:   console.log("Hello, World!");
来源：http://yac.chenlongwang.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://uxl.fzhhl.top

Java: System.out.println("Hello, World!");
来源：http://arz.pengpengdd.cyou

Go:   fmt.Println("Hello, World!")
来源：http://tdp.yonumen.top

Ruby: puts "Hello, World!"
来源：http://prc.yueranfly.top

C#:   Console.WriteLine("Hello, World!");
来源：http://tdn.quarkkingdee.top

[A02] 变量声明与赋值
来源：http://rxv.xziqi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gwk.yj202588.top

PHP:  $name = "Alex"; $age = 20;
来源：http://oxz.ywan-chungtsiang.top

JS:   let name = "Alex"; const age = 20;
来源：http://kdy.cqqwz.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kef.zhiwuduotai.top

Java: String name = "Alex"; int age = 20;
来源：http://cug.ctjpmb.com

Go:   name := "Alex"; age := 20
来源：http://and.xinyue.icu

Ruby: name = "Alex"; age = 20
来源：http://crt.zdbjq.cn

C#:   string name = "Alex"; int age = 20;
来源：http://asd.zhongyouzk.top

[A03] 常量定义
来源：http://jfy.yj202588.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://twd.ydjk.org.cn

PHP:  const PI = 3.14159;
来源：http://wts.redwolf501.top

JS:   const PI = 3.14159;
来源：http://acj.guannengcc.top

TS:   const PI: number = 3.14159;
来源：http://wlt.snrcjt.cn

Java: static final double PI = 3.14159;
来源：http://twb.yueranfly.top

Go:   const PI = 3.14159
来源：http://vuz.bbcook.cn

Ruby: PI = 3.14159
来源：http://mvm.tianlin.xyz

C#:   const double PI = 3.14159;
来源：http://izz.yj202588.top

[A04] 判断变量类型
来源：http://toj.zhengqikj.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://tcp.yj20258.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://aei.jyoumei.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nbv.zdqjudy.top

TS:   typeof x; x instanceof Date
来源：http://lgs.jinqigfzy.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dkh.svipenyu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://nuz.tanke756.top

Ruby: x.class; x.is_a?(Integer)
来源：http://mph.yj202588.top

C#:   x.GetType().Name; x is int
来源：http://moz.hysaishi.cn

[A05] 整数除法与取模
来源：http://rfv.yj20258.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rck.nanxinkj.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ozu.yanxiufei.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jdw.c1oappe.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yko.gogol.net.cn

Java: 7 / 2; 7 % 2
来源：http://nsr.wangshuangyany.cn

Go:   7 / 2; 7 % 2
来源：http://lrh.tianlin.xyz

Ruby: 7 / 2; 7 % 2
来源：http://niv.ivvv.top

C#:   7 / 2; 7 % 2
来源：http://mec.guannengcc.top

[A06] 字符串转数字
来源：http://rui.tarul.cn

Py:   int("42"); float("3.14")
来源：http://dkp.hammf.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://uuc.kuanghao11.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://oxz.bbcook.cn

TS:   parseInt("42", 10); Number("42")
来源：http://qeb.pengpengdd.cyou

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tpr.quarkkingdee.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xvw.hnxiangtu.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ztt.yfazqb.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://lpi.nanxuanxn.top

[A07] 数字转字符串
来源：http://sdb.gzhubu.top

Py:   str(42)
来源：http://eiw.yueranfly.top

PHP:  (string) 42; strval(42)
来源：http://jmu.hnxiangtu.top

JS:   String(42); (42).toString()
来源：http://kyg.zhixingplan.top

TS:   String(42)
来源：http://hyd.sweek.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://lze.birdmap.top

Go:   strconv.Itoa(42)
来源：http://cws.ivvv.top

Ruby: 42.to_s
来源：http://dga.andypj.xyz

C#:   42.ToString()
来源：http://xzc.yongpay.top

[A08] 取整与四舍五入
来源：http://zod.sjlbkw.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://tis.hammf.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lez.yongpay.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wea.52xcode.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ion.meibo888.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wlg.redwolf501.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://amk.jinghuilouyu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://qio.uphjek.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hne.uphjek.com

[A09] 绝对值与最大最小值
来源：http://uxr.guannengcc.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hbf.jyoumei.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hpw.0kj1m.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://csi.pycfn.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://dsw.yvedp.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dop.nwbrower.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://yix.dianchejie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://uwi.zhengqikj.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qzv.pengpengdd.cyou

[A10] 生成随机数
来源：http://hee.pengpengdd.cyou

Py:   import random; random.randint(1, 100)
来源：http://itk.yfazqb.com

PHP:  random_int(1, 100);
来源：http://ner.fengsongda.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mda.tanke756.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rir.nanxuanxn.top

Java: new Random().nextInt(100) + 1
来源：http://xzm.zycfv.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fai.chenjidiqi.icu

Ruby: rand(1..100)
来源：http://ack.ivvv.top

C#:   new Random().Next(1, 101)
来源：http://yfy.svipenyu.cn

[A11] 条件表达式（三元）
来源：http://hin.hammf.cn

Py:   "yes" if x > 0 else "no"
来源：http://zxi.nanxuanxn.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://jdi.yj202588.top


<!-- 参考信息 -->