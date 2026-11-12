代发 wailian999

[U69] PHP：PDO 预处理
来源：http://zbp.xylfe.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tgq.zhiwuduotai.top

[U70] PHP：PDO 事务
来源：http://aow.shangyingyoupin.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qbl.hnqzz.top

[U71] PHP：抛出异常
来源：http://fnq.cucudq.cn

throw new RuntimeException("失败", 500);
来源：http://cxp.hammf.cn

[U72] PHP：写错误日志
来源：http://mmf.gzhubu.top

error_log("失败: " . $e->getMessage());
来源：http://ant.shangyingyoupin.top

[U73] PHP：读取 ini 配置
来源：http://hyp.daxiang520.top

parse_ini_file("config.ini", true)
来源：http://dtj.quarkkingdee.top

[U74] PHP：读取环境变量
来源：http://dpt.xylfe.cn

getenv("APP_ENV") ?: "production"
来源：http://rpj.yuxming.cn

[U75] PHP：依赖注入
来源：http://tzy.shangyingyoupin.top

composer require psr/container
来源：http://vdh.aizwys.cn

[U76] PHP：简单路由
来源：http://kpf.jianghu66.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kjl.ppjwa.cn

[U77] PHP：模板渲染
来源：http://hqk.fehbvm.com

composer require twig/twig
来源：http://stm.tianlin.xyz

[U78] PHP：单元测试
来源：http://dqk.gogol.net.cn

composer require --dev phpunit/phpunit
来源：http://vnt.tarul.cn

[U79] PHP：静态分析
来源：http://dvt.xziqi.cn

composer require --dev phpstan/phpstan
来源：http://zsc.gotoacloud.top

[U80] PHP：代码规范修复
来源：http://rcj.xingfuxueyuan.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://bdm.ehwqpu.com

[U81] JS：初始化项目
来源：http://jut.hnqzz.top

npm init -y;  npm i express
来源：http://klz.kuanghao11.cn

[U82] JS：package.json 脚本
来源：http://ibv.hcnkem.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qfh.sysykeji.top

[U83] JS：ES Module 导入导出
来源：http://rlq.hfpthk.cn

export const a = 1;  import { a } from "./m.js";
来源：http://kvs.yj202588.top

[U84] JS：CommonJS 写法
来源：http://gbs.zhaomingkeji.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://ang.yueranfly.top

[U85] JS：可选链
来源：http://aob.jinyuanbaomall.cn

a?.b?.c
来源：http://pgm.cqqwz.cn

[U86] JS：空值合并
来源：http://jis.jinqigfzy.top

a ?? b
来源：http://ptd.cashguo.top

[U87] JS：解构默认值
来源：http://upl.vehdjk.com

const { a = 1, b = 2 } = obj;
来源：http://gca.jinqigfzy.top

[U88] JS：对象展开合并
来源：http://uih.fehbvm.com

{ ...a, ...b }
来源：http://cwv.aizwys.cn

[U89] JS：数组去重
来源：http://rmt.ybcxt.top

[...new Set(arr)]
来源：http://rlv.tian-w.cn

[U90] JS：数字数组排序
来源：http://rnw.smart0.xyz

[...arr].sort((a, b) => a - b)
来源：http://ddy.kuanghao11.cn

[U91] JS：对象键值遍历
来源：http://kor.cashguo.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yeu.pengpengdd.cyou

[U92] JS：深拷贝
来源：http://qgx.aibaodan.cn

structuredClone(obj)
来源：http://ymd.hnxiangtu.top

[U93] JS：模板字符串
来源：http://flb.xuetiantiany.cn

`共 ${n} 条`
来源：http://ngv.havefunace.top

[U94] JS：箭头函数
来源：http://min.zdqjudy.top

const double = x => x * 2;
来源：http://fsb.xingfuxueyuan.xyz

[U95] JS：Promise 包装
来源：http://yko.jinghuilouyu.cn

new Promise((resolve, reject) => {})
来源：http://dts.zhongyouzk.top

[U96] JS：async/await 与异常
来源：http://ilb.sysykeji.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rag.yanxiufei.cn

[U97] JS：并发请求
来源：http://rjh.yuxming.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://eua.yangfankeji.com

[U98] JS：fetch 带 JSON
来源：http://uon.zhoulong.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://slf.yj202588.top

[U99] JS：事件监听
来源：http://jlj.fehbvm.com

el.addEventListener("click", e => {})
来源：http://wul.fanxiaobao.xyz

[U100] JS：DOM 查询
来源：http://tiw.jqgufenzy.top

document.querySelector(".item")
来源：http://bxh.redwolf501.top

[U101] JS：classList 操作
来源：http://amp.aizwys.cn

el.classList.toggle("active")
来源：http://dyd.aibaodan.cn

[U102] JS：本地存储
来源：http://msi.sweek.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://uyj.jinqigfzy.top

[U103] JS：定时器
来源：http://gwr.jlsjyb.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fdw.hongshengwenyu.top

[U104] JS：防抖
来源：http://zkf.yj20258888.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://neh.iojbl.cn

[U105] JS：节流
来源：http://afl.hywenlv.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lgl.hnqzz.top

[U106] JS：日期格式化
来源：http://tqa.yj20258888.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://goc.yuanzhike.top

[U107] JS：数字千分位
来源：http://lku.cashguo.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sre.iojbl.cn

[U108] JS：随机整数
来源：http://flr.sjlbkw.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nva.hnqzz.top

[U109] JS：数组分组
来源：http://kyw.sufxvd.cn

Object.groupBy(arr, x => x.type)
来源：http://rts.ydjk.org.cn

[U110] JS：数组分块
来源：http://fuu.gogol.net.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fiu.jinghuilouyu.cn

[U111] JS：对象转 Map
来源：http://ytk.fzhhl.top

new Map(Object.entries(obj))
来源：http://vxo.daxiang520.top

[U112] JS：字符串补位
来源：http://jmy.gzhubu.top

"7".padStart(3, "0")
来源：http://gil.zhongyouzk.top

[U113] JS：正则替换全部
来源：http://hvj.jinyuanbaomall.cn

s.replaceAll("a", "b")
来源：http://ihj.havefunace.top

[U114] JS：JSON 深比较
来源：http://cbm.cashguo.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://vgx.andypj.xyz

[U115] JS：生成 UUID
来源：http://pxz.ctjpmb.com

crypto.randomUUID()
来源：http://obm.xuanzx.com

[U116] JS：类型检查（JSDoc）
来源：http://xhf.wangshuangyany.cn

/** @param {string} name */ function f(name) {}
来源：http://lpp.chenzaomai.com

[U117] JS：单元测试
来源：http://mpi.wangshuangyany.cn

npm i -D vitest;  npx vitest
来源：http://dhr.redwolf501.top

[U118] JS：开发服务器
来源：http://oqy.yanxiufei.cn

npm i -D vite;  npx vite
来源：http://wms.tarul.cn

[U119] JS：生产构建
来源：http://gbu.feifeiyinyue.top

npx vite build
来源：http://drd.sweek.top

[U120] JS：读取环境变量（Vite）
来源：http://cil.dianchejie.cn

import.meta.env.VITE_API_URL
来源：http://woz.bjfxy.top

================================================================================
来源：http://ete.sxryk.cn

统计汇总
来源：http://pny.9152youxi.cn

================================================================================
来源：http://zyd.sjlbkw.cn

按语言统计（条）：
来源：http://lqj.gotoacloud.top

Python ......... 252
来源：http://uwd.guannengcc.top

PHP ............ 252
来源：http://emw.havefunace.top

JavaScript ..... 252
来源：http://wzq.zhixingplan.top

TypeScript ..... 212
来源：http://qpo.jqgfzy.top

Java ........... 212
来源：http://qxd.nanxuanxn.top

Go ............. 212
来源：http://dvy.gotoacloud.top

Ruby ........... 212
来源：http://vpf.hnqzz.top

C# ............. 212
来源：http://hnb.sufxvd.cn

C .............. 30
来源：http://shv.zhongyouzk.top

C++ ............ 30
来源：http://qiq.redwolf501.top

SQL ............ 90
来源：http://lez.yongpay.top

Bash ........... 80
来源：http://ddx.svipenyu.cn

Kotlin ......... 15
来源：http://hax.uphjek.com

Swift .......... 15
来源：http://nxt.52xcode.cn

Lua ............ 10
来源：http://itr.ivvv.top

Perl ........... 10
来源：http://eee.zdqjudy.top

Scala .......... 10
来源：http://kzb.xylfe.cn

------------------------------------
来源：http://jos.jinqigfzy.top

合计 ........... 2106 条
来源：http://jvg.hongshengwenyu.top

按章节统计：
来源：http://abv.wangshuangyany.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rjn.yj20258888.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cbr.shzxlz.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rdj.xinyue.icu

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://enp.xuanzx.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qyr.epnwcf.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blp.yueranfly.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nta.ybcxt.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://spz.xinyue.icu

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xit.meibo888.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://onv.jqgfzy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://emt.hysaishi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lka.feifeiyinyue.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://laq.gaohongyu789.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pyj.jqgufenzy.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://phq.xuetiantiany.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qfn.vehdjk.com

Q SQL 专题                              90
来源：http://ghz.nanxinkj.top

R Bash 专题                             80
来源：http://emn.redwolf501.top

S C / C++ 专题                          60
来源：http://ugs.bbcook.cn

T 其他语言补充                          60
来源：http://qkv.hcnkem.com

U 高频实用片段                         120
来源：http://gwo.hnqzz.top

------------------------------------
来源：http://rwe.vehdjk.com

合计                                  2106 条
来源：http://wzq.svipenyu.cn

--------------------------------------------------------------------------------
来源：http://bpk.guannengcc.top

使用提醒
来源：http://bnw.nanxinkj.top

--------------------------------------------------------------------------------
来源：http://bgt.fehbvm.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fat.gzhubu.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://odf.shzxlz.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://aau.uphjek.com

在旧版本上使用前请先确认语法支持情况。
来源：http://dap.gzhubu.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wad.yj202588.top

—— 文件结束 ——
来源：http://ndl.zhengqikj.top

================================================================================
来源：http://uls.yfazqb.com

程序语言常见例子速查手册（2024 版）
来源：http://mvd.yvedp.cn

Common Programming Examples Cheat Book
来源：http://ijt.nanxinkj.top

================================================================================
来源：http://toe.cheryme.top

【收录内容】
来源：http://syd.cucudq.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://zjw.shzxlz.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qsh.fanxiaobao.xyz

SQL · Bash · C · C++
来源：http://jdc.zhixingplan.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zms.yongpay.top

【使用说明】
来源：http://umn.xziqi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ams.fehbvm.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zcp.hesvh.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gct.bjfxy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rbt.nwbrower.top

Bash:  Shell         C:     C             C++:   C++
来源：http://uph.jianghu66.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://oef.jinqigufen.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rmg.cqqwz.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vyj.ywan-chungtsiang.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rup.jlsjyb.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gos.pycfn.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tpy.andypj.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ohz.ctjpmb.com

【文件统计】
来源：http://ydk.nanxinkj.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mqo.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://zpd.feifeiyinyue.top

目  录
来源：http://imm.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://wcz.ybcxt.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yen.jiagoushi.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ykc.zdbjq.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ksg.yueranfly.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zhi.jqgfzy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jio.jyoumei.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blk.svipenyu.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ikg.zhiwuduotai.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wmc.xylfe.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://iim.xuetiantiany.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bnp.ybcxt.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://udu.ctjpmb.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cjl.gaohongyu789.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jtq.dianchejie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mpc.cashguo.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fhs.yj202588.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wle.tianlin.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fwz.yj20258888.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://dud.zhijiandao.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://egy.uphjek.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tcg.zhongyouzk.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xqm.tian-w.cn

================================================================================
来源：http://rgk.jqgfzy.top

A. 基础语法与类型
来源：http://blg.c1oappe.top

================================================================================
来源：http://rli.gaohongyu789.top

[A01] Hello World
来源：http://uou.smart0.xyz

Py:   print("Hello, World!")
来源：http://owb.shangyingyoupin.top

PHP:  echo "Hello, World!";
来源：http://jrq.hnqzz.top

JS:   console.log("Hello, World!");
来源：http://gfc.dianchejie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jcg.cucudq.cn

Java: System.out.println("Hello, World!");
来源：http://ynm.zhengqikj.top

Go:   fmt.Println("Hello, World!")
来源：http://kpn.chenjidiqi.icu

Ruby: puts "Hello, World!"
来源：http://xrd.tanke756.top

C#:   Console.WriteLine("Hello, World!");
来源：http://mxc.ehwqpu.com

[A02] 变量声明与赋值
来源：http://yhl.tanke756.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://itt.redwolf501.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ajk.jqgfzy.top

JS:   let name = "Alex"; const age = 20;
来源：http://ifc.haohaochexian.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ehb.hywenlv.cn

Java: String name = "Alex"; int age = 20;
来源：http://vxr.wangshuangyany.cn

Go:   name := "Alex"; age := 20
来源：http://pxi.shanyushiyangtech.top

Ruby: name = "Alex"; age = 20
来源：http://kya.meibo888.top

C#:   string name = "Alex"; int age = 20;
来源：http://yct.dianchejie.cn

[A03] 常量定义
来源：http://wgw.feifeiyinyue.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://uyr.shangyingyoupin.top

PHP:  const PI = 3.14159;
来源：http://fgh.redwolf501.top

JS:   const PI = 3.14159;
来源：http://jey.jianghu66.top

TS:   const PI: number = 3.14159;
来源：http://dsh.cashguo.top

Java: static final double PI = 3.14159;
来源：http://xdx.ydzc1.top

Go:   const PI = 3.14159
来源：http://epi.yj20258.top

Ruby: PI = 3.14159
来源：http://kcs.ywan-chungtsiang.top

C#:   const double PI = 3.14159;
来源：http://yvs.fengsongda.top

[A04] 判断变量类型
来源：http://dkj.sjlbkw.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ikd.guowangkeji.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wmr.gaohongyu789.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hlx.yongpay.top

TS:   typeof x; x instanceof Date
来源：http://wgl.hnqzz.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hen.jianghu66.top

Go:   reflect.TypeOf(x).Name()
来源：http://qnn.jianghu66.top

Ruby: x.class; x.is_a?(Integer)
来源：http://hcu.ydzc1.top

C#:   x.GetType().Name; x is int
来源：http://jme.ybcxt.top

[A05] 整数除法与取模
来源：http://wbr.yonumen.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://whd.guowangkeji.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://qzt.yongpay.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://obx.aibaodan.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xob.ehwqpu.com

Java: 7 / 2; 7 % 2
来源：http://wvy.hesvh.cn

Go:   7 / 2; 7 % 2
来源：http://joi.daxiang520.top

Ruby: 7 / 2; 7 % 2
来源：http://rcv.zhiwuduotai.top

C#:   7 / 2; 7 % 2
来源：http://kdb.zhengqikj.top

[A06] 字符串转数字
来源：http://ojo.uphjek.com

Py:   int("42"); float("3.14")
来源：http://xvp.tian-w.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://asq.yj20258.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hkt.zdbjq.cn

TS:   parseInt("42", 10); Number("42")
来源：http://tpk.pengpengdd.cyou

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xgk.shzxlz.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cqj.havefunace.top

Ruby: "42".to_i; "3.14".to_f
来源：http://uuj.yuanzhike.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zwj.mhx1999.top

[A07] 数字转字符串
来源：http://ytn.cashguo.top

Py:   str(42)
来源：http://tzw.chenjidiqi.icu

PHP:  (string) 42; strval(42)
来源：http://yun.jyoumei.cn

JS:   String(42); (42).toString()
来源：http://dbc.jyoumei.cn

TS:   String(42)
来源：http://rnc.haohaochexian.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://akc.gaohongyu789.top

Go:   strconv.Itoa(42)
来源：http://clp.sweek.top

Ruby: 42.to_s
来源：http://eut.pycfn.com

C#:   42.ToString()
来源：http://gfy.dianchejie.cn

[A08] 取整与四舍五入
来源：http://hpy.shuidangran.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ldk.nwbrower.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://pnv.uphjek.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mxj.yj202588.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ech.gotoacloud.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://bmc.daxiang520.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hdi.meibo888.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://cxm.guowangkeji.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ovp.daxiang520.top

[A09] 绝对值与最大最小值
来源：http://cqn.zhoulong.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lnf.daria6918.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wtg.shuidangran.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://uxl.ehwqpu.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://eap.fehbvm.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://yxr.quarkkingdee.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gvc.jlsjyb.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jfo.yj20258888.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://sfc.fktsv.cn

[A10] 生成随机数
来源：http://yov.ehwqpu.com

Py:   import random; random.randint(1, 100)
来源：http://mbj.jyoumei.cn

PHP:  random_int(1, 100);
来源：http://gzf.redwolf501.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ish.hongshengwenyu.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kvg.vehdjk.com

Java: new Random().nextInt(100) + 1
来源：http://byj.jqgufenzy.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bho.guannengcc.top

Ruby: rand(1..100)
来源：http://pek.jinqigufen.top


<!-- 参考信息 -->