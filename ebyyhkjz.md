代发 wailian999

[U61] PHP：正则
来源：http://fdk.hywenlv.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rzc.ywan-chungtsiang.top

[U62] PHP：日期对象
来源：http://pov.shuidangran.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jly.fktsv.cn

[U63] PHP：文件读写
来源：http://wbu.gogol.net.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yge.vqdsnc.cn

[U64] PHP：目录遍历
来源：http://bbj.sufxvd.cn

glob("dir/*.php");  scandir("dir");
来源：http://jli.zhaomingkeji.xyz

[U65] PHP：会话
来源：http://dcm.hnxiangtu.top

session_start();  $_SESSION["uid"] = 1;
来源：http://rxy.yj20258888.top

[U66] PHP：设置 Cookie
来源：http://ufz.bbcook.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vus.yangfankeji.com

[U67] PHP：处理文件上传
来源：http://lpk.xuetiantiany.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ryu.zhijiandao.cn

[U68] PHP：PDO 连接
来源：http://igx.jyoumei.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zxp.andypj.xyz

[U69] PHP：PDO 预处理
来源：http://nge.jinghuilouyu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ezd.hnxiangtu.top

[U70] PHP：PDO 事务
来源：http://abl.jinqigufen.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kjn.haohaochexian.top

[U71] PHP：抛出异常
来源：http://qmf.andypj.xyz

throw new RuntimeException("失败", 500);
来源：http://cmd.ydzc1.top

[U72] PHP：写错误日志
来源：http://nuj.hysaishi.cn

error_log("失败: " . $e->getMessage());
来源：http://pmd.zhoulong.xyz

[U73] PHP：读取 ini 配置
来源：http://cpw.haohaochexian.top

parse_ini_file("config.ini", true)
来源：http://upw.yfazqb.com

[U74] PHP：读取环境变量
来源：http://otn.tianlin.xyz

getenv("APP_ENV") ?: "production"
来源：http://zak.havefunace.top

[U75] PHP：依赖注入
来源：http://ald.zhongyouzk.top

composer require psr/container
来源：http://kkh.ctjpmb.com

[U76] PHP：简单路由
来源：http://ovm.vqdsnc.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://asc.fengsongda.top

[U77] PHP：模板渲染
来源：http://hbp.hnxiangtu.top

composer require twig/twig
来源：http://ens.bjfxy.top

[U78] PHP：单元测试
来源：http://dvc.svipenyu.cn

composer require --dev phpunit/phpunit
来源：http://igj.ivvv.top

[U79] PHP：静态分析
来源：http://nhj.shanyushiyangtech.top

composer require --dev phpstan/phpstan
来源：http://mrq.xinyue.icu

[U80] PHP：代码规范修复
来源：http://axw.xinyue.icu

composer require --dev friendsofphp/php-cs-fixer
来源：http://vjf.iojbl.cn

[U81] JS：初始化项目
来源：http://juk.wangdashe.top

npm init -y;  npm i express
来源：http://ffj.jiagoushi.top

[U82] JS：package.json 脚本
来源：http://etd.daxiang520.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qld.zdbjq.cn

[U83] JS：ES Module 导入导出
来源：http://gdh.0kj1m.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ppw.bjfxy.top

[U84] JS：CommonJS 写法
来源：http://boa.fehbvm.com

module.exports = { a };  const { a } = require("./m");
来源：http://dry.smart0.xyz

[U85] JS：可选链
来源：http://dpl.yfazqb.com

a?.b?.c
来源：http://nus.chenlongwang.top

[U86] JS：空值合并
来源：http://ffg.hcnkem.com

a ?? b
来源：http://pfg.ehwqpu.com

[U87] JS：解构默认值
来源：http://xzw.mhx1999.top

const { a = 1, b = 2 } = obj;
来源：http://nzc.yj20258.top

[U88] JS：对象展开合并
来源：http://euk.jinqigfzy.top

{ ...a, ...b }
来源：http://yld.shanyushiyangtech.top

[U89] JS：数组去重
来源：http://vul.gogol.net.cn

[...new Set(arr)]
来源：http://qwo.zhengqikj.top

[U90] JS：数字数组排序
来源：http://yte.zhiwuduotai.top

[...arr].sort((a, b) => a - b)
来源：http://snm.hongshengwenyu.top

[U91] JS：对象键值遍历
来源：http://reh.epnwcf.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hcq.xinyue.icu

[U92] JS：深拷贝
来源：http://fnl.cheryme.top

structuredClone(obj)
来源：http://kum.havefunace.top

[U93] JS：模板字符串
来源：http://ids.yueranfly.top

`共 ${n} 条`
来源：http://yae.zdbjq.cn

[U94] JS：箭头函数
来源：http://tho.hfpthk.cn

const double = x => x * 2;
来源：http://mya.0kj1m.cn

[U95] JS：Promise 包装
来源：http://pkb.cucudq.cn

new Promise((resolve, reject) => {})
来源：http://mde.fengsongda.top

[U96] JS：async/await 与异常
来源：http://ptn.kuanghao11.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zqj.cashguo.top

[U97] JS：并发请求
来源：http://pzv.sufxvd.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://tnd.sweek.top

[U98] JS：fetch 带 JSON
来源：http://neg.havefunace.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kbg.dianchejie.cn

[U99] JS：事件监听
来源：http://gfk.daxiang520.top

el.addEventListener("click", e => {})
来源：http://ows.snrcjt.cn

[U100] JS：DOM 查询
来源：http://nok.0kj1m.cn

document.querySelector(".item")
来源：http://gbp.sjlbkw.cn

[U101] JS：classList 操作
来源：http://qsn.9152youxi.cn

el.classList.toggle("active")
来源：http://rjk.epnwcf.com

[U102] JS：本地存储
来源：http://kid.quarkkingdee.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://zmi.cashguo.top

[U103] JS：定时器
来源：http://ljc.iojbl.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mcb.jianghu66.top

[U104] JS：防抖
来源：http://lfl.nanxuanxn.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tlu.cdnleiting.top

[U105] JS：节流
来源：http://oox.ydjk.org.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xdi.guannengcc.top

[U106] JS：日期格式化
来源：http://ifv.daria6918.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://clh.hongshengwenyu.top

[U107] JS：数字千分位
来源：http://jxz.yj202588.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dyo.wangshuangyany.cn

[U108] JS：随机整数
来源：http://kzp.yonumen.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jly.0kj1m.cn

[U109] JS：数组分组
来源：http://zwf.shangyingyoupin.top

Object.groupBy(arr, x => x.type)
来源：http://bgr.ivvv.top

[U110] JS：数组分块
来源：http://lhv.zhiwuduotai.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fis.quarkkingdee.top

[U111] JS：对象转 Map
来源：http://bqu.dashuyun.cn

new Map(Object.entries(obj))
来源：http://xwn.meibo888.top

[U112] JS：字符串补位
来源：http://vid.birdmap.top

"7".padStart(3, "0")
来源：http://pli.cheryme.top

[U113] JS：正则替换全部
来源：http://lxn.vehdjk.com

s.replaceAll("a", "b")
来源：http://tpu.pengpengdd.cyou

[U114] JS：JSON 深比较
来源：http://aws.uphjek.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://abk.cashguo.top

[U115] JS：生成 UUID
来源：http://cph.hongshengwenyu.top

crypto.randomUUID()
来源：http://clc.redwolf501.top

[U116] JS：类型检查（JSDoc）
来源：http://qgd.birdmap.top

/** @param {string} name */ function f(name) {}
来源：http://ota.bjfxy.top

[U117] JS：单元测试
来源：http://swf.ppjwa.cn

npm i -D vitest;  npx vitest
来源：http://uax.bjfxy.top

[U118] JS：开发服务器
来源：http://jsk.sweek.top

npm i -D vite;  npx vite
来源：http://wbx.sufxvd.cn

[U119] JS：生产构建
来源：http://wqc.tian-w.cn

npx vite build
来源：http://jtt.yj202588.top

[U120] JS：读取环境变量（Vite）
来源：http://pms.smart0.xyz

import.meta.env.VITE_API_URL
来源：http://oet.hnxiangtu.top

================================================================================
来源：http://ewo.andypj.xyz

统计汇总
来源：http://qlz.yj20258888.top

================================================================================
来源：http://ddm.ctjpmb.com

按语言统计（条）：
来源：http://jcz.daria6918.cn

Python ......... 252
来源：http://rpv.yuanzhike.top

PHP ............ 252
来源：http://hxj.kuanghao11.cn

JavaScript ..... 252
来源：http://tyv.ydzc1.top

TypeScript ..... 212
来源：http://zng.jiagoushi.top

Java ........... 212
来源：http://eek.svipenyu.cn

Go ............. 212
来源：http://acs.havefunace.top

Ruby ........... 212
来源：http://yap.zhijiandao.cn

C# ............. 212
来源：http://fci.iojbl.cn

C .............. 30
来源：http://nvb.c1oappe.top

C++ ............ 30
来源：http://rxn.xziqi.cn

SQL ............ 90
来源：http://wnd.xinyue.icu

Bash ........... 80
来源：http://qpl.jinyuanbaomall.cn

Kotlin ......... 15
来源：http://xpd.cucudq.cn

Swift .......... 15
来源：http://uta.bbcook.cn

Lua ............ 10
来源：http://yhl.nanxinkj.top

Perl ........... 10
来源：http://ydr.yj202588.top

Scala .......... 10
来源：http://scb.xuetiantiany.cn

------------------------------------
来源：http://ohf.vqdsnc.cn

合计 ........... 2106 条
来源：http://alv.havefunace.top

按章节统计：
来源：http://hfo.cucudq.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wzo.bjfxy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wqh.hnqzz.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hdo.ctjpmb.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://szb.vehdjk.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dmx.9152youxi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lso.ctjpmb.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gsm.wangdashe.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wxm.guowangkeji.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nrs.ivvv.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nuf.gotoacloud.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lxd.xziqi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fxg.daxiang520.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hab.jinghuilouyu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://uci.chenzaomai.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ynb.gzhubu.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ktf.bjfxy.top

Q SQL 专题                              90
来源：http://kek.jiagoushi.top

R Bash 专题                             80
来源：http://adc.svipenyu.cn

S C / C++ 专题                          60
来源：http://rxr.vqdsnc.cn

T 其他语言补充                          60
来源：http://hvb.guowangkeji.top

U 高频实用片段                         120
来源：http://kyn.vqdsnc.cn

------------------------------------
来源：http://ssf.epnwcf.com

合计                                  2106 条
来源：http://vgx.fzhhl.top

--------------------------------------------------------------------------------
来源：http://nfw.gogol.net.cn

使用提醒
来源：http://qny.cucudq.cn

--------------------------------------------------------------------------------
来源：http://tyi.sxryk.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ukq.ydjk.org.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rkh.xziqi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xus.zhengqikj.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ajy.zhiwuduotai.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://tiz.fanxiaobao.xyz

—— 文件结束 ——
来源：http://srh.cdnleiting.top

================================================================================
来源：http://waj.cqqwz.cn

程序语言常见例子速查手册（2024 版）
来源：http://iyj.fengsongda.top

Common Programming Examples Cheat Book
来源：http://pgm.52xcode.cn

================================================================================
来源：http://ntc.hnxiangtu.top

【收录内容】
来源：http://tfr.zhengqikj.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://hyd.xziqi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hyc.feifeiyinyue.top

SQL · Bash · C · C++
来源：http://qpa.birdmap.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tvp.jianghu66.top

【使用说明】
来源：http://ivz.kuanghao11.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vez.fanxiaobao.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mwx.nanxuanxn.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nfz.quarkkingdee.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rsd.vqdsnc.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://xej.fzhhl.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rqs.shangyingyoupin.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xhh.gaohongyu789.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ekf.cqqwz.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://crt.redwolf501.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://toa.hesvh.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mrq.sysykeji.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pyt.xingfuxueyuan.xyz

【文件统计】
来源：http://nub.shanyushiyangkeji.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://eed.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://iao.zhaomingkeji.xyz

目  录
来源：http://qdy.wangdashe.top

--------------------------------------------------------------------------------
来源：http://wfv.chenzaomai.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vod.fktsv.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zpf.tian-w.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://euv.jinyuanbaomall.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://nya.yanxiufei.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://clk.shuidangran.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lfs.cashguo.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jgt.gotoacloud.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://sbi.xuetiantiany.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://eej.iojbl.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xko.yj20258888.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ept.shuidangran.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pjy.yj202588.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xcy.zhijiandao.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mak.iojbl.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://sko.bbcook.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vsg.zhongyouzk.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pna.cdnleiting.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://qpu.kuanghao11.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qgr.smart0.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rsl.jinyuanbaomall.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mdc.yangfankeji.com

================================================================================
来源：http://edj.ydjk.org.cn

A. 基础语法与类型
来源：http://rib.jyoumei.cn

================================================================================
来源：http://rso.jianghu66.top

[A01] Hello World
来源：http://egn.guowangkeji.top

Py:   print("Hello, World!")
来源：http://kij.jyoumei.cn

PHP:  echo "Hello, World!";
来源：http://yso.jinqigfzy.top

JS:   console.log("Hello, World!");
来源：http://znd.daria6918.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://sse.tian-w.cn

Java: System.out.println("Hello, World!");
来源：http://oyg.yueranfly.top

Go:   fmt.Println("Hello, World!")
来源：http://lyf.jyoumei.cn

Ruby: puts "Hello, World!"
来源：http://jpb.ywan-chungtsiang.top

C#:   Console.WriteLine("Hello, World!");
来源：http://khr.xuetiantiany.cn

[A02] 变量声明与赋值
来源：http://luv.ivvv.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://pyq.ehwqpu.com

PHP:  $name = "Alex"; $age = 20;
来源：http://qic.meibo888.top

JS:   let name = "Alex"; const age = 20;
来源：http://lhi.bbcook.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xen.uphjek.com

Java: String name = "Alex"; int age = 20;
来源：http://rma.snrcjt.cn

Go:   name := "Alex"; age := 20
来源：http://fwb.shangyingyoupin.top

Ruby: name = "Alex"; age = 20
来源：http://cvl.tanke756.top

C#:   string name = "Alex"; int age = 20;
来源：http://qoi.guannengcc.top

[A03] 常量定义
来源：http://taa.sxryk.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://upa.cdnleiting.top

PHP:  const PI = 3.14159;
来源：http://gjh.cqqwz.cn

JS:   const PI = 3.14159;
来源：http://mtg.daria6918.cn

TS:   const PI: number = 3.14159;
来源：http://iwd.chenlongwang.top

Java: static final double PI = 3.14159;
来源：http://iqm.redwolf501.top

Go:   const PI = 3.14159
来源：http://rsj.yueranfly.top

Ruby: PI = 3.14159
来源：http://mhy.iojbl.cn

C#:   const double PI = 3.14159;
来源：http://vdl.haohaochexian.top

[A04] 判断变量类型
来源：http://dan.zhaomingkeji.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://kbp.guannengcc.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gdg.9152youxi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://iyb.316326.xyz

TS:   typeof x; x instanceof Date
来源：http://uvy.iojbl.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kxt.ppjwa.cn

Go:   reflect.TypeOf(x).Name()
来源：http://obh.zhijiandao.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://lhi.bbcook.cn

C#:   x.GetType().Name; x is int
来源：http://noz.sxryk.cn

[A05] 整数除法与取模
来源：http://ryt.jyoumei.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://teh.fktsv.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://wqu.smart0.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pad.vqdsnc.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fhi.sweek.top

Java: 7 / 2; 7 % 2
来源：http://fvm.tian-w.cn

Go:   7 / 2; 7 % 2
来源：http://tee.52xcode.cn

Ruby: 7 / 2; 7 % 2
来源：http://etc.xuetiantiany.cn

C#:   7 / 2; 7 % 2
来源：http://jwj.zdqjudy.top

[A06] 字符串转数字
来源：http://tyz.yuxming.cn

Py:   int("42"); float("3.14")
来源：http://iwi.svipenyu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tnh.shuidangran.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jsh.hfpthk.cn

TS:   parseInt("42", 10); Number("42")
来源：http://rbd.yueranfly.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://djh.ydjk.org.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ghk.ybcxt.top

Ruby: "42".to_i; "3.14".to_f
来源：http://xmh.316326.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://upx.ydzc1.top

[A07] 数字转字符串
来源：http://phx.c1oappe.top

Py:   str(42)
来源：http://gak.redwolf501.top

PHP:  (string) 42; strval(42)
来源：http://knw.tanke756.top

JS:   String(42); (42).toString()
来源：http://erm.chenjidiqi.icu

TS:   String(42)
来源：http://bgp.feifeiyinyue.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ujc.chenjidiqi.icu

Go:   strconv.Itoa(42)
来源：http://mxs.shanyushiyangkeji.top

Ruby: 42.to_s
来源：http://ipx.xingfuxueyuan.xyz

C#:   42.ToString()
来源：http://ryd.xuanzx.com

[A08] 取整与四舍五入
来源：http://zex.shzxlz.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ipt.sxryk.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wgy.zdqjudy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://brt.ehwqpu.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://csl.tarul.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://uii.kuanghao11.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kyr.shanyushiyangtech.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://rpy.daria6918.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dlr.vqdsnc.cn

[A09] 绝对值与最大最小值
来源：http://icb.xinyue.icu


<!-- 参考信息 -->