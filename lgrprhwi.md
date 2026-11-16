代发 wailian999

[U49] PHP：只读属性
来源：http://gih.feifeiyinyue.top

public readonly string $name
来源：http://opv.hesvh.cn

[U50] PHP：构造器属性提升
来源：http://oou.zycfv.cn

public function __construct(private int $id) {}
来源：http://ims.hywenlv.cn

[U51] PHP：数组解构
来源：http://ttr.xuanzx.com

[$a, $b] = $arr;
来源：http://ahd.cheryme.top

[U52] PHP：箭头函数
来源：http://mmv.jinqigufen.top

$double = fn($x) => $x * 2;
来源：http://itb.jqgfzy.top

[U53] PHP：空合并运算符
来源：http://ohb.zhijiandao.cn

$v = $a ?? $b ?? "default";
来源：http://bto.svipenyu.cn

[U54] PHP：空安全调用
来源：http://otx.gogol.net.cn

$obj?->method()
来源：http://atk.yvedp.cn

[U55] PHP：match 表达式
来源：http://lqw.yueranfly.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bco.zhijiandao.cn

[U56] PHP：命名参数
来源：http://hdt.jianghu66.top

f(a: 1, b: 2)
来源：http://fra.guowangkeji.top

[U57] PHP：字符串插值
来源：http://qem.chenzaomai.com

"值: {$a}"
来源：http://frq.yj20258888.top

[U58] PHP：数组三件套
来源：http://bpu.guowangkeji.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fov.aibaodan.cn

[U59] PHP：自定义排序
来源：http://pir.zhoulong.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pql.hywenlv.cn

[U60] PHP：JSON 编解码
来源：http://hdb.svipenyu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bzr.nanxuanxn.top

[U61] PHP：正则
来源：http://yoi.epnwcf.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xsr.hcnkem.com

[U62] PHP：日期对象
来源：http://fnb.fengsongda.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dmh.fehbvm.com

[U63] PHP：文件读写
来源：http://kjs.hcnkem.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hhp.jinqigufen.top

[U64] PHP：目录遍历
来源：http://dwo.yonumen.top

glob("dir/*.php");  scandir("dir");
来源：http://mgg.zdbjq.cn

[U65] PHP：会话
来源：http://ovo.shzxlz.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pdv.yj20258888.top

[U66] PHP：设置 Cookie
来源：http://npf.uphjek.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wed.yongpay.top

[U67] PHP：处理文件上传
来源：http://ldl.yanxiufei.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tod.meibo888.top

[U68] PHP：PDO 连接
来源：http://gfl.havefunace.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bna.feifeiyinyue.top

[U69] PHP：PDO 预处理
来源：http://wiv.jqgfzy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bin.c1oappe.top

[U70] PHP：PDO 事务
来源：http://loi.zhaomingkeji.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wop.wangshuangyany.cn

[U71] PHP：抛出异常
来源：http://nsg.quarkkingdee.top

throw new RuntimeException("失败", 500);
来源：http://kls.shanyushiyangtech.top

[U72] PHP：写错误日志
来源：http://lst.jinyuanbaomall.cn

error_log("失败: " . $e->getMessage());
来源：http://kdi.daxiang520.top

[U73] PHP：读取 ini 配置
来源：http://lhv.ywan-chungtsiang.top

parse_ini_file("config.ini", true)
来源：http://mbn.birdmap.top

[U74] PHP：读取环境变量
来源：http://ghm.fehbvm.com

getenv("APP_ENV") ?: "production"
来源：http://rwm.hfpthk.cn

[U75] PHP：依赖注入
来源：http://prv.jqgufenzy.top

composer require psr/container
来源：http://qyt.yfazqb.com

[U76] PHP：简单路由
来源：http://tof.hongshengwenyu.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yxy.zycfv.cn

[U77] PHP：模板渲染
来源：http://mqb.yuxming.cn

composer require twig/twig
来源：http://lkd.yanxiufei.cn

[U78] PHP：单元测试
来源：http://dbc.pengpengdd.cyou

composer require --dev phpunit/phpunit
来源：http://fsc.jinyuanbaomall.cn

[U79] PHP：静态分析
来源：http://qyv.redwolf501.top

composer require --dev phpstan/phpstan
来源：http://lgt.birdmap.top

[U80] PHP：代码规范修复
来源：http://vwe.ywan-chungtsiang.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://rpq.ppjwa.cn

[U81] JS：初始化项目
来源：http://lga.fktsv.cn

npm init -y;  npm i express
来源：http://dvn.vqdsnc.cn

[U82] JS：package.json 脚本
来源：http://nsh.bbcook.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yno.zdqjudy.top

[U83] JS：ES Module 导入导出
来源：http://diy.hesvh.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ncu.ctjpmb.com

[U84] JS：CommonJS 写法
来源：http://ikz.jqgufenzy.top

module.exports = { a };  const { a } = require("./m");
来源：http://day.316326.xyz

[U85] JS：可选链
来源：http://djd.cqqwz.cn

a?.b?.c
来源：http://wqc.shuidangran.top

[U86] JS：空值合并
来源：http://xro.zhongyouzk.top

a ?? b
来源：http://mnu.cashguo.top

[U87] JS：解构默认值
来源：http://tay.havefunace.top

const { a = 1, b = 2 } = obj;
来源：http://utt.uphjek.com

[U88] JS：对象展开合并
来源：http://ceo.andypj.xyz

{ ...a, ...b }
来源：http://wgq.hcnkem.com

[U89] JS：数组去重
来源：http://euh.andypj.xyz

[...new Set(arr)]
来源：http://hfb.feifeiyinyue.top

[U90] JS：数字数组排序
来源：http://pgv.tarul.cn

[...arr].sort((a, b) => a - b)
来源：http://syp.ppjwa.cn

[U91] JS：对象键值遍历
来源：http://aen.uphjek.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://csl.sufxvd.cn

[U92] JS：深拷贝
来源：http://zgt.shanyushiyangtech.top

structuredClone(obj)
来源：http://hlb.epnwcf.com

[U93] JS：模板字符串
来源：http://abl.chenzaomai.com

`共 ${n} 条`
来源：http://atb.chenzaomai.com

[U94] JS：箭头函数
来源：http://kys.tarul.cn

const double = x => x * 2;
来源：http://yqd.pengpengdd.cyou

[U95] JS：Promise 包装
来源：http://pgy.cashguo.top

new Promise((resolve, reject) => {})
来源：http://ron.fktsv.cn

[U96] JS：async/await 与异常
来源：http://hfn.svipenyu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gma.yuanzhike.top

[U97] JS：并发请求
来源：http://lay.hammf.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://klz.yongpay.top

[U98] JS：fetch 带 JSON
来源：http://eby.nwbrower.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hcr.yongpay.top

[U99] JS：事件监听
来源：http://pka.ehwqpu.com

el.addEventListener("click", e => {})
来源：http://dvu.sweek.top

[U100] JS：DOM 查询
来源：http://qii.hongshengwenyu.top

document.querySelector(".item")
来源：http://bjx.jyoumei.cn

[U101] JS：classList 操作
来源：http://kxi.hammf.cn

el.classList.toggle("active")
来源：http://gcx.xuetiantiany.cn

[U102] JS：本地存储
来源：http://lkz.9152youxi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bjf.xinyue.icu

[U103] JS：定时器
来源：http://edx.zdqjudy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cgy.zhiwuduotai.top

[U104] JS：防抖
来源：http://lms.yangfankeji.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ofi.redwolf501.top

[U105] JS：节流
来源：http://cen.pycfn.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ijl.ctjpmb.com

[U106] JS：日期格式化
来源：http://rnb.hnqzz.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zuo.shanyushiyangkeji.top

[U107] JS：数字千分位
来源：http://dib.chenjidiqi.icu

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zcy.sjlbkw.cn

[U108] JS：随机整数
来源：http://eav.hfpthk.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gfo.jlsjyb.cn

[U109] JS：数组分组
来源：http://qxh.smart0.xyz

Object.groupBy(arr, x => x.type)
来源：http://yyz.vehdjk.com

[U110] JS：数组分块
来源：http://iqa.daxiang520.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://khh.birdmap.top

[U111] JS：对象转 Map
来源：http://der.jianghu66.top

new Map(Object.entries(obj))
来源：http://qau.jianghu66.top

[U112] JS：字符串补位
来源：http://hnq.jqgufenzy.top

"7".padStart(3, "0")
来源：http://zqc.dianchejie.cn

[U113] JS：正则替换全部
来源：http://jpq.zhoulong.xyz

s.replaceAll("a", "b")
来源：http://ejt.jinqigfzy.top

[U114] JS：JSON 深比较
来源：http://qsk.hesvh.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://pgl.ydjk.org.cn

[U115] JS：生成 UUID
来源：http://zyr.shangyingyoupin.top

crypto.randomUUID()
来源：http://exs.hfpthk.cn

[U116] JS：类型检查（JSDoc）
来源：http://ntr.fzhhl.top

/** @param {string} name */ function f(name) {}
来源：http://txe.yj20258888.top

[U117] JS：单元测试
来源：http://qfx.316326.xyz

npm i -D vitest;  npx vitest
来源：http://pek.hfpthk.cn

[U118] JS：开发服务器
来源：http://bea.hnxiangtu.top

npm i -D vite;  npx vite
来源：http://lpf.tian-w.cn

[U119] JS：生产构建
来源：http://gta.xziqi.cn

npx vite build
来源：http://zon.sweek.top

[U120] JS：读取环境变量（Vite）
来源：http://coy.daria6918.cn

import.meta.env.VITE_API_URL
来源：http://aea.jinyuanbaomall.cn

================================================================================
来源：http://zmc.jinyuanbaomall.cn

统计汇总
来源：http://cwv.quarkkingdee.top

================================================================================
来源：http://gph.havefunace.top

按语言统计（条）：
来源：http://ylh.jqgufenzy.top

Python ......... 252
来源：http://fnw.vehdjk.com

PHP ............ 252
来源：http://yve.gzhubu.top

JavaScript ..... 252
来源：http://ieq.birdmap.top

TypeScript ..... 212
来源：http://vqr.zhiwuduotai.top

Java ........... 212
来源：http://fnp.c1oappe.top

Go ............. 212
来源：http://wmt.andypj.xyz

Ruby ........... 212
来源：http://mum.hnxiangtu.top

C# ............. 212
来源：http://uws.ywan-chungtsiang.top

C .............. 30
来源：http://mnt.zhiwuduotai.top

C++ ............ 30
来源：http://qoy.ehwqpu.com

SQL ............ 90
来源：http://pwd.shuidangran.top

Bash ........... 80
来源：http://qjl.yangfankeji.com

Kotlin ......... 15
来源：http://ulu.shangyingyoupin.top

Swift .......... 15
来源：http://tov.fehbvm.com

Lua ............ 10
来源：http://zaw.xinyue.icu

Perl ........... 10
来源：http://brn.xinyue.icu

Scala .......... 10
来源：http://xrq.jinghuilouyu.cn

------------------------------------
来源：http://sxy.hesvh.cn

合计 ........... 2106 条
来源：http://ukb.cashguo.top

按章节统计：
来源：http://zpk.fanxiaobao.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zse.uphjek.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fps.zycfv.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nuc.yj20258888.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ydb.cqqwz.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hvx.jinghuilouyu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lwz.uphjek.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tdn.xinyue.icu

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fku.ehwqpu.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://czx.tanke756.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ief.iojbl.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kbx.zhiwuduotai.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tey.smart0.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://eer.cdnleiting.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://koo.xingfuxueyuan.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nor.tarul.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://pgn.sufxvd.cn

Q SQL 专题                              90
来源：http://adc.bjfxy.top

R Bash 专题                             80
来源：http://uec.cdnleiting.top

S C / C++ 专题                          60
来源：http://vol.yonumen.top

T 其他语言补充                          60
来源：http://cdb.9152youxi.cn

U 高频实用片段                         120
来源：http://uoi.dianchejie.cn

------------------------------------
来源：http://tuy.yj20258888.top

合计                                  2106 条
来源：http://qmy.yj20258.top

--------------------------------------------------------------------------------
来源：http://chp.hywenlv.cn

使用提醒
来源：http://xsb.daxiang520.top

--------------------------------------------------------------------------------
来源：http://qcs.fktsv.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wuz.svipenyu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://snq.svipenyu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xdu.jinghuilouyu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://jgz.uphjek.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://iio.jinqigufen.top

—— 文件结束 ——
来源：http://odk.cheryme.top

================================================================================
来源：http://met.yonumen.top

程序语言常见例子速查手册（2024 版）
来源：http://meh.xuanzx.com

Common Programming Examples Cheat Book
来源：http://otz.pycfn.com

================================================================================
来源：http://tcd.gotoacloud.top

【收录内容】
来源：http://jmy.hnxiangtu.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://yjz.epnwcf.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://svi.shanyushiyangtech.top

SQL · Bash · C · C++
来源：http://ycc.ydzc1.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xtt.chenjidiqi.icu

【使用说明】
来源：http://qgr.gzhubu.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://leq.yanxiufei.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kre.vqdsnc.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vjw.xinyue.icu

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lpk.dashuyun.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://mmm.haohaochexian.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rrz.yonumen.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ack.hfpthk.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vtg.yueranfly.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ocx.epnwcf.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xje.hcnkem.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ybl.uphjek.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://thz.zhaomingkeji.xyz

【文件统计】
来源：http://tfh.xingfuxueyuan.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mwc.zhaomingkeji.xyz

--------------------------------------------------------------------------------
来源：http://dwf.hesvh.cn

目  录
来源：http://cxy.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://fip.birdmap.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://laa.xinyue.icu

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://nwl.xingfuxueyuan.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zxl.fengsongda.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://btu.yuanzhike.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qie.yj20258.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kih.shanyushiyangtech.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://aoi.ppjwa.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://egj.ctjpmb.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qmx.shanyushiyangkeji.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ose.wangdashe.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://tkh.fktsv.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qfk.cucudq.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://psw.hywenlv.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cun.andypj.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xpu.xingfuxueyuan.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://iqq.ivvv.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zki.hfpthk.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://fhl.fzhhl.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cvh.zdqjudy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cqp.ppjwa.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zgf.iojbl.cn

================================================================================
来源：http://huv.cheryme.top

A. 基础语法与类型
来源：http://tgm.yfazqb.com

================================================================================
来源：http://vsr.cashguo.top

[A01] Hello World
来源：http://nhs.nwbrower.top

Py:   print("Hello, World!")
来源：http://rsy.hnxiangtu.top

PHP:  echo "Hello, World!";
来源：http://pdh.yueranfly.top

JS:   console.log("Hello, World!");
来源：http://nnl.tianlin.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pqw.zdqjudy.top

Java: System.out.println("Hello, World!");
来源：http://zny.jinqigufen.top

Go:   fmt.Println("Hello, World!")
来源：http://nsa.yueranfly.top

Ruby: puts "Hello, World!"
来源：http://qez.xingfuxueyuan.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://cli.redwolf501.top

[A02] 变量声明与赋值
来源：http://clj.shanyushiyangtech.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bbt.gotoacloud.top

PHP:  $name = "Alex"; $age = 20;
来源：http://hvv.sjlbkw.cn

JS:   let name = "Alex"; const age = 20;
来源：http://qhv.iojbl.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ufs.redwolf501.top

Java: String name = "Alex"; int age = 20;
来源：http://gdc.guannengcc.top

Go:   name := "Alex"; age := 20
来源：http://bog.uphjek.com

Ruby: name = "Alex"; age = 20
来源：http://fof.fengsongda.top

C#:   string name = "Alex"; int age = 20;
来源：http://dto.zhaomingkeji.xyz

[A03] 常量定义
来源：http://cop.sxryk.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mxg.daxiang520.top

PHP:  const PI = 3.14159;
来源：http://zjq.yonumen.top

JS:   const PI = 3.14159;
来源：http://vbb.dianchejie.cn

TS:   const PI: number = 3.14159;
来源：http://qfy.hysaishi.cn

Java: static final double PI = 3.14159;
来源：http://jgb.0kj1m.cn

Go:   const PI = 3.14159
来源：http://pne.zycfv.cn

Ruby: PI = 3.14159
来源：http://tdy.jinghuilouyu.cn

C#:   const double PI = 3.14159;
来源：http://gwm.guannengcc.top

[A04] 判断变量类型
来源：http://ato.chenjidiqi.icu

Py:   type(x).__name__; isinstance(x, int)
来源：http://uoc.ctjpmb.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rxh.xylfe.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ojk.sufxvd.cn

TS:   typeof x; x instanceof Date
来源：http://vnm.xuanzx.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kzc.chenzaomai.com

Go:   reflect.TypeOf(x).Name()
来源：http://nhi.zdbjq.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://fzi.daria6918.cn

C#:   x.GetType().Name; x is int
来源：http://guq.iojbl.cn

[A05] 整数除法与取模
来源：http://vdw.yfazqb.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nva.shuidangran.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://adh.svipenyu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ael.hesvh.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mjd.zdbjq.cn

Java: 7 / 2; 7 % 2
来源：http://xhn.ybcxt.top

Go:   7 / 2; 7 % 2
来源：http://swx.yonumen.top

Ruby: 7 / 2; 7 % 2
来源：http://vmn.wangshuangyany.cn

C#:   7 / 2; 7 % 2
来源：http://odf.hammf.cn

[A06] 字符串转数字
来源：http://wru.zhixingplan.top

Py:   int("42"); float("3.14")
来源：http://xff.zhaomingkeji.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://axg.jqgfzy.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pic.xuanzx.com


<!-- 参考信息 -->