代发 wailian999

[U69] PHP：PDO 预处理
来源：http://ymj.yj202588.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://szy.316326.xyz

[U70] PHP：PDO 事务
来源：http://uto.snrcjt.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hfx.xylfe.cn

[U71] PHP：抛出异常
来源：http://pfg.ydzc1.top

throw new RuntimeException("失败", 500);
来源：http://uhf.guannengcc.top

[U72] PHP：写错误日志
来源：http://sop.shzxlz.cn

error_log("失败: " . $e->getMessage());
来源：http://oix.yj202588.top

[U73] PHP：读取 ini 配置
来源：http://wer.chenzaomai.com

parse_ini_file("config.ini", true)
来源：http://vof.jyoumei.cn

[U74] PHP：读取环境变量
来源：http://soj.hnqzz.top

getenv("APP_ENV") ?: "production"
来源：http://aim.xuetiantiany.cn

[U75] PHP：依赖注入
来源：http://xbl.zhixingplan.top

composer require psr/container
来源：http://qar.guowangkeji.top

[U76] PHP：简单路由
来源：http://ovq.shuidangran.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bcx.yueranfly.top

[U77] PHP：模板渲染
来源：http://wcb.svipenyu.cn

composer require twig/twig
来源：http://ujh.pycfn.com

[U78] PHP：单元测试
来源：http://dpl.xylfe.cn

composer require --dev phpunit/phpunit
来源：http://oxr.jqgufenzy.top

[U79] PHP：静态分析
来源：http://bpr.daria6918.cn

composer require --dev phpstan/phpstan
来源：http://igo.ydjk.org.cn

[U80] PHP：代码规范修复
来源：http://tcl.zhaomingkeji.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://mlp.bbcook.cn

[U81] JS：初始化项目
来源：http://rbu.guowangkeji.top

npm init -y;  npm i express
来源：http://efz.bbcook.cn

[U82] JS：package.json 脚本
来源：http://vpn.shuidangran.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wvc.mhx1999.top

[U83] JS：ES Module 导入导出
来源：http://ypj.dashuyun.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vhe.zhengqikj.top

[U84] JS：CommonJS 写法
来源：http://omx.hnxiangtu.top

module.exports = { a };  const { a } = require("./m");
来源：http://pok.nanxinkj.top

[U85] JS：可选链
来源：http://xyt.bbcook.cn

a?.b?.c
来源：http://dhx.yvedp.cn

[U86] JS：空值合并
来源：http://lmo.chenzaomai.com

a ?? b
来源：http://jgl.pycfn.com

[U87] JS：解构默认值
来源：http://mxk.hnqzz.top

const { a = 1, b = 2 } = obj;
来源：http://sfu.dianchejie.cn

[U88] JS：对象展开合并
来源：http://vdg.bbcook.cn

{ ...a, ...b }
来源：http://gpq.tianlin.xyz

[U89] JS：数组去重
来源：http://blt.zhijiandao.cn

[...new Set(arr)]
来源：http://tcf.zdqjudy.top

[U90] JS：数字数组排序
来源：http://ghn.fzhhl.top

[...arr].sort((a, b) => a - b)
来源：http://vxb.zhijiandao.cn

[U91] JS：对象键值遍历
来源：http://rpw.ywan-chungtsiang.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kus.ppjwa.cn

[U92] JS：深拷贝
来源：http://cgn.shanyushiyangtech.top

structuredClone(obj)
来源：http://cbu.zhongyouzk.top

[U93] JS：模板字符串
来源：http://nvx.feifeiyinyue.top

`共 ${n} 条`
来源：http://pfx.ppjwa.cn

[U94] JS：箭头函数
来源：http://eqy.xylfe.cn

const double = x => x * 2;
来源：http://dmo.cheryme.top

[U95] JS：Promise 包装
来源：http://fmo.gaohongyu789.top

new Promise((resolve, reject) => {})
来源：http://vma.fengsongda.top

[U96] JS：async/await 与异常
来源：http://cng.xuanzx.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cha.yj20258888.top

[U97] JS：并发请求
来源：http://aox.sysykeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://iub.hcnkem.com

[U98] JS：fetch 带 JSON
来源：http://ghe.zhongyouzk.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cxy.jqgfzy.top

[U99] JS：事件监听
来源：http://dkf.sweek.top

el.addEventListener("click", e => {})
来源：http://sqw.tarul.cn

[U100] JS：DOM 查询
来源：http://mix.hfpthk.cn

document.querySelector(".item")
来源：http://iso.cheryme.top

[U101] JS：classList 操作
来源：http://pon.gotoacloud.top

el.classList.toggle("active")
来源：http://vwj.ydjk.org.cn

[U102] JS：本地存储
来源：http://ove.xuetiantiany.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://mxm.snrcjt.cn

[U103] JS：定时器
来源：http://wqu.daria6918.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wmx.yuxming.cn

[U104] JS：防抖
来源：http://kja.tianlin.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rpk.gogol.net.cn

[U105] JS：节流
来源：http://rtg.chenjidiqi.icu

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bvp.shuidangran.top

[U106] JS：日期格式化
来源：http://isg.tanke756.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xdm.yueranfly.top

[U107] JS：数字千分位
来源：http://pqa.smart0.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nbg.ppjwa.cn

[U108] JS：随机整数
来源：http://oub.zhixingplan.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tyj.svipenyu.cn

[U109] JS：数组分组
来源：http://rbu.sysykeji.top

Object.groupBy(arr, x => x.type)
来源：http://xsq.vehdjk.com

[U110] JS：数组分块
来源：http://tcr.sufxvd.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jtb.gaohongyu789.top

[U111] JS：对象转 Map
来源：http://ehb.wangshuangyany.cn

new Map(Object.entries(obj))
来源：http://ejx.jqgufenzy.top

[U112] JS：字符串补位
来源：http://sdd.yuanzhike.top

"7".padStart(3, "0")
来源：http://hqj.ivvv.top

[U113] JS：正则替换全部
来源：http://dtj.kuanghao11.cn

s.replaceAll("a", "b")
来源：http://zoc.jinghuilouyu.cn

[U114] JS：JSON 深比较
来源：http://vbv.yuanzhike.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://arj.shanyushiyangtech.top

[U115] JS：生成 UUID
来源：http://nyr.hesvh.cn

crypto.randomUUID()
来源：http://bgb.316326.xyz

[U116] JS：类型检查（JSDoc）
来源：http://vtm.zhaomingkeji.xyz

/** @param {string} name */ function f(name) {}
来源：http://ytl.yongpay.top

[U117] JS：单元测试
来源：http://pis.zhongyouzk.top

npm i -D vitest;  npx vitest
来源：http://hzi.jiagoushi.top

[U118] JS：开发服务器
来源：http://iof.yuxming.cn

npm i -D vite;  npx vite
来源：http://esl.fzhhl.top

[U119] JS：生产构建
来源：http://otn.xingfuxueyuan.xyz

npx vite build
来源：http://dnm.quarkkingdee.top

[U120] JS：读取环境变量（Vite）
来源：http://qii.hysaishi.cn

import.meta.env.VITE_API_URL
来源：http://wwf.xziqi.cn

================================================================================
来源：http://poe.cashguo.top

统计汇总
来源：http://kbl.jqgfzy.top

================================================================================
来源：http://pcr.yonumen.top

按语言统计（条）：
来源：http://fer.guowangkeji.top

Python ......... 252
来源：http://mzb.andypj.xyz

PHP ............ 252
来源：http://bll.ydjk.org.cn

JavaScript ..... 252
来源：http://dzy.nanxuanxn.top

TypeScript ..... 212
来源：http://qig.sjlbkw.cn

Java ........... 212
来源：http://hst.iojbl.cn

Go ............. 212
来源：http://lvi.zhijiandao.cn

Ruby ........... 212
来源：http://suy.uphjek.com

C# ............. 212
来源：http://tlr.hongshengwenyu.top

C .............. 30
来源：http://hsc.yj20258888.top

C++ ............ 30
来源：http://bcl.dianchejie.cn

SQL ............ 90
来源：http://lnl.jinghuilouyu.cn

Bash ........... 80
来源：http://kvw.fanxiaobao.xyz

Kotlin ......... 15
来源：http://pco.ivvv.top

Swift .......... 15
来源：http://etv.fehbvm.com

Lua ............ 10
来源：http://xqm.xylfe.cn

Perl ........... 10
来源：http://ild.dianchejie.cn

Scala .......... 10
来源：http://sjo.xylfe.cn

------------------------------------
来源：http://acg.yj202588.top

合计 ........... 2106 条
来源：http://fju.zhongyouzk.top

按章节统计：
来源：http://fhi.epnwcf.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cfe.zhoulong.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dba.jianghu66.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gzw.yanxiufei.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dpl.hywenlv.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yzz.c1oappe.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nie.nanxuanxn.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ivf.ywan-chungtsiang.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hka.zhaomingkeji.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fzk.fengsongda.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ypu.xziqi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rvt.xylfe.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qhn.ivvv.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zre.fehbvm.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://nui.feifeiyinyue.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qxi.shanyushiyangtech.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tuv.nwbrower.top

Q SQL 专题                              90
来源：http://mvi.ivvv.top

R Bash 专题                             80
来源：http://zad.chenzaomai.com

S C / C++ 专题                          60
来源：http://kfk.aibaodan.cn

T 其他语言补充                          60
来源：http://dbv.0kj1m.cn

U 高频实用片段                         120
来源：http://xzz.smart0.xyz

------------------------------------
来源：http://ihw.redwolf501.top

合计                                  2106 条
来源：http://etg.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://pkl.cqqwz.cn

使用提醒
来源：http://iyi.yongpay.top

--------------------------------------------------------------------------------
来源：http://izr.gogol.net.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fuw.havefunace.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hmx.fehbvm.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://cdc.iojbl.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://von.hcnkem.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bwf.chenzaomai.com

—— 文件结束 ——
来源：http://chy.hnqzz.top

================================================================================
来源：http://ahq.sweek.top

程序语言常见例子速查手册（2024 版）
来源：http://kck.zhiwuduotai.top

Common Programming Examples Cheat Book
来源：http://dtd.ydzc1.top

================================================================================
来源：http://kih.9152youxi.cn

【收录内容】
来源：http://kcc.ybcxt.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://bne.tanke756.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qvr.tanke756.top

SQL · Bash · C · C++
来源：http://rcm.9152youxi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hbk.shanyushiyangkeji.top

【使用说明】
来源：http://xyj.hesvh.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pwe.xingfuxueyuan.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wrb.zdqjudy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mdx.vqdsnc.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qxx.kuanghao11.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://axe.xziqi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://cfm.wangdashe.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kss.tianlin.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://sgo.shuidangran.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xga.fktsv.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nno.ppjwa.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jiv.aibaodan.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gre.aibaodan.cn

【文件统计】
来源：http://jfz.havefunace.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rzg.yongpay.top

--------------------------------------------------------------------------------
来源：http://kpg.yj20258888.top

目  录
来源：http://thj.guannengcc.top

--------------------------------------------------------------------------------
来源：http://gzq.bbcook.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ihe.daxiang520.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gqu.chenjidiqi.icu

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jhn.pengpengdd.cyou

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://nmi.zdbjq.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://muv.cdnleiting.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zyh.zhaomingkeji.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nsm.hesvh.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qdj.zhiwuduotai.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lux.jinyuanbaomall.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rjy.cucudq.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xah.kuanghao11.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://opv.hcnkem.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://oqo.meibo888.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jsz.bbcook.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ydp.fktsv.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jvb.zhixingplan.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://urp.chenjidiqi.icu

R. Bash 专题                   （第 18 节，80 条）
来源：http://nmf.xinyue.icu

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jba.yueranfly.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://plf.ehwqpu.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yvl.fzhhl.top

================================================================================
来源：http://zei.yanxiufei.cn

A. 基础语法与类型
来源：http://adv.ivvv.top

================================================================================
来源：http://cda.birdmap.top

[A01] Hello World
来源：http://iib.xuetiantiany.cn

Py:   print("Hello, World!")
来源：http://xim.jinqigfzy.top

PHP:  echo "Hello, World!";
来源：http://oai.hcnkem.com

JS:   console.log("Hello, World!");
来源：http://ymy.yfazqb.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://puj.yonumen.top

Java: System.out.println("Hello, World!");
来源：http://jux.birdmap.top

Go:   fmt.Println("Hello, World!")
来源：http://mra.havefunace.top

Ruby: puts "Hello, World!"
来源：http://nly.hnqzz.top

C#:   Console.WriteLine("Hello, World!");
来源：http://dix.gotoacloud.top

[A02] 变量声明与赋值
来源：http://waj.quarkkingdee.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://utm.jyoumei.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://cax.cashguo.top

JS:   let name = "Alex"; const age = 20;
来源：http://vrz.chenzaomai.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://esp.cdnleiting.top

Java: String name = "Alex"; int age = 20;
来源：http://ajj.ydjk.org.cn

Go:   name := "Alex"; age := 20
来源：http://cdz.bjfxy.top

Ruby: name = "Alex"; age = 20
来源：http://iek.fengsongda.top

C#:   string name = "Alex"; int age = 20;
来源：http://qfd.bjfxy.top

[A03] 常量定义
来源：http://iql.smart0.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bpt.gotoacloud.top

PHP:  const PI = 3.14159;
来源：http://fnn.gotoacloud.top

JS:   const PI = 3.14159;
来源：http://ocg.jinyuanbaomall.cn

TS:   const PI: number = 3.14159;
来源：http://csi.chenjidiqi.icu

Java: static final double PI = 3.14159;
来源：http://yxj.guannengcc.top

Go:   const PI = 3.14159
来源：http://umu.zhaomingkeji.xyz

Ruby: PI = 3.14159
来源：http://nfa.meibo888.top

C#:   const double PI = 3.14159;
来源：http://ufh.fengsongda.top

[A04] 判断变量类型
来源：http://viz.pycfn.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://kdz.hesvh.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hdy.chenjidiqi.icu

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rjt.daxiang520.top

TS:   typeof x; x instanceof Date
来源：http://ofj.jinghuilouyu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mtz.gaohongyu789.top

Go:   reflect.TypeOf(x).Name()
来源：http://tgz.hesvh.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://erl.vqdsnc.cn

C#:   x.GetType().Name; x is int
来源：http://tym.ybcxt.top

[A05] 整数除法与取模
来源：http://kpb.c1oappe.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wfi.svipenyu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://uic.shanyushiyangtech.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zlx.jyoumei.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://iwa.ydjk.org.cn

Java: 7 / 2; 7 % 2
来源：http://pjx.andypj.xyz

Go:   7 / 2; 7 % 2
来源：http://gcy.jianghu66.top

Ruby: 7 / 2; 7 % 2
来源：http://jeg.cucudq.cn

C#:   7 / 2; 7 % 2
来源：http://qbl.zhongyouzk.top

[A06] 字符串转数字
来源：http://ewk.meibo888.top

Py:   int("42"); float("3.14")
来源：http://kck.zhaomingkeji.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://shq.cucudq.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ctu.cashguo.top

TS:   parseInt("42", 10); Number("42")
来源：http://hne.shanyushiyangtech.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zrt.yj202588.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wzi.cashguo.top

Ruby: "42".to_i; "3.14".to_f
来源：http://dnv.0kj1m.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hgg.chenjidiqi.icu

[A07] 数字转字符串
来源：http://vju.zdbjq.cn

Py:   str(42)
来源：http://rhv.jyoumei.cn

PHP:  (string) 42; strval(42)
来源：http://nlc.jinqigfzy.top

JS:   String(42); (42).toString()
来源：http://evb.xuetiantiany.cn

TS:   String(42)
来源：http://yxz.zhoulong.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://oet.nanxuanxn.top

Go:   strconv.Itoa(42)
来源：http://bxe.shangyingyoupin.top

Ruby: 42.to_s
来源：http://qmo.316326.xyz

C#:   42.ToString()
来源：http://amr.sjlbkw.cn

[A08] 取整与四舍五入
来源：http://aax.jianghu66.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yhg.zhengqikj.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kvl.wangdashe.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://oug.redwolf501.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://pmn.yongpay.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://iyf.tian-w.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://inf.fanxiaobao.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://fmn.shanyushiyangkeji.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://nax.hfpthk.cn

[A09] 绝对值与最大最小值
来源：http://rfk.zhengqikj.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jxq.zdbjq.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qyc.wangshuangyany.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://acl.0kj1m.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vok.gaohongyu789.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://oyh.andypj.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://eli.tarul.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://urq.daria6918.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pna.guowangkeji.top

[A10] 生成随机数
来源：http://jvc.aizwys.cn

Py:   import random; random.randint(1, 100)
来源：http://fjx.xuanzx.com

PHP:  random_int(1, 100);
来源：http://mtc.havefunace.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://crf.fehbvm.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://soc.gotoacloud.top

Java: new Random().nextInt(100) + 1
来源：http://gat.birdmap.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dpb.cashguo.top

Ruby: rand(1..100)
来源：http://jlg.zhoulong.xyz


<!-- 参考信息 -->