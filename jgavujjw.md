代发 wailian999

[U67] PHP：处理文件上传
来源：http://hif.pycfn.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://roi.jyoumei.cn

[U68] PHP：PDO 连接
来源：http://xce.dianchejie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wql.bjfxy.top

[U69] PHP：PDO 预处理
来源：http://tmg.hammf.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wux.jqgfzy.top

[U70] PHP：PDO 事务
来源：http://hva.pengpengdd.cyou

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wcf.shangyingyoupin.top

[U71] PHP：抛出异常
来源：http://grb.chenjidiqi.icu

throw new RuntimeException("失败", 500);
来源：http://zut.yvedp.cn

[U72] PHP：写错误日志
来源：http://frd.yuxming.cn

error_log("失败: " . $e->getMessage());
来源：http://dss.jlsjyb.cn

[U73] PHP：读取 ini 配置
来源：http://ehu.shangyingyoupin.top

parse_ini_file("config.ini", true)
来源：http://qlo.ehwqpu.com

[U74] PHP：读取环境变量
来源：http://wnr.shangyingyoupin.top

getenv("APP_ENV") ?: "production"
来源：http://lbf.fzhhl.top

[U75] PHP：依赖注入
来源：http://obp.mhx1999.top

composer require psr/container
来源：http://ypw.shangyingyoupin.top

[U76] PHP：简单路由
来源：http://izg.hysaishi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://whu.feifeiyinyue.top

[U77] PHP：模板渲染
来源：http://jgn.zdbjq.cn

composer require twig/twig
来源：http://owy.yj202588.top

[U78] PHP：单元测试
来源：http://sjz.iojbl.cn

composer require --dev phpunit/phpunit
来源：http://ylo.cqqwz.cn

[U79] PHP：静态分析
来源：http://ubl.hywenlv.cn

composer require --dev phpstan/phpstan
来源：http://diq.yuxming.cn

[U80] PHP：代码规范修复
来源：http://joy.birdmap.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://gtt.hysaishi.cn

[U81] JS：初始化项目
来源：http://ljc.snrcjt.cn

npm init -y;  npm i express
来源：http://fyk.chenlongwang.top

[U82] JS：package.json 脚本
来源：http://clt.jiagoushi.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bba.sweek.top

[U83] JS：ES Module 导入导出
来源：http://omv.cashguo.top

export const a = 1;  import { a } from "./m.js";
来源：http://yyd.xuanzx.com

[U84] JS：CommonJS 写法
来源：http://phs.jiagoushi.top

module.exports = { a };  const { a } = require("./m");
来源：http://geh.uphjek.com

[U85] JS：可选链
来源：http://bac.xinyue.icu

a?.b?.c
来源：http://fqq.feifeiyinyue.top

[U86] JS：空值合并
来源：http://oui.nanxinkj.top

a ?? b
来源：http://fca.yj20258.top

[U87] JS：解构默认值
来源：http://fll.sweek.top

const { a = 1, b = 2 } = obj;
来源：http://hgp.dianchejie.cn

[U88] JS：对象展开合并
来源：http://vkx.ivvv.top

{ ...a, ...b }
来源：http://hia.316326.xyz

[U89] JS：数组去重
来源：http://esl.jqgfzy.top

[...new Set(arr)]
来源：http://orl.hnxiangtu.top

[U90] JS：数字数组排序
来源：http://ene.hysaishi.cn

[...arr].sort((a, b) => a - b)
来源：http://xkb.iojbl.cn

[U91] JS：对象键值遍历
来源：http://lgq.daxiang520.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qjg.ctjpmb.com

[U92] JS：深拷贝
来源：http://siy.c1oappe.top

structuredClone(obj)
来源：http://rsr.fktsv.cn

[U93] JS：模板字符串
来源：http://vva.jinqigufen.top

`共 ${n} 条`
来源：http://wno.cashguo.top

[U94] JS：箭头函数
来源：http://xeo.hysaishi.cn

const double = x => x * 2;
来源：http://jql.birdmap.top

[U95] JS：Promise 包装
来源：http://ftv.chenjidiqi.icu

new Promise((resolve, reject) => {})
来源：http://bxn.tanke756.top

[U96] JS：async/await 与异常
来源：http://ire.0kj1m.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ves.pengpengdd.cyou

[U97] JS：并发请求
来源：http://nuh.sufxvd.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vez.ywan-chungtsiang.top

[U98] JS：fetch 带 JSON
来源：http://iqo.c1oappe.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ncs.jiagoushi.top

[U99] JS：事件监听
来源：http://yxt.aizwys.cn

el.addEventListener("click", e => {})
来源：http://fnm.wangdashe.top

[U100] JS：DOM 查询
来源：http://jhm.shangyingyoupin.top

document.querySelector(".item")
来源：http://cpy.zdbjq.cn

[U101] JS：classList 操作
来源：http://uuq.fehbvm.com

el.classList.toggle("active")
来源：http://mty.ydzc1.top

[U102] JS：本地存储
来源：http://akl.fehbvm.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://vze.redwolf501.top

[U103] JS：定时器
来源：http://lmi.jinyuanbaomall.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hvl.jinqigufen.top

[U104] JS：防抖
来源：http://kmr.xylfe.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nrl.dashuyun.cn

[U105] JS：节流
来源：http://tzw.yj20258888.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hfp.gotoacloud.top

[U106] JS：日期格式化
来源：http://uho.vehdjk.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://uky.jyoumei.cn

[U107] JS：数字千分位
来源：http://xze.wangdashe.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vmn.jlsjyb.cn

[U108] JS：随机整数
来源：http://tto.chenzaomai.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fbx.xylfe.cn

[U109] JS：数组分组
来源：http://day.cdnleiting.top

Object.groupBy(arr, x => x.type)
来源：http://dho.vqdsnc.cn

[U110] JS：数组分块
来源：http://asf.sweek.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yxh.ybcxt.top

[U111] JS：对象转 Map
来源：http://zlc.fzhhl.top

new Map(Object.entries(obj))
来源：http://ylx.shanyushiyangkeji.top

[U112] JS：字符串补位
来源：http://dcd.zhijiandao.cn

"7".padStart(3, "0")
来源：http://rod.uphjek.com

[U113] JS：正则替换全部
来源：http://lsv.0kj1m.cn

s.replaceAll("a", "b")
来源：http://ada.ydzc1.top

[U114] JS：JSON 深比较
来源：http://odc.daxiang520.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://urx.gotoacloud.top

[U115] JS：生成 UUID
来源：http://hte.zdqjudy.top

crypto.randomUUID()
来源：http://bcd.fanxiaobao.xyz

[U116] JS：类型检查（JSDoc）
来源：http://vjf.xylfe.cn

/** @param {string} name */ function f(name) {}
来源：http://ryn.hammf.cn

[U117] JS：单元测试
来源：http://fuz.sufxvd.cn

npm i -D vitest;  npx vitest
来源：http://btk.gogol.net.cn

[U118] JS：开发服务器
来源：http://tcb.daxiang520.top

npm i -D vite;  npx vite
来源：http://fao.svipenyu.cn

[U119] JS：生产构建
来源：http://dhk.dashuyun.cn

npx vite build
来源：http://mcf.sjlbkw.cn

[U120] JS：读取环境变量（Vite）
来源：http://oxs.xuetiantiany.cn

import.meta.env.VITE_API_URL
来源：http://nqt.feifeiyinyue.top

================================================================================
来源：http://xol.mhx1999.top

统计汇总
来源：http://vmz.fanxiaobao.xyz

================================================================================
来源：http://cbv.cheryme.top

按语言统计（条）：
来源：http://gim.c1oappe.top

Python ......... 252
来源：http://jcv.yongpay.top

PHP ............ 252
来源：http://wbh.daria6918.cn

JavaScript ..... 252
来源：http://icz.ydzc1.top

TypeScript ..... 212
来源：http://pvi.hywenlv.cn

Java ........... 212
来源：http://rdt.fehbvm.com

Go ............. 212
来源：http://gwr.ctjpmb.com

Ruby ........... 212
来源：http://fjn.sufxvd.cn

C# ............. 212
来源：http://hvu.jinqigufen.top

C .............. 30
来源：http://dbb.snrcjt.cn

C++ ............ 30
来源：http://goq.iojbl.cn

SQL ............ 90
来源：http://pjq.meibo888.top

Bash ........... 80
来源：http://zok.aizwys.cn

Kotlin ......... 15
来源：http://ajy.ivvv.top

Swift .......... 15
来源：http://dad.jiagoushi.top

Lua ............ 10
来源：http://lds.c1oappe.top

Perl ........... 10
来源：http://sxo.ppjwa.cn

Scala .......... 10
来源：http://ncn.jinyuanbaomall.cn

------------------------------------
来源：http://rmt.cucudq.cn

合计 ........... 2106 条
来源：http://vru.hnqzz.top

按章节统计：
来源：http://tmq.nwbrower.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zen.hammf.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://njz.jqgfzy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://obj.shuidangran.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hps.fehbvm.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://azh.kuanghao11.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tax.smart0.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vcu.chenzaomai.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://syg.zhixingplan.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ife.feifeiyinyue.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pzr.quarkkingdee.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://uvz.cheryme.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://npu.ydjk.org.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hzq.jinqigufen.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vme.smart0.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tnl.zhiwuduotai.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yev.dianchejie.cn

Q SQL 专题                              90
来源：http://noo.jqgfzy.top

R Bash 专题                             80
来源：http://iur.snrcjt.cn

S C / C++ 专题                          60
来源：http://aaq.mhx1999.top

T 其他语言补充                          60
来源：http://twi.xinyue.icu

U 高频实用片段                         120
来源：http://esd.zhengqikj.top

------------------------------------
来源：http://edd.zycfv.cn

合计                                  2106 条
来源：http://uqb.yuxming.cn

--------------------------------------------------------------------------------
来源：http://wis.hammf.cn

使用提醒
来源：http://aap.ivvv.top

--------------------------------------------------------------------------------
来源：http://sff.tian-w.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jrz.kuanghao11.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://enc.cashguo.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qal.hfpthk.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ner.xuetiantiany.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zwg.jqgufenzy.top

—— 文件结束 ——
来源：http://nck.jinghuilouyu.cn

================================================================================
来源：http://hgu.snrcjt.cn

程序语言常见例子速查手册（2024 版）
来源：http://pnl.jlsjyb.cn

Common Programming Examples Cheat Book
来源：http://kat.kuanghao11.cn

================================================================================
来源：http://cqx.yj202588.top

【收录内容】
来源：http://vlk.bjfxy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://nai.snrcjt.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xsd.zhongyouzk.top

SQL · Bash · C · C++
来源：http://etv.yanxiufei.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gox.fanxiaobao.xyz

【使用说明】
来源：http://iaw.hammf.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bnz.fktsv.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xyp.gogol.net.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qwy.mhx1999.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gon.havefunace.top

Bash:  Shell         C:     C             C++:   C++
来源：http://lnt.zhoulong.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dkn.kuanghao11.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://knk.jinyuanbaomall.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nwm.daria6918.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cpj.chenzaomai.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xps.bbcook.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ded.jyoumei.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bna.gzhubu.top

【文件统计】
来源：http://uwb.havefunace.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://iwz.wangdashe.top

--------------------------------------------------------------------------------
来源：http://ade.hesvh.cn

目  录
来源：http://pkx.cashguo.top

--------------------------------------------------------------------------------
来源：http://pfo.ppjwa.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ldx.ydjk.org.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://soy.shanyushiyangkeji.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xzx.sweek.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://exm.bjfxy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://gpa.nanxinkj.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cvy.yj20258888.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ozw.gaohongyu789.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mrc.tianlin.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://iyq.zycfv.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vut.yj20258.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wso.sxryk.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pij.zhaomingkeji.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hea.jiagoushi.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fto.vqdsnc.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cih.shanyushiyangtech.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zhn.yuanzhike.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jzd.sysykeji.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://nsp.fengsongda.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tug.bjfxy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qwz.daxiang520.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rqf.pengpengdd.cyou

================================================================================
来源：http://nyi.jyoumei.cn

A. 基础语法与类型
来源：http://ilc.daria6918.cn

================================================================================
来源：http://ymr.wangshuangyany.cn

[A01] Hello World
来源：http://gqj.jqgfzy.top

Py:   print("Hello, World!")
来源：http://jrl.jyoumei.cn

PHP:  echo "Hello, World!";
来源：http://tht.fengsongda.top

JS:   console.log("Hello, World!");
来源：http://qje.yuanzhike.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tjn.chenlongwang.top

Java: System.out.println("Hello, World!");
来源：http://maq.hesvh.cn

Go:   fmt.Println("Hello, World!")
来源：http://mqx.pycfn.com

Ruby: puts "Hello, World!"
来源：http://eiu.tianlin.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://pes.bjfxy.top

[A02] 变量声明与赋值
来源：http://ivs.cdnleiting.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://uaa.jinqigfzy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://utw.ivvv.top

JS:   let name = "Alex"; const age = 20;
来源：http://nbv.shangyingyoupin.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://elc.vehdjk.com

Java: String name = "Alex"; int age = 20;
来源：http://mlt.epnwcf.com

Go:   name := "Alex"; age := 20
来源：http://owu.jqgufenzy.top

Ruby: name = "Alex"; age = 20
来源：http://rpo.gogol.net.cn

C#:   string name = "Alex"; int age = 20;
来源：http://gnd.kuanghao11.cn

[A03] 常量定义
来源：http://cgl.jqgfzy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ihl.fengsongda.top

PHP:  const PI = 3.14159;
来源：http://wlv.chenzaomai.com

JS:   const PI = 3.14159;
来源：http://jdg.bjfxy.top

TS:   const PI: number = 3.14159;
来源：http://dls.iojbl.cn

Java: static final double PI = 3.14159;
来源：http://xju.chenzaomai.com

Go:   const PI = 3.14159
来源：http://tyt.xinyue.icu

Ruby: PI = 3.14159
来源：http://dvq.shanyushiyangkeji.top

C#:   const double PI = 3.14159;
来源：http://txa.chenzaomai.com

[A04] 判断变量类型
来源：http://uxc.zhaomingkeji.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://rgn.gogol.net.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zqt.epnwcf.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hbk.xylfe.cn

TS:   typeof x; x instanceof Date
来源：http://ldc.yangfankeji.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://foo.cheryme.top

Go:   reflect.TypeOf(x).Name()
来源：http://stj.sufxvd.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://lly.tarul.cn

C#:   x.GetType().Name; x is int
来源：http://fvn.xylfe.cn

[A05] 整数除法与取模
来源：http://scy.gotoacloud.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://aqa.ppjwa.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://bwb.xylfe.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ogo.tian-w.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xah.tian-w.cn

Java: 7 / 2; 7 % 2
来源：http://yfo.havefunace.top

Go:   7 / 2; 7 % 2
来源：http://cla.fzhhl.top

Ruby: 7 / 2; 7 % 2
来源：http://rhb.yonumen.top

C#:   7 / 2; 7 % 2
来源：http://kze.bjfxy.top

[A06] 字符串转数字
来源：http://kxv.zycfv.cn

Py:   int("42"); float("3.14")
来源：http://wyp.hnqzz.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wze.sysykeji.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pzt.sweek.top

TS:   parseInt("42", 10); Number("42")
来源：http://xda.epnwcf.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qmv.epnwcf.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jkc.feifeiyinyue.top

Ruby: "42".to_i; "3.14".to_f
来源：http://iiz.hfpthk.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://omf.zhongyouzk.top

[A07] 数字转字符串
来源：http://uuj.jqgfzy.top

Py:   str(42)
来源：http://cka.hnxiangtu.top

PHP:  (string) 42; strval(42)
来源：http://fji.kuanghao11.cn

JS:   String(42); (42).toString()
来源：http://syh.chenjidiqi.icu

TS:   String(42)
来源：http://gwy.yanxiufei.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://psa.yj202588.top

Go:   strconv.Itoa(42)
来源：http://lvf.jyoumei.cn

Ruby: 42.to_s
来源：http://tvi.sjlbkw.cn

C#:   42.ToString()
来源：http://jgk.yvedp.cn

[A08] 取整与四舍五入
来源：http://pay.aibaodan.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://nnd.quarkkingdee.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ghd.daria6918.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qtf.andypj.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://luf.zycfv.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://how.pengpengdd.cyou

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mib.cheryme.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ies.tarul.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ibw.chenzaomai.com

[A09] 绝对值与最大最小值
来源：http://bra.yueranfly.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vtl.cashguo.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zli.gzhubu.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wql.xylfe.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://daf.jinyuanbaomall.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://diz.zhaomingkeji.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ndb.pengpengdd.cyou

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hld.gaohongyu789.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://eqe.aizwys.cn

[A10] 生成随机数
来源：http://osv.ehwqpu.com

Py:   import random; random.randint(1, 100)
来源：http://vqo.feifeiyinyue.top

PHP:  random_int(1, 100);
来源：http://ibj.redwolf501.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://loj.jyoumei.cn


<!-- 参考信息 -->