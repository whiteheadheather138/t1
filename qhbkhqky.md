代发 wailian999

[U69] PHP：PDO 预处理
来源：http://vso.andypj.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jed.aizwys.cn

[U70] PHP：PDO 事务
来源：http://uyv.shzxlz.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rjc.gogol.net.cn

[U71] PHP：抛出异常
来源：http://oyo.cheryme.top

throw new RuntimeException("失败", 500);
来源：http://eyr.tanke756.top

[U72] PHP：写错误日志
来源：http://wux.shanyushiyangkeji.top

error_log("失败: " . $e->getMessage());
来源：http://cpu.fzhhl.top

[U73] PHP：读取 ini 配置
来源：http://clq.sysykeji.top

parse_ini_file("config.ini", true)
来源：http://oiu.jinyuanbaomall.cn

[U74] PHP：读取环境变量
来源：http://iuh.xuanzx.com

getenv("APP_ENV") ?: "production"
来源：http://uid.feifeiyinyue.top

[U75] PHP：依赖注入
来源：http://gvy.nanxinkj.top

composer require psr/container
来源：http://icf.uphjek.com

[U76] PHP：简单路由
来源：http://fiw.xziqi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bzs.yfazqb.com

[U77] PHP：模板渲染
来源：http://lqi.yanxiufei.cn

composer require twig/twig
来源：http://itu.yvedp.cn

[U78] PHP：单元测试
来源：http://jka.xziqi.cn

composer require --dev phpunit/phpunit
来源：http://dag.zhiwuduotai.top

[U79] PHP：静态分析
来源：http://kfm.yonumen.top

composer require --dev phpstan/phpstan
来源：http://wwi.zhixingplan.top

[U80] PHP：代码规范修复
来源：http://bpm.xinyue.icu

composer require --dev friendsofphp/php-cs-fixer
来源：http://pgy.smart0.xyz

[U81] JS：初始化项目
来源：http://bym.wangshuangyany.cn

npm init -y;  npm i express
来源：http://wue.yongpay.top

[U82] JS：package.json 脚本
来源：http://lxr.yuanzhike.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mtj.hammf.cn

[U83] JS：ES Module 导入导出
来源：http://usu.fktsv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://eps.chenjidiqi.icu

[U84] JS：CommonJS 写法
来源：http://rto.sufxvd.cn

module.exports = { a };  const { a } = require("./m");
来源：http://adh.feifeiyinyue.top

[U85] JS：可选链
来源：http://lqz.zhaomingkeji.xyz

a?.b?.c
来源：http://udi.hysaishi.cn

[U86] JS：空值合并
来源：http://jrm.zdbjq.cn

a ?? b
来源：http://owo.yanxiufei.cn

[U87] JS：解构默认值
来源：http://sff.ywan-chungtsiang.top

const { a = 1, b = 2 } = obj;
来源：http://zne.xuanzx.com

[U88] JS：对象展开合并
来源：http://elb.yongpay.top

{ ...a, ...b }
来源：http://jht.redwolf501.top

[U89] JS：数组去重
来源：http://brm.jlsjyb.cn

[...new Set(arr)]
来源：http://azx.chenjidiqi.icu

[U90] JS：数字数组排序
来源：http://qoh.andypj.xyz

[...arr].sort((a, b) => a - b)
来源：http://whm.0kj1m.cn

[U91] JS：对象键值遍历
来源：http://umr.snrcjt.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://csg.hysaishi.cn

[U92] JS：深拷贝
来源：http://kkt.jqgfzy.top

structuredClone(obj)
来源：http://aeq.52xcode.cn

[U93] JS：模板字符串
来源：http://xhe.zdbjq.cn

`共 ${n} 条`
来源：http://erg.gzhubu.top

[U94] JS：箭头函数
来源：http://veu.fzhhl.top

const double = x => x * 2;
来源：http://fdh.tanke756.top

[U95] JS：Promise 包装
来源：http://vsp.hywenlv.cn

new Promise((resolve, reject) => {})
来源：http://zsb.havefunace.top

[U96] JS：async/await 与异常
来源：http://dvr.nanxinkj.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ksm.svipenyu.cn

[U97] JS：并发请求
来源：http://rfb.yvedp.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://wqf.yj20258.top

[U98] JS：fetch 带 JSON
来源：http://aoh.hesvh.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jia.aibaodan.cn

[U99] JS：事件监听
来源：http://dxc.quarkkingdee.top

el.addEventListener("click", e => {})
来源：http://wox.kuanghao11.cn

[U100] JS：DOM 查询
来源：http://jgx.guowangkeji.top

document.querySelector(".item")
来源：http://uct.hnxiangtu.top

[U101] JS：classList 操作
来源：http://cbf.jyoumei.cn

el.classList.toggle("active")
来源：http://cpl.tian-w.cn

[U102] JS：本地存储
来源：http://yfn.meibo888.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://crz.aibaodan.cn

[U103] JS：定时器
来源：http://ajm.yfazqb.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ose.gotoacloud.top

[U104] JS：防抖
来源：http://tbk.zhijiandao.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xir.haohaochexian.top

[U105] JS：节流
来源：http://jem.gzhubu.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wfu.guannengcc.top

[U106] JS：日期格式化
来源：http://uct.xylfe.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xko.yj20258.top

[U107] JS：数字千分位
来源：http://yyy.tianlin.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qqu.smart0.xyz

[U108] JS：随机整数
来源：http://xks.snrcjt.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://poq.shanyushiyangkeji.top

[U109] JS：数组分组
来源：http://mqo.wangdashe.top

Object.groupBy(arr, x => x.type)
来源：http://pyi.andypj.xyz

[U110] JS：数组分块
来源：http://zet.yfazqb.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cdj.zycfv.cn

[U111] JS：对象转 Map
来源：http://qfd.svipenyu.cn

new Map(Object.entries(obj))
来源：http://jie.jiagoushi.top

[U112] JS：字符串补位
来源：http://gzk.zhongyouzk.top

"7".padStart(3, "0")
来源：http://qht.jinyuanbaomall.cn

[U113] JS：正则替换全部
来源：http://hws.yuxming.cn

s.replaceAll("a", "b")
来源：http://ksq.zhiwuduotai.top

[U114] JS：JSON 深比较
来源：http://ymc.fehbvm.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://rol.tian-w.cn

[U115] JS：生成 UUID
来源：http://jig.jianghu66.top

crypto.randomUUID()
来源：http://qnd.gzhubu.top

[U116] JS：类型检查（JSDoc）
来源：http://hab.yj20258.top

/** @param {string} name */ function f(name) {}
来源：http://dip.cheryme.top

[U117] JS：单元测试
来源：http://dpi.shangyingyoupin.top

npm i -D vitest;  npx vitest
来源：http://zqs.ctjpmb.com

[U118] JS：开发服务器
来源：http://fwg.wangshuangyany.cn

npm i -D vite;  npx vite
来源：http://mhn.yangfankeji.com

[U119] JS：生产构建
来源：http://uel.xziqi.cn

npx vite build
来源：http://tdk.yfazqb.com

[U120] JS：读取环境变量（Vite）
来源：http://cun.chenlongwang.top

import.meta.env.VITE_API_URL
来源：http://aar.yueranfly.top

================================================================================
来源：http://xwc.kuanghao11.cn

统计汇总
来源：http://twh.pengpengdd.cyou

================================================================================
来源：http://drc.jyoumei.cn

按语言统计（条）：
来源：http://dop.ehwqpu.com

Python ......... 252
来源：http://bkn.snrcjt.cn

PHP ............ 252
来源：http://pmq.hcnkem.com

JavaScript ..... 252
来源：http://qln.hesvh.cn

TypeScript ..... 212
来源：http://erq.aizwys.cn

Java ........... 212
来源：http://wqh.dashuyun.cn

Go ............. 212
来源：http://fpk.shzxlz.cn

Ruby ........... 212
来源：http://wec.shzxlz.cn

C# ............. 212
来源：http://fbp.c1oappe.top

C .............. 30
来源：http://cos.wangshuangyany.cn

C++ ............ 30
来源：http://plf.jinqigfzy.top

SQL ............ 90
来源：http://afd.guannengcc.top

Bash ........... 80
来源：http://cts.nanxuanxn.top

Kotlin ......... 15
来源：http://iie.sysykeji.top

Swift .......... 15
来源：http://fac.zhaomingkeji.xyz

Lua ............ 10
来源：http://yfl.smart0.xyz

Perl ........... 10
来源：http://qia.zhaomingkeji.xyz

Scala .......... 10
来源：http://nsv.zhijiandao.cn

------------------------------------
来源：http://lck.snrcjt.cn

合计 ........... 2106 条
来源：http://mjg.gotoacloud.top

按章节统计：
来源：http://nyg.nanxinkj.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ivt.guowangkeji.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://elt.fktsv.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gyh.316326.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ghi.gotoacloud.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gib.zhongyouzk.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rqb.yangfankeji.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xln.daxiang520.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://udb.jiagoushi.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nei.chenjidiqi.icu

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hkz.jlsjyb.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lkw.zhongyouzk.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qhg.bjfxy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://etq.havefunace.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://alh.xuetiantiany.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gkm.yuanzhike.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tkt.vqdsnc.cn

Q SQL 专题                              90
来源：http://sru.haohaochexian.top

R Bash 专题                             80
来源：http://aih.316326.xyz

S C / C++ 专题                          60
来源：http://zzw.feifeiyinyue.top

T 其他语言补充                          60
来源：http://siv.smart0.xyz

U 高频实用片段                         120
来源：http://isv.yvedp.cn

------------------------------------
来源：http://tbk.ivvv.top

合计                                  2106 条
来源：http://kjf.meibo888.top

--------------------------------------------------------------------------------
来源：http://ouo.fengsongda.top

使用提醒
来源：http://ltr.yj20258.top

--------------------------------------------------------------------------------
来源：http://suc.fanxiaobao.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wcl.fehbvm.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mxd.feifeiyinyue.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mmb.fanxiaobao.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://bhc.yuxming.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ckq.yanxiufei.cn

—— 文件结束 ——
来源：http://qnm.vqdsnc.cn

================================================================================
来源：http://ess.xuetiantiany.cn

程序语言常见例子速查手册（2024 版）
来源：http://sni.yj20258888.top

Common Programming Examples Cheat Book
来源：http://tjw.gogol.net.cn

================================================================================
来源：http://snp.hammf.cn

【收录内容】
来源：http://tku.bjfxy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ubi.yj20258.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dpy.iojbl.cn

SQL · Bash · C · C++
来源：http://myt.chenlongwang.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wqx.gzhubu.top

【使用说明】
来源：http://jya.yonumen.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tqf.jianghu66.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://shu.uphjek.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://eqd.jinghuilouyu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gxc.hammf.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://srp.hnqzz.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xfx.cashguo.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://pdm.nwbrower.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lwk.316326.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fmg.shanyushiyangtech.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lqg.jiagoushi.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://oss.shangyingyoupin.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qzs.zdqjudy.top

【文件统计】
来源：http://lba.yonumen.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vqa.gzhubu.top

--------------------------------------------------------------------------------
来源：http://gqv.daria6918.cn

目  录
来源：http://dtq.yj20258888.top

--------------------------------------------------------------------------------
来源：http://nog.ctjpmb.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pnz.ivvv.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://vnm.yj202588.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kla.chenjidiqi.icu

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://onl.yj20258.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://udo.52xcode.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pnc.hongshengwenyu.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hbi.wangdashe.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nyn.birdmap.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hva.shangyingyoupin.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jub.ivvv.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fna.vehdjk.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qcd.smart0.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wcf.redwolf501.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://phd.cashguo.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://apd.cashguo.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dnx.ivvv.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gnc.vehdjk.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://gah.aibaodan.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://kev.hysaishi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://asv.yj20258888.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://koo.jinghuilouyu.cn

================================================================================
来源：http://ksv.redwolf501.top

A. 基础语法与类型
来源：http://yrw.ybcxt.top

================================================================================
来源：http://hzw.bbcook.cn

[A01] Hello World
来源：http://wnm.yj20258.top

Py:   print("Hello, World!")
来源：http://vmp.quarkkingdee.top

PHP:  echo "Hello, World!";
来源：http://bzh.jiagoushi.top

JS:   console.log("Hello, World!");
来源：http://gbs.fanxiaobao.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://brd.tarul.cn

Java: System.out.println("Hello, World!");
来源：http://abs.gaohongyu789.top

Go:   fmt.Println("Hello, World!")
来源：http://jjx.daxiang520.top

Ruby: puts "Hello, World!"
来源：http://dtr.yuxming.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://lar.chenjidiqi.icu

[A02] 变量声明与赋值
来源：http://czj.zycfv.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wbv.guowangkeji.top

PHP:  $name = "Alex"; $age = 20;
来源：http://cge.zhongyouzk.top

JS:   let name = "Alex"; const age = 20;
来源：http://myh.feifeiyinyue.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://tba.sxryk.cn

Java: String name = "Alex"; int age = 20;
来源：http://ejd.wangdashe.top

Go:   name := "Alex"; age := 20
来源：http://mbj.hongshengwenyu.top

Ruby: name = "Alex"; age = 20
来源：http://vtx.gaohongyu789.top

C#:   string name = "Alex"; int age = 20;
来源：http://xfi.xinyue.icu

[A03] 常量定义
来源：http://qit.gotoacloud.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ezq.tanke756.top

PHP:  const PI = 3.14159;
来源：http://fug.fehbvm.com

JS:   const PI = 3.14159;
来源：http://tmj.cashguo.top

TS:   const PI: number = 3.14159;
来源：http://fxv.guannengcc.top

Java: static final double PI = 3.14159;
来源：http://str.iojbl.cn

Go:   const PI = 3.14159
来源：http://csv.yanxiufei.cn

Ruby: PI = 3.14159
来源：http://gra.jinyuanbaomall.cn

C#:   const double PI = 3.14159;
来源：http://yns.yangfankeji.com

[A04] 判断变量类型
来源：http://yfm.xylfe.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://klm.yonumen.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://oem.hammf.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://owh.cheryme.top

TS:   typeof x; x instanceof Date
来源：http://mia.hesvh.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://psd.meibo888.top

Go:   reflect.TypeOf(x).Name()
来源：http://tag.pengpengdd.cyou

Ruby: x.class; x.is_a?(Integer)
来源：http://dyv.cashguo.top

C#:   x.GetType().Name; x is int
来源：http://jxx.cqqwz.cn

[A05] 整数除法与取模
来源：http://uzk.zdbjq.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hwt.sufxvd.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://xhk.shanyushiyangkeji.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qro.xingfuxueyuan.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://dya.yonumen.top

Java: 7 / 2; 7 % 2
来源：http://hjp.quarkkingdee.top

Go:   7 / 2; 7 % 2
来源：http://usj.xingfuxueyuan.xyz

Ruby: 7 / 2; 7 % 2
来源：http://yhb.shuidangran.top

C#:   7 / 2; 7 % 2
来源：http://nva.yj20258888.top

[A06] 字符串转数字
来源：http://lju.smart0.xyz

Py:   int("42"); float("3.14")
来源：http://veh.fktsv.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ffn.yuanzhike.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://yry.fehbvm.com

TS:   parseInt("42", 10); Number("42")
来源：http://kxp.svipenyu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ulw.jinyuanbaomall.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xxh.ehwqpu.com

Ruby: "42".to_i; "3.14".to_f
来源：http://oha.yuxming.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rgt.yvedp.cn

[A07] 数字转字符串
来源：http://wzq.kuanghao11.cn

Py:   str(42)
来源：http://spr.zdqjudy.top

PHP:  (string) 42; strval(42)
来源：http://bdx.tarul.cn

JS:   String(42); (42).toString()
来源：http://cmo.xziqi.cn

TS:   String(42)
来源：http://tjy.zhengqikj.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://wfd.ehwqpu.com

Go:   strconv.Itoa(42)
来源：http://hym.jlsjyb.cn

Ruby: 42.to_s
来源：http://xos.jqgfzy.top

C#:   42.ToString()
来源：http://npt.pycfn.com

[A08] 取整与四舍五入
来源：http://lyi.zdbjq.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ihb.gzhubu.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rtt.yangfankeji.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tyc.fanxiaobao.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://opf.hcnkem.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dfv.yangfankeji.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baq.zhixingplan.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ehs.zhoulong.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wdx.yvedp.cn

[A09] 绝对值与最大最小值
来源：http://mnf.hywenlv.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://egx.sxryk.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hpl.hywenlv.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qtn.yj20258.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://clx.wangdashe.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://inp.shangyingyoupin.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://owv.vehdjk.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://clk.feifeiyinyue.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wsh.jlsjyb.cn

[A10] 生成随机数
来源：http://nmp.yvedp.cn

Py:   import random; random.randint(1, 100)
来源：http://yzp.epnwcf.com

PHP:  random_int(1, 100);
来源：http://moy.mhx1999.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ucy.hesvh.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://deb.wangdashe.top

Java: new Random().nextInt(100) + 1
来源：http://nfj.mhx1999.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://msy.aizwys.cn

Ruby: rand(1..100)
来源：http://jad.zhaomingkeji.xyz


<!-- 参考信息 -->