代发 wailian999

[U67] PHP：处理文件上传
来源：http://fok.zhijiandao.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kiy.sysykeji.top

[U68] PHP：PDO 连接
来源：http://ynn.birdmap.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gie.ctjpmb.com

[U69] PHP：PDO 预处理
来源：http://ubj.jqgfzy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hbr.fehbvm.com

[U70] PHP：PDO 事务
来源：http://ffr.c1oappe.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vsw.xuetiantiany.cn

[U71] PHP：抛出异常
来源：http://oxf.meibo888.top

throw new RuntimeException("失败", 500);
来源：http://mwu.zhongyouzk.top

[U72] PHP：写错误日志
来源：http://xas.fehbvm.com

error_log("失败: " . $e->getMessage());
来源：http://ocb.jinyuanbaomall.cn

[U73] PHP：读取 ini 配置
来源：http://xya.ivvv.top

parse_ini_file("config.ini", true)
来源：http://stx.xuanzx.com

[U74] PHP：读取环境变量
来源：http://xdm.yonumen.top

getenv("APP_ENV") ?: "production"
来源：http://bir.iojbl.cn

[U75] PHP：依赖注入
来源：http://ewm.redwolf501.top

composer require psr/container
来源：http://yzq.sufxvd.cn

[U76] PHP：简单路由
来源：http://gjo.zhaomingkeji.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zzo.jinyuanbaomall.cn

[U77] PHP：模板渲染
来源：http://dys.chenlongwang.top

composer require twig/twig
来源：http://mtx.jinyuanbaomall.cn

[U78] PHP：单元测试
来源：http://swc.yj20258.top

composer require --dev phpunit/phpunit
来源：http://zxf.ybcxt.top

[U79] PHP：静态分析
来源：http://dag.sxryk.cn

composer require --dev phpstan/phpstan
来源：http://coz.cucudq.cn

[U80] PHP：代码规范修复
来源：http://nav.dianchejie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jpa.9152youxi.cn

[U81] JS：初始化项目
来源：http://bib.kuanghao11.cn

npm init -y;  npm i express
来源：http://fke.9152youxi.cn

[U82] JS：package.json 脚本
来源：http://cof.iojbl.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wjh.snrcjt.cn

[U83] JS：ES Module 导入导出
来源：http://bmc.daxiang520.top

export const a = 1;  import { a } from "./m.js";
来源：http://eoc.aibaodan.cn

[U84] JS：CommonJS 写法
来源：http://ajd.gotoacloud.top

module.exports = { a };  const { a } = require("./m");
来源：http://hjr.chenzaomai.com

[U85] JS：可选链
来源：http://fbg.xuetiantiany.cn

a?.b?.c
来源：http://dzb.tianlin.xyz

[U86] JS：空值合并
来源：http://vmd.bbcook.cn

a ?? b
来源：http://oeu.andypj.xyz

[U87] JS：解构默认值
来源：http://nen.cqqwz.cn

const { a = 1, b = 2 } = obj;
来源：http://jwr.daxiang520.top

[U88] JS：对象展开合并
来源：http://ikq.gzhubu.top

{ ...a, ...b }
来源：http://yzz.xinyue.icu

[U89] JS：数组去重
来源：http://gfk.xziqi.cn

[...new Set(arr)]
来源：http://osr.fzhhl.top

[U90] JS：数字数组排序
来源：http://srs.shzxlz.cn

[...arr].sort((a, b) => a - b)
来源：http://lnz.jlsjyb.cn

[U91] JS：对象键值遍历
来源：http://jvl.ybcxt.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qix.chenlongwang.top

[U92] JS：深拷贝
来源：http://qrs.yj20258888.top

structuredClone(obj)
来源：http://zgy.zhengqikj.top

[U93] JS：模板字符串
来源：http://vpd.iojbl.cn

`共 ${n} 条`
来源：http://wwo.andypj.xyz

[U94] JS：箭头函数
来源：http://zrd.zdqjudy.top

const double = x => x * 2;
来源：http://iav.haohaochexian.top

[U95] JS：Promise 包装
来源：http://haa.meibo888.top

new Promise((resolve, reject) => {})
来源：http://unk.hywenlv.cn

[U96] JS：async/await 与异常
来源：http://rde.fzhhl.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xbc.guowangkeji.top

[U97] JS：并发请求
来源：http://hmo.gotoacloud.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://dua.vehdjk.com

[U98] JS：fetch 带 JSON
来源：http://qpl.vehdjk.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xwx.xuetiantiany.cn

[U99] JS：事件监听
来源：http://jny.pycfn.com

el.addEventListener("click", e => {})
来源：http://jhf.zhengqikj.top

[U100] JS：DOM 查询
来源：http://zpy.jiagoushi.top

document.querySelector(".item")
来源：http://lzr.guannengcc.top

[U101] JS：classList 操作
来源：http://exd.cucudq.cn

el.classList.toggle("active")
来源：http://kcu.daxiang520.top

[U102] JS：本地存储
来源：http://vcv.zdqjudy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://xdt.zhongyouzk.top

[U103] JS：定时器
来源：http://zgn.jlsjyb.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ysv.cheryme.top

[U104] JS：防抖
来源：http://qfe.9152youxi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ufe.jqgfzy.top

[U105] JS：节流
来源：http://jlt.wangdashe.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://iue.tarul.cn

[U106] JS：日期格式化
来源：http://cgf.kuanghao11.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yda.kuanghao11.cn

[U107] JS：数字千分位
来源：http://zce.zhaomingkeji.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ycy.ppjwa.cn

[U108] JS：随机整数
来源：http://kkp.gzhubu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pns.vqdsnc.cn

[U109] JS：数组分组
来源：http://rmu.pycfn.com

Object.groupBy(arr, x => x.type)
来源：http://vgy.xingfuxueyuan.xyz

[U110] JS：数组分块
来源：http://wjm.daria6918.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vlg.52xcode.cn

[U111] JS：对象转 Map
来源：http://rwa.yueranfly.top

new Map(Object.entries(obj))
来源：http://nte.vqdsnc.cn

[U112] JS：字符串补位
来源：http://hqo.shuidangran.top

"7".padStart(3, "0")
来源：http://lrc.hcnkem.com

[U113] JS：正则替换全部
来源：http://ldp.shanyushiyangkeji.top

s.replaceAll("a", "b")
来源：http://haw.guannengcc.top

[U114] JS：JSON 深比较
来源：http://kmu.hnqzz.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://bsc.yuanzhike.top

[U115] JS：生成 UUID
来源：http://jzn.nwbrower.top

crypto.randomUUID()
来源：http://zem.smart0.xyz

[U116] JS：类型检查（JSDoc）
来源：http://ivk.daxiang520.top

/** @param {string} name */ function f(name) {}
来源：http://igv.daxiang520.top

[U117] JS：单元测试
来源：http://hoz.pycfn.com

npm i -D vitest;  npx vitest
来源：http://lqh.ctjpmb.com

[U118] JS：开发服务器
来源：http://aul.jyoumei.cn

npm i -D vite;  npx vite
来源：http://xoo.redwolf501.top

[U119] JS：生产构建
来源：http://bmu.hongshengwenyu.top

npx vite build
来源：http://xig.yonumen.top

[U120] JS：读取环境变量（Vite）
来源：http://qik.shzxlz.cn

import.meta.env.VITE_API_URL
来源：http://ezc.haohaochexian.top

================================================================================
来源：http://cav.bbcook.cn

统计汇总
来源：http://ohq.hysaishi.cn

================================================================================
来源：http://fzu.kuanghao11.cn

按语言统计（条）：
来源：http://msd.havefunace.top

Python ......... 252
来源：http://jfh.guannengcc.top

PHP ............ 252
来源：http://hfs.zhoulong.xyz

JavaScript ..... 252
来源：http://tpv.cheryme.top

TypeScript ..... 212
来源：http://eke.iojbl.cn

Java ........... 212
来源：http://ofv.yongpay.top

Go ............. 212
来源：http://lfa.nanxuanxn.top

Ruby ........... 212
来源：http://mhs.cdnleiting.top

C# ............. 212
来源：http://nen.ywan-chungtsiang.top

C .............. 30
来源：http://pms.xuetiantiany.cn

C++ ............ 30
来源：http://hvo.guannengcc.top

SQL ............ 90
来源：http://jtj.xuanzx.com

Bash ........... 80
来源：http://hzm.epnwcf.com

Kotlin ......... 15
来源：http://rrw.zycfv.cn

Swift .......... 15
来源：http://gya.yuanzhike.top

Lua ............ 10
来源：http://bct.ctjpmb.com

Perl ........... 10
来源：http://vtf.ybcxt.top

Scala .......... 10
来源：http://jnj.svipenyu.cn

------------------------------------
来源：http://uga.xuanzx.com

合计 ........... 2106 条
来源：http://boy.ivvv.top

按章节统计：
来源：http://emj.zhengqikj.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://juq.bjfxy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qyf.jiagoushi.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nxj.ydzc1.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ryh.svipenyu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vxe.birdmap.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://twj.iojbl.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lye.quarkkingdee.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ngp.yj20258.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wmj.birdmap.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://amw.yanxiufei.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rul.shzxlz.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ben.nanxinkj.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jsm.tarul.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dwx.xingfuxueyuan.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ahj.yj202588.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kdi.pycfn.com

Q SQL 专题                              90
来源：http://mpn.guowangkeji.top

R Bash 专题                             80
来源：http://bck.svipenyu.cn

S C / C++ 专题                          60
来源：http://bxl.uphjek.com

T 其他语言补充                          60
来源：http://tit.jianghu66.top

U 高频实用片段                         120
来源：http://rft.ydjk.org.cn

------------------------------------
来源：http://shg.snrcjt.cn

合计                                  2106 条
来源：http://tgd.9152youxi.cn

--------------------------------------------------------------------------------
来源：http://zcm.wangshuangyany.cn

使用提醒
来源：http://zen.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://aak.ctjpmb.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://eme.daria6918.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gjd.pycfn.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zbk.ctjpmb.com

在旧版本上使用前请先确认语法支持情况。
来源：http://xao.cdnleiting.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dcc.dianchejie.cn

—— 文件结束 ——
来源：http://evm.yj20258888.top

================================================================================
来源：http://zbt.jinqigufen.top

程序语言常见例子速查手册（2024 版）
来源：http://lsi.hysaishi.cn

Common Programming Examples Cheat Book
来源：http://svw.vehdjk.com

================================================================================
来源：http://qtz.vqdsnc.cn

【收录内容】
来源：http://cfq.chenlongwang.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://oxa.xuetiantiany.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://lpr.yongpay.top

SQL · Bash · C · C++
来源：http://thp.chenjidiqi.icu

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qqc.tanke756.top

【使用说明】
来源：http://qva.jlsjyb.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://muu.xinyue.icu

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nws.daxiang520.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://onx.xingfuxueyuan.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dhx.aizwys.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://uko.yanxiufei.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xlu.tianlin.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yra.hywenlv.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ftm.yj20258.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pra.ydjk.org.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lmk.jqgufenzy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://cnb.yj20258888.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ear.sxryk.cn

【文件统计】
来源：http://tkl.chenjidiqi.icu

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ihh.cheryme.top

--------------------------------------------------------------------------------
来源：http://vty.zdqjudy.top

目  录
来源：http://odg.meibo888.top

--------------------------------------------------------------------------------
来源：http://wpt.yfazqb.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ttk.daria6918.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qig.hysaishi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jjg.316326.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pom.zhoulong.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yas.jinqigfzy.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cbs.hongshengwenyu.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wrb.guowangkeji.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bjj.jqgufenzy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://nlc.hammf.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gxm.hammf.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://acp.fktsv.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pdi.ctjpmb.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jxh.hammf.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tzx.jinyuanbaomall.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://uiq.fanxiaobao.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wbz.vqdsnc.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://enr.wangdashe.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://pck.sweek.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qxa.hcnkem.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kyr.zycfv.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xsx.fzhhl.top

================================================================================
来源：http://est.andypj.xyz

A. 基础语法与类型
来源：http://jdq.guannengcc.top

================================================================================
来源：http://ikp.zhijiandao.cn

[A01] Hello World
来源：http://lze.havefunace.top

Py:   print("Hello, World!")
来源：http://npu.daxiang520.top

PHP:  echo "Hello, World!";
来源：http://awa.hysaishi.cn

JS:   console.log("Hello, World!");
来源：http://hea.sysykeji.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zmc.zdbjq.cn

Java: System.out.println("Hello, World!");
来源：http://jrp.52xcode.cn

Go:   fmt.Println("Hello, World!")
来源：http://ksy.tarul.cn

Ruby: puts "Hello, World!"
来源：http://rmy.bjfxy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ity.wangshuangyany.cn

[A02] 变量声明与赋值
来源：http://ewz.wangshuangyany.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://pqi.jqgfzy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://prb.ywan-chungtsiang.top

JS:   let name = "Alex"; const age = 20;
来源：http://wfz.vehdjk.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qqv.wangdashe.top

Java: String name = "Alex"; int age = 20;
来源：http://yfr.vqdsnc.cn

Go:   name := "Alex"; age := 20
来源：http://gey.jinyuanbaomall.cn

Ruby: name = "Alex"; age = 20
来源：http://azj.hnxiangtu.top

C#:   string name = "Alex"; int age = 20;
来源：http://jhc.yj202588.top

[A03] 常量定义
来源：http://mfk.tanke756.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kvy.ivvv.top

PHP:  const PI = 3.14159;
来源：http://zgv.vqdsnc.cn

JS:   const PI = 3.14159;
来源：http://euo.meibo888.top

TS:   const PI: number = 3.14159;
来源：http://nws.cucudq.cn

Java: static final double PI = 3.14159;
来源：http://jrf.tarul.cn

Go:   const PI = 3.14159
来源：http://zoj.quarkkingdee.top

Ruby: PI = 3.14159
来源：http://jih.jinqigufen.top

C#:   const double PI = 3.14159;
来源：http://swi.wangdashe.top

[A04] 判断变量类型
来源：http://bsv.zhoulong.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://pzw.yonumen.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qjn.shzxlz.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gqv.yj202588.top

TS:   typeof x; x instanceof Date
来源：http://zfw.nwbrower.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hvi.snrcjt.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ugx.shangyingyoupin.top

Ruby: x.class; x.is_a?(Integer)
来源：http://psi.zhengqikj.top

C#:   x.GetType().Name; x is int
来源：http://pjn.sjlbkw.cn

[A05] 整数除法与取模
来源：http://gof.uphjek.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mve.wangdashe.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://qfu.daxiang520.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://stg.guowangkeji.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qvp.birdmap.top

Java: 7 / 2; 7 % 2
来源：http://etj.hysaishi.cn

Go:   7 / 2; 7 % 2
来源：http://jca.yuanzhike.top

Ruby: 7 / 2; 7 % 2
来源：http://ilm.ywan-chungtsiang.top

C#:   7 / 2; 7 % 2
来源：http://mfb.jqgufenzy.top

[A06] 字符串转数字
来源：http://ycl.sysykeji.top

Py:   int("42"); float("3.14")
来源：http://wso.meibo888.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://txv.daria6918.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jrb.fehbvm.com

TS:   parseInt("42", 10); Number("42")
来源：http://qec.pycfn.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mqm.feifeiyinyue.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ivs.dashuyun.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://kvx.wangdashe.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://spi.c1oappe.top

[A07] 数字转字符串
来源：http://git.yj20258.top

Py:   str(42)
来源：http://zji.gogol.net.cn

PHP:  (string) 42; strval(42)
来源：http://qyn.aibaodan.cn

JS:   String(42); (42).toString()
来源：http://jzq.fzhhl.top

TS:   String(42)
来源：http://ybj.hammf.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://clg.jiagoushi.top

Go:   strconv.Itoa(42)
来源：http://qii.ywan-chungtsiang.top

Ruby: 42.to_s
来源：http://ikk.svipenyu.cn

C#:   42.ToString()
来源：http://lcd.tian-w.cn

[A08] 取整与四舍五入
来源：http://bqd.guowangkeji.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hym.jqgufenzy.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vvd.jlsjyb.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://doh.haohaochexian.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://tch.chenjidiqi.icu

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ehd.mhx1999.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rbx.zycfv.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://zbm.epnwcf.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://umc.bbcook.cn

[A09] 绝对值与最大最小值
来源：http://eoz.feifeiyinyue.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vql.andypj.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://lsv.snrcjt.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vtj.cqqwz.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://pqc.yonumen.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kki.kuanghao11.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rua.sweek.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xts.fehbvm.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://nzb.aibaodan.cn

[A10] 生成随机数
来源：http://bgf.0kj1m.cn

Py:   import random; random.randint(1, 100)
来源：http://ahp.zhiwuduotai.top

PHP:  random_int(1, 100);
来源：http://wld.jiagoushi.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://omh.bjfxy.top


<!-- 参考信息 -->