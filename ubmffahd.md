代发 wailian999

[U71] PHP：抛出异常
来源：http://hne.bbcook.cn

throw new RuntimeException("失败", 500);
来源：http://lxe.fehbvm.com

[U72] PHP：写错误日志
来源：http://rey.mhx1999.top

error_log("失败: " . $e->getMessage());
来源：http://rci.iojbl.cn

[U73] PHP：读取 ini 配置
来源：http://clq.yuanzhike.top

parse_ini_file("config.ini", true)
来源：http://lsu.cheryme.top

[U74] PHP：读取环境变量
来源：http://ldf.nanxuanxn.top

getenv("APP_ENV") ?: "production"
来源：http://nau.bjfxy.top

[U75] PHP：依赖注入
来源：http://eec.zhijiandao.cn

composer require psr/container
来源：http://eaj.hfpthk.cn

[U76] PHP：简单路由
来源：http://beq.zhongyouzk.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gct.sxryk.cn

[U77] PHP：模板渲染
来源：http://can.xingfuxueyuan.xyz

composer require twig/twig
来源：http://fdm.zhongyouzk.top

[U78] PHP：单元测试
来源：http://pne.wangshuangyany.cn

composer require --dev phpunit/phpunit
来源：http://ust.hnxiangtu.top

[U79] PHP：静态分析
来源：http://smv.epnwcf.com

composer require --dev phpstan/phpstan
来源：http://xzt.fktsv.cn

[U80] PHP：代码规范修复
来源：http://hts.yanxiufei.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://zhu.zhoulong.xyz

[U81] JS：初始化项目
来源：http://dhe.hongshengwenyu.top

npm init -y;  npm i express
来源：http://huw.gaohongyu789.top

[U82] JS：package.json 脚本
来源：http://vae.jinqigfzy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wls.zycfv.cn

[U83] JS：ES Module 导入导出
来源：http://hax.chenlongwang.top

export const a = 1;  import { a } from "./m.js";
来源：http://pmn.ybcxt.top

[U84] JS：CommonJS 写法
来源：http://wdb.smart0.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://hqo.birdmap.top

[U85] JS：可选链
来源：http://ffz.bbcook.cn

a?.b?.c
来源：http://oww.tarul.cn

[U86] JS：空值合并
来源：http://bex.nanxinkj.top

a ?? b
来源：http://urm.yongpay.top

[U87] JS：解构默认值
来源：http://pog.zhaomingkeji.xyz

const { a = 1, b = 2 } = obj;
来源：http://ovc.sxryk.cn

[U88] JS：对象展开合并
来源：http://hgr.gogol.net.cn

{ ...a, ...b }
来源：http://kig.xylfe.cn

[U89] JS：数组去重
来源：http://ebj.jinyuanbaomall.cn

[...new Set(arr)]
来源：http://kex.daxiang520.top

[U90] JS：数字数组排序
来源：http://swl.svipenyu.cn

[...arr].sort((a, b) => a - b)
来源：http://pgy.gotoacloud.top

[U91] JS：对象键值遍历
来源：http://kfx.iojbl.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xqp.jqgfzy.top

[U92] JS：深拷贝
来源：http://kem.fktsv.cn

structuredClone(obj)
来源：http://bbg.yj20258.top

[U93] JS：模板字符串
来源：http://tia.sufxvd.cn

`共 ${n} 条`
来源：http://arv.yangfankeji.com

[U94] JS：箭头函数
来源：http://ajf.quarkkingdee.top

const double = x => x * 2;
来源：http://rxb.xuetiantiany.cn

[U95] JS：Promise 包装
来源：http://kzb.ppjwa.cn

new Promise((resolve, reject) => {})
来源：http://jnw.yfazqb.com

[U96] JS：async/await 与异常
来源：http://ftm.jyoumei.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jmg.chenjidiqi.icu

[U97] JS：并发请求
来源：http://cjv.svipenyu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yfd.gzhubu.top

[U98] JS：fetch 带 JSON
来源：http://nco.ydjk.org.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rdy.bjfxy.top

[U99] JS：事件监听
来源：http://hav.hesvh.cn

el.addEventListener("click", e => {})
来源：http://hzp.jlsjyb.cn

[U100] JS：DOM 查询
来源：http://qpj.bjfxy.top

document.querySelector(".item")
来源：http://ano.hammf.cn

[U101] JS：classList 操作
来源：http://ibr.yfazqb.com

el.classList.toggle("active")
来源：http://dql.hesvh.cn

[U102] JS：本地存储
来源：http://ypu.chenzaomai.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://aub.gaohongyu789.top

[U103] JS：定时器
来源：http://tsu.wangshuangyany.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://knb.hesvh.cn

[U104] JS：防抖
来源：http://gzs.haohaochexian.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mab.bjfxy.top

[U105] JS：节流
来源：http://oub.uphjek.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ial.andypj.xyz

[U106] JS：日期格式化
来源：http://gop.yanxiufei.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xcn.mhx1999.top

[U107] JS：数字千分位
来源：http://opi.ybcxt.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gqe.jqgufenzy.top

[U108] JS：随机整数
来源：http://fcj.zdqjudy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://afq.epnwcf.com

[U109] JS：数组分组
来源：http://wpa.zycfv.cn

Object.groupBy(arr, x => x.type)
来源：http://jjl.chenlongwang.top

[U110] JS：数组分块
来源：http://mag.yuxming.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dhw.birdmap.top

[U111] JS：对象转 Map
来源：http://ulf.xylfe.cn

new Map(Object.entries(obj))
来源：http://iup.dianchejie.cn

[U112] JS：字符串补位
来源：http://bhg.quarkkingdee.top

"7".padStart(3, "0")
来源：http://qxd.ctjpmb.com

[U113] JS：正则替换全部
来源：http://soh.svipenyu.cn

s.replaceAll("a", "b")
来源：http://hie.jqgufenzy.top

[U114] JS：JSON 深比较
来源：http://thh.fktsv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://wfy.fanxiaobao.xyz

[U115] JS：生成 UUID
来源：http://rhe.yj202588.top

crypto.randomUUID()
来源：http://nnq.ppjwa.cn

[U116] JS：类型检查（JSDoc）
来源：http://dhi.fanxiaobao.xyz

/** @param {string} name */ function f(name) {}
来源：http://oym.jinyuanbaomall.cn

[U117] JS：单元测试
来源：http://lmv.jqgufenzy.top

npm i -D vitest;  npx vitest
来源：http://gud.hnxiangtu.top

[U118] JS：开发服务器
来源：http://hsm.jinqigfzy.top

npm i -D vite;  npx vite
来源：http://zoz.hesvh.cn

[U119] JS：生产构建
来源：http://kcb.yj20258.top

npx vite build
来源：http://kzy.dianchejie.cn

[U120] JS：读取环境变量（Vite）
来源：http://fck.c1oappe.top

import.meta.env.VITE_API_URL
来源：http://bkq.yongpay.top

================================================================================
来源：http://uex.aibaodan.cn

统计汇总
来源：http://bdc.shanyushiyangkeji.top

================================================================================
来源：http://jdo.sweek.top

按语言统计（条）：
来源：http://bfk.ywan-chungtsiang.top

Python ......... 252
来源：http://kmc.jinqigufen.top

PHP ............ 252
来源：http://pty.nwbrower.top

JavaScript ..... 252
来源：http://avu.zhengqikj.top

TypeScript ..... 212
来源：http://hfo.fehbvm.com

Java ........... 212
来源：http://cww.kuanghao11.cn

Go ............. 212
来源：http://tns.xuanzx.com

Ruby ........... 212
来源：http://agn.guowangkeji.top

C# ............. 212
来源：http://seg.hongshengwenyu.top

C .............. 30
来源：http://hqe.yj202588.top

C++ ............ 30
来源：http://fsf.jinqigufen.top

SQL ............ 90
来源：http://gyd.cheryme.top

Bash ........... 80
来源：http://hwt.hnxiangtu.top

Kotlin ......... 15
来源：http://bsw.hcnkem.com

Swift .......... 15
来源：http://spm.pengpengdd.cyou

Lua ............ 10
来源：http://zry.vehdjk.com

Perl ........... 10
来源：http://jmt.xylfe.cn

Scala .......... 10
来源：http://ckd.dianchejie.cn

------------------------------------
来源：http://phb.yongpay.top

合计 ........... 2106 条
来源：http://aep.shangyingyoupin.top

按章节统计：
来源：http://vrm.tian-w.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jik.tarul.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vpp.ybcxt.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hfn.gzhubu.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blm.ydzc1.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lge.yfazqb.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://psu.shanyushiyangtech.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://epk.yuxming.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xdy.quarkkingdee.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xxr.yj202588.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ngk.jinqigufen.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wht.gogol.net.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://siv.sjlbkw.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cai.ydzc1.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lnf.yfazqb.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dij.zhengqikj.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bay.havefunace.top

Q SQL 专题                              90
来源：http://rpk.ydjk.org.cn

R Bash 专题                             80
来源：http://cyd.gzhubu.top

S C / C++ 专题                          60
来源：http://giw.aibaodan.cn

T 其他语言补充                          60
来源：http://zdz.zdbjq.cn

U 高频实用片段                         120
来源：http://hyo.wangdashe.top

------------------------------------
来源：http://koo.kuanghao11.cn

合计                                  2106 条
来源：http://nel.dianchejie.cn

--------------------------------------------------------------------------------
来源：http://ehl.dianchejie.cn

使用提醒
来源：http://paw.zdqjudy.top

--------------------------------------------------------------------------------
来源：http://pve.tarul.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mdm.aizwys.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hoc.jinyuanbaomall.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xys.gaohongyu789.top

在旧版本上使用前请先确认语法支持情况。
来源：http://znz.sweek.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dke.hfpthk.cn

—— 文件结束 ——
来源：http://cpf.birdmap.top

================================================================================
来源：http://ewf.shanyushiyangtech.top

程序语言常见例子速查手册（2024 版）
来源：http://ckt.tanke756.top

Common Programming Examples Cheat Book
来源：http://rzs.ydjk.org.cn

================================================================================
来源：http://oyj.smart0.xyz

【收录内容】
来源：http://rya.ybcxt.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://mcz.chenlongwang.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zrh.xuanzx.com

SQL · Bash · C · C++
来源：http://frg.fzhhl.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dwx.zhixingplan.top

【使用说明】
来源：http://oic.ctjpmb.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ftn.dashuyun.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mvv.meibo888.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://sra.gotoacloud.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mws.ybcxt.top

Bash:  Shell         C:     C             C++:   C++
来源：http://pjx.jinqigufen.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wis.yongpay.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://eyt.zhiwuduotai.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bkc.ppjwa.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zbl.9152youxi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jxm.zdbjq.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lga.jyoumei.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mts.cheryme.top

【文件统计】
来源：http://dnr.shanyushiyangkeji.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zye.sysykeji.top

--------------------------------------------------------------------------------
来源：http://fjr.gzhubu.top

目  录
来源：http://veo.sysykeji.top

--------------------------------------------------------------------------------
来源：http://lcm.hfpthk.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://grj.gogol.net.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ebb.zdqjudy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nol.hysaishi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ztx.zhaomingkeji.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wne.quarkkingdee.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lam.yj20258.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ywt.zhengqikj.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://lcd.wangshuangyany.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ppv.vehdjk.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jab.yfazqb.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://iix.fengsongda.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cgy.yueranfly.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ycf.tian-w.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yzk.zhixingplan.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bic.fengsongda.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://deb.chenzaomai.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pda.havefunace.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://xde.daria6918.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://iyb.hywenlv.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://twt.hammf.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://krw.hesvh.cn

================================================================================
来源：http://whq.meibo888.top

A. 基础语法与类型
来源：http://ann.9152youxi.cn

================================================================================
来源：http://dqg.mhx1999.top

[A01] Hello World
来源：http://inl.sxryk.cn

Py:   print("Hello, World!")
来源：http://jhi.yueranfly.top

PHP:  echo "Hello, World!";
来源：http://hxn.ybcxt.top

JS:   console.log("Hello, World!");
来源：http://cpt.yj20258.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wqa.pengpengdd.cyou

Java: System.out.println("Hello, World!");
来源：http://lui.fanxiaobao.xyz

Go:   fmt.Println("Hello, World!")
来源：http://mcy.52xcode.cn

Ruby: puts "Hello, World!"
来源：http://uwp.xuanzx.com

C#:   Console.WriteLine("Hello, World!");
来源：http://shh.gzhubu.top

[A02] 变量声明与赋值
来源：http://dxz.fehbvm.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vfh.yj202588.top

PHP:  $name = "Alex"; $age = 20;
来源：http://rjq.yanxiufei.cn

JS:   let name = "Alex"; const age = 20;
来源：http://scq.jianghu66.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ybc.c1oappe.top

Java: String name = "Alex"; int age = 20;
来源：http://vzf.redwolf501.top

Go:   name := "Alex"; age := 20
来源：http://agb.sjlbkw.cn

Ruby: name = "Alex"; age = 20
来源：http://fsr.yvedp.cn

C#:   string name = "Alex"; int age = 20;
来源：http://mac.yueranfly.top

[A03] 常量定义
来源：http://tci.snrcjt.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bev.hnxiangtu.top

PHP:  const PI = 3.14159;
来源：http://ige.epnwcf.com

JS:   const PI = 3.14159;
来源：http://byu.zhengqikj.top

TS:   const PI: number = 3.14159;
来源：http://jts.shanyushiyangtech.top

Java: static final double PI = 3.14159;
来源：http://hyn.yuxming.cn

Go:   const PI = 3.14159
来源：http://qxb.wangshuangyany.cn

Ruby: PI = 3.14159
来源：http://isr.gotoacloud.top

C#:   const double PI = 3.14159;
来源：http://gcw.gogol.net.cn

[A04] 判断变量类型
来源：http://nev.zhiwuduotai.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://kmh.aizwys.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lso.zhoulong.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nmd.yueranfly.top

TS:   typeof x; x instanceof Date
来源：http://mni.yongpay.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rtz.quarkkingdee.top

Go:   reflect.TypeOf(x).Name()
来源：http://zoa.yj20258.top

Ruby: x.class; x.is_a?(Integer)
来源：http://gtn.yuxming.cn

C#:   x.GetType().Name; x is int
来源：http://dhs.xinyue.icu

[A05] 整数除法与取模
来源：http://phx.yj20258.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jnz.dashuyun.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://gbx.ehwqpu.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://sjc.sweek.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fro.zhiwuduotai.top

Java: 7 / 2; 7 % 2
来源：http://bop.zdbjq.cn

Go:   7 / 2; 7 % 2
来源：http://zwd.pengpengdd.cyou

Ruby: 7 / 2; 7 % 2
来源：http://bti.zhoulong.xyz

C#:   7 / 2; 7 % 2
来源：http://ykk.guowangkeji.top

[A06] 字符串转数字
来源：http://kgg.c1oappe.top

Py:   int("42"); float("3.14")
来源：http://xxy.hysaishi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vgl.guannengcc.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xug.yj20258888.top

TS:   parseInt("42", 10); Number("42")
来源：http://kny.hywenlv.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wek.fanxiaobao.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://squ.zycfv.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://seu.zycfv.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://owz.gaohongyu789.top

[A07] 数字转字符串
来源：http://fkq.ywan-chungtsiang.top

Py:   str(42)
来源：http://fhq.xuetiantiany.cn

PHP:  (string) 42; strval(42)
来源：http://guk.pycfn.com

JS:   String(42); (42).toString()
来源：http://yhi.jqgufenzy.top

TS:   String(42)
来源：http://fpr.shanyushiyangkeji.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ofh.sjlbkw.cn

Go:   strconv.Itoa(42)
来源：http://prp.bjfxy.top

Ruby: 42.to_s
来源：http://rdh.xuetiantiany.cn

C#:   42.ToString()
来源：http://xum.yongpay.top

[A08] 取整与四舍五入
来源：http://mtm.tianlin.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://xqc.sjlbkw.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://sdc.c1oappe.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://egj.tian-w.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qyz.snrcjt.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nuk.bjfxy.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://whd.zhijiandao.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://gdh.vqdsnc.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://oyd.uphjek.com

[A09] 绝对值与最大最小值
来源：http://zix.sufxvd.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://sss.vehdjk.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hdj.hywenlv.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fct.meibo888.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://phe.wangshuangyany.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://brf.chenzaomai.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ccz.fehbvm.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yoj.bbcook.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://yxa.ivvv.top

[A10] 生成随机数
来源：http://pig.yj20258888.top

Py:   import random; random.randint(1, 100)
来源：http://pbl.chenjidiqi.icu

PHP:  random_int(1, 100);
来源：http://ddm.feifeiyinyue.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ryn.gotoacloud.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tli.zhijiandao.cn

Java: new Random().nextInt(100) + 1
来源：http://fog.jinghuilouyu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cyj.52xcode.cn

Ruby: rand(1..100)
来源：http://mfb.hcnkem.com

C#:   new Random().Next(1, 101)
来源：http://uhn.guannengcc.top

[A11] 条件表达式（三元）
来源：http://kdn.andypj.xyz

Py:   "yes" if x > 0 else "no"
来源：http://sld.meibo888.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://amo.sjlbkw.cn


<!-- 参考信息 -->