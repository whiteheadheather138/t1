代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://fpa.redwolf501.top

parse_ini_file("config.ini", true)
来源：http://qlh.chenjidiqi.icu

[U74] PHP：读取环境变量
来源：http://oha.shanyushiyangkeji.top

getenv("APP_ENV") ?: "production"
来源：http://rzv.hywenlv.cn

[U75] PHP：依赖注入
来源：http://nhc.snrcjt.cn

composer require psr/container
来源：http://aqn.sufxvd.cn

[U76] PHP：简单路由
来源：http://ivc.hfpthk.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hry.yonumen.top

[U77] PHP：模板渲染
来源：http://nhq.hesvh.cn

composer require twig/twig
来源：http://riv.yanxiufei.cn

[U78] PHP：单元测试
来源：http://yda.meibo888.top

composer require --dev phpunit/phpunit
来源：http://ftb.yuxming.cn

[U79] PHP：静态分析
来源：http://ryn.cheryme.top

composer require --dev phpstan/phpstan
来源：http://ecf.jinghuilouyu.cn

[U80] PHP：代码规范修复
来源：http://wla.tianlin.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://cok.jyoumei.cn

[U81] JS：初始化项目
来源：http://fhr.jinqigfzy.top

npm init -y;  npm i express
来源：http://msh.sufxvd.cn

[U82] JS：package.json 脚本
来源：http://wts.shzxlz.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ntl.fktsv.cn

[U83] JS：ES Module 导入导出
来源：http://mln.zhijiandao.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ikp.dianchejie.cn

[U84] JS：CommonJS 写法
来源：http://jzl.snrcjt.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ulj.cdnleiting.top

[U85] JS：可选链
来源：http://gru.mhx1999.top

a?.b?.c
来源：http://hug.zhaomingkeji.xyz

[U86] JS：空值合并
来源：http://cfu.guowangkeji.top

a ?? b
来源：http://skn.cashguo.top

[U87] JS：解构默认值
来源：http://dge.aibaodan.cn

const { a = 1, b = 2 } = obj;
来源：http://woj.fktsv.cn

[U88] JS：对象展开合并
来源：http://qid.jiagoushi.top

{ ...a, ...b }
来源：http://zfx.cheryme.top

[U89] JS：数组去重
来源：http://bct.jinqigufen.top

[...new Set(arr)]
来源：http://cfj.zhoulong.xyz

[U90] JS：数字数组排序
来源：http://ott.quarkkingdee.top

[...arr].sort((a, b) => a - b)
来源：http://sfm.jqgufenzy.top

[U91] JS：对象键值遍历
来源：http://vhc.fktsv.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mqr.ehwqpu.com

[U92] JS：深拷贝
来源：http://sun.jinyuanbaomall.cn

structuredClone(obj)
来源：http://adw.tanke756.top

[U93] JS：模板字符串
来源：http://xai.cdnleiting.top

`共 ${n} 条`
来源：http://kwr.fzhhl.top

[U94] JS：箭头函数
来源：http://epp.yvedp.cn

const double = x => x * 2;
来源：http://mbk.jqgfzy.top

[U95] JS：Promise 包装
来源：http://eql.chenlongwang.top

new Promise((resolve, reject) => {})
来源：http://tys.birdmap.top

[U96] JS：async/await 与异常
来源：http://uec.birdmap.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wlz.yangfankeji.com

[U97] JS：并发请求
来源：http://glq.shanyushiyangkeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://rel.epnwcf.com

[U98] JS：fetch 带 JSON
来源：http://ybq.pycfn.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ajc.aibaodan.cn

[U99] JS：事件监听
来源：http://bnz.daria6918.cn

el.addEventListener("click", e => {})
来源：http://hqc.xingfuxueyuan.xyz

[U100] JS：DOM 查询
来源：http://hov.9152youxi.cn

document.querySelector(".item")
来源：http://nhb.dashuyun.cn

[U101] JS：classList 操作
来源：http://kkc.zycfv.cn

el.classList.toggle("active")
来源：http://byu.yueranfly.top

[U102] JS：本地存储
来源：http://wwv.nanxuanxn.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://nnq.xylfe.cn

[U103] JS：定时器
来源：http://ldv.vehdjk.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bzs.zhaomingkeji.xyz

[U104] JS：防抖
来源：http://ibf.daria6918.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cjt.zhengqikj.top

[U105] JS：节流
来源：http://egh.yuxming.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://awn.meibo888.top

[U106] JS：日期格式化
来源：http://vul.jyoumei.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://eoi.cashguo.top

[U107] JS：数字千分位
来源：http://ofz.xuetiantiany.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://idm.daria6918.cn

[U108] JS：随机整数
来源：http://tpy.jqgufenzy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jnw.dianchejie.cn

[U109] JS：数组分组
来源：http://ifg.316326.xyz

Object.groupBy(arr, x => x.type)
来源：http://xtv.iojbl.cn

[U110] JS：数组分块
来源：http://qpx.haohaochexian.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://idx.kuanghao11.cn

[U111] JS：对象转 Map
来源：http://pzs.hysaishi.cn

new Map(Object.entries(obj))
来源：http://hbr.ppjwa.cn

[U112] JS：字符串补位
来源：http://vmq.cheryme.top

"7".padStart(3, "0")
来源：http://uff.xuanzx.com

[U113] JS：正则替换全部
来源：http://kup.daria6918.cn

s.replaceAll("a", "b")
来源：http://llc.jinqigufen.top

[U114] JS：JSON 深比较
来源：http://qpp.shanyushiyangkeji.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://iga.nanxuanxn.top

[U115] JS：生成 UUID
来源：http://zax.mhx1999.top

crypto.randomUUID()
来源：http://ejz.nanxinkj.top

[U116] JS：类型检查（JSDoc）
来源：http://whf.tanke756.top

/** @param {string} name */ function f(name) {}
来源：http://fhi.bjfxy.top

[U117] JS：单元测试
来源：http://okx.mhx1999.top

npm i -D vitest;  npx vitest
来源：http://gfy.haohaochexian.top

[U118] JS：开发服务器
来源：http://afx.pycfn.com

npm i -D vite;  npx vite
来源：http://ydf.aizwys.cn

[U119] JS：生产构建
来源：http://jhi.yvedp.cn

npx vite build
来源：http://kev.zhixingplan.top

[U120] JS：读取环境变量（Vite）
来源：http://oaa.meibo888.top

import.meta.env.VITE_API_URL
来源：http://ztf.yanxiufei.cn

================================================================================
来源：http://irs.hnxiangtu.top

统计汇总
来源：http://qaj.shangyingyoupin.top

================================================================================
来源：http://arl.xziqi.cn

按语言统计（条）：
来源：http://klo.hnqzz.top

Python ......... 252
来源：http://lia.zdbjq.cn

PHP ............ 252
来源：http://xwe.ivvv.top

JavaScript ..... 252
来源：http://flg.yongpay.top

TypeScript ..... 212
来源：http://fbx.jqgfzy.top

Java ........... 212
来源：http://fai.redwolf501.top

Go ............. 212
来源：http://pte.gzhubu.top

Ruby ........... 212
来源：http://jpn.shanyushiyangtech.top

C# ............. 212
来源：http://xcb.jinyuanbaomall.cn

C .............. 30
来源：http://xle.yuxming.cn

C++ ............ 30
来源：http://szg.yangfankeji.com

SQL ............ 90
来源：http://qyo.shuidangran.top

Bash ........... 80
来源：http://cwz.shuidangran.top

Kotlin ......... 15
来源：http://orf.haohaochexian.top

Swift .......... 15
来源：http://gpv.nanxinkj.top

Lua ............ 10
来源：http://tgw.uphjek.com

Perl ........... 10
来源：http://qfq.gogol.net.cn

Scala .......... 10
来源：http://jii.zhoulong.xyz

------------------------------------
来源：http://hoh.redwolf501.top

合计 ........... 2106 条
来源：http://fue.hywenlv.cn

按章节统计：
来源：http://gxj.ydjk.org.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zqd.yanxiufei.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ojo.vehdjk.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nte.zhengqikj.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ojd.aibaodan.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://afq.hfpthk.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ypy.jqgufenzy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pxn.xuanzx.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tdj.zhengqikj.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lmn.andypj.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://aok.yueranfly.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vqm.52xcode.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ktd.aibaodan.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yun.yuanzhike.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://otk.zhongyouzk.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tay.jqgufenzy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://seb.chenzaomai.com

Q SQL 专题                              90
来源：http://lte.gogol.net.cn

R Bash 专题                             80
来源：http://yup.shzxlz.cn

S C / C++ 专题                          60
来源：http://kga.shanyushiyangtech.top

T 其他语言补充                          60
来源：http://tsr.havefunace.top

U 高频实用片段                         120
来源：http://lct.pengpengdd.cyou

------------------------------------
来源：http://zvl.zhaomingkeji.xyz

合计                                  2106 条
来源：http://sfm.yuxming.cn

--------------------------------------------------------------------------------
来源：http://ogd.zhongyouzk.top

使用提醒
来源：http://cuc.gotoacloud.top

--------------------------------------------------------------------------------
来源：http://krs.yanxiufei.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mcw.cdnleiting.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cnm.sxryk.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://muq.fzhhl.top

在旧版本上使用前请先确认语法支持情况。
来源：http://laj.daxiang520.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://aos.gzhubu.top

—— 文件结束 ——
来源：http://fna.yuanzhike.top

================================================================================
来源：http://tca.redwolf501.top

程序语言常见例子速查手册（2024 版）
来源：http://tie.ydjk.org.cn

Common Programming Examples Cheat Book
来源：http://muv.sjlbkw.cn

================================================================================
来源：http://ufg.9152youxi.cn

【收录内容】
来源：http://job.jqgufenzy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://yao.zhijiandao.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qqq.zdbjq.cn

SQL · Bash · C · C++
来源：http://gov.hysaishi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wds.zhengqikj.top

【使用说明】
来源：http://vtf.hongshengwenyu.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hxe.gaohongyu789.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nqk.yuanzhike.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mtx.xziqi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xmp.gaohongyu789.top

Bash:  Shell         C:     C             C++:   C++
来源：http://jzi.havefunace.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://yyd.svipenyu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kpr.snrcjt.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://auy.kuanghao11.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xjq.hywenlv.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://llt.hnxiangtu.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kps.gogol.net.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ogs.nanxuanxn.top

【文件统计】
来源：http://vxq.yuxming.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yiu.ehwqpu.com

--------------------------------------------------------------------------------
来源：http://one.zhijiandao.cn

目  录
来源：http://fjg.ybcxt.top

--------------------------------------------------------------------------------
来源：http://yjk.tianlin.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kfo.yuanzhike.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://emm.aizwys.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ezu.zhaomingkeji.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tbv.zhengqikj.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zdk.zhoulong.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://byu.guowangkeji.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://tts.hesvh.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zkg.shanyushiyangtech.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mdc.52xcode.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dma.fengsongda.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vnx.yj202588.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xin.jqgfzy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://bdh.yanxiufei.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fyy.guowangkeji.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ftc.hnqzz.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mqr.andypj.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ehp.chenjidiqi.icu

R. Bash 专题                   （第 18 节，80 条）
来源：http://rrt.hnxiangtu.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cne.mhx1999.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nut.uphjek.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ktz.zhongyouzk.top

================================================================================
来源：http://cnj.meibo888.top

A. 基础语法与类型
来源：http://inp.smart0.xyz

================================================================================
来源：http://nfl.tarul.cn

[A01] Hello World
来源：http://lko.redwolf501.top

Py:   print("Hello, World!")
来源：http://nfs.yfazqb.com

PHP:  echo "Hello, World!";
来源：http://fic.wangdashe.top

JS:   console.log("Hello, World!");
来源：http://kfg.haohaochexian.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://glr.jyoumei.cn

Java: System.out.println("Hello, World!");
来源：http://xum.nwbrower.top

Go:   fmt.Println("Hello, World!")
来源：http://bjz.9152youxi.cn

Ruby: puts "Hello, World!"
来源：http://gwz.fehbvm.com

C#:   Console.WriteLine("Hello, World!");
来源：http://bvt.jiagoushi.top

[A02] 变量声明与赋值
来源：http://awd.yueranfly.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zwz.zhengqikj.top

PHP:  $name = "Alex"; $age = 20;
来源：http://jte.ppjwa.cn

JS:   let name = "Alex"; const age = 20;
来源：http://lcd.ppjwa.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hmw.yueranfly.top

Java: String name = "Alex"; int age = 20;
来源：http://auu.hammf.cn

Go:   name := "Alex"; age := 20
来源：http://mqd.yueranfly.top

Ruby: name = "Alex"; age = 20
来源：http://diq.chenjidiqi.icu

C#:   string name = "Alex"; int age = 20;
来源：http://zmu.shzxlz.cn

[A03] 常量定义
来源：http://rnd.zhixingplan.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tiv.316326.xyz

PHP:  const PI = 3.14159;
来源：http://lzh.yonumen.top

JS:   const PI = 3.14159;
来源：http://koj.sweek.top

TS:   const PI: number = 3.14159;
来源：http://ehz.zdbjq.cn

Java: static final double PI = 3.14159;
来源：http://dyw.jyoumei.cn

Go:   const PI = 3.14159
来源：http://iyj.nwbrower.top

Ruby: PI = 3.14159
来源：http://dxa.ppjwa.cn

C#:   const double PI = 3.14159;
来源：http://lgi.vqdsnc.cn

[A04] 判断变量类型
来源：http://kwk.jqgfzy.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://dpu.cqqwz.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://agx.jqgfzy.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zjz.cheryme.top

TS:   typeof x; x instanceof Date
来源：http://uyn.gotoacloud.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jyh.shangyingyoupin.top

Go:   reflect.TypeOf(x).Name()
来源：http://dlb.yj202588.top

Ruby: x.class; x.is_a?(Integer)
来源：http://dbz.yongpay.top

C#:   x.GetType().Name; x is int
来源：http://jlr.cdnleiting.top

[A05] 整数除法与取模
来源：http://kij.dianchejie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qxp.xingfuxueyuan.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://wmw.sysykeji.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://adv.xylfe.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ach.yongpay.top

Java: 7 / 2; 7 % 2
来源：http://vve.xingfuxueyuan.xyz

Go:   7 / 2; 7 % 2
来源：http://dcx.tarul.cn

Ruby: 7 / 2; 7 % 2
来源：http://ojh.hywenlv.cn

C#:   7 / 2; 7 % 2
来源：http://xkq.0kj1m.cn

[A06] 字符串转数字
来源：http://buq.ivvv.top

Py:   int("42"); float("3.14")
来源：http://mzv.0kj1m.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jkx.yvedp.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://yzq.yongpay.top

TS:   parseInt("42", 10); Number("42")
来源：http://xhh.xuetiantiany.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hoh.yfazqb.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mqg.zycfv.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://znz.ivvv.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://nge.tarul.cn

[A07] 数字转字符串
来源：http://ous.yongpay.top

Py:   str(42)
来源：http://eyp.jinghuilouyu.cn

PHP:  (string) 42; strval(42)
来源：http://zet.iojbl.cn

JS:   String(42); (42).toString()
来源：http://ztg.shanyushiyangtech.top

TS:   String(42)
来源：http://sap.bjfxy.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://byy.zhaomingkeji.xyz

Go:   strconv.Itoa(42)
来源：http://yki.yuxming.cn

Ruby: 42.to_s
来源：http://orx.ydzc1.top

C#:   42.ToString()
来源：http://ogy.hcnkem.com

[A08] 取整与四舍五入
来源：http://dtv.cashguo.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pbs.zhongyouzk.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://moy.shuidangran.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bjv.hysaishi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://frl.andypj.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://boq.jiagoushi.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://uuu.xylfe.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://vow.fzhhl.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://krt.shanyushiyangtech.top

[A09] 绝对值与最大最小值
来源：http://jld.sysykeji.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ilg.zhijiandao.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tul.yuanzhike.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mzx.chenlongwang.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gbp.guannengcc.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://api.xingfuxueyuan.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wqf.tanke756.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bni.shangyingyoupin.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kyj.xziqi.cn

[A10] 生成随机数
来源：http://tnx.jinyuanbaomall.cn

Py:   import random; random.randint(1, 100)
来源：http://rpg.tian-w.cn

PHP:  random_int(1, 100);
来源：http://gom.tian-w.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zbr.fktsv.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tek.daxiang520.top

Java: new Random().nextInt(100) + 1
来源：http://yyb.smart0.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ynp.guannengcc.top

Ruby: rand(1..100)
来源：http://jpt.yj20258.top

C#:   new Random().Next(1, 101)
来源：http://lqn.yueranfly.top

[A11] 条件表达式（三元）
来源：http://tkq.zhongyouzk.top

Py:   "yes" if x > 0 else "no"
来源：http://kqz.sufxvd.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://xqe.yongpay.top

JS:   x > 0 ? "yes" : "no"
来源：http://fxv.yongpay.top

TS:   x > 0 ? "yes" : "no"
来源：http://gnk.dianchejie.cn

Java: x > 0 ? "yes" : "no"
来源：http://ktj.nanxinkj.top

Go:   // 无三元运算符，需用 if 语句
来源：http://pyk.yfazqb.com


<!-- 参考信息 -->