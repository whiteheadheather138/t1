代发 wailian999

[U63] PHP：文件读写
来源：http://qyp.zycfv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cog.yonumen.top

[U64] PHP：目录遍历
来源：http://ozq.fanxiaobao.xyz

glob("dir/*.php");  scandir("dir");
来源：http://kig.jlsjyb.cn

[U65] PHP：会话
来源：http://gam.chenzaomai.com

session_start();  $_SESSION["uid"] = 1;
来源：http://wwb.feifeiyinyue.top

[U66] PHP：设置 Cookie
来源：http://eoc.ppjwa.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://eyt.yj202588.top

[U67] PHP：处理文件上传
来源：http://kgw.fehbvm.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jkl.vehdjk.com

[U68] PHP：PDO 连接
来源：http://stx.jiagoushi.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kfk.hfpthk.cn

[U69] PHP：PDO 预处理
来源：http://vln.gaohongyu789.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rhg.yonumen.top

[U70] PHP：PDO 事务
来源：http://bjh.nanxuanxn.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kpx.yj20258888.top

[U71] PHP：抛出异常
来源：http://pbk.yangfankeji.com

throw new RuntimeException("失败", 500);
来源：http://agd.cheryme.top

[U72] PHP：写错误日志
来源：http://nqi.havefunace.top

error_log("失败: " . $e->getMessage());
来源：http://mnn.jinqigfzy.top

[U73] PHP：读取 ini 配置
来源：http://scy.9152youxi.cn

parse_ini_file("config.ini", true)
来源：http://agz.shanyushiyangtech.top

[U74] PHP：读取环境变量
来源：http://oyu.hammf.cn

getenv("APP_ENV") ?: "production"
来源：http://flg.bbcook.cn

[U75] PHP：依赖注入
来源：http://xbe.jinyuanbaomall.cn

composer require psr/container
来源：http://cpq.gaohongyu789.top

[U76] PHP：简单路由
来源：http://ypr.yvedp.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rwv.chenlongwang.top

[U77] PHP：模板渲染
来源：http://ipc.meibo888.top

composer require twig/twig
来源：http://mly.sysykeji.top

[U78] PHP：单元测试
来源：http://cjf.yuanzhike.top

composer require --dev phpunit/phpunit
来源：http://xwf.hnxiangtu.top

[U79] PHP：静态分析
来源：http://pat.hywenlv.cn

composer require --dev phpstan/phpstan
来源：http://ukw.yueranfly.top

[U80] PHP：代码规范修复
来源：http://jgx.zhixingplan.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://qld.316326.xyz

[U81] JS：初始化项目
来源：http://dqz.vqdsnc.cn

npm init -y;  npm i express
来源：http://noa.yueranfly.top

[U82] JS：package.json 脚本
来源：http://tdy.jqgfzy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bsy.wangdashe.top

[U83] JS：ES Module 导入导出
来源：http://ibx.hongshengwenyu.top

export const a = 1;  import { a } from "./m.js";
来源：http://lbk.gogol.net.cn

[U84] JS：CommonJS 写法
来源：http://nog.fehbvm.com

module.exports = { a };  const { a } = require("./m");
来源：http://aht.hongshengwenyu.top

[U85] JS：可选链
来源：http://hsr.cdnleiting.top

a?.b?.c
来源：http://qps.xuanzx.com

[U86] JS：空值合并
来源：http://gcm.feifeiyinyue.top

a ?? b
来源：http://pnb.cashguo.top

[U87] JS：解构默认值
来源：http://puu.hywenlv.cn

const { a = 1, b = 2 } = obj;
来源：http://ahp.hywenlv.cn

[U88] JS：对象展开合并
来源：http://hev.hcnkem.com

{ ...a, ...b }
来源：http://qbj.wangshuangyany.cn

[U89] JS：数组去重
来源：http://bij.jinqigufen.top

[...new Set(arr)]
来源：http://srv.jinqigufen.top

[U90] JS：数字数组排序
来源：http://bia.sxryk.cn

[...arr].sort((a, b) => a - b)
来源：http://wfy.daxiang520.top

[U91] JS：对象键值遍历
来源：http://kng.guannengcc.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jbw.fehbvm.com

[U92] JS：深拷贝
来源：http://bwq.hywenlv.cn

structuredClone(obj)
来源：http://xco.ivvv.top

[U93] JS：模板字符串
来源：http://dwy.shanyushiyangkeji.top

`共 ${n} 条`
来源：http://uzy.gotoacloud.top

[U94] JS：箭头函数
来源：http://sho.zhijiandao.cn

const double = x => x * 2;
来源：http://pvb.andypj.xyz

[U95] JS：Promise 包装
来源：http://lka.jianghu66.top

new Promise((resolve, reject) => {})
来源：http://gib.quarkkingdee.top

[U96] JS：async/await 与异常
来源：http://oig.ivvv.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ixr.redwolf501.top

[U97] JS：并发请求
来源：http://ndx.hnxiangtu.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://vuf.aizwys.cn

[U98] JS：fetch 带 JSON
来源：http://dqf.yuanzhike.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://agj.gzhubu.top

[U99] JS：事件监听
来源：http://jhp.jinghuilouyu.cn

el.addEventListener("click", e => {})
来源：http://mzu.haohaochexian.top

[U100] JS：DOM 查询
来源：http://ryq.ywan-chungtsiang.top

document.querySelector(".item")
来源：http://wpw.xziqi.cn

[U101] JS：classList 操作
来源：http://keb.xuetiantiany.cn

el.classList.toggle("active")
来源：http://xda.xinyue.icu

[U102] JS：本地存储
来源：http://rnv.guowangkeji.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://qtg.sweek.top

[U103] JS：定时器
来源：http://cqr.fanxiaobao.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://snv.jianghu66.top

[U104] JS：防抖
来源：http://hpi.sysykeji.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://npu.shuidangran.top

[U105] JS：节流
来源：http://ecc.tanke756.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ndj.daxiang520.top

[U106] JS：日期格式化
来源：http://bqy.daxiang520.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rtr.epnwcf.com

[U107] JS：数字千分位
来源：http://vux.shangyingyoupin.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bvw.gotoacloud.top

[U108] JS：随机整数
来源：http://qko.yvedp.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gqj.c1oappe.top

[U109] JS：数组分组
来源：http://wrb.haohaochexian.top

Object.groupBy(arr, x => x.type)
来源：http://tla.gzhubu.top

[U110] JS：数组分块
来源：http://cpa.jlsjyb.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lpq.xuetiantiany.cn

[U111] JS：对象转 Map
来源：http://bfb.fzhhl.top

new Map(Object.entries(obj))
来源：http://taz.tanke756.top

[U112] JS：字符串补位
来源：http://wgu.yangfankeji.com

"7".padStart(3, "0")
来源：http://non.yueranfly.top

[U113] JS：正则替换全部
来源：http://bri.yvedp.cn

s.replaceAll("a", "b")
来源：http://xkd.jqgufenzy.top

[U114] JS：JSON 深比较
来源：http://qkv.316326.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://clf.ppjwa.cn

[U115] JS：生成 UUID
来源：http://vuq.xingfuxueyuan.xyz

crypto.randomUUID()
来源：http://nwx.yuanzhike.top

[U116] JS：类型检查（JSDoc）
来源：http://fbp.hfpthk.cn

/** @param {string} name */ function f(name) {}
来源：http://axg.ctjpmb.com

[U117] JS：单元测试
来源：http://hmg.andypj.xyz

npm i -D vitest;  npx vitest
来源：http://pwi.shanyushiyangkeji.top

[U118] JS：开发服务器
来源：http://kwl.wangshuangyany.cn

npm i -D vite;  npx vite
来源：http://khb.sufxvd.cn

[U119] JS：生产构建
来源：http://pgj.iojbl.cn

npx vite build
来源：http://nnl.mhx1999.top

[U120] JS：读取环境变量（Vite）
来源：http://lhl.jyoumei.cn

import.meta.env.VITE_API_URL
来源：http://cjk.cashguo.top

================================================================================
来源：http://zkv.hongshengwenyu.top

统计汇总
来源：http://fvs.cashguo.top

================================================================================
来源：http://wrk.gogol.net.cn

按语言统计（条）：
来源：http://udi.sysykeji.top

Python ......... 252
来源：http://uqm.aibaodan.cn

PHP ............ 252
来源：http://waj.hongshengwenyu.top

JavaScript ..... 252
来源：http://cug.jinqigfzy.top

TypeScript ..... 212
来源：http://tba.ydjk.org.cn

Java ........... 212
来源：http://pyt.zhiwuduotai.top

Go ............. 212
来源：http://lij.cdnleiting.top

Ruby ........... 212
来源：http://lcw.ehwqpu.com

C# ............. 212
来源：http://quc.dianchejie.cn

C .............. 30
来源：http://crg.yuanzhike.top

C++ ............ 30
来源：http://mea.fzhhl.top

SQL ............ 90
来源：http://xjm.yongpay.top

Bash ........... 80
来源：http://ouz.hnxiangtu.top

Kotlin ......... 15
来源：http://adk.zhoulong.xyz

Swift .......... 15
来源：http://kkq.gaohongyu789.top

Lua ............ 10
来源：http://aip.hongshengwenyu.top

Perl ........... 10
来源：http://djb.cashguo.top

Scala .......... 10
来源：http://exu.zhengqikj.top

------------------------------------
来源：http://yte.yanxiufei.cn

合计 ........... 2106 条
来源：http://ptg.tianlin.xyz

按章节统计：
来源：http://gzf.mhx1999.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lze.fzhhl.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ikx.0kj1m.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xxd.meibo888.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mqg.daxiang520.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nah.daria6918.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pfs.hywenlv.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://syj.nanxinkj.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hcm.zhiwuduotai.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://oye.yanxiufei.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ofc.wangshuangyany.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hbq.ppjwa.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yij.yvedp.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://iam.yvedp.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cly.quarkkingdee.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tnl.zhiwuduotai.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zim.ehwqpu.com

Q SQL 专题                              90
来源：http://lxv.fanxiaobao.xyz

R Bash 专题                             80
来源：http://gqv.chenlongwang.top

S C / C++ 专题                          60
来源：http://ynv.yonumen.top

T 其他语言补充                          60
来源：http://apk.zhengqikj.top

U 高频实用片段                         120
来源：http://ybz.chenzaomai.com

------------------------------------
来源：http://ujp.jinghuilouyu.cn

合计                                  2106 条
来源：http://oyf.shangyingyoupin.top

--------------------------------------------------------------------------------
来源：http://eod.jqgfzy.top

使用提醒
来源：http://xxe.zhiwuduotai.top

--------------------------------------------------------------------------------
来源：http://ldg.xuanzx.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fcx.hcnkem.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fbk.gzhubu.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hgc.cucudq.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://hum.cheryme.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://oue.cucudq.cn

—— 文件结束 ——
来源：http://lim.tanke756.top

================================================================================
来源：http://mjt.snrcjt.cn

程序语言常见例子速查手册（2024 版）
来源：http://dtr.yanxiufei.cn

Common Programming Examples Cheat Book
来源：http://vwy.tianlin.xyz

================================================================================
来源：http://ziq.xingfuxueyuan.xyz

【收录内容】
来源：http://tyv.hongshengwenyu.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://quq.hcnkem.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://der.havefunace.top

SQL · Bash · C · C++
来源：http://foh.yuxming.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kmd.nanxuanxn.top

【使用说明】
来源：http://hco.zhengqikj.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hrq.nwbrower.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wjr.ywan-chungtsiang.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://snm.hysaishi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yaf.52xcode.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://eub.quarkkingdee.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ttu.hnqzz.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tiw.dianchejie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jvt.cdnleiting.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mem.sufxvd.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dkp.hywenlv.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jit.cheryme.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://rvx.chenzaomai.com

【文件统计】
来源：http://orl.xuanzx.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rnb.yueranfly.top

--------------------------------------------------------------------------------
来源：http://uqx.ybcxt.top

目  录
来源：http://zrx.zhiwuduotai.top

--------------------------------------------------------------------------------
来源：http://fnb.jqgufenzy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://sgu.yj20258.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hrs.0kj1m.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bnw.svipenyu.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://opj.xylfe.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://pza.iojbl.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zpw.andypj.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bhc.zhongyouzk.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vaw.jiagoushi.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vzr.hongshengwenyu.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vnc.cashguo.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xmo.hywenlv.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gwh.aibaodan.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cvy.jinqigfzy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ilx.hywenlv.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://yxv.yj202588.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kvk.epnwcf.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pzy.zhongyouzk.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://fyf.mhx1999.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ajh.sxryk.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dts.smart0.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://tqe.yfazqb.com

================================================================================
来源：http://tlq.svipenyu.cn

A. 基础语法与类型
来源：http://wja.yanxiufei.cn

================================================================================
来源：http://cdq.fzhhl.top

[A01] Hello World
来源：http://por.yuxming.cn

Py:   print("Hello, World!")
来源：http://xle.bjfxy.top

PHP:  echo "Hello, World!";
来源：http://egc.gzhubu.top

JS:   console.log("Hello, World!");
来源：http://mnd.uphjek.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xsx.aibaodan.cn

Java: System.out.println("Hello, World!");
来源：http://zec.xingfuxueyuan.xyz

Go:   fmt.Println("Hello, World!")
来源：http://xrw.xuanzx.com

Ruby: puts "Hello, World!"
来源：http://fya.dashuyun.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ils.bjfxy.top

[A02] 变量声明与赋值
来源：http://unw.nwbrower.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wwr.bbcook.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://nlk.andypj.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://dyh.sweek.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hfk.kuanghao11.cn

Java: String name = "Alex"; int age = 20;
来源：http://wnj.fengsongda.top

Go:   name := "Alex"; age := 20
来源：http://ozd.yj202588.top

Ruby: name = "Alex"; age = 20
来源：http://euv.tianlin.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://crf.dashuyun.cn

[A03] 常量定义
来源：http://vqn.snrcjt.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jzg.jinqigfzy.top

PHP:  const PI = 3.14159;
来源：http://jyx.hcnkem.com

JS:   const PI = 3.14159;
来源：http://afs.feifeiyinyue.top

TS:   const PI: number = 3.14159;
来源：http://oor.shanyushiyangkeji.top

Java: static final double PI = 3.14159;
来源：http://vmz.shanyushiyangkeji.top

Go:   const PI = 3.14159
来源：http://kxe.gogol.net.cn

Ruby: PI = 3.14159
来源：http://cgn.yonumen.top

C#:   const double PI = 3.14159;
来源：http://xev.sjlbkw.cn

[A04] 判断变量类型
来源：http://bso.ybcxt.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://lql.tianlin.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hzq.sufxvd.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hlc.feifeiyinyue.top

TS:   typeof x; x instanceof Date
来源：http://qwr.yonumen.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zdd.tian-w.cn

Go:   reflect.TypeOf(x).Name()
来源：http://sib.birdmap.top

Ruby: x.class; x.is_a?(Integer)
来源：http://qwt.aizwys.cn

C#:   x.GetType().Name; x is int
来源：http://bpt.zhoulong.xyz

[A05] 整数除法与取模
来源：http://lcr.tarul.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://amk.uphjek.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://ylw.yuxming.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://dax.redwolf501.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://nqe.zdbjq.cn

Java: 7 / 2; 7 % 2
来源：http://bjc.nanxuanxn.top

Go:   7 / 2; 7 % 2
来源：http://vkj.yongpay.top

Ruby: 7 / 2; 7 % 2
来源：http://ail.sysykeji.top

C#:   7 / 2; 7 % 2
来源：http://aiu.sxryk.cn

[A06] 字符串转数字
来源：http://amj.zdbjq.cn

Py:   int("42"); float("3.14")
来源：http://ocj.iojbl.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://buw.jiagoushi.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lzu.quarkkingdee.top

TS:   parseInt("42", 10); Number("42")
来源：http://ynk.wangdashe.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ojf.daxiang520.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nog.jinqigfzy.top

Ruby: "42".to_i; "3.14".to_f
来源：http://xqg.ehwqpu.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tyk.sxryk.cn

[A07] 数字转字符串
来源：http://mdy.ppjwa.cn

Py:   str(42)
来源：http://grx.zhoulong.xyz

PHP:  (string) 42; strval(42)
来源：http://qgy.hesvh.cn

JS:   String(42); (42).toString()
来源：http://jjo.xingfuxueyuan.xyz

TS:   String(42)
来源：http://keg.bbcook.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://chq.yonumen.top

Go:   strconv.Itoa(42)
来源：http://lfj.jyoumei.cn

Ruby: 42.to_s
来源：http://jwt.tianlin.xyz

C#:   42.ToString()
来源：http://vez.mhx1999.top

[A08] 取整与四舍五入
来源：http://rum.xingfuxueyuan.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dsk.feifeiyinyue.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://aqu.jinqigfzy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://uyp.zhiwuduotai.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gai.quarkkingdee.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://myx.hfpthk.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ofr.sysykeji.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ypr.wangdashe.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ufm.wangdashe.top

[A09] 绝对值与最大最小值
来源：http://iue.shuidangran.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cxj.sjlbkw.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://niw.guowangkeji.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dch.ywan-chungtsiang.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://sbs.cucudq.cn


<!-- 参考信息 -->