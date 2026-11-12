代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://vrc.ctjpmb.com

parse_ini_file("config.ini", true)
来源：http://cgj.xuetiantiany.cn

[U74] PHP：读取环境变量
来源：http://ngz.shangyingyoupin.top

getenv("APP_ENV") ?: "production"
来源：http://lbm.feifeiyinyue.top

[U75] PHP：依赖注入
来源：http://kod.316326.xyz

composer require psr/container
来源：http://luk.bjfxy.top

[U76] PHP：简单路由
来源：http://xxq.dianchejie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qbu.xinyue.icu

[U77] PHP：模板渲染
来源：http://mts.feifeiyinyue.top

composer require twig/twig
来源：http://err.yuxming.cn

[U78] PHP：单元测试
来源：http://def.pengpengdd.cyou

composer require --dev phpunit/phpunit
来源：http://lrl.zhongyouzk.top

[U79] PHP：静态分析
来源：http://kvp.iojbl.cn

composer require --dev phpstan/phpstan
来源：http://cdp.ivvv.top

[U80] PHP：代码规范修复
来源：http://lym.epnwcf.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://was.sxryk.cn

[U81] JS：初始化项目
来源：http://klp.nanxinkj.top

npm init -y;  npm i express
来源：http://fzb.fktsv.cn

[U82] JS：package.json 脚本
来源：http://jwg.feifeiyinyue.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jpm.wangdashe.top

[U83] JS：ES Module 导入导出
来源：http://xtl.ydjk.org.cn

export const a = 1;  import { a } from "./m.js";
来源：http://wpo.guannengcc.top

[U84] JS：CommonJS 写法
来源：http://kbl.fktsv.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fvo.tarul.cn

[U85] JS：可选链
来源：http://qkf.sjlbkw.cn

a?.b?.c
来源：http://mce.hfpthk.cn

[U86] JS：空值合并
来源：http://iau.tarul.cn

a ?? b
来源：http://gvk.sjlbkw.cn

[U87] JS：解构默认值
来源：http://qfy.yueranfly.top

const { a = 1, b = 2 } = obj;
来源：http://ham.ybcxt.top

[U88] JS：对象展开合并
来源：http://shz.smart0.xyz

{ ...a, ...b }
来源：http://zuk.jianghu66.top

[U89] JS：数组去重
来源：http://hwe.nwbrower.top

[...new Set(arr)]
来源：http://fjh.uphjek.com

[U90] JS：数字数组排序
来源：http://rdg.fengsongda.top

[...arr].sort((a, b) => a - b)
来源：http://sng.zhengqikj.top

[U91] JS：对象键值遍历
来源：http://mrx.haohaochexian.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lxx.chenzaomai.com

[U92] JS：深拷贝
来源：http://btu.ctjpmb.com

structuredClone(obj)
来源：http://lzh.epnwcf.com

[U93] JS：模板字符串
来源：http://sis.fktsv.cn

`共 ${n} 条`
来源：http://pkz.yj20258888.top

[U94] JS：箭头函数
来源：http://rmy.shuidangran.top

const double = x => x * 2;
来源：http://ruc.jinqigufen.top

[U95] JS：Promise 包装
来源：http://tra.jiagoushi.top

new Promise((resolve, reject) => {})
来源：http://hdm.jqgfzy.top

[U96] JS：async/await 与异常
来源：http://nou.jinqigfzy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hul.yuxming.cn

[U97] JS：并发请求
来源：http://lcg.316326.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://kno.fzhhl.top

[U98] JS：fetch 带 JSON
来源：http://his.shanyushiyangkeji.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bac.shanyushiyangtech.top

[U99] JS：事件监听
来源：http://jwc.svipenyu.cn

el.addEventListener("click", e => {})
来源：http://sud.aizwys.cn

[U100] JS：DOM 查询
来源：http://qzy.fzhhl.top

document.querySelector(".item")
来源：http://qbm.sysykeji.top

[U101] JS：classList 操作
来源：http://www.gzhubu.top

el.classList.toggle("active")
来源：http://vjn.9152youxi.cn

[U102] JS：本地存储
来源：http://fae.yonumen.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://jpl.jinyuanbaomall.cn

[U103] JS：定时器
来源：http://hrm.haohaochexian.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uao.cucudq.cn

[U104] JS：防抖
来源：http://ktv.bjfxy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qqs.andypj.xyz

[U105] JS：节流
来源：http://jvt.gaohongyu789.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gsj.hesvh.cn

[U106] JS：日期格式化
来源：http://sqs.jyoumei.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rcc.sufxvd.cn

[U107] JS：数字千分位
来源：http://bkt.316326.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gul.epnwcf.com

[U108] JS：随机整数
来源：http://srn.c1oappe.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://umm.gotoacloud.top

[U109] JS：数组分组
来源：http://eax.yj20258888.top

Object.groupBy(arr, x => x.type)
来源：http://yif.cqqwz.cn

[U110] JS：数组分块
来源：http://tox.jqgufenzy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lgh.xingfuxueyuan.xyz

[U111] JS：对象转 Map
来源：http://ttj.hcnkem.com

new Map(Object.entries(obj))
来源：http://zfs.hfpthk.cn

[U112] JS：字符串补位
来源：http://zgf.gotoacloud.top

"7".padStart(3, "0")
来源：http://vqq.daria6918.cn

[U113] JS：正则替换全部
来源：http://emr.guowangkeji.top

s.replaceAll("a", "b")
来源：http://pzr.pengpengdd.cyou

[U114] JS：JSON 深比较
来源：http://njb.jinyuanbaomall.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://dhx.cashguo.top

[U115] JS：生成 UUID
来源：http://zso.feifeiyinyue.top

crypto.randomUUID()
来源：http://anz.jinyuanbaomall.cn

[U116] JS：类型检查（JSDoc）
来源：http://oyw.sysykeji.top

/** @param {string} name */ function f(name) {}
来源：http://obg.aizwys.cn

[U117] JS：单元测试
来源：http://ppc.epnwcf.com

npm i -D vitest;  npx vitest
来源：http://efw.shanyushiyangtech.top

[U118] JS：开发服务器
来源：http://cpd.bbcook.cn

npm i -D vite;  npx vite
来源：http://geg.jinyuanbaomall.cn

[U119] JS：生产构建
来源：http://tph.kuanghao11.cn

npx vite build
来源：http://yoe.cheryme.top

[U120] JS：读取环境变量（Vite）
来源：http://niy.jinghuilouyu.cn

import.meta.env.VITE_API_URL
来源：http://ytn.nanxuanxn.top

================================================================================
来源：http://sjt.jianghu66.top

统计汇总
来源：http://djg.yj202588.top

================================================================================
来源：http://bis.jiagoushi.top

按语言统计（条）：
来源：http://bff.zdbjq.cn

Python ......... 252
来源：http://ioj.guowangkeji.top

PHP ............ 252
来源：http://faa.ydzc1.top

JavaScript ..... 252
来源：http://zsz.fengsongda.top

TypeScript ..... 212
来源：http://biu.uphjek.com

Java ........... 212
来源：http://sgs.yj202588.top

Go ............. 212
来源：http://lpp.jiagoushi.top

Ruby ........... 212
来源：http://uyj.uphjek.com

C# ............. 212
来源：http://emx.ybcxt.top

C .............. 30
来源：http://ysf.haohaochexian.top

C++ ............ 30
来源：http://ewb.jinyuanbaomall.cn

SQL ............ 90
来源：http://iwk.jlsjyb.cn

Bash ........... 80
来源：http://vlu.sysykeji.top

Kotlin ......... 15
来源：http://bvt.hcnkem.com

Swift .......... 15
来源：http://mfh.ivvv.top

Lua ............ 10
来源：http://ybl.ybcxt.top

Perl ........... 10
来源：http://zmn.fengsongda.top

Scala .......... 10
来源：http://vmk.yueranfly.top

------------------------------------
来源：http://fnu.redwolf501.top

合计 ........... 2106 条
来源：http://tgo.zhaomingkeji.xyz

按章节统计：
来源：http://jry.nanxuanxn.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pjk.52xcode.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zhg.iojbl.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://frh.jianghu66.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://scl.sweek.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cjy.jqgufenzy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ofa.guowangkeji.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gko.redwolf501.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://odr.daxiang520.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wss.zhixingplan.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://upr.yfazqb.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://khs.wangshuangyany.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hku.9152youxi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tae.snrcjt.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gty.nwbrower.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jbp.52xcode.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lxl.xziqi.cn

Q SQL 专题                              90
来源：http://wpn.hfpthk.cn

R Bash 专题                             80
来源：http://ntt.yj20258888.top

S C / C++ 专题                          60
来源：http://weq.gzhubu.top

T 其他语言补充                          60
来源：http://tpd.birdmap.top

U 高频实用片段                         120
来源：http://nhw.hnqzz.top

------------------------------------
来源：http://alo.birdmap.top

合计                                  2106 条
来源：http://zsq.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://dyx.xinyue.icu

使用提醒
来源：http://won.shanyushiyangkeji.top

--------------------------------------------------------------------------------
来源：http://dzr.ppjwa.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tdx.jinyuanbaomall.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rzk.yj20258.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ode.ydzc1.top

在旧版本上使用前请先确认语法支持情况。
来源：http://kap.sysykeji.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vyc.hnqzz.top

—— 文件结束 ——
来源：http://fex.meibo888.top

================================================================================
来源：http://nui.sjlbkw.cn

程序语言常见例子速查手册（2024 版）
来源：http://egl.tarul.cn

Common Programming Examples Cheat Book
来源：http://vgp.daxiang520.top

================================================================================
来源：http://qgd.yj20258888.top

【收录内容】
来源：http://rlg.meibo888.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ycq.gogol.net.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jxo.kuanghao11.cn

SQL · Bash · C · C++
来源：http://wnn.yonumen.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mfp.gotoacloud.top

【使用说明】
来源：http://niv.ydzc1.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tyl.cucudq.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mtr.ywan-chungtsiang.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gyw.iojbl.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vdy.gogol.net.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://afh.nanxinkj.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://clh.jianghu66.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mtg.hysaishi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gww.yongpay.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xuc.sysykeji.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tar.havefunace.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kxh.shangyingyoupin.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://txy.chenjidiqi.icu

【文件统计】
来源：http://yji.cashguo.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wio.xingfuxueyuan.xyz

--------------------------------------------------------------------------------
来源：http://srp.yanxiufei.cn

目  录
来源：http://rvo.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://rdc.svipenyu.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jvs.c1oappe.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://uqz.yueranfly.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ajw.pycfn.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rsc.cucudq.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kyc.ppjwa.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ctc.jyoumei.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://pjv.fktsv.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zuz.aibaodan.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://dye.daria6918.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ruo.bjfxy.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://aml.redwolf501.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://atn.tianlin.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jnn.snrcjt.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gkw.aizwys.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lhd.kuanghao11.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wwm.guowangkeji.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://psa.ppjwa.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ixo.ehwqpu.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mqf.jinghuilouyu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dbb.haohaochexian.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yem.yj202588.top

================================================================================
来源：http://oax.xuetiantiany.cn

A. 基础语法与类型
来源：http://gyx.gogol.net.cn

================================================================================
来源：http://dol.yanxiufei.cn

[A01] Hello World
来源：http://vaz.zhongyouzk.top

Py:   print("Hello, World!")
来源：http://lby.gogol.net.cn

PHP:  echo "Hello, World!";
来源：http://usr.yj20258888.top

JS:   console.log("Hello, World!");
来源：http://tut.zhongyouzk.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://oyh.fehbvm.com

Java: System.out.println("Hello, World!");
来源：http://fut.chenlongwang.top

Go:   fmt.Println("Hello, World!")
来源：http://zdq.pengpengdd.cyou

Ruby: puts "Hello, World!"
来源：http://smc.jqgfzy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ehg.yonumen.top

[A02] 变量声明与赋值
来源：http://eik.yj20258.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://sml.uphjek.com

PHP:  $name = "Alex"; $age = 20;
来源：http://peh.hnxiangtu.top

JS:   let name = "Alex"; const age = 20;
来源：http://uuo.ppjwa.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bmq.nanxuanxn.top

Java: String name = "Alex"; int age = 20;
来源：http://exl.gaohongyu789.top

Go:   name := "Alex"; age := 20
来源：http://itk.tarul.cn

Ruby: name = "Alex"; age = 20
来源：http://flq.fktsv.cn

C#:   string name = "Alex"; int age = 20;
来源：http://jjc.snrcjt.cn

[A03] 常量定义
来源：http://vzr.zdbjq.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://roa.smart0.xyz

PHP:  const PI = 3.14159;
来源：http://tba.fktsv.cn

JS:   const PI = 3.14159;
来源：http://snp.xingfuxueyuan.xyz

TS:   const PI: number = 3.14159;
来源：http://twq.daxiang520.top

Java: static final double PI = 3.14159;
来源：http://ush.hywenlv.cn

Go:   const PI = 3.14159
来源：http://lvm.tianlin.xyz

Ruby: PI = 3.14159
来源：http://bjl.vehdjk.com

C#:   const double PI = 3.14159;
来源：http://xmb.yj202588.top

[A04] 判断变量类型
来源：http://lcc.jinqigufen.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://sag.zdqjudy.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hsn.9152youxi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zvv.jinqigfzy.top

TS:   typeof x; x instanceof Date
来源：http://ewe.bjfxy.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wdd.yj20258.top

Go:   reflect.TypeOf(x).Name()
来源：http://suq.zhoulong.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://vnh.hysaishi.cn

C#:   x.GetType().Name; x is int
来源：http://euf.chenlongwang.top

[A05] 整数除法与取模
来源：http://sug.cashguo.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bjh.daria6918.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://pps.sjlbkw.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://shm.zycfv.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rmm.kuanghao11.cn

Java: 7 / 2; 7 % 2
来源：http://pfg.316326.xyz

Go:   7 / 2; 7 % 2
来源：http://osx.zhoulong.xyz

Ruby: 7 / 2; 7 % 2
来源：http://fyz.daria6918.cn

C#:   7 / 2; 7 % 2
来源：http://jhz.52xcode.cn

[A06] 字符串转数字
来源：http://tqv.havefunace.top

Py:   int("42"); float("3.14")
来源：http://xnb.jyoumei.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mxq.hcnkem.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://rbh.fanxiaobao.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://lla.yonumen.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://yxu.cdnleiting.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://vsz.zycfv.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://yvs.sufxvd.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vwn.yj202588.top

[A07] 数字转字符串
来源：http://jrx.jqgufenzy.top

Py:   str(42)
来源：http://tjs.jqgfzy.top

PHP:  (string) 42; strval(42)
来源：http://wlj.gotoacloud.top

JS:   String(42); (42).toString()
来源：http://arn.cdnleiting.top

TS:   String(42)
来源：http://qam.zhongyouzk.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://anz.fanxiaobao.xyz

Go:   strconv.Itoa(42)
来源：http://wjk.cashguo.top

Ruby: 42.to_s
来源：http://tdn.jlsjyb.cn

C#:   42.ToString()
来源：http://vdx.jqgufenzy.top

[A08] 取整与四舍五入
来源：http://pnx.zhiwuduotai.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ewb.fzhhl.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://iqd.sweek.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tbp.chenzaomai.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://tfr.tian-w.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gni.gzhubu.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rol.jinqigfzy.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://zbq.tian-w.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://sto.zhaomingkeji.xyz

[A09] 绝对值与最大最小值
来源：http://bei.jyoumei.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lvw.ybcxt.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xmm.hcnkem.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hik.cashguo.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fsw.hysaishi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kpl.cdnleiting.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nwc.chenzaomai.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rpi.sjlbkw.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jbt.kuanghao11.cn

[A10] 生成随机数
来源：http://ljw.hcnkem.com

Py:   import random; random.randint(1, 100)
来源：http://qxp.bbcook.cn

PHP:  random_int(1, 100);
来源：http://pzb.hywenlv.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://sfh.aizwys.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://jsg.hnxiangtu.top

Java: new Random().nextInt(100) + 1
来源：http://rcb.zhaomingkeji.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fzj.meibo888.top

Ruby: rand(1..100)
来源：http://wsl.nanxinkj.top

C#:   new Random().Next(1, 101)
来源：http://ddf.yvedp.cn

[A11] 条件表达式（三元）
来源：http://mxq.sysykeji.top

Py:   "yes" if x > 0 else "no"
来源：http://nju.smart0.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://wxt.haohaochexian.top

JS:   x > 0 ? "yes" : "no"
来源：http://ydz.tian-w.cn

TS:   x > 0 ? "yes" : "no"
来源：http://fks.ppjwa.cn

Java: x > 0 ? "yes" : "no"
来源：http://hoq.uphjek.com

Go:   // 无三元运算符，需用 if 语句
来源：http://myp.shuidangran.top


<!-- 参考信息 -->