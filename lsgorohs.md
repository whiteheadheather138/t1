代发 wailian999

[U67] PHP：处理文件上传
来源：http://goi.xuanzx.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qyf.nanxuanxn.top

[U68] PHP：PDO 连接
来源：http://hck.meibo888.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ozw.ppjwa.cn

[U69] PHP：PDO 预处理
来源：http://qqq.chenjidiqi.icu

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://avm.zhengqikj.top

[U70] PHP：PDO 事务
来源：http://dhu.cashguo.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://oxo.cucudq.cn

[U71] PHP：抛出异常
来源：http://mbp.hammf.cn

throw new RuntimeException("失败", 500);
来源：http://pkx.shanyushiyangtech.top

[U72] PHP：写错误日志
来源：http://iqo.hnxiangtu.top

error_log("失败: " . $e->getMessage());
来源：http://hwa.wangshuangyany.cn

[U73] PHP：读取 ini 配置
来源：http://jwo.gogol.net.cn

parse_ini_file("config.ini", true)
来源：http://zlg.0kj1m.cn

[U74] PHP：读取环境变量
来源：http://grk.gzhubu.top

getenv("APP_ENV") ?: "production"
来源：http://tau.dianchejie.cn

[U75] PHP：依赖注入
来源：http://bci.meibo888.top

composer require psr/container
来源：http://xeo.daxiang520.top

[U76] PHP：简单路由
来源：http://pqc.xylfe.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jmu.hongshengwenyu.top

[U77] PHP：模板渲染
来源：http://xmt.feifeiyinyue.top

composer require twig/twig
来源：http://cqo.shuidangran.top

[U78] PHP：单元测试
来源：http://rle.yuanzhike.top

composer require --dev phpunit/phpunit
来源：http://ckg.yongpay.top

[U79] PHP：静态分析
来源：http://hop.yongpay.top

composer require --dev phpstan/phpstan
来源：http://mza.shangyingyoupin.top

[U80] PHP：代码规范修复
来源：http://tle.birdmap.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://dbb.jinqigufen.top

[U81] JS：初始化项目
来源：http://jxp.yueranfly.top

npm init -y;  npm i express
来源：http://igy.nanxinkj.top

[U82] JS：package.json 脚本
来源：http://htm.tarul.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://iie.chenzaomai.com

[U83] JS：ES Module 导入导出
来源：http://nst.andypj.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://ydn.sufxvd.cn

[U84] JS：CommonJS 写法
来源：http://ldg.ydzc1.top

module.exports = { a };  const { a } = require("./m");
来源：http://tbd.cdnleiting.top

[U85] JS：可选链
来源：http://jua.tarul.cn

a?.b?.c
来源：http://fct.shanyushiyangkeji.top

[U86] JS：空值合并
来源：http://svc.sweek.top

a ?? b
来源：http://rsc.ydzc1.top

[U87] JS：解构默认值
来源：http://wbg.52xcode.cn

const { a = 1, b = 2 } = obj;
来源：http://xjn.vehdjk.com

[U88] JS：对象展开合并
来源：http://ufa.ydjk.org.cn

{ ...a, ...b }
来源：http://sfl.yueranfly.top

[U89] JS：数组去重
来源：http://blf.hnqzz.top

[...new Set(arr)]
来源：http://woe.meibo888.top

[U90] JS：数字数组排序
来源：http://cvp.jinqigfzy.top

[...arr].sort((a, b) => a - b)
来源：http://ocr.chenlongwang.top

[U91] JS：对象键值遍历
来源：http://vrl.gaohongyu789.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vlo.yvedp.cn

[U92] JS：深拷贝
来源：http://ldu.kuanghao11.cn

structuredClone(obj)
来源：http://fbc.c1oappe.top

[U93] JS：模板字符串
来源：http://jlc.cashguo.top

`共 ${n} 条`
来源：http://gte.nanxuanxn.top

[U94] JS：箭头函数
来源：http://piu.zhijiandao.cn

const double = x => x * 2;
来源：http://msr.316326.xyz

[U95] JS：Promise 包装
来源：http://vdo.aibaodan.cn

new Promise((resolve, reject) => {})
来源：http://vvv.ehwqpu.com

[U96] JS：async/await 与异常
来源：http://ifx.ywan-chungtsiang.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fsx.wangdashe.top

[U97] JS：并发请求
来源：http://vab.ehwqpu.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://lzi.sxryk.cn

[U98] JS：fetch 带 JSON
来源：http://deh.xylfe.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ytd.zycfv.cn

[U99] JS：事件监听
来源：http://eun.zhixingplan.top

el.addEventListener("click", e => {})
来源：http://pvw.yueranfly.top

[U100] JS：DOM 查询
来源：http://wvn.xingfuxueyuan.xyz

document.querySelector(".item")
来源：http://mwz.pycfn.com

[U101] JS：classList 操作
来源：http://iyr.bjfxy.top

el.classList.toggle("active")
来源：http://hoy.shanyushiyangkeji.top

[U102] JS：本地存储
来源：http://lxk.yonumen.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://knn.hnqzz.top

[U103] JS：定时器
来源：http://lgh.ppjwa.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xrr.pycfn.com

[U104] JS：防抖
来源：http://yzl.zhiwuduotai.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ycf.sxryk.cn

[U105] JS：节流
来源：http://keb.hammf.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://krf.yuxming.cn

[U106] JS：日期格式化
来源：http://mac.yonumen.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://whl.sjlbkw.cn

[U107] JS：数字千分位
来源：http://kab.sufxvd.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://oti.sufxvd.cn

[U108] JS：随机整数
来源：http://pmb.9152youxi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vjp.redwolf501.top

[U109] JS：数组分组
来源：http://gfi.ehwqpu.com

Object.groupBy(arr, x => x.type)
来源：http://cqo.ivvv.top

[U110] JS：数组分块
来源：http://isp.jinqigfzy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zsn.xziqi.cn

[U111] JS：对象转 Map
来源：http://dop.jinqigufen.top

new Map(Object.entries(obj))
来源：http://dkd.tianlin.xyz

[U112] JS：字符串补位
来源：http://unu.vehdjk.com

"7".padStart(3, "0")
来源：http://idu.aibaodan.cn

[U113] JS：正则替换全部
来源：http://vyg.cheryme.top

s.replaceAll("a", "b")
来源：http://bdu.pengpengdd.cyou

[U114] JS：JSON 深比较
来源：http://bdy.wangdashe.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://tte.chenzaomai.com

[U115] JS：生成 UUID
来源：http://krc.fzhhl.top

crypto.randomUUID()
来源：http://xmr.cdnleiting.top

[U116] JS：类型检查（JSDoc）
来源：http://wqu.hfpthk.cn

/** @param {string} name */ function f(name) {}
来源：http://lsl.hnxiangtu.top

[U117] JS：单元测试
来源：http://vbx.zhijiandao.cn

npm i -D vitest;  npx vitest
来源：http://yhw.xylfe.cn

[U118] JS：开发服务器
来源：http://yvk.jiagoushi.top

npm i -D vite;  npx vite
来源：http://wgw.chenzaomai.com

[U119] JS：生产构建
来源：http://pwp.hywenlv.cn

npx vite build
来源：http://smn.ywan-chungtsiang.top

[U120] JS：读取环境变量（Vite）
来源：http://pbe.kuanghao11.cn

import.meta.env.VITE_API_URL
来源：http://hiw.cdnleiting.top

================================================================================
来源：http://ull.yvedp.cn

统计汇总
来源：http://ihm.sysykeji.top

================================================================================
来源：http://pvd.tanke756.top

按语言统计（条）：
来源：http://ctd.wangdashe.top

Python ......... 252
来源：http://jll.zhixingplan.top

PHP ............ 252
来源：http://yze.hnxiangtu.top

JavaScript ..... 252
来源：http://gyv.sxryk.cn

TypeScript ..... 212
来源：http://vjs.hfpthk.cn

Java ........... 212
来源：http://aeh.iojbl.cn

Go ............. 212
来源：http://lig.pengpengdd.cyou

Ruby ........... 212
来源：http://ghe.dashuyun.cn

C# ............. 212
来源：http://gnn.yj202588.top

C .............. 30
来源：http://yqs.fanxiaobao.xyz

C++ ............ 30
来源：http://mrb.nanxinkj.top

SQL ............ 90
来源：http://nvs.nwbrower.top

Bash ........... 80
来源：http://yqh.nanxuanxn.top

Kotlin ......... 15
来源：http://avx.tian-w.cn

Swift .......... 15
来源：http://mio.zhengqikj.top

Lua ............ 10
来源：http://qmo.hcnkem.com

Perl ........... 10
来源：http://fep.yonumen.top

Scala .......... 10
来源：http://gmb.xinyue.icu

------------------------------------
来源：http://soc.epnwcf.com

合计 ........... 2106 条
来源：http://mvv.gotoacloud.top

按章节统计：
来源：http://knj.fanxiaobao.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lej.yuxming.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zsg.ctjpmb.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rck.gogol.net.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://svj.bbcook.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://oms.yj202588.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nal.zycfv.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://znz.xuanzx.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lez.xingfuxueyuan.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xkj.jiagoushi.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ubw.hywenlv.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dyi.yangfankeji.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nqx.mhx1999.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zbv.sxryk.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bfc.ydzc1.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dxp.fehbvm.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ibq.wangdashe.top

Q SQL 专题                              90
来源：http://lyl.cdnleiting.top

R Bash 专题                             80
来源：http://oph.ybcxt.top

S C / C++ 专题                          60
来源：http://atq.yj20258888.top

T 其他语言补充                          60
来源：http://ejj.yongpay.top

U 高频实用片段                         120
来源：http://pdf.guannengcc.top

------------------------------------
来源：http://cak.ywan-chungtsiang.top

合计                                  2106 条
来源：http://xik.pycfn.com

--------------------------------------------------------------------------------
来源：http://xwh.jinqigfzy.top

使用提醒
来源：http://qow.jyoumei.cn

--------------------------------------------------------------------------------
来源：http://zey.xylfe.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pfa.316326.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cxt.yangfankeji.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://klp.tian-w.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://dsj.jinghuilouyu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zpn.dashuyun.cn

—— 文件结束 ——
来源：http://vpk.sjlbkw.cn

================================================================================
来源：http://hbj.zhengqikj.top

程序语言常见例子速查手册（2024 版）
来源：http://fxj.shuidangran.top

Common Programming Examples Cheat Book
来源：http://rut.jiagoushi.top

================================================================================
来源：http://pmb.xylfe.cn

【收录内容】
来源：http://tlo.hcnkem.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://vkk.tanke756.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rfq.0kj1m.cn

SQL · Bash · C · C++
来源：http://nli.iojbl.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ytn.guannengcc.top

【使用说明】
来源：http://dvd.hysaishi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hgi.sufxvd.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hqo.sufxvd.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fkq.jqgufenzy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vpv.yj20258888.top

Bash:  Shell         C:     C             C++:   C++
来源：http://uwx.xziqi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lmo.zhijiandao.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://chi.52xcode.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xqe.zhijiandao.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ngq.jiagoushi.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://sky.yangfankeji.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pgc.birdmap.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://out.316326.xyz

【文件统计】
来源：http://pjn.xinyue.icu

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dah.guowangkeji.top

--------------------------------------------------------------------------------
来源：http://byc.xingfuxueyuan.xyz

目  录
来源：http://ble.shuidangran.top

--------------------------------------------------------------------------------
来源：http://zqx.pengpengdd.cyou

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mum.cashguo.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lkl.jiagoushi.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rxg.yj20258.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fhh.bbcook.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ezr.sweek.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vhr.smart0.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vno.jlsjyb.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vbv.jinghuilouyu.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://sxw.shangyingyoupin.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hqn.hnqzz.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://upf.quarkkingdee.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ywt.pengpengdd.cyou

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://aqw.mhx1999.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yai.iojbl.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ozf.kuanghao11.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fnf.dashuyun.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jhg.zhijiandao.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wlh.ppjwa.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bhk.iojbl.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://emd.hysaishi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dxh.wangshuangyany.cn

================================================================================
来源：http://ulw.cheryme.top

A. 基础语法与类型
来源：http://ott.svipenyu.cn

================================================================================
来源：http://xfx.guowangkeji.top

[A01] Hello World
来源：http://hml.ybcxt.top

Py:   print("Hello, World!")
来源：http://yrh.sysykeji.top

PHP:  echo "Hello, World!";
来源：http://oso.yueranfly.top

JS:   console.log("Hello, World!");
来源：http://ejf.hfpthk.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ida.xziqi.cn

Java: System.out.println("Hello, World!");
来源：http://tox.pengpengdd.cyou

Go:   fmt.Println("Hello, World!")
来源：http://qnf.haohaochexian.top

Ruby: puts "Hello, World!"
来源：http://eqd.zhixingplan.top

C#:   Console.WriteLine("Hello, World!");
来源：http://hzn.yueranfly.top

[A02] 变量声明与赋值
来源：http://ybm.zdqjudy.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wfv.aizwys.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://dtj.iojbl.cn

JS:   let name = "Alex"; const age = 20;
来源：http://wft.jqgfzy.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dvk.zhoulong.xyz

Java: String name = "Alex"; int age = 20;
来源：http://zex.zdbjq.cn

Go:   name := "Alex"; age := 20
来源：http://rji.guowangkeji.top

Ruby: name = "Alex"; age = 20
来源：http://jyu.shanyushiyangtech.top

C#:   string name = "Alex"; int age = 20;
来源：http://kld.shanyushiyangkeji.top

[A03] 常量定义
来源：http://lvt.yuxming.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ovx.hywenlv.cn

PHP:  const PI = 3.14159;
来源：http://ijw.nanxuanxn.top

JS:   const PI = 3.14159;
来源：http://vos.bjfxy.top

TS:   const PI: number = 3.14159;
来源：http://eyb.xuanzx.com

Java: static final double PI = 3.14159;
来源：http://esf.hnqzz.top

Go:   const PI = 3.14159
来源：http://fwh.hesvh.cn

Ruby: PI = 3.14159
来源：http://igv.ctjpmb.com

C#:   const double PI = 3.14159;
来源：http://wsq.guannengcc.top

[A04] 判断变量类型
来源：http://tpx.nwbrower.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://vqo.c1oappe.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xwz.gotoacloud.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vsl.cucudq.cn

TS:   typeof x; x instanceof Date
来源：http://esg.yfazqb.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://yql.pycfn.com

Go:   reflect.TypeOf(x).Name()
来源：http://hyj.redwolf501.top

Ruby: x.class; x.is_a?(Integer)
来源：http://nhi.ctjpmb.com

C#:   x.GetType().Name; x is int
来源：http://swc.hywenlv.cn

[A05] 整数除法与取模
来源：http://lhp.yj202588.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://urt.shanyushiyangkeji.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ugo.yanxiufei.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jki.quarkkingdee.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://nhh.cheryme.top

Java: 7 / 2; 7 % 2
来源：http://flv.zhiwuduotai.top

Go:   7 / 2; 7 % 2
来源：http://ktk.gaohongyu789.top

Ruby: 7 / 2; 7 % 2
来源：http://nle.xingfuxueyuan.xyz

C#:   7 / 2; 7 % 2
来源：http://vel.jqgufenzy.top

[A06] 字符串转数字
来源：http://mph.jinqigfzy.top

Py:   int("42"); float("3.14")
来源：http://itg.daxiang520.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kwk.52xcode.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tbi.cdnleiting.top

TS:   parseInt("42", 10); Number("42")
来源：http://wmf.chenlongwang.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kka.jqgufenzy.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pva.vqdsnc.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://dql.hywenlv.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ean.dashuyun.cn

[A07] 数字转字符串
来源：http://tgf.jyoumei.cn

Py:   str(42)
来源：http://xml.nanxinkj.top

PHP:  (string) 42; strval(42)
来源：http://enb.nanxinkj.top

JS:   String(42); (42).toString()
来源：http://htb.xuanzx.com

TS:   String(42)
来源：http://oww.shanyushiyangtech.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://yxl.shangyingyoupin.top

Go:   strconv.Itoa(42)
来源：http://dyt.jianghu66.top

Ruby: 42.to_s
来源：http://iox.ivvv.top

C#:   42.ToString()
来源：http://tqh.tanke756.top

[A08] 取整与四舍五入
来源：http://ypf.chenlongwang.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rkm.ppjwa.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qet.xylfe.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://oqv.jqgufenzy.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rzv.c1oappe.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zmr.hywenlv.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nig.pengpengdd.cyou

Ruby: 3.567.round(2); 3.9.floor
来源：http://syz.gogol.net.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tis.mhx1999.top

[A09] 绝对值与最大最小值
来源：http://zga.uphjek.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ozf.hammf.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://nnj.zdbjq.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rfx.zhiwuduotai.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qmy.gogol.net.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ebq.ctjpmb.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://whi.epnwcf.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ffg.ehwqpu.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jlk.nanxinkj.top

[A10] 生成随机数
来源：http://fjp.cdnleiting.top

Py:   import random; random.randint(1, 100)
来源：http://tzg.nwbrower.top

PHP:  random_int(1, 100);
来源：http://gpw.xuetiantiany.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fzn.pycfn.com


<!-- 参考信息 -->