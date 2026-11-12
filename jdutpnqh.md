代发 wailian999

[U67] PHP：处理文件上传
来源：http://quv.jlsjyb.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://djr.yueranfly.top

[U68] PHP：PDO 连接
来源：http://fjs.52xcode.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tzy.jinyuanbaomall.cn

[U69] PHP：PDO 预处理
来源：http://zok.cdnleiting.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xap.kuanghao11.cn

[U70] PHP：PDO 事务
来源：http://olh.tarul.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pwf.smart0.xyz

[U71] PHP：抛出异常
来源：http://bwe.guannengcc.top

throw new RuntimeException("失败", 500);
来源：http://mts.xingfuxueyuan.xyz

[U72] PHP：写错误日志
来源：http://pev.cqqwz.cn

error_log("失败: " . $e->getMessage());
来源：http://xec.haohaochexian.top

[U73] PHP：读取 ini 配置
来源：http://zye.mhx1999.top

parse_ini_file("config.ini", true)
来源：http://hai.yongpay.top

[U74] PHP：读取环境变量
来源：http://xkm.ydjk.org.cn

getenv("APP_ENV") ?: "production"
来源：http://ceh.yfazqb.com

[U75] PHP：依赖注入
来源：http://iuy.bjfxy.top

composer require psr/container
来源：http://xod.havefunace.top

[U76] PHP：简单路由
来源：http://hvy.zhongyouzk.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://puw.zhengqikj.top

[U77] PHP：模板渲染
来源：http://rga.gaohongyu789.top

composer require twig/twig
来源：http://ogl.hfpthk.cn

[U78] PHP：单元测试
来源：http://zrp.yanxiufei.cn

composer require --dev phpunit/phpunit
来源：http://xun.yj202588.top

[U79] PHP：静态分析
来源：http://umh.yj20258.top

composer require --dev phpstan/phpstan
来源：http://uzw.nanxuanxn.top

[U80] PHP：代码规范修复
来源：http://hzs.epnwcf.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://xhc.sweek.top

[U81] JS：初始化项目
来源：http://nog.52xcode.cn

npm init -y;  npm i express
来源：http://mlo.zycfv.cn

[U82] JS：package.json 脚本
来源：http://riw.sxryk.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lsb.gzhubu.top

[U83] JS：ES Module 导入导出
来源：http://ntq.haohaochexian.top

export const a = 1;  import { a } from "./m.js";
来源：http://fcw.hnqzz.top

[U84] JS：CommonJS 写法
来源：http://tgn.nanxinkj.top

module.exports = { a };  const { a } = require("./m");
来源：http://wsa.cashguo.top

[U85] JS：可选链
来源：http://lsy.jinyuanbaomall.cn

a?.b?.c
来源：http://qgg.52xcode.cn

[U86] JS：空值合并
来源：http://dhm.chenjidiqi.icu

a ?? b
来源：http://bqk.hammf.cn

[U87] JS：解构默认值
来源：http://puw.jiagoushi.top

const { a = 1, b = 2 } = obj;
来源：http://xed.iojbl.cn

[U88] JS：对象展开合并
来源：http://iqg.redwolf501.top

{ ...a, ...b }
来源：http://rvs.cheryme.top

[U89] JS：数组去重
来源：http://chk.epnwcf.com

[...new Set(arr)]
来源：http://kbu.316326.xyz

[U90] JS：数字数组排序
来源：http://rbv.shanyushiyangkeji.top

[...arr].sort((a, b) => a - b)
来源：http://rbw.mhx1999.top

[U91] JS：对象键值遍历
来源：http://pms.ehwqpu.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pwy.tian-w.cn

[U92] JS：深拷贝
来源：http://sbp.yongpay.top

structuredClone(obj)
来源：http://sby.shanyushiyangkeji.top

[U93] JS：模板字符串
来源：http://ycl.jlsjyb.cn

`共 ${n} 条`
来源：http://bza.hywenlv.cn

[U94] JS：箭头函数
来源：http://erv.tian-w.cn

const double = x => x * 2;
来源：http://eup.pengpengdd.cyou

[U95] JS：Promise 包装
来源：http://sxc.jinqigufen.top

new Promise((resolve, reject) => {})
来源：http://jre.zhixingplan.top

[U96] JS：async/await 与异常
来源：http://sal.wangdashe.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vhw.jqgufenzy.top

[U97] JS：并发请求
来源：http://orr.smart0.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://fho.feifeiyinyue.top

[U98] JS：fetch 带 JSON
来源：http://cvt.fengsongda.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ebi.cheryme.top

[U99] JS：事件监听
来源：http://yaq.cqqwz.cn

el.addEventListener("click", e => {})
来源：http://wgy.gzhubu.top

[U100] JS：DOM 查询
来源：http://eyc.sxryk.cn

document.querySelector(".item")
来源：http://sne.cashguo.top

[U101] JS：classList 操作
来源：http://rzk.jinghuilouyu.cn

el.classList.toggle("active")
来源：http://fsz.jinyuanbaomall.cn

[U102] JS：本地存储
来源：http://jmz.zdqjudy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://wno.zycfv.cn

[U103] JS：定时器
来源：http://wbu.yongpay.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vns.yongpay.top

[U104] JS：防抖
来源：http://jlh.jqgufenzy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://okk.tianlin.xyz

[U105] JS：节流
来源：http://bxt.zhiwuduotai.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zva.yuanzhike.top

[U106] JS：日期格式化
来源：http://tcr.shanyushiyangtech.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tgz.kuanghao11.cn

[U107] JS：数字千分位
来源：http://ymo.zhoulong.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wyy.quarkkingdee.top

[U108] JS：随机整数
来源：http://ugm.xinyue.icu

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ige.zycfv.cn

[U109] JS：数组分组
来源：http://kue.hywenlv.cn

Object.groupBy(arr, x => x.type)
来源：http://ltu.9152youxi.cn

[U110] JS：数组分块
来源：http://udt.zdqjudy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vvx.bjfxy.top

[U111] JS：对象转 Map
来源：http://mug.xuetiantiany.cn

new Map(Object.entries(obj))
来源：http://guj.yuxming.cn

[U112] JS：字符串补位
来源：http://its.jqgufenzy.top

"7".padStart(3, "0")
来源：http://dpl.kuanghao11.cn

[U113] JS：正则替换全部
来源：http://hxc.birdmap.top

s.replaceAll("a", "b")
来源：http://ssv.zhiwuduotai.top

[U114] JS：JSON 深比较
来源：http://kio.dianchejie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ggx.ywan-chungtsiang.top

[U115] JS：生成 UUID
来源：http://udi.xuanzx.com

crypto.randomUUID()
来源：http://ssm.jyoumei.cn

[U116] JS：类型检查（JSDoc）
来源：http://uxv.sysykeji.top

/** @param {string} name */ function f(name) {}
来源：http://kfh.redwolf501.top

[U117] JS：单元测试
来源：http://vbj.sweek.top

npm i -D vitest;  npx vitest
来源：http://pkh.ydzc1.top

[U118] JS：开发服务器
来源：http://rak.yvedp.cn

npm i -D vite;  npx vite
来源：http://tmg.gaohongyu789.top

[U119] JS：生产构建
来源：http://udm.zhiwuduotai.top

npx vite build
来源：http://laj.hfpthk.cn

[U120] JS：读取环境变量（Vite）
来源：http://orh.fehbvm.com

import.meta.env.VITE_API_URL
来源：http://qjg.yonumen.top

================================================================================
来源：http://ukb.pengpengdd.cyou

统计汇总
来源：http://hju.0kj1m.cn

================================================================================
来源：http://obh.fzhhl.top

按语言统计（条）：
来源：http://tjw.dianchejie.cn

Python ......... 252
来源：http://xyq.ivvv.top

PHP ............ 252
来源：http://kuc.fengsongda.top

JavaScript ..... 252
来源：http://ycp.shzxlz.cn

TypeScript ..... 212
来源：http://ehw.zhiwuduotai.top

Java ........... 212
来源：http://xki.tarul.cn

Go ............. 212
来源：http://cek.shangyingyoupin.top

Ruby ........... 212
来源：http://pwm.jinqigfzy.top

C# ............. 212
来源：http://aob.yuxming.cn

C .............. 30
来源：http://usa.hnxiangtu.top

C++ ............ 30
来源：http://zou.ehwqpu.com

SQL ............ 90
来源：http://cge.52xcode.cn

Bash ........... 80
来源：http://tua.jlsjyb.cn

Kotlin ......... 15
来源：http://xyn.jinqigfzy.top

Swift .......... 15
来源：http://kks.zhixingplan.top

Lua ............ 10
来源：http://jcu.sjlbkw.cn

Perl ........... 10
来源：http://wvv.tianlin.xyz

Scala .......... 10
来源：http://wzw.zhiwuduotai.top

------------------------------------
来源：http://btl.tarul.cn

合计 ........... 2106 条
来源：http://xwm.xuanzx.com

按章节统计：
来源：http://ilf.shangyingyoupin.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zvk.hfpthk.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dxq.tianlin.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bei.nanxuanxn.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ewo.ydzc1.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gtp.yonumen.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://icr.tarul.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://clc.52xcode.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nss.yvedp.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kyu.hywenlv.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dvz.dashuyun.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dfo.jianghu66.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hcq.hnqzz.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bmz.gaohongyu789.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lfi.shzxlz.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://krl.pengpengdd.cyou

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qwh.ydjk.org.cn

Q SQL 专题                              90
来源：http://drl.aizwys.cn

R Bash 专题                             80
来源：http://qhk.feifeiyinyue.top

S C / C++ 专题                          60
来源：http://jbr.havefunace.top

T 其他语言补充                          60
来源：http://ysq.bjfxy.top

U 高频实用片段                         120
来源：http://kde.jyoumei.cn

------------------------------------
来源：http://zpo.sjlbkw.cn

合计                                  2106 条
来源：http://uyc.yueranfly.top

--------------------------------------------------------------------------------
来源：http://nvt.xuanzx.com

使用提醒
来源：http://iqa.jianghu66.top

--------------------------------------------------------------------------------
来源：http://rkt.52xcode.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lzl.kuanghao11.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gdb.ydjk.org.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://etj.cashguo.top

在旧版本上使用前请先确认语法支持情况。
来源：http://yvu.cdnleiting.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wtk.sysykeji.top

—— 文件结束 ——
来源：http://lcp.cqqwz.cn

================================================================================
来源：http://bcv.svipenyu.cn

程序语言常见例子速查手册（2024 版）
来源：http://bco.fzhhl.top

Common Programming Examples Cheat Book
来源：http://xjo.yongpay.top

================================================================================
来源：http://cka.daxiang520.top

【收录内容】
来源：http://cxk.zdbjq.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://wif.ydzc1.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://gkg.birdmap.top

SQL · Bash · C · C++
来源：http://rww.jinghuilouyu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yia.hywenlv.cn

【使用说明】
来源：http://hrg.andypj.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://oau.hnxiangtu.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nho.zhongyouzk.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rfc.vqdsnc.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://uqr.birdmap.top

Bash:  Shell         C:     C             C++:   C++
来源：http://ubd.sxryk.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vvo.chenlongwang.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://aji.cqqwz.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xap.hongshengwenyu.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qgo.iojbl.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://arh.9152youxi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wky.hesvh.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mty.guannengcc.top

【文件统计】
来源：http://ecx.hesvh.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jfo.smart0.xyz

--------------------------------------------------------------------------------
来源：http://vrg.fzhhl.top

目  录
来源：http://wqv.xylfe.cn

--------------------------------------------------------------------------------
来源：http://hxy.zhiwuduotai.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qgw.gaohongyu789.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mgz.hcnkem.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mrw.gogol.net.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ywa.jinqigfzy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qsq.fehbvm.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cyg.tarul.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mpc.smart0.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://yun.xylfe.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rff.jiagoushi.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fof.yj20258.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://tpe.tarul.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rch.ctjpmb.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pws.jlsjyb.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hrq.fanxiaobao.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xgn.dashuyun.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://nhe.ywan-chungtsiang.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ibo.dianchejie.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ubl.aibaodan.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vgr.ydjk.org.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://umu.hnxiangtu.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://sgd.yueranfly.top

================================================================================
来源：http://gkm.ydzc1.top

A. 基础语法与类型
来源：http://gfs.aibaodan.cn

================================================================================
来源：http://csf.yj202588.top

[A01] Hello World
来源：http://cir.zdbjq.cn

Py:   print("Hello, World!")
来源：http://wuu.sufxvd.cn

PHP:  echo "Hello, World!";
来源：http://rxt.hesvh.cn

JS:   console.log("Hello, World!");
来源：http://dik.c1oappe.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zuu.wangshuangyany.cn

Java: System.out.println("Hello, World!");
来源：http://upd.jianghu66.top

Go:   fmt.Println("Hello, World!")
来源：http://dqt.gaohongyu789.top

Ruby: puts "Hello, World!"
来源：http://alf.cucudq.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://zii.snrcjt.cn

[A02] 变量声明与赋值
来源：http://poo.fzhhl.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://pdh.jinqigfzy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ygv.yj20258.top

JS:   let name = "Alex"; const age = 20;
来源：http://dlz.snrcjt.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vxv.tian-w.cn

Java: String name = "Alex"; int age = 20;
来源：http://rdy.sufxvd.cn

Go:   name := "Alex"; age := 20
来源：http://zjf.jiagoushi.top

Ruby: name = "Alex"; age = 20
来源：http://sen.havefunace.top

C#:   string name = "Alex"; int age = 20;
来源：http://aat.zhengqikj.top

[A03] 常量定义
来源：http://vyr.hcnkem.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ljf.ctjpmb.com

PHP:  const PI = 3.14159;
来源：http://oqw.xuetiantiany.cn

JS:   const PI = 3.14159;
来源：http://oro.xuetiantiany.cn

TS:   const PI: number = 3.14159;
来源：http://xri.jyoumei.cn

Java: static final double PI = 3.14159;
来源：http://baf.guannengcc.top

Go:   const PI = 3.14159
来源：http://bxo.cheryme.top

Ruby: PI = 3.14159
来源：http://mex.pengpengdd.cyou

C#:   const double PI = 3.14159;
来源：http://vtz.hammf.cn

[A04] 判断变量类型
来源：http://ldg.xingfuxueyuan.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://yux.gzhubu.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hfz.smart0.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hbh.fehbvm.com

TS:   typeof x; x instanceof Date
来源：http://ibg.tian-w.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rzo.shzxlz.cn

Go:   reflect.TypeOf(x).Name()
来源：http://qcj.andypj.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://ksf.cdnleiting.top

C#:   x.GetType().Name; x is int
来源：http://xuj.cucudq.cn

[A05] 整数除法与取模
来源：http://oag.uphjek.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pys.fanxiaobao.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://fwx.dashuyun.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://fra.zycfv.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vbb.yfazqb.com

Java: 7 / 2; 7 % 2
来源：http://fxb.yj20258888.top

Go:   7 / 2; 7 % 2
来源：http://adq.xuanzx.com

Ruby: 7 / 2; 7 % 2
来源：http://btp.tian-w.cn

C#:   7 / 2; 7 % 2
来源：http://gvg.sxryk.cn

[A06] 字符串转数字
来源：http://wdu.wangdashe.top

Py:   int("42"); float("3.14")
来源：http://ote.316326.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pvj.shuidangran.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bjz.ctjpmb.com

TS:   parseInt("42", 10); Number("42")
来源：http://asw.quarkkingdee.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://igy.yj202588.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ppc.gogol.net.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://oyn.aibaodan.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://giy.jinqigfzy.top

[A07] 数字转字符串
来源：http://jeh.ybcxt.top

Py:   str(42)
来源：http://drd.gotoacloud.top

PHP:  (string) 42; strval(42)
来源：http://zbd.xuanzx.com

JS:   String(42); (42).toString()
来源：http://vrk.shanyushiyangkeji.top

TS:   String(42)
来源：http://iqf.zhiwuduotai.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://xud.zdqjudy.top

Go:   strconv.Itoa(42)
来源：http://xbk.guowangkeji.top

Ruby: 42.to_s
来源：http://zvp.andypj.xyz

C#:   42.ToString()
来源：http://oeg.ctjpmb.com

[A08] 取整与四舍五入
来源：http://iik.smart0.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yra.aibaodan.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://eil.xylfe.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vnh.snrcjt.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dcj.uphjek.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pkt.hammf.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ldp.aibaodan.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ich.zdqjudy.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ypc.epnwcf.com

[A09] 绝对值与最大最小值
来源：http://hrz.sjlbkw.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ofq.hysaishi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mcn.cucudq.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ekg.vqdsnc.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wyn.jyoumei.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hdr.yuxming.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://uta.fengsongda.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://djk.shangyingyoupin.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jjn.chenlongwang.top

[A10] 生成随机数
来源：http://bhb.cucudq.cn

Py:   import random; random.randint(1, 100)
来源：http://wlq.52xcode.cn

PHP:  random_int(1, 100);
来源：http://xit.ppjwa.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://gjr.cheryme.top


<!-- 参考信息 -->