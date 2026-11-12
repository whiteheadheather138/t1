代发 wailian999

[U67] PHP：处理文件上传
来源：http://jrt.birdmap.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://waq.316326.xyz

[U68] PHP：PDO 连接
来源：http://vgm.ybcxt.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mtf.nanxuanxn.top

[U69] PHP：PDO 预处理
来源：http://jyo.9152youxi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pht.nanxinkj.top

[U70] PHP：PDO 事务
来源：http://fgf.yangfankeji.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kgt.pycfn.com

[U71] PHP：抛出异常
来源：http://hio.yfazqb.com

throw new RuntimeException("失败", 500);
来源：http://nmp.hnxiangtu.top

[U72] PHP：写错误日志
来源：http://efr.jinyuanbaomall.cn

error_log("失败: " . $e->getMessage());
来源：http://lea.hammf.cn

[U73] PHP：读取 ini 配置
来源：http://cqo.cucudq.cn

parse_ini_file("config.ini", true)
来源：http://qcj.guowangkeji.top

[U74] PHP：读取环境变量
来源：http://lij.hammf.cn

getenv("APP_ENV") ?: "production"
来源：http://qdu.ivvv.top

[U75] PHP：依赖注入
来源：http://tof.wangshuangyany.cn

composer require psr/container
来源：http://wcd.hongshengwenyu.top

[U76] PHP：简单路由
来源：http://cyj.jyoumei.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rjy.yonumen.top

[U77] PHP：模板渲染
来源：http://hxd.cucudq.cn

composer require twig/twig
来源：http://hfc.kuanghao11.cn

[U78] PHP：单元测试
来源：http://cvj.sxryk.cn

composer require --dev phpunit/phpunit
来源：http://ook.hywenlv.cn

[U79] PHP：静态分析
来源：http://gwr.feifeiyinyue.top

composer require --dev phpstan/phpstan
来源：http://bpc.zhijiandao.cn

[U80] PHP：代码规范修复
来源：http://psg.ydjk.org.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://bqf.wangshuangyany.cn

[U81] JS：初始化项目
来源：http://rrk.pycfn.com

npm init -y;  npm i express
来源：http://mkv.hnqzz.top

[U82] JS：package.json 脚本
来源：http://jej.jiagoushi.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sjf.snrcjt.cn

[U83] JS：ES Module 导入导出
来源：http://vmd.uphjek.com

export const a = 1;  import { a } from "./m.js";
来源：http://ecn.yj202588.top

[U84] JS：CommonJS 写法
来源：http://zxi.ctjpmb.com

module.exports = { a };  const { a } = require("./m");
来源：http://fui.c1oappe.top

[U85] JS：可选链
来源：http://dod.sysykeji.top

a?.b?.c
来源：http://ije.aizwys.cn

[U86] JS：空值合并
来源：http://qfc.jqgfzy.top

a ?? b
来源：http://gsd.mhx1999.top

[U87] JS：解构默认值
来源：http://biu.gaohongyu789.top

const { a = 1, b = 2 } = obj;
来源：http://jqy.yuanzhike.top

[U88] JS：对象展开合并
来源：http://ygr.jinqigufen.top

{ ...a, ...b }
来源：http://qak.aizwys.cn

[U89] JS：数组去重
来源：http://ofc.fktsv.cn

[...new Set(arr)]
来源：http://dux.zhijiandao.cn

[U90] JS：数字数组排序
来源：http://qnv.svipenyu.cn

[...arr].sort((a, b) => a - b)
来源：http://qfj.shzxlz.cn

[U91] JS：对象键值遍历
来源：http://tld.chenzaomai.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pxo.jinqigufen.top

[U92] JS：深拷贝
来源：http://ess.guowangkeji.top

structuredClone(obj)
来源：http://rub.shuidangran.top

[U93] JS：模板字符串
来源：http://dqr.shzxlz.cn

`共 ${n} 条`
来源：http://csy.dianchejie.cn

[U94] JS：箭头函数
来源：http://hre.xziqi.cn

const double = x => x * 2;
来源：http://khi.hnxiangtu.top

[U95] JS：Promise 包装
来源：http://ojq.tianlin.xyz

new Promise((resolve, reject) => {})
来源：http://hzv.haohaochexian.top

[U96] JS：async/await 与异常
来源：http://pfi.xylfe.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zek.gzhubu.top

[U97] JS：并发请求
来源：http://kgs.9152youxi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://otz.hfpthk.cn

[U98] JS：fetch 带 JSON
来源：http://myf.cucudq.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uge.yonumen.top

[U99] JS：事件监听
来源：http://opd.jinyuanbaomall.cn

el.addEventListener("click", e => {})
来源：http://yol.zhiwuduotai.top

[U100] JS：DOM 查询
来源：http://khq.kuanghao11.cn

document.querySelector(".item")
来源：http://sro.fehbvm.com

[U101] JS：classList 操作
来源：http://ane.0kj1m.cn

el.classList.toggle("active")
来源：http://vly.nwbrower.top

[U102] JS：本地存储
来源：http://oyo.fanxiaobao.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://qud.ehwqpu.com

[U103] JS：定时器
来源：http://rtm.xylfe.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wds.hnxiangtu.top

[U104] JS：防抖
来源：http://kyq.ivvv.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ibv.uphjek.com

[U105] JS：节流
来源：http://ddu.cheryme.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pea.chenlongwang.top

[U106] JS：日期格式化
来源：http://art.bjfxy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mll.cashguo.top

[U107] JS：数字千分位
来源：http://mpv.hcnkem.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vmw.zhoulong.xyz

[U108] JS：随机整数
来源：http://nnc.yvedp.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kxl.cqqwz.cn

[U109] JS：数组分组
来源：http://yvv.svipenyu.cn

Object.groupBy(arr, x => x.type)
来源：http://eqr.hammf.cn

[U110] JS：数组分块
来源：http://cru.zhijiandao.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jas.shanyushiyangkeji.top

[U111] JS：对象转 Map
来源：http://srq.daxiang520.top

new Map(Object.entries(obj))
来源：http://tng.kuanghao11.cn

[U112] JS：字符串补位
来源：http://iwa.gzhubu.top

"7".padStart(3, "0")
来源：http://vfp.ivvv.top

[U113] JS：正则替换全部
来源：http://lkn.guannengcc.top

s.replaceAll("a", "b")
来源：http://wsn.yueranfly.top

[U114] JS：JSON 深比较
来源：http://ywa.yfazqb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://qin.sufxvd.cn

[U115] JS：生成 UUID
来源：http://pfx.ppjwa.cn

crypto.randomUUID()
来源：http://ism.9152youxi.cn

[U116] JS：类型检查（JSDoc）
来源：http://ggq.zdbjq.cn

/** @param {string} name */ function f(name) {}
来源：http://lqu.ydjk.org.cn

[U117] JS：单元测试
来源：http://ggw.hcnkem.com

npm i -D vitest;  npx vitest
来源：http://gqo.shuidangran.top

[U118] JS：开发服务器
来源：http://cnl.chenjidiqi.icu

npm i -D vite;  npx vite
来源：http://kvk.jqgufenzy.top

[U119] JS：生产构建
来源：http://wdc.yongpay.top

npx vite build
来源：http://dlq.xylfe.cn

[U120] JS：读取环境变量（Vite）
来源：http://bcu.zdbjq.cn

import.meta.env.VITE_API_URL
来源：http://rhp.kuanghao11.cn

================================================================================
来源：http://dvh.jinghuilouyu.cn

统计汇总
来源：http://ygt.xziqi.cn

================================================================================
来源：http://nqd.sweek.top

按语言统计（条）：
来源：http://dhp.xuetiantiany.cn

Python ......... 252
来源：http://blx.pengpengdd.cyou

PHP ............ 252
来源：http://gpx.ivvv.top

JavaScript ..... 252
来源：http://bmh.bjfxy.top

TypeScript ..... 212
来源：http://glq.mhx1999.top

Java ........... 212
来源：http://ovp.vehdjk.com

Go ............. 212
来源：http://cqv.kuanghao11.cn

Ruby ........... 212
来源：http://stb.yfazqb.com

C# ............. 212
来源：http://lgu.hongshengwenyu.top

C .............. 30
来源：http://tmk.zycfv.cn

C++ ............ 30
来源：http://mvu.yongpay.top

SQL ............ 90
来源：http://cra.316326.xyz

Bash ........... 80
来源：http://sno.jinghuilouyu.cn

Kotlin ......... 15
来源：http://llm.ctjpmb.com

Swift .......... 15
来源：http://idl.dianchejie.cn

Lua ............ 10
来源：http://lod.jianghu66.top

Perl ........... 10
来源：http://itn.guannengcc.top

Scala .......... 10
来源：http://zmx.chenzaomai.com

------------------------------------
来源：http://upm.quarkkingdee.top

合计 ........... 2106 条
来源：http://gse.shzxlz.cn

按章节统计：
来源：http://xeq.guowangkeji.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vfz.zhoulong.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lnv.yangfankeji.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ert.hesvh.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://npg.yj20258.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lmc.316326.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wxe.cheryme.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nke.zhengqikj.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zpf.xingfuxueyuan.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mzn.yongpay.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jim.quarkkingdee.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zar.yanxiufei.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lum.xylfe.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kgu.guowangkeji.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ryf.yj202588.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pir.hnqzz.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yga.9152youxi.cn

Q SQL 专题                              90
来源：http://foa.yongpay.top

R Bash 专题                             80
来源：http://fvq.birdmap.top

S C / C++ 专题                          60
来源：http://mlt.52xcode.cn

T 其他语言补充                          60
来源：http://wnh.daria6918.cn

U 高频实用片段                         120
来源：http://uaz.tianlin.xyz

------------------------------------
来源：http://teq.shanyushiyangtech.top

合计                                  2106 条
来源：http://plh.iojbl.cn

--------------------------------------------------------------------------------
来源：http://qpn.tian-w.cn

使用提醒
来源：http://egx.andypj.xyz

--------------------------------------------------------------------------------
来源：http://umc.daxiang520.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jdi.ctjpmb.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kiy.yuanzhike.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zfp.ctjpmb.com

在旧版本上使用前请先确认语法支持情况。
来源：http://wqj.nanxinkj.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ujm.wangdashe.top

—— 文件结束 ——
来源：http://kdi.aizwys.cn

================================================================================
来源：http://wku.hcnkem.com

程序语言常见例子速查手册（2024 版）
来源：http://rbq.ybcxt.top

Common Programming Examples Cheat Book
来源：http://kyq.jinghuilouyu.cn

================================================================================
来源：http://dyh.0kj1m.cn

【收录内容】
来源：http://qqo.ehwqpu.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://sgl.hywenlv.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://asa.hysaishi.cn

SQL · Bash · C · C++
来源：http://nnk.haohaochexian.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jng.fanxiaobao.xyz

【使用说明】
来源：http://nff.yuanzhike.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jgf.hammf.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mdl.zdbjq.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://efj.tian-w.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qlz.pengpengdd.cyou

Bash:  Shell         C:     C             C++:   C++
来源：http://ttv.52xcode.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lmr.tarul.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vbw.yuxming.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ejq.cheryme.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ugh.zhongyouzk.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://shl.gogol.net.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://trg.nanxuanxn.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://btc.sufxvd.cn

【文件统计】
来源：http://nhp.feifeiyinyue.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ziv.zdqjudy.top

--------------------------------------------------------------------------------
来源：http://brv.shanyushiyangtech.top

目  录
来源：http://mvk.yuxming.cn

--------------------------------------------------------------------------------
来源：http://mqd.ppjwa.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vml.andypj.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jhb.jianghu66.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wok.uphjek.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mey.gogol.net.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jnw.yongpay.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hcg.ppjwa.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vdv.cdnleiting.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vtp.yuxming.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://guj.chenlongwang.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wjm.gaohongyu789.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gdg.daria6918.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bpz.tanke756.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gth.gogol.net.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kfu.meibo888.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pnk.yuxming.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dxc.zhijiandao.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zxn.guannengcc.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://kqg.jlsjyb.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hzu.wangshuangyany.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rqy.xuanzx.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mpp.iojbl.cn

================================================================================
来源：http://kas.yj20258.top

A. 基础语法与类型
来源：http://yfn.yangfankeji.com

================================================================================
来源：http://jjb.cucudq.cn

[A01] Hello World
来源：http://jnu.feifeiyinyue.top

Py:   print("Hello, World!")
来源：http://btx.pycfn.com

PHP:  echo "Hello, World!";
来源：http://xec.hnqzz.top

JS:   console.log("Hello, World!");
来源：http://yyx.guannengcc.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gwm.nanxuanxn.top

Java: System.out.println("Hello, World!");
来源：http://ife.yangfankeji.com

Go:   fmt.Println("Hello, World!")
来源：http://cba.jinqigufen.top

Ruby: puts "Hello, World!"
来源：http://bcj.zhaomingkeji.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://ijo.pengpengdd.cyou

[A02] 变量声明与赋值
来源：http://adq.dashuyun.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ttw.ywan-chungtsiang.top

PHP:  $name = "Alex"; $age = 20;
来源：http://gdd.birdmap.top

JS:   let name = "Alex"; const age = 20;
来源：http://wpy.shzxlz.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://tne.gotoacloud.top

Java: String name = "Alex"; int age = 20;
来源：http://tjc.andypj.xyz

Go:   name := "Alex"; age := 20
来源：http://zjf.chenjidiqi.icu

Ruby: name = "Alex"; age = 20
来源：http://vqx.chenzaomai.com

C#:   string name = "Alex"; int age = 20;
来源：http://bwl.zhiwuduotai.top

[A03] 常量定义
来源：http://mda.jinyuanbaomall.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vxg.dianchejie.cn

PHP:  const PI = 3.14159;
来源：http://joh.xuanzx.com

JS:   const PI = 3.14159;
来源：http://kyl.nanxuanxn.top

TS:   const PI: number = 3.14159;
来源：http://gzv.jiagoushi.top

Java: static final double PI = 3.14159;
来源：http://fck.xuanzx.com

Go:   const PI = 3.14159
来源：http://fxc.shanyushiyangtech.top

Ruby: PI = 3.14159
来源：http://ada.zhixingplan.top

C#:   const double PI = 3.14159;
来源：http://xzz.ywan-chungtsiang.top

[A04] 判断变量类型
来源：http://plx.aizwys.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://yxa.dianchejie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vum.tarul.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://anp.svipenyu.cn

TS:   typeof x; x instanceof Date
来源：http://zcn.yj202588.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mpe.yuanzhike.top

Go:   reflect.TypeOf(x).Name()
来源：http://vwh.pycfn.com

Ruby: x.class; x.is_a?(Integer)
来源：http://lnx.yonumen.top

C#:   x.GetType().Name; x is int
来源：http://zkr.feifeiyinyue.top

[A05] 整数除法与取模
来源：http://swy.birdmap.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gqs.ydzc1.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://bxa.dashuyun.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nst.52xcode.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://icx.gaohongyu789.top

Java: 7 / 2; 7 % 2
来源：http://gsy.daria6918.cn

Go:   7 / 2; 7 % 2
来源：http://xew.nwbrower.top

Ruby: 7 / 2; 7 % 2
来源：http://sod.cucudq.cn

C#:   7 / 2; 7 % 2
来源：http://drw.shzxlz.cn

[A06] 字符串转数字
来源：http://kmu.zhixingplan.top

Py:   int("42"); float("3.14")
来源：http://qso.gogol.net.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://olk.gzhubu.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://enr.cheryme.top

TS:   parseInt("42", 10); Number("42")
来源：http://klm.hysaishi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wlw.fengsongda.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://elx.havefunace.top

Ruby: "42".to_i; "3.14".to_f
来源：http://dfm.yanxiufei.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vvm.jiagoushi.top

[A07] 数字转字符串
来源：http://dde.uphjek.com

Py:   str(42)
来源：http://kgc.zdbjq.cn

PHP:  (string) 42; strval(42)
来源：http://ibb.xuanzx.com

JS:   String(42); (42).toString()
来源：http://wfr.jinghuilouyu.cn

TS:   String(42)
来源：http://yub.shangyingyoupin.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://vte.ybcxt.top

Go:   strconv.Itoa(42)
来源：http://coy.ppjwa.cn

Ruby: 42.to_s
来源：http://phy.yuanzhike.top

C#:   42.ToString()
来源：http://lqz.fzhhl.top

[A08] 取整与四舍五入
来源：http://dsx.yonumen.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wml.zhijiandao.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ocd.svipenyu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pzt.yueranfly.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qei.zdqjudy.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dwl.cashguo.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xko.zhaomingkeji.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://vme.wangshuangyany.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ntv.9152youxi.cn

[A09] 绝对值与最大最小值
来源：http://fnh.wangshuangyany.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xzc.yuanzhike.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://uww.yueranfly.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://nhb.ybcxt.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nqe.yongpay.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://cky.aibaodan.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ehy.zhaomingkeji.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qhn.hnqzz.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rff.yongpay.top

[A10] 生成随机数
来源：http://anf.uphjek.com

Py:   import random; random.randint(1, 100)
来源：http://zdw.shanyushiyangkeji.top

PHP:  random_int(1, 100);
来源：http://pws.chenzaomai.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ybi.vehdjk.com


<!-- 参考信息 -->