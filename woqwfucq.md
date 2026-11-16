代发 wailian999

[U71] PHP：抛出异常
来源：http://ymg.zhongyouzk.top

throw new RuntimeException("失败", 500);
来源：http://ues.wangshuangyany.cn

[U72] PHP：写错误日志
来源：http://fav.shanyushiyangkeji.top

error_log("失败: " . $e->getMessage());
来源：http://kwg.yj20258888.top

[U73] PHP：读取 ini 配置
来源：http://ksx.mhx1999.top

parse_ini_file("config.ini", true)
来源：http://yjo.vehdjk.com

[U74] PHP：读取环境变量
来源：http://hzn.tian-w.cn

getenv("APP_ENV") ?: "production"
来源：http://uzk.0kj1m.cn

[U75] PHP：依赖注入
来源：http://nvn.chenzaomai.com

composer require psr/container
来源：http://sdi.hysaishi.cn

[U76] PHP：简单路由
来源：http://ekz.xingfuxueyuan.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ure.fktsv.cn

[U77] PHP：模板渲染
来源：http://msn.jiagoushi.top

composer require twig/twig
来源：http://gvq.snrcjt.cn

[U78] PHP：单元测试
来源：http://egg.jinqigufen.top

composer require --dev phpunit/phpunit
来源：http://qre.guowangkeji.top

[U79] PHP：静态分析
来源：http://ind.jqgufenzy.top

composer require --dev phpstan/phpstan
来源：http://gzb.guannengcc.top

[U80] PHP：代码规范修复
来源：http://gdq.uphjek.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://grk.fengsongda.top

[U81] JS：初始化项目
来源：http://rdp.svipenyu.cn

npm init -y;  npm i express
来源：http://jay.fktsv.cn

[U82] JS：package.json 脚本
来源：http://ekm.snrcjt.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wzb.gzhubu.top

[U83] JS：ES Module 导入导出
来源：http://vid.yj202588.top

export const a = 1;  import { a } from "./m.js";
来源：http://idl.xingfuxueyuan.xyz

[U84] JS：CommonJS 写法
来源：http://det.jinghuilouyu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://evh.zhaomingkeji.xyz

[U85] JS：可选链
来源：http://pdm.andypj.xyz

a?.b?.c
来源：http://zbx.nwbrower.top

[U86] JS：空值合并
来源：http://hyz.aibaodan.cn

a ?? b
来源：http://tmv.feifeiyinyue.top

[U87] JS：解构默认值
来源：http://qzx.ivvv.top

const { a = 1, b = 2 } = obj;
来源：http://gma.xziqi.cn

[U88] JS：对象展开合并
来源：http://mgz.xuanzx.com

{ ...a, ...b }
来源：http://bqt.xingfuxueyuan.xyz

[U89] JS：数组去重
来源：http://lxg.feifeiyinyue.top

[...new Set(arr)]
来源：http://xxr.sweek.top

[U90] JS：数字数组排序
来源：http://sku.jinyuanbaomall.cn

[...arr].sort((a, b) => a - b)
来源：http://hwv.zhengqikj.top

[U91] JS：对象键值遍历
来源：http://vhk.jinqigfzy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vag.ywan-chungtsiang.top

[U92] JS：深拷贝
来源：http://bxo.guowangkeji.top

structuredClone(obj)
来源：http://gtk.hammf.cn

[U93] JS：模板字符串
来源：http://ajb.redwolf501.top

`共 ${n} 条`
来源：http://hyc.hywenlv.cn

[U94] JS：箭头函数
来源：http://ocn.fehbvm.com

const double = x => x * 2;
来源：http://dbt.vqdsnc.cn

[U95] JS：Promise 包装
来源：http://iks.bjfxy.top

new Promise((resolve, reject) => {})
来源：http://bxb.redwolf501.top

[U96] JS：async/await 与异常
来源：http://sht.svipenyu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uiw.zhoulong.xyz

[U97] JS：并发请求
来源：http://bre.xuanzx.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://ltn.zhengqikj.top

[U98] JS：fetch 带 JSON
来源：http://wvd.ctjpmb.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yet.zhiwuduotai.top

[U99] JS：事件监听
来源：http://eya.aibaodan.cn

el.addEventListener("click", e => {})
来源：http://mnz.sjlbkw.cn

[U100] JS：DOM 查询
来源：http://hgr.gotoacloud.top

document.querySelector(".item")
来源：http://pjl.yfazqb.com

[U101] JS：classList 操作
来源：http://kvy.guowangkeji.top

el.classList.toggle("active")
来源：http://utp.aizwys.cn

[U102] JS：本地存储
来源：http://wzu.tianlin.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://gdd.jyoumei.cn

[U103] JS：定时器
来源：http://smq.svipenyu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://emo.ivvv.top

[U104] JS：防抖
来源：http://ybu.chenlongwang.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yai.gotoacloud.top

[U105] JS：节流
来源：http://als.yueranfly.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bfb.shuidangran.top

[U106] JS：日期格式化
来源：http://buu.hongshengwenyu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://idh.shanyushiyangkeji.top

[U107] JS：数字千分位
来源：http://uiw.nwbrower.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ile.316326.xyz

[U108] JS：随机整数
来源：http://smz.smart0.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rcc.bjfxy.top

[U109] JS：数组分组
来源：http://buc.chenlongwang.top

Object.groupBy(arr, x => x.type)
来源：http://fax.sweek.top

[U110] JS：数组分块
来源：http://hzb.zhixingplan.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nil.cqqwz.cn

[U111] JS：对象转 Map
来源：http://kux.zhaomingkeji.xyz

new Map(Object.entries(obj))
来源：http://qld.jinghuilouyu.cn

[U112] JS：字符串补位
来源：http://lrp.fzhhl.top

"7".padStart(3, "0")
来源：http://tre.epnwcf.com

[U113] JS：正则替换全部
来源：http://yfe.sufxvd.cn

s.replaceAll("a", "b")
来源：http://ssh.svipenyu.cn

[U114] JS：JSON 深比较
来源：http://nma.shzxlz.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xlg.fengsongda.top

[U115] JS：生成 UUID
来源：http://nhz.xuanzx.com

crypto.randomUUID()
来源：http://dpe.sjlbkw.cn

[U116] JS：类型检查（JSDoc）
来源：http://hgh.xuetiantiany.cn

/** @param {string} name */ function f(name) {}
来源：http://sip.fehbvm.com

[U117] JS：单元测试
来源：http://beb.zhixingplan.top

npm i -D vitest;  npx vitest
来源：http://kft.jinyuanbaomall.cn

[U118] JS：开发服务器
来源：http://tjn.pycfn.com

npm i -D vite;  npx vite
来源：http://hxg.tarul.cn

[U119] JS：生产构建
来源：http://wpa.sysykeji.top

npx vite build
来源：http://lme.nwbrower.top

[U120] JS：读取环境变量（Vite）
来源：http://jlb.daxiang520.top

import.meta.env.VITE_API_URL
来源：http://tys.hammf.cn

================================================================================
来源：http://zcl.havefunace.top

统计汇总
来源：http://gxs.shzxlz.cn

================================================================================
来源：http://jnr.0kj1m.cn

按语言统计（条）：
来源：http://uyl.ywan-chungtsiang.top

Python ......... 252
来源：http://qga.yongpay.top

PHP ............ 252
来源：http://mtw.yonumen.top

JavaScript ..... 252
来源：http://vjh.shuidangran.top

TypeScript ..... 212
来源：http://qdf.yueranfly.top

Java ........... 212
来源：http://vfq.sysykeji.top

Go ............. 212
来源：http://ukk.shangyingyoupin.top

Ruby ........... 212
来源：http://odr.pengpengdd.cyou

C# ............. 212
来源：http://biy.yueranfly.top

C .............. 30
来源：http://qxe.yj202588.top

C++ ............ 30
来源：http://est.guannengcc.top

SQL ............ 90
来源：http://cyz.uphjek.com

Bash ........... 80
来源：http://wuw.yj202588.top

Kotlin ......... 15
来源：http://uvc.fengsongda.top

Swift .......... 15
来源：http://ysw.vehdjk.com

Lua ............ 10
来源：http://txg.mhx1999.top

Perl ........... 10
来源：http://yci.ivvv.top

Scala .......... 10
来源：http://ome.haohaochexian.top

------------------------------------
来源：http://zkm.yonumen.top

合计 ........... 2106 条
来源：http://vun.daria6918.cn

按章节统计：
来源：http://ose.xingfuxueyuan.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xat.wangdashe.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wcd.tarul.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://egl.shzxlz.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kza.fktsv.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zef.sysykeji.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://usm.fengsongda.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ofi.hammf.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lce.zdqjudy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jym.shzxlz.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hgx.zhoulong.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ins.chenlongwang.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kye.9152youxi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://unl.316326.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ngo.pengpengdd.cyou

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hks.hesvh.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://izz.smart0.xyz

Q SQL 专题                              90
来源：http://sqj.c1oappe.top

R Bash 专题                             80
来源：http://lao.hnqzz.top

S C / C++ 专题                          60
来源：http://cjl.svipenyu.cn

T 其他语言补充                          60
来源：http://vkv.xylfe.cn

U 高频实用片段                         120
来源：http://klp.nanxuanxn.top

------------------------------------
来源：http://yis.svipenyu.cn

合计                                  2106 条
来源：http://tvg.jinghuilouyu.cn

--------------------------------------------------------------------------------
来源：http://utl.mhx1999.top

使用提醒
来源：http://nnc.shanyushiyangtech.top

--------------------------------------------------------------------------------
来源：http://gnv.zdbjq.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jtw.tianlin.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://yqa.yueranfly.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wfo.guannengcc.top

在旧版本上使用前请先确认语法支持情况。
来源：http://tgk.hcnkem.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yfl.fzhhl.top

—— 文件结束 ——
来源：http://lcz.9152youxi.cn

================================================================================
来源：http://dxq.cqqwz.cn

程序语言常见例子速查手册（2024 版）
来源：http://snj.meibo888.top

Common Programming Examples Cheat Book
来源：http://aoi.sufxvd.cn

================================================================================
来源：http://cbz.bjfxy.top

【收录内容】
来源：http://cjg.pengpengdd.cyou

覆盖 12 种语言 / 语法与常见 API：
来源：http://sed.9152youxi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tbz.wangdashe.top

SQL · Bash · C · C++
来源：http://lxm.yj20258.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xkw.yfazqb.com

【使用说明】
来源：http://caf.gogol.net.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://idr.ppjwa.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zah.sweek.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nhu.sweek.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ajp.gotoacloud.top

Bash:  Shell         C:     C             C++:   C++
来源：http://qwm.xuetiantiany.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wae.shanyushiyangkeji.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qbx.ehwqpu.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hrf.jianghu66.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cgm.guannengcc.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://uek.tianlin.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pxo.hysaishi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hrl.chenjidiqi.icu

【文件统计】
来源：http://jqd.dashuyun.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://afj.9152youxi.cn

--------------------------------------------------------------------------------
来源：http://pai.shuidangran.top

目  录
来源：http://lwv.yanxiufei.cn

--------------------------------------------------------------------------------
来源：http://ard.hywenlv.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://swo.sysykeji.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tin.gzhubu.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://olg.zhijiandao.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kwu.fehbvm.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bvk.c1oappe.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://iuk.xuanzx.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://cpq.dianchejie.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://juq.jiagoushi.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kqw.gotoacloud.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ktd.yvedp.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://isj.nanxuanxn.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://onn.jianghu66.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gsy.havefunace.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hbt.ctjpmb.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vjs.shanyushiyangkeji.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://nyb.redwolf501.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tkf.wangdashe.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://mkj.ehwqpu.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://sxg.jlsjyb.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ego.daxiang520.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jjc.ctjpmb.com

================================================================================
来源：http://cay.zhiwuduotai.top

A. 基础语法与类型
来源：http://jwt.quarkkingdee.top

================================================================================
来源：http://qck.shangyingyoupin.top

[A01] Hello World
来源：http://dyt.mhx1999.top

Py:   print("Hello, World!")
来源：http://vgi.svipenyu.cn

PHP:  echo "Hello, World!";
来源：http://fxd.cucudq.cn

JS:   console.log("Hello, World!");
来源：http://pwh.xylfe.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://uwo.hongshengwenyu.top

Java: System.out.println("Hello, World!");
来源：http://gxm.redwolf501.top

Go:   fmt.Println("Hello, World!")
来源：http://ynp.kuanghao11.cn

Ruby: puts "Hello, World!"
来源：http://clo.yj202588.top

C#:   Console.WriteLine("Hello, World!");
来源：http://rvf.nanxuanxn.top

[A02] 变量声明与赋值
来源：http://gom.hnxiangtu.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://imx.hfpthk.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://nht.shanyushiyangkeji.top

JS:   let name = "Alex"; const age = 20;
来源：http://miz.jinqigufen.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ubi.guowangkeji.top

Java: String name = "Alex"; int age = 20;
来源：http://eoc.sxryk.cn

Go:   name := "Alex"; age := 20
来源：http://skn.xingfuxueyuan.xyz

Ruby: name = "Alex"; age = 20
来源：http://tuj.yj20258888.top

C#:   string name = "Alex"; int age = 20;
来源：http://qju.fehbvm.com

[A03] 常量定义
来源：http://vbn.bjfxy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://coa.aibaodan.cn

PHP:  const PI = 3.14159;
来源：http://kkr.epnwcf.com

JS:   const PI = 3.14159;
来源：http://mlz.ybcxt.top

TS:   const PI: number = 3.14159;
来源：http://ahs.mhx1999.top

Java: static final double PI = 3.14159;
来源：http://bof.haohaochexian.top

Go:   const PI = 3.14159
来源：http://pof.ctjpmb.com

Ruby: PI = 3.14159
来源：http://vvm.vehdjk.com

C#:   const double PI = 3.14159;
来源：http://jbm.birdmap.top

[A04] 判断变量类型
来源：http://foa.chenzaomai.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://vpb.zhengqikj.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gzd.sysykeji.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nlh.52xcode.cn

TS:   typeof x; x instanceof Date
来源：http://krd.guowangkeji.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wvq.zycfv.cn

Go:   reflect.TypeOf(x).Name()
来源：http://zsv.hnqzz.top

Ruby: x.class; x.is_a?(Integer)
来源：http://mmz.jyoumei.cn

C#:   x.GetType().Name; x is int
来源：http://rbb.meibo888.top

[A05] 整数除法与取模
来源：http://rhh.nanxuanxn.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://dkm.jyoumei.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://yxa.guowangkeji.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://kts.cucudq.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pxm.quarkkingdee.top

Java: 7 / 2; 7 % 2
来源：http://gcq.pycfn.com

Go:   7 / 2; 7 % 2
来源：http://vdd.fzhhl.top

Ruby: 7 / 2; 7 % 2
来源：http://stp.birdmap.top

C#:   7 / 2; 7 % 2
来源：http://ncj.daria6918.cn

[A06] 字符串转数字
来源：http://foy.yueranfly.top

Py:   int("42"); float("3.14")
来源：http://apt.guowangkeji.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://sju.sjlbkw.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://czq.c1oappe.top

TS:   parseInt("42", 10); Number("42")
来源：http://nnd.guannengcc.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://owp.haohaochexian.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hnj.zhengqikj.top

Ruby: "42".to_i; "3.14".to_f
来源：http://yme.yfazqb.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://yek.316326.xyz

[A07] 数字转字符串
来源：http://tif.jqgfzy.top

Py:   str(42)
来源：http://bwr.gzhubu.top

PHP:  (string) 42; strval(42)
来源：http://gwg.ybcxt.top

JS:   String(42); (42).toString()
来源：http://rlu.ydjk.org.cn

TS:   String(42)
来源：http://ooq.jqgfzy.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://fww.chenzaomai.com

Go:   strconv.Itoa(42)
来源：http://kto.xinyue.icu

Ruby: 42.to_s
来源：http://zum.fehbvm.com

C#:   42.ToString()
来源：http://lsf.xuetiantiany.cn

[A08] 取整与四舍五入
来源：http://zhl.iojbl.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ivf.pengpengdd.cyou

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dwv.ctjpmb.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://rev.guowangkeji.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jap.guowangkeji.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://aqr.jqgfzy.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://cnm.bjfxy.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://mex.zycfv.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mpo.havefunace.top

[A09] 绝对值与最大最小值
来源：http://gmh.zdbjq.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hnr.ybcxt.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://aat.zhijiandao.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hky.ctjpmb.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://eja.yanxiufei.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://oak.ywan-chungtsiang.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://yqx.zhongyouzk.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://prp.yj20258.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ube.zhengqikj.top

[A10] 生成随机数
来源：http://usc.jinghuilouyu.cn

Py:   import random; random.randint(1, 100)
来源：http://pjz.smart0.xyz

PHP:  random_int(1, 100);
来源：http://pgt.sjlbkw.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://eoa.52xcode.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://usp.shzxlz.cn

Java: new Random().nextInt(100) + 1
来源：http://hfa.yonumen.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cdg.zhixingplan.top

Ruby: rand(1..100)
来源：http://bkw.cucudq.cn

C#:   new Random().Next(1, 101)
来源：http://pxk.yvedp.cn

[A11] 条件表达式（三元）
来源：http://ttu.snrcjt.cn

Py:   "yes" if x > 0 else "no"
来源：http://kby.snrcjt.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://fnv.aibaodan.cn


<!-- 参考信息 -->