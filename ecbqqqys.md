代发 wailian999

[U65] PHP：会话
来源：http://ocg.hesvh.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ljs.xinyue.icu

[U66] PHP：设置 Cookie
来源：http://apd.xinyue.icu

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pgi.xylfe.cn

[U67] PHP：处理文件上传
来源：http://eyr.bjfxy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://iya.mhx1999.top

[U68] PHP：PDO 连接
来源：http://npr.yongpay.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fwk.ivvv.top

[U69] PHP：PDO 预处理
来源：http://ifu.jinqigufen.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jap.zhijiandao.cn

[U70] PHP：PDO 事务
来源：http://nhr.zhoulong.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bop.jianghu66.top

[U71] PHP：抛出异常
来源：http://evo.jyoumei.cn

throw new RuntimeException("失败", 500);
来源：http://pny.aibaodan.cn

[U72] PHP：写错误日志
来源：http://rra.meibo888.top

error_log("失败: " . $e->getMessage());
来源：http://bjn.fzhhl.top

[U73] PHP：读取 ini 配置
来源：http://gcy.zdqjudy.top

parse_ini_file("config.ini", true)
来源：http://jcm.xinyue.icu

[U74] PHP：读取环境变量
来源：http://ssd.cqqwz.cn

getenv("APP_ENV") ?: "production"
来源：http://rag.daria6918.cn

[U75] PHP：依赖注入
来源：http://pkh.gotoacloud.top

composer require psr/container
来源：http://mvf.ydjk.org.cn

[U76] PHP：简单路由
来源：http://whe.jlsjyb.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cni.ybcxt.top

[U77] PHP：模板渲染
来源：http://asi.cheryme.top

composer require twig/twig
来源：http://xmj.dashuyun.cn

[U78] PHP：单元测试
来源：http://usw.ctjpmb.com

composer require --dev phpunit/phpunit
来源：http://gmp.epnwcf.com

[U79] PHP：静态分析
来源：http://hxi.yangfankeji.com

composer require --dev phpstan/phpstan
来源：http://gsf.sxryk.cn

[U80] PHP：代码规范修复
来源：http://bpc.jinyuanbaomall.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ppw.xinyue.icu

[U81] JS：初始化项目
来源：http://rsg.xuetiantiany.cn

npm init -y;  npm i express
来源：http://ojz.gaohongyu789.top

[U82] JS：package.json 脚本
来源：http://izw.yangfankeji.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ilh.gaohongyu789.top

[U83] JS：ES Module 导入导出
来源：http://tul.nanxuanxn.top

export const a = 1;  import { a } from "./m.js";
来源：http://bnw.shuidangran.top

[U84] JS：CommonJS 写法
来源：http://ytd.fzhhl.top

module.exports = { a };  const { a } = require("./m");
来源：http://mfe.cucudq.cn

[U85] JS：可选链
来源：http://fxa.tian-w.cn

a?.b?.c
来源：http://vip.zhaomingkeji.xyz

[U86] JS：空值合并
来源：http://tva.ctjpmb.com

a ?? b
来源：http://dso.cucudq.cn

[U87] JS：解构默认值
来源：http://iit.yj20258888.top

const { a = 1, b = 2 } = obj;
来源：http://sfg.iojbl.cn

[U88] JS：对象展开合并
来源：http://fcg.fktsv.cn

{ ...a, ...b }
来源：http://zqb.chenjidiqi.icu

[U89] JS：数组去重
来源：http://cop.cqqwz.cn

[...new Set(arr)]
来源：http://ogh.feifeiyinyue.top

[U90] JS：数字数组排序
来源：http://xcl.ehwqpu.com

[...arr].sort((a, b) => a - b)
来源：http://kiw.yj20258888.top

[U91] JS：对象键值遍历
来源：http://vpm.hnxiangtu.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dwr.52xcode.cn

[U92] JS：深拷贝
来源：http://iui.yanxiufei.cn

structuredClone(obj)
来源：http://ykc.xingfuxueyuan.xyz

[U93] JS：模板字符串
来源：http://moy.yonumen.top

`共 ${n} 条`
来源：http://sie.jianghu66.top

[U94] JS：箭头函数
来源：http://biu.tian-w.cn

const double = x => x * 2;
来源：http://zju.jyoumei.cn

[U95] JS：Promise 包装
来源：http://qmz.snrcjt.cn

new Promise((resolve, reject) => {})
来源：http://unc.zycfv.cn

[U96] JS：async/await 与异常
来源：http://cga.nwbrower.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xzy.snrcjt.cn

[U97] JS：并发请求
来源：http://mza.cheryme.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://mba.iojbl.cn

[U98] JS：fetch 带 JSON
来源：http://lvz.vehdjk.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xrs.hnxiangtu.top

[U99] JS：事件监听
来源：http://nbd.epnwcf.com

el.addEventListener("click", e => {})
来源：http://cnt.yonumen.top

[U100] JS：DOM 查询
来源：http://ozc.vehdjk.com

document.querySelector(".item")
来源：http://rii.jinghuilouyu.cn

[U101] JS：classList 操作
来源：http://xcd.fzhhl.top

el.classList.toggle("active")
来源：http://eha.yvedp.cn

[U102] JS：本地存储
来源：http://kth.shuidangran.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://rvr.shanyushiyangtech.top

[U103] JS：定时器
来源：http://ajz.zhiwuduotai.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ops.hcnkem.com

[U104] JS：防抖
来源：http://hzd.fehbvm.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ajc.yj20258.top

[U105] JS：节流
来源：http://fwv.gaohongyu789.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://brp.hnqzz.top

[U106] JS：日期格式化
来源：http://idd.yuxming.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lpf.hesvh.cn

[U107] JS：数字千分位
来源：http://mgd.cashguo.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://igw.iojbl.cn

[U108] JS：随机整数
来源：http://ysn.wangshuangyany.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://iox.zhaomingkeji.xyz

[U109] JS：数组分组
来源：http://yzk.chenlongwang.top

Object.groupBy(arr, x => x.type)
来源：http://nor.chenlongwang.top

[U110] JS：数组分块
来源：http://lgt.cashguo.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lgi.jyoumei.cn

[U111] JS：对象转 Map
来源：http://oyg.zhongyouzk.top

new Map(Object.entries(obj))
来源：http://abl.chenjidiqi.icu

[U112] JS：字符串补位
来源：http://pxq.gzhubu.top

"7".padStart(3, "0")
来源：http://bwy.andypj.xyz

[U113] JS：正则替换全部
来源：http://hla.hnxiangtu.top

s.replaceAll("a", "b")
来源：http://bxq.yj20258888.top

[U114] JS：JSON 深比较
来源：http://rfg.smart0.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://brp.shangyingyoupin.top

[U115] JS：生成 UUID
来源：http://lxm.guannengcc.top

crypto.randomUUID()
来源：http://vir.sufxvd.cn

[U116] JS：类型检查（JSDoc）
来源：http://iee.zhijiandao.cn

/** @param {string} name */ function f(name) {}
来源：http://qbm.cqqwz.cn

[U117] JS：单元测试
来源：http://mof.hesvh.cn

npm i -D vitest;  npx vitest
来源：http://vtp.sufxvd.cn

[U118] JS：开发服务器
来源：http://tzm.svipenyu.cn

npm i -D vite;  npx vite
来源：http://jrs.xingfuxueyuan.xyz

[U119] JS：生产构建
来源：http://zzf.gzhubu.top

npx vite build
来源：http://gpn.shzxlz.cn

[U120] JS：读取环境变量（Vite）
来源：http://zvz.tanke756.top

import.meta.env.VITE_API_URL
来源：http://xnl.zhijiandao.cn

================================================================================
来源：http://dqy.gaohongyu789.top

统计汇总
来源：http://pcz.zhiwuduotai.top

================================================================================
来源：http://rqc.yj20258888.top

按语言统计（条）：
来源：http://ywl.sweek.top

Python ......... 252
来源：http://lfh.yuanzhike.top

PHP ............ 252
来源：http://scu.ehwqpu.com

JavaScript ..... 252
来源：http://ube.feifeiyinyue.top

TypeScript ..... 212
来源：http://lje.0kj1m.cn

Java ........... 212
来源：http://aun.zhaomingkeji.xyz

Go ............. 212
来源：http://pge.hesvh.cn

Ruby ........... 212
来源：http://twk.yfazqb.com

C# ............. 212
来源：http://zhz.yueranfly.top

C .............. 30
来源：http://gon.dianchejie.cn

C++ ............ 30
来源：http://ugg.ivvv.top

SQL ............ 90
来源：http://eyc.jiagoushi.top

Bash ........... 80
来源：http://utf.xinyue.icu

Kotlin ......... 15
来源：http://fdx.ivvv.top

Swift .......... 15
来源：http://tsa.sysykeji.top

Lua ............ 10
来源：http://nix.havefunace.top

Perl ........... 10
来源：http://cnt.vqdsnc.cn

Scala .......... 10
来源：http://smw.xuanzx.com

------------------------------------
来源：http://weq.yj20258.top

合计 ........... 2106 条
来源：http://bcx.epnwcf.com

按章节统计：
来源：http://nvu.iojbl.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rid.jinqigfzy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bls.cqqwz.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ktg.tianlin.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://new.sxryk.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gro.jiagoushi.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zuz.bbcook.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zcu.shangyingyoupin.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rvs.bbcook.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pbb.sweek.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jbv.guowangkeji.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://obx.cashguo.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://evp.pycfn.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yxg.kuanghao11.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rtw.nwbrower.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ovq.nanxinkj.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qju.shuidangran.top

Q SQL 专题                              90
来源：http://hty.yanxiufei.cn

R Bash 专题                             80
来源：http://gbh.xingfuxueyuan.xyz

S C / C++ 专题                          60
来源：http://hvo.ywan-chungtsiang.top

T 其他语言补充                          60
来源：http://ilq.zhijiandao.cn

U 高频实用片段                         120
来源：http://ruq.havefunace.top

------------------------------------
来源：http://iyh.pycfn.com

合计                                  2106 条
来源：http://sau.52xcode.cn

--------------------------------------------------------------------------------
来源：http://fsd.fanxiaobao.xyz

使用提醒
来源：http://kbj.jqgfzy.top

--------------------------------------------------------------------------------
来源：http://mxt.snrcjt.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zml.zhoulong.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://sda.xuanzx.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lap.ybcxt.top

在旧版本上使用前请先确认语法支持情况。
来源：http://rgp.smart0.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xyc.quarkkingdee.top

—— 文件结束 ——
来源：http://ggu.kuanghao11.cn

================================================================================
来源：http://kbi.ywan-chungtsiang.top

程序语言常见例子速查手册（2024 版）
来源：http://gmi.jqgufenzy.top

Common Programming Examples Cheat Book
来源：http://nnt.tian-w.cn

================================================================================
来源：http://zdi.zhoulong.xyz

【收录内容】
来源：http://iyq.jiagoushi.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://hjn.shanyushiyangkeji.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://eqw.haohaochexian.top

SQL · Bash · C · C++
来源：http://kwb.zdqjudy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://bcz.gaohongyu789.top

【使用说明】
来源：http://hzp.fanxiaobao.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tzb.wangdashe.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ouo.daxiang520.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ybj.gzhubu.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jxl.sxryk.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://twa.zhaomingkeji.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nhe.shanyushiyangtech.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://dlx.haohaochexian.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mtw.sufxvd.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://oga.nanxuanxn.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qyi.fzhhl.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://acv.ybcxt.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zwh.wangdashe.top

【文件统计】
来源：http://pwb.fzhhl.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fgh.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://ubv.xingfuxueyuan.xyz

目  录
来源：http://bpy.mhx1999.top

--------------------------------------------------------------------------------
来源：http://ypy.jqgufenzy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xay.yongpay.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hla.shangyingyoupin.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://prk.316326.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://sma.fktsv.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bip.bjfxy.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vhe.hnqzz.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://iha.iojbl.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://spr.zdqjudy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zlm.pycfn.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rfi.pycfn.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zpr.xuetiantiany.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://nfl.dashuyun.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gip.ctjpmb.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bhm.sjlbkw.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ckr.birdmap.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bvs.bjfxy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jlv.meibo888.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ucx.hammf.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xoi.jinqigfzy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dmy.epnwcf.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://tgi.xylfe.cn

================================================================================
来源：http://yji.shanyushiyangkeji.top

A. 基础语法与类型
来源：http://tsw.pengpengdd.cyou

================================================================================
来源：http://rof.ivvv.top

[A01] Hello World
来源：http://ppd.fzhhl.top

Py:   print("Hello, World!")
来源：http://wox.0kj1m.cn

PHP:  echo "Hello, World!";
来源：http://lky.yj202588.top

JS:   console.log("Hello, World!");
来源：http://efs.sufxvd.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mcr.epnwcf.com

Java: System.out.println("Hello, World!");
来源：http://ddc.kuanghao11.cn

Go:   fmt.Println("Hello, World!")
来源：http://usy.ppjwa.cn

Ruby: puts "Hello, World!"
来源：http://dqa.jqgfzy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://yte.hnqzz.top

[A02] 变量声明与赋值
来源：http://hvc.yfazqb.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fpr.ybcxt.top

PHP:  $name = "Alex"; $age = 20;
来源：http://uia.xuanzx.com

JS:   let name = "Alex"; const age = 20;
来源：http://cqq.xziqi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jkt.shangyingyoupin.top

Java: String name = "Alex"; int age = 20;
来源：http://bxm.chenjidiqi.icu

Go:   name := "Alex"; age := 20
来源：http://zrp.pengpengdd.cyou

Ruby: name = "Alex"; age = 20
来源：http://nig.ppjwa.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ofm.c1oappe.top

[A03] 常量定义
来源：http://uvz.hammf.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://abb.tian-w.cn

PHP:  const PI = 3.14159;
来源：http://xrr.0kj1m.cn

JS:   const PI = 3.14159;
来源：http://qba.gaohongyu789.top

TS:   const PI: number = 3.14159;
来源：http://yxq.cdnleiting.top

Java: static final double PI = 3.14159;
来源：http://drc.sysykeji.top

Go:   const PI = 3.14159
来源：http://omf.yj202588.top

Ruby: PI = 3.14159
来源：http://tob.ppjwa.cn

C#:   const double PI = 3.14159;
来源：http://luk.chenjidiqi.icu

[A04] 判断变量类型
来源：http://zwe.fktsv.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://qyg.hnqzz.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://cmz.gotoacloud.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hmw.birdmap.top

TS:   typeof x; x instanceof Date
来源：http://myz.iojbl.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://nck.ppjwa.cn

Go:   reflect.TypeOf(x).Name()
来源：http://evy.yanxiufei.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://enj.daxiang520.top

C#:   x.GetType().Name; x is int
来源：http://gdj.xuanzx.com

[A05] 整数除法与取模
来源：http://wfi.nwbrower.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://opd.jinyuanbaomall.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ppk.yj20258888.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://kcu.nanxuanxn.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zln.cashguo.top

Java: 7 / 2; 7 % 2
来源：http://wza.nanxuanxn.top

Go:   7 / 2; 7 % 2
来源：http://gvy.nanxinkj.top

Ruby: 7 / 2; 7 % 2
来源：http://lia.sjlbkw.cn

C#:   7 / 2; 7 % 2
来源：http://pes.ydjk.org.cn

[A06] 字符串转数字
来源：http://pag.bbcook.cn

Py:   int("42"); float("3.14")
来源：http://zei.ivvv.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://asp.birdmap.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vhv.gzhubu.top

TS:   parseInt("42", 10); Number("42")
来源：http://roo.nwbrower.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mcs.zhixingplan.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yzz.hesvh.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://xzo.tarul.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rwy.shanyushiyangkeji.top

[A07] 数字转字符串
来源：http://oae.aizwys.cn

Py:   str(42)
来源：http://sdl.feifeiyinyue.top

PHP:  (string) 42; strval(42)
来源：http://sgg.vqdsnc.cn

JS:   String(42); (42).toString()
来源：http://myj.shangyingyoupin.top

TS:   String(42)
来源：http://oyk.vehdjk.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://toa.daxiang520.top

Go:   strconv.Itoa(42)
来源：http://xwy.yangfankeji.com

Ruby: 42.to_s
来源：http://wat.c1oappe.top

C#:   42.ToString()
来源：http://irq.shzxlz.cn

[A08] 取整与四舍五入
来源：http://lxh.havefunace.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gsy.birdmap.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://czv.aibaodan.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://oxe.snrcjt.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nnh.hammf.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ayy.gotoacloud.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vzl.shanyushiyangtech.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://cyx.yueranfly.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rxg.xziqi.cn

[A09] 绝对值与最大最小值
来源：http://bqw.tarul.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://aru.meibo888.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://lnm.guannengcc.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://lpu.ybcxt.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://dnp.svipenyu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tdm.chenjidiqi.icu

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ops.dashuyun.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ndt.jinghuilouyu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ope.jinghuilouyu.cn


<!-- 参考信息 -->