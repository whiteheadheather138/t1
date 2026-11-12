代发 wailian999

[U49] PHP：只读属性
来源：http://hqx.gzhubu.top

public readonly string $name
来源：http://qxp.yj20258.top

[U50] PHP：构造器属性提升
来源：http://hxi.xylfe.cn

public function __construct(private int $id) {}
来源：http://rkz.jinqigfzy.top

[U51] PHP：数组解构
来源：http://jfa.jinqigfzy.top

[$a, $b] = $arr;
来源：http://vwt.aizwys.cn

[U52] PHP：箭头函数
来源：http://xjq.dashuyun.cn

$double = fn($x) => $x * 2;
来源：http://yof.daria6918.cn

[U53] PHP：空合并运算符
来源：http://lrl.ywan-chungtsiang.top

$v = $a ?? $b ?? "default";
来源：http://bjf.jinghuilouyu.cn

[U54] PHP：空安全调用
来源：http://keu.yfazqb.com

$obj?->method()
来源：http://zoh.zhijiandao.cn

[U55] PHP：match 表达式
来源：http://ywf.0kj1m.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ugq.haohaochexian.top

[U56] PHP：命名参数
来源：http://oue.zhijiandao.cn

f(a: 1, b: 2)
来源：http://zbc.hnqzz.top

[U57] PHP：字符串插值
来源：http://rvk.ydzc1.top

"值: {$a}"
来源：http://gjb.iojbl.cn

[U58] PHP：数组三件套
来源：http://qaw.xinyue.icu

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lxi.yongpay.top

[U59] PHP：自定义排序
来源：http://hiu.shuidangran.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fvh.fktsv.cn

[U60] PHP：JSON 编解码
来源：http://trs.svipenyu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rux.jyoumei.cn

[U61] PHP：正则
来源：http://omu.zhaomingkeji.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ejv.wangshuangyany.cn

[U62] PHP：日期对象
来源：http://ces.vqdsnc.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nbz.c1oappe.top

[U63] PHP：文件读写
来源：http://krk.ydjk.org.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://smw.vehdjk.com

[U64] PHP：目录遍历
来源：http://phb.hongshengwenyu.top

glob("dir/*.php");  scandir("dir");
来源：http://xup.dashuyun.cn

[U65] PHP：会话
来源：http://pkz.hysaishi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kcu.hysaishi.cn

[U66] PHP：设置 Cookie
来源：http://rre.havefunace.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pez.pengpengdd.cyou

[U67] PHP：处理文件上传
来源：http://nbq.jianghu66.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hjo.hywenlv.cn

[U68] PHP：PDO 连接
来源：http://yqs.zhoulong.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tfa.hfpthk.cn

[U69] PHP：PDO 预处理
来源：http://wdc.zycfv.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dso.meibo888.top

[U70] PHP：PDO 事务
来源：http://adz.ydjk.org.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fbq.nwbrower.top

[U71] PHP：抛出异常
来源：http://czh.yj20258.top

throw new RuntimeException("失败", 500);
来源：http://mgl.xinyue.icu

[U72] PHP：写错误日志
来源：http://bzf.shanyushiyangtech.top

error_log("失败: " . $e->getMessage());
来源：http://bwp.pengpengdd.cyou

[U73] PHP：读取 ini 配置
来源：http://mbb.xinyue.icu

parse_ini_file("config.ini", true)
来源：http://dea.gaohongyu789.top

[U74] PHP：读取环境变量
来源：http://tsi.zhijiandao.cn

getenv("APP_ENV") ?: "production"
来源：http://ahm.yanxiufei.cn

[U75] PHP：依赖注入
来源：http://prf.316326.xyz

composer require psr/container
来源：http://kvb.tianlin.xyz

[U76] PHP：简单路由
来源：http://xly.nwbrower.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ojq.hesvh.cn

[U77] PHP：模板渲染
来源：http://kxv.hnqzz.top

composer require twig/twig
来源：http://jfw.epnwcf.com

[U78] PHP：单元测试
来源：http://zsg.meibo888.top

composer require --dev phpunit/phpunit
来源：http://nrf.hcnkem.com

[U79] PHP：静态分析
来源：http://fcd.zhengqikj.top

composer require --dev phpstan/phpstan
来源：http://hij.aibaodan.cn

[U80] PHP：代码规范修复
来源：http://lhl.sufxvd.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ldc.hfpthk.cn

[U81] JS：初始化项目
来源：http://lnd.fehbvm.com

npm init -y;  npm i express
来源：http://aaz.sysykeji.top

[U82] JS：package.json 脚本
来源：http://sxd.chenlongwang.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wvr.ctjpmb.com

[U83] JS：ES Module 导入导出
来源：http://vol.cheryme.top

export const a = 1;  import { a } from "./m.js";
来源：http://suk.dashuyun.cn

[U84] JS：CommonJS 写法
来源：http://xdr.ydjk.org.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yos.zdbjq.cn

[U85] JS：可选链
来源：http://tjn.tanke756.top

a?.b?.c
来源：http://ubx.feifeiyinyue.top

[U86] JS：空值合并
来源：http://gzi.jqgfzy.top

a ?? b
来源：http://aqs.fanxiaobao.xyz

[U87] JS：解构默认值
来源：http://zhs.jinqigfzy.top

const { a = 1, b = 2 } = obj;
来源：http://wsd.xingfuxueyuan.xyz

[U88] JS：对象展开合并
来源：http://jte.pengpengdd.cyou

{ ...a, ...b }
来源：http://aku.chenlongwang.top

[U89] JS：数组去重
来源：http://tjj.aizwys.cn

[...new Set(arr)]
来源：http://emy.fzhhl.top

[U90] JS：数字数组排序
来源：http://xlf.pengpengdd.cyou

[...arr].sort((a, b) => a - b)
来源：http://yzi.nanxuanxn.top

[U91] JS：对象键值遍历
来源：http://zio.yj20258.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mbw.zhixingplan.top

[U92] JS：深拷贝
来源：http://djs.hnqzz.top

structuredClone(obj)
来源：http://vuu.meibo888.top

[U93] JS：模板字符串
来源：http://mjo.hfpthk.cn

`共 ${n} 条`
来源：http://max.snrcjt.cn

[U94] JS：箭头函数
来源：http://txd.ydjk.org.cn

const double = x => x * 2;
来源：http://ofe.redwolf501.top

[U95] JS：Promise 包装
来源：http://div.hfpthk.cn

new Promise((resolve, reject) => {})
来源：http://ytl.shanyushiyangtech.top

[U96] JS：async/await 与异常
来源：http://jdc.svipenyu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bei.yuanzhike.top

[U97] JS：并发请求
来源：http://itp.smart0.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://ouf.zhiwuduotai.top

[U98] JS：fetch 带 JSON
来源：http://rqz.pycfn.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qki.ivvv.top

[U99] JS：事件监听
来源：http://ujw.yueranfly.top

el.addEventListener("click", e => {})
来源：http://gtn.dianchejie.cn

[U100] JS：DOM 查询
来源：http://afl.xinyue.icu

document.querySelector(".item")
来源：http://ifq.vqdsnc.cn

[U101] JS：classList 操作
来源：http://ace.ywan-chungtsiang.top

el.classList.toggle("active")
来源：http://qio.svipenyu.cn

[U102] JS：本地存储
来源：http://hnq.yfazqb.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://cyz.pycfn.com

[U103] JS：定时器
来源：http://dkw.iojbl.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wyk.zhaomingkeji.xyz

[U104] JS：防抖
来源：http://ygw.quarkkingdee.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gwl.epnwcf.com

[U105] JS：节流
来源：http://ylp.ydzc1.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cgf.gogol.net.cn

[U106] JS：日期格式化
来源：http://cwc.dashuyun.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xnd.tanke756.top

[U107] JS：数字千分位
来源：http://dgt.kuanghao11.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xya.zhongyouzk.top

[U108] JS：随机整数
来源：http://zcb.sysykeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uct.xziqi.cn

[U109] JS：数组分组
来源：http://vdm.gaohongyu789.top

Object.groupBy(arr, x => x.type)
来源：http://pew.pycfn.com

[U110] JS：数组分块
来源：http://rnh.sysykeji.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dyd.quarkkingdee.top

[U111] JS：对象转 Map
来源：http://tpf.316326.xyz

new Map(Object.entries(obj))
来源：http://cls.feifeiyinyue.top

[U112] JS：字符串补位
来源：http://pmc.tanke756.top

"7".padStart(3, "0")
来源：http://vpc.gaohongyu789.top

[U113] JS：正则替换全部
来源：http://msl.sufxvd.cn

s.replaceAll("a", "b")
来源：http://xpu.fzhhl.top

[U114] JS：JSON 深比较
来源：http://tsq.fehbvm.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://rzz.sjlbkw.cn

[U115] JS：生成 UUID
来源：http://wjz.tianlin.xyz

crypto.randomUUID()
来源：http://uuk.svipenyu.cn

[U116] JS：类型检查（JSDoc）
来源：http://lqe.redwolf501.top

/** @param {string} name */ function f(name) {}
来源：http://xow.daxiang520.top

[U117] JS：单元测试
来源：http://for.cashguo.top

npm i -D vitest;  npx vitest
来源：http://lua.yongpay.top

[U118] JS：开发服务器
来源：http://phv.shangyingyoupin.top

npm i -D vite;  npx vite
来源：http://owd.yuanzhike.top

[U119] JS：生产构建
来源：http://vem.52xcode.cn

npx vite build
来源：http://zyc.epnwcf.com

[U120] JS：读取环境变量（Vite）
来源：http://xpj.jqgfzy.top

import.meta.env.VITE_API_URL
来源：http://ydv.yueranfly.top

================================================================================
来源：http://deq.vqdsnc.cn

统计汇总
来源：http://bmh.epnwcf.com

================================================================================
来源：http://tmp.jinqigufen.top

按语言统计（条）：
来源：http://pmy.meibo888.top

Python ......... 252
来源：http://oll.zhongyouzk.top

PHP ............ 252
来源：http://xwx.cheryme.top

JavaScript ..... 252
来源：http://had.wangshuangyany.cn

TypeScript ..... 212
来源：http://qls.zhengqikj.top

Java ........... 212
来源：http://mqj.zhengqikj.top

Go ............. 212
来源：http://hxj.yj20258888.top

Ruby ........... 212
来源：http://blu.316326.xyz

C# ............. 212
来源：http://lor.nwbrower.top

C .............. 30
来源：http://hoa.hammf.cn

C++ ............ 30
来源：http://yps.xinyue.icu

SQL ............ 90
来源：http://lfz.yanxiufei.cn

Bash ........... 80
来源：http://gtt.shuidangran.top

Kotlin ......... 15
来源：http://kvs.guowangkeji.top

Swift .......... 15
来源：http://qrn.gogol.net.cn

Lua ............ 10
来源：http://xeq.jyoumei.cn

Perl ........... 10
来源：http://qrr.mhx1999.top

Scala .......... 10
来源：http://euu.gzhubu.top

------------------------------------
来源：http://wsb.hywenlv.cn

合计 ........... 2106 条
来源：http://smi.gogol.net.cn

按章节统计：
来源：http://qow.zycfv.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zbg.0kj1m.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qwl.tarul.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nvy.yj20258.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ycs.fengsongda.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ald.bjfxy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dsv.chenjidiqi.icu

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ryx.tianlin.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://uqx.jqgfzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://scx.tanke756.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://num.cheryme.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cvc.haohaochexian.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xlp.yuxming.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fuz.ppjwa.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ouu.cheryme.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ovb.gogol.net.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ybl.shangyingyoupin.top

Q SQL 专题                              90
来源：http://hxn.cdnleiting.top

R Bash 专题                             80
来源：http://hmy.jlsjyb.cn

S C / C++ 专题                          60
来源：http://usy.gogol.net.cn

T 其他语言补充                          60
来源：http://ttk.vehdjk.com

U 高频实用片段                         120
来源：http://uag.ydjk.org.cn

------------------------------------
来源：http://opt.hammf.cn

合计                                  2106 条
来源：http://dve.zhaomingkeji.xyz

--------------------------------------------------------------------------------
来源：http://tod.c1oappe.top

使用提醒
来源：http://lsl.guowangkeji.top

--------------------------------------------------------------------------------
来源：http://uut.jiagoushi.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jri.hcnkem.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rwj.0kj1m.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xiq.gzhubu.top

在旧版本上使用前请先确认语法支持情况。
来源：http://oqp.jinyuanbaomall.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lim.nanxuanxn.top

—— 文件结束 ——
来源：http://udr.gaohongyu789.top

================================================================================
来源：http://qmv.jlsjyb.cn

程序语言常见例子速查手册（2024 版）
来源：http://bnz.ydjk.org.cn

Common Programming Examples Cheat Book
来源：http://vje.hywenlv.cn

================================================================================
来源：http://qsq.ehwqpu.com

【收录内容】
来源：http://bkz.epnwcf.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://goa.nanxinkj.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://law.ppjwa.cn

SQL · Bash · C · C++
来源：http://fyp.tianlin.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vch.pengpengdd.cyou

【使用说明】
来源：http://hyl.fzhhl.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bft.ctjpmb.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mmw.jyoumei.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pwp.yfazqb.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cdc.sufxvd.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://mzy.bjfxy.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xkp.yuanzhike.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hhx.xylfe.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gbz.yuanzhike.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rkp.guowangkeji.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hzc.sysykeji.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jam.dashuyun.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://cez.cqqwz.cn

【文件统计】
来源：http://zgp.cucudq.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wgl.tianlin.xyz

--------------------------------------------------------------------------------
来源：http://bpp.nanxuanxn.top

目  录
来源：http://zkf.jianghu66.top

--------------------------------------------------------------------------------
来源：http://rzp.zhiwuduotai.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xsh.tian-w.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dgy.hywenlv.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://num.zhixingplan.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hvq.hcnkem.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hqt.xuanzx.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hdy.316326.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vkp.chenzaomai.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ltf.sjlbkw.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jqe.jqgfzy.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dej.ybcxt.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ptw.c1oappe.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ibz.yonumen.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fxf.yuanzhike.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kdh.sweek.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://uhc.guannengcc.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qaz.xziqi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://liy.pengpengdd.cyou

R. Bash 专题                   （第 18 节，80 条）
来源：http://xcw.cashguo.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://htg.jinqigfzy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://uvg.c1oappe.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://aum.ivvv.top

================================================================================
来源：http://glg.hesvh.cn

A. 基础语法与类型
来源：http://ybe.cdnleiting.top

================================================================================
来源：http://pmi.guowangkeji.top

[A01] Hello World
来源：http://ydn.fktsv.cn

Py:   print("Hello, World!")
来源：http://nqt.zhixingplan.top

PHP:  echo "Hello, World!";
来源：http://rhj.sjlbkw.cn

JS:   console.log("Hello, World!");
来源：http://agm.shzxlz.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tqx.tian-w.cn

Java: System.out.println("Hello, World!");
来源：http://xiz.bbcook.cn

Go:   fmt.Println("Hello, World!")
来源：http://pss.sufxvd.cn

Ruby: puts "Hello, World!"
来源：http://xiv.fzhhl.top

C#:   Console.WriteLine("Hello, World!");
来源：http://gwm.gzhubu.top

[A02] 变量声明与赋值
来源：http://ldu.sweek.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bbr.yuanzhike.top

PHP:  $name = "Alex"; $age = 20;
来源：http://yhx.feifeiyinyue.top

JS:   let name = "Alex"; const age = 20;
来源：http://ttm.xuanzx.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://crp.gaohongyu789.top

Java: String name = "Alex"; int age = 20;
来源：http://jnk.jianghu66.top

Go:   name := "Alex"; age := 20
来源：http://bky.hongshengwenyu.top

Ruby: name = "Alex"; age = 20
来源：http://loc.zhijiandao.cn

C#:   string name = "Alex"; int age = 20;
来源：http://aea.ydzc1.top

[A03] 常量定义
来源：http://rjy.daxiang520.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gso.hesvh.cn

PHP:  const PI = 3.14159;
来源：http://pam.birdmap.top

JS:   const PI = 3.14159;
来源：http://pgf.zhiwuduotai.top

TS:   const PI: number = 3.14159;
来源：http://fjw.jlsjyb.cn

Java: static final double PI = 3.14159;
来源：http://amt.birdmap.top

Go:   const PI = 3.14159
来源：http://crh.smart0.xyz

Ruby: PI = 3.14159
来源：http://ekx.zhiwuduotai.top

C#:   const double PI = 3.14159;
来源：http://wfr.zycfv.cn

[A04] 判断变量类型
来源：http://did.hongshengwenyu.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://tce.mhx1999.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mfn.tian-w.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gsh.hnqzz.top

TS:   typeof x; x instanceof Date
来源：http://sgk.tarul.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zwr.sysykeji.top

Go:   reflect.TypeOf(x).Name()
来源：http://nhw.xziqi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://tri.uphjek.com

C#:   x.GetType().Name; x is int
来源：http://ffu.yuanzhike.top

[A05] 整数除法与取模
来源：http://gbq.zhiwuduotai.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://why.redwolf501.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://zpo.cqqwz.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gbj.zycfv.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cgv.andypj.xyz

Java: 7 / 2; 7 % 2
来源：http://xeo.xuanzx.com

Go:   7 / 2; 7 % 2
来源：http://zor.haohaochexian.top

Ruby: 7 / 2; 7 % 2
来源：http://pey.meibo888.top

C#:   7 / 2; 7 % 2
来源：http://cfa.ydjk.org.cn

[A06] 字符串转数字
来源：http://mjj.sysykeji.top

Py:   int("42"); float("3.14")
来源：http://xiu.ybcxt.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://stl.zdbjq.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zsk.sjlbkw.cn


<!-- 参考信息 -->