代发 wailian999

[U59] PHP：自定义排序
来源：http://umn.gotoacloud.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dyg.ywan-chungtsiang.top

[U60] PHP：JSON 编解码
来源：http://lds.zhaomingkeji.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wmx.hnxiangtu.top

[U61] PHP：正则
来源：http://jjh.dianchejie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ijs.uphjek.com

[U62] PHP：日期对象
来源：http://ozf.316326.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tlk.yangfankeji.com

[U63] PHP：文件读写
来源：http://jzk.daria6918.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://atr.hfpthk.cn

[U64] PHP：目录遍历
来源：http://pwn.gogol.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://zsm.guowangkeji.top

[U65] PHP：会话
来源：http://uot.52xcode.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fvx.yongpay.top

[U66] PHP：设置 Cookie
来源：http://gkc.daxiang520.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hkz.dashuyun.cn

[U67] PHP：处理文件上传
来源：http://ucz.xziqi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pfz.zdqjudy.top

[U68] PHP：PDO 连接
来源：http://ixc.hysaishi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xta.jinqigfzy.top

[U69] PHP：PDO 预处理
来源：http://hmn.yj20258.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mdd.zhixingplan.top

[U70] PHP：PDO 事务
来源：http://biq.hnqzz.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://evr.hesvh.cn

[U71] PHP：抛出异常
来源：http://tkd.kuanghao11.cn

throw new RuntimeException("失败", 500);
来源：http://qdl.cdnleiting.top

[U72] PHP：写错误日志
来源：http://ybi.pycfn.com

error_log("失败: " . $e->getMessage());
来源：http://ojz.wangdashe.top

[U73] PHP：读取 ini 配置
来源：http://mhw.sweek.top

parse_ini_file("config.ini", true)
来源：http://edk.ywan-chungtsiang.top

[U74] PHP：读取环境变量
来源：http://fgh.chenjidiqi.icu

getenv("APP_ENV") ?: "production"
来源：http://kql.hfpthk.cn

[U75] PHP：依赖注入
来源：http://vuy.meibo888.top

composer require psr/container
来源：http://yoj.zhongyouzk.top

[U76] PHP：简单路由
来源：http://vrh.gaohongyu789.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ebz.dianchejie.cn

[U77] PHP：模板渲染
来源：http://wei.xinyue.icu

composer require twig/twig
来源：http://yeo.yanxiufei.cn

[U78] PHP：单元测试
来源：http://rry.tarul.cn

composer require --dev phpunit/phpunit
来源：http://ywf.xuetiantiany.cn

[U79] PHP：静态分析
来源：http://bdh.xziqi.cn

composer require --dev phpstan/phpstan
来源：http://ijo.vehdjk.com

[U80] PHP：代码规范修复
来源：http://cyb.cqqwz.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://vyv.sysykeji.top

[U81] JS：初始化项目
来源：http://ukn.jlsjyb.cn

npm init -y;  npm i express
来源：http://mws.52xcode.cn

[U82] JS：package.json 脚本
来源：http://qhn.zdbjq.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://aao.zhiwuduotai.top

[U83] JS：ES Module 导入导出
来源：http://lbu.fanxiaobao.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://xel.zycfv.cn

[U84] JS：CommonJS 写法
来源：http://vuc.kuanghao11.cn

module.exports = { a };  const { a } = require("./m");
来源：http://stm.haohaochexian.top

[U85] JS：可选链
来源：http://nuj.meibo888.top

a?.b?.c
来源：http://lil.chenzaomai.com

[U86] JS：空值合并
来源：http://diq.shanyushiyangkeji.top

a ?? b
来源：http://gdl.guowangkeji.top

[U87] JS：解构默认值
来源：http://lzd.yueranfly.top

const { a = 1, b = 2 } = obj;
来源：http://zlh.smart0.xyz

[U88] JS：对象展开合并
来源：http://bih.fengsongda.top

{ ...a, ...b }
来源：http://vlp.yj20258.top

[U89] JS：数组去重
来源：http://yrn.xingfuxueyuan.xyz

[...new Set(arr)]
来源：http://rsp.hammf.cn

[U90] JS：数字数组排序
来源：http://obn.zdqjudy.top

[...arr].sort((a, b) => a - b)
来源：http://urr.yongpay.top

[U91] JS：对象键值遍历
来源：http://jph.ydzc1.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ulk.xingfuxueyuan.xyz

[U92] JS：深拷贝
来源：http://rzh.cashguo.top

structuredClone(obj)
来源：http://bzy.gotoacloud.top

[U93] JS：模板字符串
来源：http://jqo.hongshengwenyu.top

`共 ${n} 条`
来源：http://jod.xylfe.cn

[U94] JS：箭头函数
来源：http://mov.yj202588.top

const double = x => x * 2;
来源：http://xcr.xuanzx.com

[U95] JS：Promise 包装
来源：http://bxf.bjfxy.top

new Promise((resolve, reject) => {})
来源：http://xbr.jiagoushi.top

[U96] JS：async/await 与异常
来源：http://poa.guowangkeji.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ped.quarkkingdee.top

[U97] JS：并发请求
来源：http://ejh.cucudq.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://dbm.sysykeji.top

[U98] JS：fetch 带 JSON
来源：http://jgd.svipenyu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ryg.xylfe.cn

[U99] JS：事件监听
来源：http://mwj.fanxiaobao.xyz

el.addEventListener("click", e => {})
来源：http://lbo.feifeiyinyue.top

[U100] JS：DOM 查询
来源：http://xfd.guowangkeji.top

document.querySelector(".item")
来源：http://rua.jinqigufen.top

[U101] JS：classList 操作
来源：http://hwk.zhijiandao.cn

el.classList.toggle("active")
来源：http://ypq.9152youxi.cn

[U102] JS：本地存储
来源：http://nsh.tianlin.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://woi.jinqigfzy.top

[U103] JS：定时器
来源：http://rqi.fehbvm.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kxw.meibo888.top

[U104] JS：防抖
来源：http://gdw.gaohongyu789.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dpd.yuxming.cn

[U105] JS：节流
来源：http://lkp.vqdsnc.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://noj.bjfxy.top

[U106] JS：日期格式化
来源：http://atz.yuxming.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dpy.yuanzhike.top

[U107] JS：数字千分位
来源：http://rye.cqqwz.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zgi.316326.xyz

[U108] JS：随机整数
来源：http://eze.zdqjudy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dxd.ivvv.top

[U109] JS：数组分组
来源：http://fai.birdmap.top

Object.groupBy(arr, x => x.type)
来源：http://peb.gotoacloud.top

[U110] JS：数组分块
来源：http://abw.yuanzhike.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://crq.chenlongwang.top

[U111] JS：对象转 Map
来源：http://znc.cheryme.top

new Map(Object.entries(obj))
来源：http://vrq.xuanzx.com

[U112] JS：字符串补位
来源：http://myg.0kj1m.cn

"7".padStart(3, "0")
来源：http://keb.ydjk.org.cn

[U113] JS：正则替换全部
来源：http://khs.andypj.xyz

s.replaceAll("a", "b")
来源：http://xau.yueranfly.top

[U114] JS：JSON 深比较
来源：http://ith.gotoacloud.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://emf.ybcxt.top

[U115] JS：生成 UUID
来源：http://thu.svipenyu.cn

crypto.randomUUID()
来源：http://tio.zhaomingkeji.xyz

[U116] JS：类型检查（JSDoc）
来源：http://lkg.xuanzx.com

/** @param {string} name */ function f(name) {}
来源：http://ajx.ivvv.top

[U117] JS：单元测试
来源：http://zuj.xuetiantiany.cn

npm i -D vitest;  npx vitest
来源：http://ooe.cashguo.top

[U118] JS：开发服务器
来源：http://enz.shanyushiyangtech.top

npm i -D vite;  npx vite
来源：http://oaw.haohaochexian.top

[U119] JS：生产构建
来源：http://gar.jqgufenzy.top

npx vite build
来源：http://sls.ydzc1.top

[U120] JS：读取环境变量（Vite）
来源：http://zsh.jinqigufen.top

import.meta.env.VITE_API_URL
来源：http://nob.ydjk.org.cn

================================================================================
来源：http://hta.yonumen.top

统计汇总
来源：http://lny.aibaodan.cn

================================================================================
来源：http://zrs.c1oappe.top

按语言统计（条）：
来源：http://nwo.jinyuanbaomall.cn

Python ......... 252
来源：http://ldr.cdnleiting.top

PHP ............ 252
来源：http://qfo.sxryk.cn

JavaScript ..... 252
来源：http://wql.xuetiantiany.cn

TypeScript ..... 212
来源：http://hvt.haohaochexian.top

Java ........... 212
来源：http://erk.xuanzx.com

Go ............. 212
来源：http://shy.aibaodan.cn

Ruby ........... 212
来源：http://uka.jiagoushi.top

C# ............. 212
来源：http://oib.hywenlv.cn

C .............. 30
来源：http://yct.guannengcc.top

C++ ............ 30
来源：http://pvp.hcnkem.com

SQL ............ 90
来源：http://dsu.xuanzx.com

Bash ........... 80
来源：http://xoe.yfazqb.com

Kotlin ......... 15
来源：http://zsr.hammf.cn

Swift .......... 15
来源：http://owg.nwbrower.top

Lua ............ 10
来源：http://czv.cheryme.top

Perl ........... 10
来源：http://otm.ivvv.top

Scala .......... 10
来源：http://luu.sjlbkw.cn

------------------------------------
来源：http://atr.cdnleiting.top

合计 ........... 2106 条
来源：http://riy.yfazqb.com

按章节统计：
来源：http://jbe.xingfuxueyuan.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mbo.ivvv.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://loy.pycfn.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://edg.hongshengwenyu.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://okn.cashguo.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://prw.ydzc1.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dfx.yj20258888.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vov.wangdashe.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://azx.c1oappe.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://axb.yj202588.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nhh.shzxlz.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://idy.sxryk.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qsa.nanxuanxn.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ghf.jinghuilouyu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://eze.nanxuanxn.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vgb.ydjk.org.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zgv.zhengqikj.top

Q SQL 专题                              90
来源：http://axy.quarkkingdee.top

R Bash 专题                             80
来源：http://mhx.hysaishi.cn

S C / C++ 专题                          60
来源：http://jbd.ivvv.top

T 其他语言补充                          60
来源：http://ist.iojbl.cn

U 高频实用片段                         120
来源：http://ojr.jqgufenzy.top

------------------------------------
来源：http://kyh.havefunace.top

合计                                  2106 条
来源：http://vrp.yueranfly.top

--------------------------------------------------------------------------------
来源：http://pwx.guannengcc.top

使用提醒
来源：http://epm.shangyingyoupin.top

--------------------------------------------------------------------------------
来源：http://ngn.nanxinkj.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://aal.sxryk.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fod.pengpengdd.cyou

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rze.sufxvd.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://wvq.zhoulong.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://okv.yj202588.top

—— 文件结束 ——
来源：http://rsx.tarul.cn

================================================================================
来源：http://pxy.chenjidiqi.icu

程序语言常见例子速查手册（2024 版）
来源：http://rky.svipenyu.cn

Common Programming Examples Cheat Book
来源：http://iel.vqdsnc.cn

================================================================================
来源：http://slw.ydzc1.top

【收录内容】
来源：http://gni.gzhubu.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://glm.xuetiantiany.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yoh.yj202588.top

SQL · Bash · C · C++
来源：http://wbp.wangshuangyany.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xkf.chenzaomai.com

【使用说明】
来源：http://gvt.fktsv.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yod.cdnleiting.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mch.cashguo.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xpv.hammf.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jnl.fanxiaobao.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://mlv.zhongyouzk.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vym.gaohongyu789.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://waw.jqgfzy.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zpy.haohaochexian.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ehy.wangshuangyany.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://svu.iojbl.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fiq.birdmap.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ney.zhongyouzk.top

【文件统计】
来源：http://zfp.dashuyun.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://peg.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://rui.hongshengwenyu.top

目  录
来源：http://ncc.hysaishi.cn

--------------------------------------------------------------------------------
来源：http://urf.jqgufenzy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mrp.bbcook.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rah.hysaishi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://cnc.jlsjyb.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dho.sxryk.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://afr.vqdsnc.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://dmr.fktsv.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://uhb.svipenyu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://evc.cqqwz.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://nio.aizwys.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://oeu.aibaodan.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://sml.nanxinkj.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ugy.yanxiufei.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kzy.fktsv.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fem.redwolf501.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gvm.kuanghao11.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://iab.havefunace.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mge.havefunace.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://kkm.vehdjk.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://aak.aizwys.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ssf.jinqigfzy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://neb.aizwys.cn

================================================================================
来源：http://eyo.jinyuanbaomall.cn

A. 基础语法与类型
来源：http://rac.snrcjt.cn

================================================================================
来源：http://mbk.hfpthk.cn

[A01] Hello World
来源：http://cip.ppjwa.cn

Py:   print("Hello, World!")
来源：http://nhh.shangyingyoupin.top

PHP:  echo "Hello, World!";
来源：http://rtu.uphjek.com

JS:   console.log("Hello, World!");
来源：http://zkh.fzhhl.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zup.tanke756.top

Java: System.out.println("Hello, World!");
来源：http://djc.epnwcf.com

Go:   fmt.Println("Hello, World!")
来源：http://rnl.fanxiaobao.xyz

Ruby: puts "Hello, World!"
来源：http://yew.epnwcf.com

C#:   Console.WriteLine("Hello, World!");
来源：http://gxq.cdnleiting.top

[A02] 变量声明与赋值
来源：http://eiq.yangfankeji.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ujr.316326.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://gdy.cucudq.cn

JS:   let name = "Alex"; const age = 20;
来源：http://wtq.chenjidiqi.icu

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jvm.quarkkingdee.top

Java: String name = "Alex"; int age = 20;
来源：http://hob.fengsongda.top

Go:   name := "Alex"; age := 20
来源：http://jon.andypj.xyz

Ruby: name = "Alex"; age = 20
来源：http://krq.dianchejie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://asv.tian-w.cn

[A03] 常量定义
来源：http://tld.yfazqb.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://uec.nanxuanxn.top

PHP:  const PI = 3.14159;
来源：http://kii.epnwcf.com

JS:   const PI = 3.14159;
来源：http://hzp.tianlin.xyz

TS:   const PI: number = 3.14159;
来源：http://uqt.zhongyouzk.top

Java: static final double PI = 3.14159;
来源：http://izv.xziqi.cn

Go:   const PI = 3.14159
来源：http://jtt.fehbvm.com

Ruby: PI = 3.14159
来源：http://rsf.redwolf501.top

C#:   const double PI = 3.14159;
来源：http://jur.jqgufenzy.top

[A04] 判断变量类型
来源：http://fbu.shuidangran.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://utx.andypj.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zix.yfazqb.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://caf.hcnkem.com

TS:   typeof x; x instanceof Date
来源：http://ddf.jinqigufen.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dvo.316326.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://rzr.shanyushiyangkeji.top

Ruby: x.class; x.is_a?(Integer)
来源：http://tra.wangdashe.top

C#:   x.GetType().Name; x is int
来源：http://apz.yongpay.top

[A05] 整数除法与取模
来源：http://pmh.xingfuxueyuan.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://khq.fengsongda.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://rws.tian-w.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wbk.cdnleiting.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ojq.hesvh.cn

Java: 7 / 2; 7 % 2
来源：http://dtd.xingfuxueyuan.xyz

Go:   7 / 2; 7 % 2
来源：http://rot.zhengqikj.top

Ruby: 7 / 2; 7 % 2
来源：http://smj.daxiang520.top

C#:   7 / 2; 7 % 2
来源：http://psw.316326.xyz

[A06] 字符串转数字
来源：http://jzw.sxryk.cn

Py:   int("42"); float("3.14")
来源：http://hal.snrcjt.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fcn.jqgfzy.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://emz.jinqigfzy.top

TS:   parseInt("42", 10); Number("42")
来源：http://brf.shuidangran.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hbb.guowangkeji.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mfc.wangshuangyany.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://jcm.xinyue.icu

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zqz.zhengqikj.top

[A07] 数字转字符串
来源：http://dqs.jqgfzy.top

Py:   str(42)
来源：http://hxz.fktsv.cn

PHP:  (string) 42; strval(42)
来源：http://qlx.xuetiantiany.cn

JS:   String(42); (42).toString()
来源：http://gwz.epnwcf.com

TS:   String(42)
来源：http://dve.shanyushiyangkeji.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://qnj.zhijiandao.cn

Go:   strconv.Itoa(42)
来源：http://hjz.smart0.xyz

Ruby: 42.to_s
来源：http://kck.yonumen.top

C#:   42.ToString()
来源：http://drk.yfazqb.com

[A08] 取整与四舍五入
来源：http://cmf.ctjpmb.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dhd.zhijiandao.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ner.ydjk.org.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://fhq.ydzc1.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://exd.daxiang520.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://tlk.cqqwz.cn


<!-- 参考信息 -->