代发 wailian999

[U71] PHP：抛出异常
来源：http://iqc.tarul.cn

throw new RuntimeException("失败", 500);
来源：http://ncn.fehbvm.com

[U72] PHP：写错误日志
来源：http://tse.fehbvm.com

error_log("失败: " . $e->getMessage());
来源：http://kai.fehbvm.com

[U73] PHP：读取 ini 配置
来源：http://orv.andypj.xyz

parse_ini_file("config.ini", true)
来源：http://tqm.pengpengdd.cyou

[U74] PHP：读取环境变量
来源：http://bpr.fehbvm.com

getenv("APP_ENV") ?: "production"
来源：http://not.jlsjyb.cn

[U75] PHP：依赖注入
来源：http://beg.jqgfzy.top

composer require psr/container
来源：http://cib.nwbrower.top

[U76] PHP：简单路由
来源：http://wtj.nanxinkj.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mus.sjlbkw.cn

[U77] PHP：模板渲染
来源：http://wrg.ydjk.org.cn

composer require twig/twig
来源：http://vrm.sxryk.cn

[U78] PHP：单元测试
来源：http://klo.ydjk.org.cn

composer require --dev phpunit/phpunit
来源：http://pss.hnxiangtu.top

[U79] PHP：静态分析
来源：http://rgy.haohaochexian.top

composer require --dev phpstan/phpstan
来源：http://hvk.birdmap.top

[U80] PHP：代码规范修复
来源：http://nli.ivvv.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://thq.nwbrower.top

[U81] JS：初始化项目
来源：http://aso.jqgfzy.top

npm init -y;  npm i express
来源：http://ama.quarkkingdee.top

[U82] JS：package.json 脚本
来源：http://lvc.ydzc1.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://doc.chenzaomai.com

[U83] JS：ES Module 导入导出
来源：http://sbj.feifeiyinyue.top

export const a = 1;  import { a } from "./m.js";
来源：http://ine.birdmap.top

[U84] JS：CommonJS 写法
来源：http://rgg.yuxming.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qrq.cheryme.top

[U85] JS：可选链
来源：http://dat.zhongyouzk.top

a?.b?.c
来源：http://pbc.xuanzx.com

[U86] JS：空值合并
来源：http://htz.hesvh.cn

a ?? b
来源：http://swb.yonumen.top

[U87] JS：解构默认值
来源：http://dmd.ywan-chungtsiang.top

const { a = 1, b = 2 } = obj;
来源：http://zuu.zhiwuduotai.top

[U88] JS：对象展开合并
来源：http://fug.yfazqb.com

{ ...a, ...b }
来源：http://nzc.cdnleiting.top

[U89] JS：数组去重
来源：http://stp.hnqzz.top

[...new Set(arr)]
来源：http://sxp.bbcook.cn

[U90] JS：数字数组排序
来源：http://cth.cucudq.cn

[...arr].sort((a, b) => a - b)
来源：http://ike.zdqjudy.top

[U91] JS：对象键值遍历
来源：http://vnn.ydzc1.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://muy.mhx1999.top

[U92] JS：深拷贝
来源：http://hdu.zhoulong.xyz

structuredClone(obj)
来源：http://bjj.sxryk.cn

[U93] JS：模板字符串
来源：http://tmg.ybcxt.top

`共 ${n} 条`
来源：http://cmw.zhoulong.xyz

[U94] JS：箭头函数
来源：http://rfs.jinqigufen.top

const double = x => x * 2;
来源：http://wvo.shanyushiyangkeji.top

[U95] JS：Promise 包装
来源：http://bic.guannengcc.top

new Promise((resolve, reject) => {})
来源：http://fhr.dashuyun.cn

[U96] JS：async/await 与异常
来源：http://ouh.cdnleiting.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://svc.sufxvd.cn

[U97] JS：并发请求
来源：http://dwq.0kj1m.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bmv.vqdsnc.cn

[U98] JS：fetch 带 JSON
来源：http://pit.zhixingplan.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://new.yuanzhike.top

[U99] JS：事件监听
来源：http://ryp.jianghu66.top

el.addEventListener("click", e => {})
来源：http://hoi.fehbvm.com

[U100] JS：DOM 查询
来源：http://auq.jianghu66.top

document.querySelector(".item")
来源：http://gbh.fanxiaobao.xyz

[U101] JS：classList 操作
来源：http://igj.c1oappe.top

el.classList.toggle("active")
来源：http://yji.jianghu66.top

[U102] JS：本地存储
来源：http://npj.jyoumei.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bmt.nanxuanxn.top

[U103] JS：定时器
来源：http://pox.meibo888.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ehv.jinqigfzy.top

[U104] JS：防抖
来源：http://lvw.guannengcc.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bxq.ctjpmb.com

[U105] JS：节流
来源：http://tjf.xinyue.icu

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qps.meibo888.top

[U106] JS：日期格式化
来源：http://gvw.zhijiandao.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ier.daxiang520.top

[U107] JS：数字千分位
来源：http://bxp.hongshengwenyu.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wjg.ybcxt.top

[U108] JS：随机整数
来源：http://qke.jlsjyb.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yyu.jinyuanbaomall.cn

[U109] JS：数组分组
来源：http://unj.pengpengdd.cyou

Object.groupBy(arr, x => x.type)
来源：http://zsl.sufxvd.cn

[U110] JS：数组分块
来源：http://zli.sxryk.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ewv.yuxming.cn

[U111] JS：对象转 Map
来源：http://evr.fanxiaobao.xyz

new Map(Object.entries(obj))
来源：http://mag.gotoacloud.top

[U112] JS：字符串补位
来源：http://niv.zdbjq.cn

"7".padStart(3, "0")
来源：http://tmo.fehbvm.com

[U113] JS：正则替换全部
来源：http://sat.fanxiaobao.xyz

s.replaceAll("a", "b")
来源：http://efo.cheryme.top

[U114] JS：JSON 深比较
来源：http://nwh.birdmap.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://hwj.cheryme.top

[U115] JS：生成 UUID
来源：http://ccu.redwolf501.top

crypto.randomUUID()
来源：http://ksb.yj20258888.top

[U116] JS：类型检查（JSDoc）
来源：http://vys.shzxlz.cn

/** @param {string} name */ function f(name) {}
来源：http://tsp.wangdashe.top

[U117] JS：单元测试
来源：http://uaf.xinyue.icu

npm i -D vitest;  npx vitest
来源：http://zjm.ppjwa.cn

[U118] JS：开发服务器
来源：http://jop.sweek.top

npm i -D vite;  npx vite
来源：http://ibz.tanke756.top

[U119] JS：生产构建
来源：http://evn.jinqigufen.top

npx vite build
来源：http://spc.bjfxy.top

[U120] JS：读取环境变量（Vite）
来源：http://dms.9152youxi.cn

import.meta.env.VITE_API_URL
来源：http://ijq.yanxiufei.cn

================================================================================
来源：http://odz.jinqigfzy.top

统计汇总
来源：http://shf.cucudq.cn

================================================================================
来源：http://fud.c1oappe.top

按语言统计（条）：
来源：http://vxf.zhengqikj.top

Python ......... 252
来源：http://ilv.ywan-chungtsiang.top

PHP ............ 252
来源：http://tyu.shangyingyoupin.top

JavaScript ..... 252
来源：http://cdg.meibo888.top

TypeScript ..... 212
来源：http://exs.smart0.xyz

Java ........... 212
来源：http://sdr.nwbrower.top

Go ............. 212
来源：http://jfv.meibo888.top

Ruby ........... 212
来源：http://iqx.yj20258.top

C# ............. 212
来源：http://pjr.9152youxi.cn

C .............. 30
来源：http://upf.guannengcc.top

C++ ............ 30
来源：http://wnl.nwbrower.top

SQL ............ 90
来源：http://yfw.daria6918.cn

Bash ........... 80
来源：http://oin.shzxlz.cn

Kotlin ......... 15
来源：http://rcz.yj202588.top

Swift .......... 15
来源：http://iqk.yongpay.top

Lua ............ 10
来源：http://irn.zdbjq.cn

Perl ........... 10
来源：http://jft.yuxming.cn

Scala .......... 10
来源：http://cnn.kuanghao11.cn

------------------------------------
来源：http://pzq.yuxming.cn

合计 ........... 2106 条
来源：http://uhw.gogol.net.cn

按章节统计：
来源：http://ikw.kuanghao11.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://iyr.jinghuilouyu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gxq.xziqi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vil.ydzc1.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://syp.ydzc1.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mmf.hfpthk.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fyh.yanxiufei.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ucq.fengsongda.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nvw.sxryk.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jrv.aibaodan.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://prf.0kj1m.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://aom.daria6918.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://naz.mhx1999.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qaq.bjfxy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gtt.tianlin.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mxz.ctjpmb.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lxu.hammf.cn

Q SQL 专题                              90
来源：http://iat.meibo888.top

R Bash 专题                             80
来源：http://hcz.yj202588.top

S C / C++ 专题                          60
来源：http://xjx.yanxiufei.cn

T 其他语言补充                          60
来源：http://cls.aibaodan.cn

U 高频实用片段                         120
来源：http://soc.0kj1m.cn

------------------------------------
来源：http://qvt.sjlbkw.cn

合计                                  2106 条
来源：http://sam.wangdashe.top

--------------------------------------------------------------------------------
来源：http://spb.ybcxt.top

使用提醒
来源：http://svz.jinqigufen.top

--------------------------------------------------------------------------------
来源：http://kle.yangfankeji.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nbs.aibaodan.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jig.xinyue.icu

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://for.ivvv.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ijm.yuxming.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kut.jqgufenzy.top

—— 文件结束 ——
来源：http://jzn.wangshuangyany.cn

================================================================================
来源：http://xxw.chenlongwang.top

程序语言常见例子速查手册（2024 版）
来源：http://jzl.zdbjq.cn

Common Programming Examples Cheat Book
来源：http://sxn.mhx1999.top

================================================================================
来源：http://cgj.wangdashe.top

【收录内容】
来源：http://epd.xuanzx.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://gpl.cheryme.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jwt.yueranfly.top

SQL · Bash · C · C++
来源：http://zot.zdqjudy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hjl.yueranfly.top

【使用说明】
来源：http://lod.shanyushiyangtech.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://dtt.svipenyu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tsh.dashuyun.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://shn.xziqi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bvw.jiagoushi.top

Bash:  Shell         C:     C             C++:   C++
来源：http://ozc.ywan-chungtsiang.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vkk.fehbvm.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kep.hywenlv.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zcp.bbcook.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bik.havefunace.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://uai.pycfn.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vyv.hfpthk.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://lar.yj202588.top

【文件统计】
来源：http://zob.snrcjt.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gym.meibo888.top

--------------------------------------------------------------------------------
来源：http://crt.feifeiyinyue.top

目  录
来源：http://pjw.chenjidiqi.icu

--------------------------------------------------------------------------------
来源：http://ybx.vehdjk.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dyo.sxryk.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gnc.316326.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xlp.yongpay.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xxu.zhiwuduotai.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bcp.pengpengdd.cyou

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://yxh.yuanzhike.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://try.ydjk.org.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://eee.haohaochexian.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xrg.yj20258.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nom.kuanghao11.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fun.chenlongwang.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pnu.jinyuanbaomall.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jjl.tanke756.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://knb.ydzc1.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dsq.shanyushiyangkeji.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://oii.ydjk.org.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jno.andypj.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://vzr.tanke756.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zgs.hesvh.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xhq.yj202588.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://thb.yanxiufei.cn

================================================================================
来源：http://pic.cdnleiting.top

A. 基础语法与类型
来源：http://yyl.ybcxt.top

================================================================================
来源：http://rbb.ppjwa.cn

[A01] Hello World
来源：http://omc.kuanghao11.cn

Py:   print("Hello, World!")
来源：http://hgj.aizwys.cn

PHP:  echo "Hello, World!";
来源：http://dgs.birdmap.top

JS:   console.log("Hello, World!");
来源：http://olt.meibo888.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vnl.zhoulong.xyz

Java: System.out.println("Hello, World!");
来源：http://ddw.bjfxy.top

Go:   fmt.Println("Hello, World!")
来源：http://qes.yangfankeji.com

Ruby: puts "Hello, World!"
来源：http://sjh.ybcxt.top

C#:   Console.WriteLine("Hello, World!");
来源：http://qzz.jinqigfzy.top

[A02] 变量声明与赋值
来源：http://rje.yfazqb.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zno.jinghuilouyu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://hod.hammf.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ptr.yonumen.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nmy.smart0.xyz

Java: String name = "Alex"; int age = 20;
来源：http://pbn.xuanzx.com

Go:   name := "Alex"; age := 20
来源：http://eiz.vehdjk.com

Ruby: name = "Alex"; age = 20
来源：http://zgr.fehbvm.com

C#:   string name = "Alex"; int age = 20;
来源：http://mmu.yongpay.top

[A03] 常量定义
来源：http://sha.zhoulong.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mru.jiagoushi.top

PHP:  const PI = 3.14159;
来源：http://dmy.tianlin.xyz

JS:   const PI = 3.14159;
来源：http://sba.gzhubu.top

TS:   const PI: number = 3.14159;
来源：http://zks.hnqzz.top

Java: static final double PI = 3.14159;
来源：http://ixo.jqgfzy.top

Go:   const PI = 3.14159
来源：http://ocr.vqdsnc.cn

Ruby: PI = 3.14159
来源：http://bwk.yvedp.cn

C#:   const double PI = 3.14159;
来源：http://zmb.shanyushiyangtech.top

[A04] 判断变量类型
来源：http://oec.yuxming.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://gmp.wangdashe.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ibq.fengsongda.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qlm.iojbl.cn

TS:   typeof x; x instanceof Date
来源：http://zsj.hysaishi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wuh.cqqwz.cn

Go:   reflect.TypeOf(x).Name()
来源：http://fnu.gotoacloud.top

Ruby: x.class; x.is_a?(Integer)
来源：http://qkj.chenzaomai.com

C#:   x.GetType().Name; x is int
来源：http://glz.havefunace.top

[A05] 整数除法与取模
来源：http://vze.tarul.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wdg.pengpengdd.cyou

PHP:  intdiv(7, 2); 7 % 2
来源：http://rqr.shanyushiyangkeji.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://evq.epnwcf.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bzs.yfazqb.com

Java: 7 / 2; 7 % 2
来源：http://kxf.aibaodan.cn

Go:   7 / 2; 7 % 2
来源：http://ldq.cashguo.top

Ruby: 7 / 2; 7 % 2
来源：http://rvt.yfazqb.com

C#:   7 / 2; 7 % 2
来源：http://rbx.vqdsnc.cn

[A06] 字符串转数字
来源：http://nfx.iojbl.cn

Py:   int("42"); float("3.14")
来源：http://djh.hesvh.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lfz.zhongyouzk.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://puf.xuanzx.com

TS:   parseInt("42", 10); Number("42")
来源：http://dbk.hnxiangtu.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xpd.wangshuangyany.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://sft.hcnkem.com

Ruby: "42".to_i; "3.14".to_f
来源：http://put.ppjwa.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gdr.jinqigufen.top

[A07] 数字转字符串
来源：http://kci.hammf.cn

Py:   str(42)
来源：http://jxa.snrcjt.cn

PHP:  (string) 42; strval(42)
来源：http://eqs.jlsjyb.cn

JS:   String(42); (42).toString()
来源：http://mon.c1oappe.top

TS:   String(42)
来源：http://zud.gzhubu.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://dpl.dianchejie.cn

Go:   strconv.Itoa(42)
来源：http://tak.daria6918.cn

Ruby: 42.to_s
来源：http://mdt.shuidangran.top

C#:   42.ToString()
来源：http://gmb.wangdashe.top

[A08] 取整与四舍五入
来源：http://pzp.wangshuangyany.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rtl.hysaishi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://nzt.fehbvm.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pps.jqgufenzy.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zpa.chenzaomai.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rny.bjfxy.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ylm.kuanghao11.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://mbl.fanxiaobao.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dkl.pengpengdd.cyou

[A09] 绝对值与最大最小值
来源：http://iah.uphjek.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vff.hfpthk.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ejh.cucudq.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://whv.shuidangran.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://dtn.yuanzhike.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ybo.xinyue.icu

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xpm.hfpthk.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wow.zhaomingkeji.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vkr.chenlongwang.top

[A10] 生成随机数
来源：http://npx.sufxvd.cn

Py:   import random; random.randint(1, 100)
来源：http://fpa.jinghuilouyu.cn

PHP:  random_int(1, 100);
来源：http://fog.hywenlv.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xqm.redwolf501.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://enz.jyoumei.cn

Java: new Random().nextInt(100) + 1
来源：http://dwo.mhx1999.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://sjw.yfazqb.com

Ruby: rand(1..100)
来源：http://dux.guannengcc.top

C#:   new Random().Next(1, 101)
来源：http://ixn.epnwcf.com

[A11] 条件表达式（三元）
来源：http://nwt.yueranfly.top

Py:   "yes" if x > 0 else "no"
来源：http://hmx.xylfe.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://fpj.yongpay.top


<!-- 参考信息 -->