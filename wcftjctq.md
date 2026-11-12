代发 wailian999

[U47] PHP：联合类型
来源：http://stc.xziqi.cn

int|string $id
来源：http://crz.chenlongwang.top

[U48] PHP：纯枚举
来源：http://dbu.yueranfly.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pht.zhengqikj.top

[U49] PHP：只读属性
来源：http://hph.daria6918.cn

public readonly string $name
来源：http://kvz.jlsjyb.cn

[U50] PHP：构造器属性提升
来源：http://lgm.svipenyu.cn

public function __construct(private int $id) {}
来源：http://wdg.wangdashe.top

[U51] PHP：数组解构
来源：http://bga.gotoacloud.top

[$a, $b] = $arr;
来源：http://kib.aibaodan.cn

[U52] PHP：箭头函数
来源：http://wup.shanyushiyangkeji.top

$double = fn($x) => $x * 2;
来源：http://gzb.vehdjk.com

[U53] PHP：空合并运算符
来源：http://hws.cucudq.cn

$v = $a ?? $b ?? "default";
来源：http://miu.guowangkeji.top

[U54] PHP：空安全调用
来源：http://vgy.cashguo.top

$obj?->method()
来源：http://yxc.hnqzz.top

[U55] PHP：match 表达式
来源：http://qtu.yuanzhike.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dee.9152youxi.cn

[U56] PHP：命名参数
来源：http://pfh.yongpay.top

f(a: 1, b: 2)
来源：http://qts.gotoacloud.top

[U57] PHP：字符串插值
来源：http://rzo.yuxming.cn

"值: {$a}"
来源：http://qef.yfazqb.com

[U58] PHP：数组三件套
来源：http://gnr.tianlin.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mfc.fzhhl.top

[U59] PHP：自定义排序
来源：http://zmf.hnxiangtu.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bmo.tarul.cn

[U60] PHP：JSON 编解码
来源：http://xyg.9152youxi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://enp.smart0.xyz

[U61] PHP：正则
来源：http://vlk.zhongyouzk.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zvt.sxryk.cn

[U62] PHP：日期对象
来源：http://xje.pengpengdd.cyou

(new DateTimeImmutable())->format("Y-m-d");
来源：http://szc.sufxvd.cn

[U63] PHP：文件读写
来源：http://ctt.ivvv.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cdi.xylfe.cn

[U64] PHP：目录遍历
来源：http://gue.jianghu66.top

glob("dir/*.php");  scandir("dir");
来源：http://szy.yj20258888.top

[U65] PHP：会话
来源：http://sru.wangshuangyany.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vpt.fanxiaobao.xyz

[U66] PHP：设置 Cookie
来源：http://vxb.sweek.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rao.zhengqikj.top

[U67] PHP：处理文件上传
来源：http://awb.bjfxy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://niq.yongpay.top

[U68] PHP：PDO 连接
来源：http://jak.sjlbkw.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jkv.pycfn.com

[U69] PHP：PDO 预处理
来源：http://yjd.aibaodan.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ugx.xziqi.cn

[U70] PHP：PDO 事务
来源：http://zwc.52xcode.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yzp.aizwys.cn

[U71] PHP：抛出异常
来源：http://xmw.ppjwa.cn

throw new RuntimeException("失败", 500);
来源：http://mhw.zdqjudy.top

[U72] PHP：写错误日志
来源：http://sda.redwolf501.top

error_log("失败: " . $e->getMessage());
来源：http://oyk.xingfuxueyuan.xyz

[U73] PHP：读取 ini 配置
来源：http://vtp.xziqi.cn

parse_ini_file("config.ini", true)
来源：http://hzz.nwbrower.top

[U74] PHP：读取环境变量
来源：http://fwy.nwbrower.top

getenv("APP_ENV") ?: "production"
来源：http://wgo.jinghuilouyu.cn

[U75] PHP：依赖注入
来源：http://wjh.52xcode.cn

composer require psr/container
来源：http://ohk.guowangkeji.top

[U76] PHP：简单路由
来源：http://mku.xingfuxueyuan.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fux.jlsjyb.cn

[U77] PHP：模板渲染
来源：http://krb.redwolf501.top

composer require twig/twig
来源：http://dts.jianghu66.top

[U78] PHP：单元测试
来源：http://hyt.ywan-chungtsiang.top

composer require --dev phpunit/phpunit
来源：http://nvw.cqqwz.cn

[U79] PHP：静态分析
来源：http://lrs.hysaishi.cn

composer require --dev phpstan/phpstan
来源：http://euf.tarul.cn

[U80] PHP：代码规范修复
来源：http://ysh.gaohongyu789.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://nle.xziqi.cn

[U81] JS：初始化项目
来源：http://roz.xuanzx.com

npm init -y;  npm i express
来源：http://rti.guowangkeji.top

[U82] JS：package.json 脚本
来源：http://rcf.sufxvd.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mjz.birdmap.top

[U83] JS：ES Module 导入导出
来源：http://bgd.vqdsnc.cn

export const a = 1;  import { a } from "./m.js";
来源：http://crq.0kj1m.cn

[U84] JS：CommonJS 写法
来源：http://wix.fengsongda.top

module.exports = { a };  const { a } = require("./m");
来源：http://ekg.hywenlv.cn

[U85] JS：可选链
来源：http://dsz.andypj.xyz

a?.b?.c
来源：http://hhk.ctjpmb.com

[U86] JS：空值合并
来源：http://ozs.yueranfly.top

a ?? b
来源：http://cge.pengpengdd.cyou

[U87] JS：解构默认值
来源：http://cat.zhaomingkeji.xyz

const { a = 1, b = 2 } = obj;
来源：http://hol.hysaishi.cn

[U88] JS：对象展开合并
来源：http://pob.snrcjt.cn

{ ...a, ...b }
来源：http://dit.jyoumei.cn

[U89] JS：数组去重
来源：http://qel.yj20258888.top

[...new Set(arr)]
来源：http://jnz.haohaochexian.top

[U90] JS：数字数组排序
来源：http://ojp.chenlongwang.top

[...arr].sort((a, b) => a - b)
来源：http://jvf.xinyue.icu

[U91] JS：对象键值遍历
来源：http://maq.zdbjq.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bid.cqqwz.cn

[U92] JS：深拷贝
来源：http://gwo.shangyingyoupin.top

structuredClone(obj)
来源：http://svf.smart0.xyz

[U93] JS：模板字符串
来源：http://bvm.pengpengdd.cyou

`共 ${n} 条`
来源：http://sim.shangyingyoupin.top

[U94] JS：箭头函数
来源：http://epb.cucudq.cn

const double = x => x * 2;
来源：http://oal.yj202588.top

[U95] JS：Promise 包装
来源：http://jhw.yj202588.top

new Promise((resolve, reject) => {})
来源：http://ttk.shzxlz.cn

[U96] JS：async/await 与异常
来源：http://pmu.yueranfly.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dny.xuetiantiany.cn

[U97] JS：并发请求
来源：http://msb.zhiwuduotai.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://wrv.andypj.xyz

[U98] JS：fetch 带 JSON
来源：http://sol.dashuyun.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://alp.shanyushiyangkeji.top

[U99] JS：事件监听
来源：http://zzi.9152youxi.cn

el.addEventListener("click", e => {})
来源：http://pup.chenjidiqi.icu

[U100] JS：DOM 查询
来源：http://qal.gotoacloud.top

document.querySelector(".item")
来源：http://sjq.nwbrower.top

[U101] JS：classList 操作
来源：http://dvh.ybcxt.top

el.classList.toggle("active")
来源：http://kqw.guowangkeji.top

[U102] JS：本地存储
来源：http://wab.quarkkingdee.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://fop.jyoumei.cn

[U103] JS：定时器
来源：http://nff.ehwqpu.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nly.zhaomingkeji.xyz

[U104] JS：防抖
来源：http://qiu.hnqzz.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://amu.yuanzhike.top

[U105] JS：节流
来源：http://tmh.zhengqikj.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uae.shanyushiyangtech.top

[U106] JS：日期格式化
来源：http://cyv.svipenyu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://arb.haohaochexian.top

[U107] JS：数字千分位
来源：http://ufw.zhongyouzk.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dcp.ctjpmb.com

[U108] JS：随机整数
来源：http://snt.gotoacloud.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uzl.9152youxi.cn

[U109] JS：数组分组
来源：http://bcr.yuxming.cn

Object.groupBy(arr, x => x.type)
来源：http://mmh.fehbvm.com

[U110] JS：数组分块
来源：http://uee.cucudq.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ktm.zycfv.cn

[U111] JS：对象转 Map
来源：http://qio.fehbvm.com

new Map(Object.entries(obj))
来源：http://dnc.hnqzz.top

[U112] JS：字符串补位
来源：http://lts.yongpay.top

"7".padStart(3, "0")
来源：http://smc.pycfn.com

[U113] JS：正则替换全部
来源：http://cpp.aizwys.cn

s.replaceAll("a", "b")
来源：http://dgx.cdnleiting.top

[U114] JS：JSON 深比较
来源：http://chx.ivvv.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://oxp.zhengqikj.top

[U115] JS：生成 UUID
来源：http://biq.vehdjk.com

crypto.randomUUID()
来源：http://qch.nwbrower.top

[U116] JS：类型检查（JSDoc）
来源：http://zqp.316326.xyz

/** @param {string} name */ function f(name) {}
来源：http://axx.yuanzhike.top

[U117] JS：单元测试
来源：http://fxp.cashguo.top

npm i -D vitest;  npx vitest
来源：http://qni.jianghu66.top

[U118] JS：开发服务器
来源：http://blf.hcnkem.com

npm i -D vite;  npx vite
来源：http://sxd.wangdashe.top

[U119] JS：生产构建
来源：http://vyn.andypj.xyz

npx vite build
来源：http://qjx.hnxiangtu.top

[U120] JS：读取环境变量（Vite）
来源：http://mie.aibaodan.cn

import.meta.env.VITE_API_URL
来源：http://mpn.fengsongda.top

================================================================================
来源：http://ahn.hcnkem.com

统计汇总
来源：http://zaj.bjfxy.top

================================================================================
来源：http://llq.chenjidiqi.icu

按语言统计（条）：
来源：http://dgi.shuidangran.top

Python ......... 252
来源：http://hon.iojbl.cn

PHP ............ 252
来源：http://cja.jlsjyb.cn

JavaScript ..... 252
来源：http://owk.shuidangran.top

TypeScript ..... 212
来源：http://epe.c1oappe.top

Java ........... 212
来源：http://mtz.fzhhl.top

Go ............. 212
来源：http://uxk.yuanzhike.top

Ruby ........... 212
来源：http://btj.hnqzz.top

C# ............. 212
来源：http://plg.gaohongyu789.top

C .............. 30
来源：http://leg.hnqzz.top

C++ ............ 30
来源：http://hjt.ydjk.org.cn

SQL ............ 90
来源：http://lck.aizwys.cn

Bash ........... 80
来源：http://zrq.gaohongyu789.top

Kotlin ......... 15
来源：http://iqm.bjfxy.top

Swift .......... 15
来源：http://nni.jiagoushi.top

Lua ............ 10
来源：http://hdk.yj20258888.top

Perl ........... 10
来源：http://qmj.pengpengdd.cyou

Scala .......... 10
来源：http://zha.zhijiandao.cn

------------------------------------
来源：http://sin.jqgufenzy.top

合计 ........... 2106 条
来源：http://pxs.hnxiangtu.top

按章节统计：
来源：http://gef.dianchejie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cey.sysykeji.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://edc.daria6918.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dpr.zycfv.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://djp.guowangkeji.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rfx.vqdsnc.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ukh.svipenyu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://itw.birdmap.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://orl.uphjek.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://cpa.sxryk.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://olz.ydjk.org.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kgm.shzxlz.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jdc.yj20258.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zty.yuxming.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jgx.zhiwuduotai.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gsh.yueranfly.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ify.zhoulong.xyz

Q SQL 专题                              90
来源：http://wxl.zhixingplan.top

R Bash 专题                             80
来源：http://cuy.shuidangran.top

S C / C++ 专题                          60
来源：http://uhp.bjfxy.top

T 其他语言补充                          60
来源：http://byu.yongpay.top

U 高频实用片段                         120
来源：http://vah.xylfe.cn

------------------------------------
来源：http://hby.hywenlv.cn

合计                                  2106 条
来源：http://iro.yanxiufei.cn

--------------------------------------------------------------------------------
来源：http://huz.vehdjk.com

使用提醒
来源：http://ikb.cashguo.top

--------------------------------------------------------------------------------
来源：http://jqm.zhoulong.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://azc.shanyushiyangtech.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xhs.0kj1m.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tyz.hcnkem.com

在旧版本上使用前请先确认语法支持情况。
来源：http://wzi.zdbjq.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qpv.shanyushiyangkeji.top

—— 文件结束 ——
来源：http://djt.zhaomingkeji.xyz

================================================================================
来源：http://afp.tianlin.xyz

程序语言常见例子速查手册（2024 版）
来源：http://uyl.bjfxy.top

Common Programming Examples Cheat Book
来源：http://buk.yueranfly.top

================================================================================
来源：http://sly.ppjwa.cn

【收录内容】
来源：http://xuc.sufxvd.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://zys.svipenyu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fnc.xylfe.cn

SQL · Bash · C · C++
来源：http://wke.zhongyouzk.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://njr.yfazqb.com

【使用说明】
来源：http://hsq.jlsjyb.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nyg.hywenlv.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hbo.vqdsnc.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tkw.sxryk.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://uqq.hnqzz.top

Bash:  Shell         C:     C             C++:   C++
来源：http://gnb.fzhhl.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://map.hnqzz.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mdl.cashguo.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://tgl.jiagoushi.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lgh.zycfv.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pdq.yj20258.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://spa.xingfuxueyuan.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dpv.c1oappe.top

【文件统计】
来源：http://sqp.ydjk.org.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://avt.cucudq.cn

--------------------------------------------------------------------------------
来源：http://npf.xuetiantiany.cn

目  录
来源：http://gek.yuxming.cn

--------------------------------------------------------------------------------
来源：http://rvm.ydjk.org.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kkh.yuxming.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://spo.jinqigufen.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://uyv.uphjek.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ktl.cashguo.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mwt.andypj.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qwf.hysaishi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fbb.birdmap.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wvw.ywan-chungtsiang.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hva.zycfv.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://uku.yfazqb.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://puq.andypj.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://taf.tarul.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gqa.uphjek.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rxn.c1oappe.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qvc.chenzaomai.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hsd.sjlbkw.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qzy.jqgufenzy.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://vii.sufxvd.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jyz.ivvv.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nza.zhixingplan.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://miy.yanxiufei.cn

================================================================================
来源：http://ikx.fzhhl.top

A. 基础语法与类型
来源：http://lfa.nwbrower.top

================================================================================
来源：http://lui.gaohongyu789.top

[A01] Hello World
来源：http://opy.kuanghao11.cn

Py:   print("Hello, World!")
来源：http://pgp.birdmap.top

PHP:  echo "Hello, World!";
来源：http://yys.zhixingplan.top

JS:   console.log("Hello, World!");
来源：http://rur.vehdjk.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zqq.sxryk.cn

Java: System.out.println("Hello, World!");
来源：http://hag.jinyuanbaomall.cn

Go:   fmt.Println("Hello, World!")
来源：http://ejv.gaohongyu789.top

Ruby: puts "Hello, World!"
来源：http://dch.redwolf501.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ypm.zhijiandao.cn

[A02] 变量声明与赋值
来源：http://uat.fehbvm.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wpv.uphjek.com

PHP:  $name = "Alex"; $age = 20;
来源：http://itu.xuanzx.com

JS:   let name = "Alex"; const age = 20;
来源：http://mhx.nanxinkj.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://okf.jianghu66.top

Java: String name = "Alex"; int age = 20;
来源：http://vvv.smart0.xyz

Go:   name := "Alex"; age := 20
来源：http://bec.yvedp.cn

Ruby: name = "Alex"; age = 20
来源：http://fds.xziqi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://yve.yuxming.cn

[A03] 常量定义
来源：http://azp.feifeiyinyue.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fyu.daxiang520.top

PHP:  const PI = 3.14159;
来源：http://dwd.andypj.xyz

JS:   const PI = 3.14159;
来源：http://btz.shzxlz.cn

TS:   const PI: number = 3.14159;
来源：http://nmo.c1oappe.top

Java: static final double PI = 3.14159;
来源：http://aji.ybcxt.top

Go:   const PI = 3.14159
来源：http://cfv.yueranfly.top

Ruby: PI = 3.14159
来源：http://yhe.cucudq.cn

C#:   const double PI = 3.14159;
来源：http://yrd.haohaochexian.top

[A04] 判断变量类型
来源：http://qgx.zdbjq.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://qor.gzhubu.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mrr.jianghu66.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://sor.0kj1m.cn

TS:   typeof x; x instanceof Date
来源：http://sdn.hongshengwenyu.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ajf.fanxiaobao.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://vhd.xinyue.icu

Ruby: x.class; x.is_a?(Integer)
来源：http://ced.cdnleiting.top

C#:   x.GetType().Name; x is int
来源：http://ybk.zhaomingkeji.xyz

[A05] 整数除法与取模
来源：http://xys.jinyuanbaomall.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hfq.cashguo.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://qnb.hnxiangtu.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://fiw.aibaodan.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fml.tanke756.top

Java: 7 / 2; 7 % 2
来源：http://ixi.aizwys.cn

Go:   7 / 2; 7 % 2
来源：http://oua.jinyuanbaomall.cn

Ruby: 7 / 2; 7 % 2
来源：http://gug.tarul.cn

C#:   7 / 2; 7 % 2
来源：http://tzl.xylfe.cn


<!-- 参考信息 -->