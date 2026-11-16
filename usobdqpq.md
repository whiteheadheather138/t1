代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://jco.zycfv.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://fte.dashuyun.cn

[U46] PHP：可空类型
来源：http://qye.bjfxy.top

?string $name = null
来源：http://hto.guowangkeji.top

[U47] PHP：联合类型
来源：http://vbk.tanke756.top

int|string $id
来源：http://wag.xingfuxueyuan.xyz

[U48] PHP：纯枚举
来源：http://umt.cdnleiting.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rbx.smart0.xyz

[U49] PHP：只读属性
来源：http://iip.yfazqb.com

public readonly string $name
来源：http://tdj.jianghu66.top

[U50] PHP：构造器属性提升
来源：http://tpz.xylfe.cn

public function __construct(private int $id) {}
来源：http://eoe.sjlbkw.cn

[U51] PHP：数组解构
来源：http://ybq.yueranfly.top

[$a, $b] = $arr;
来源：http://hbh.hfpthk.cn

[U52] PHP：箭头函数
来源：http://rij.hnqzz.top

$double = fn($x) => $x * 2;
来源：http://ram.sxryk.cn

[U53] PHP：空合并运算符
来源：http://dop.ppjwa.cn

$v = $a ?? $b ?? "default";
来源：http://wcx.yfazqb.com

[U54] PHP：空安全调用
来源：http://iqi.guannengcc.top

$obj?->method()
来源：http://gau.ivvv.top

[U55] PHP：match 表达式
来源：http://kpv.jinghuilouyu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gfa.smart0.xyz

[U56] PHP：命名参数
来源：http://nmk.zhoulong.xyz

f(a: 1, b: 2)
来源：http://rgf.xingfuxueyuan.xyz

[U57] PHP：字符串插值
来源：http://ycm.jinqigufen.top

"值: {$a}"
来源：http://vqg.sjlbkw.cn

[U58] PHP：数组三件套
来源：http://gnh.ivvv.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://aqo.yongpay.top

[U59] PHP：自定义排序
来源：http://xfk.vehdjk.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ydq.gaohongyu789.top

[U60] PHP：JSON 编解码
来源：http://cze.hysaishi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hex.zhiwuduotai.top

[U61] PHP：正则
来源：http://psh.smart0.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yib.yj20258888.top

[U62] PHP：日期对象
来源：http://hvh.shangyingyoupin.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jlh.ywan-chungtsiang.top

[U63] PHP：文件读写
来源：http://yyt.ppjwa.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hzz.gogol.net.cn

[U64] PHP：目录遍历
来源：http://kfv.quarkkingdee.top

glob("dir/*.php");  scandir("dir");
来源：http://xtf.jiagoushi.top

[U65] PHP：会话
来源：http://eny.dashuyun.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://xsc.yonumen.top

[U66] PHP：设置 Cookie
来源：http://lag.hammf.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zxn.sjlbkw.cn

[U67] PHP：处理文件上传
来源：http://jtp.xinyue.icu

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://oqm.ivvv.top

[U68] PHP：PDO 连接
来源：http://qdy.hnxiangtu.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://def.uphjek.com

[U69] PHP：PDO 预处理
来源：http://ene.svipenyu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://czr.chenlongwang.top

[U70] PHP：PDO 事务
来源：http://kwa.nanxinkj.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sbf.xylfe.cn

[U71] PHP：抛出异常
来源：http://avp.cheryme.top

throw new RuntimeException("失败", 500);
来源：http://xxs.jqgufenzy.top

[U72] PHP：写错误日志
来源：http://geh.epnwcf.com

error_log("失败: " . $e->getMessage());
来源：http://chk.sufxvd.cn

[U73] PHP：读取 ini 配置
来源：http://grl.yueranfly.top

parse_ini_file("config.ini", true)
来源：http://qrd.ehwqpu.com

[U74] PHP：读取环境变量
来源：http://kzl.quarkkingdee.top

getenv("APP_ENV") ?: "production"
来源：http://zwx.vehdjk.com

[U75] PHP：依赖注入
来源：http://hsq.jiagoushi.top

composer require psr/container
来源：http://rwh.ywan-chungtsiang.top

[U76] PHP：简单路由
来源：http://qbo.jyoumei.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://krl.yj202588.top

[U77] PHP：模板渲染
来源：http://iyw.chenjidiqi.icu

composer require twig/twig
来源：http://mie.0kj1m.cn

[U78] PHP：单元测试
来源：http://rry.wangdashe.top

composer require --dev phpunit/phpunit
来源：http://kuy.shanyushiyangkeji.top

[U79] PHP：静态分析
来源：http://wfe.jyoumei.cn

composer require --dev phpstan/phpstan
来源：http://rrd.yueranfly.top

[U80] PHP：代码规范修复
来源：http://yyi.yfazqb.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://qlr.jlsjyb.cn

[U81] JS：初始化项目
来源：http://guq.zhongyouzk.top

npm init -y;  npm i express
来源：http://xgl.zhoulong.xyz

[U82] JS：package.json 脚本
来源：http://hnq.ydzc1.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mhg.yfazqb.com

[U83] JS：ES Module 导入导出
来源：http://esq.ivvv.top

export const a = 1;  import { a } from "./m.js";
来源：http://glh.ehwqpu.com

[U84] JS：CommonJS 写法
来源：http://vsn.cashguo.top

module.exports = { a };  const { a } = require("./m");
来源：http://ocx.pengpengdd.cyou

[U85] JS：可选链
来源：http://uwh.cdnleiting.top

a?.b?.c
来源：http://rae.zhiwuduotai.top

[U86] JS：空值合并
来源：http://ynw.redwolf501.top

a ?? b
来源：http://ske.vehdjk.com

[U87] JS：解构默认值
来源：http://nsq.svipenyu.cn

const { a = 1, b = 2 } = obj;
来源：http://ptp.ppjwa.cn

[U88] JS：对象展开合并
来源：http://dwy.gotoacloud.top

{ ...a, ...b }
来源：http://jir.jianghu66.top

[U89] JS：数组去重
来源：http://ohf.ywan-chungtsiang.top

[...new Set(arr)]
来源：http://fwf.hcnkem.com

[U90] JS：数字数组排序
来源：http://gkm.yanxiufei.cn

[...arr].sort((a, b) => a - b)
来源：http://xtc.sweek.top

[U91] JS：对象键值遍历
来源：http://wrp.hesvh.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vea.316326.xyz

[U92] JS：深拷贝
来源：http://xbr.zycfv.cn

structuredClone(obj)
来源：http://pba.jqgufenzy.top

[U93] JS：模板字符串
来源：http://jyg.gzhubu.top

`共 ${n} 条`
来源：http://vlu.zhengqikj.top

[U94] JS：箭头函数
来源：http://djc.chenzaomai.com

const double = x => x * 2;
来源：http://vwx.tian-w.cn

[U95] JS：Promise 包装
来源：http://weh.zhoulong.xyz

new Promise((resolve, reject) => {})
来源：http://jgp.fzhhl.top

[U96] JS：async/await 与异常
来源：http://adp.tanke756.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://reh.yuxming.cn

[U97] JS：并发请求
来源：http://pio.daxiang520.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://mfq.daria6918.cn

[U98] JS：fetch 带 JSON
来源：http://jbp.hammf.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pdw.aizwys.cn

[U99] JS：事件监听
来源：http://nzs.nanxinkj.top

el.addEventListener("click", e => {})
来源：http://ugi.cashguo.top

[U100] JS：DOM 查询
来源：http://sxv.hywenlv.cn

document.querySelector(".item")
来源：http://xbl.yuanzhike.top

[U101] JS：classList 操作
来源：http://pnt.316326.xyz

el.classList.toggle("active")
来源：http://fvf.daxiang520.top

[U102] JS：本地存储
来源：http://iem.havefunace.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://bdh.jlsjyb.cn

[U103] JS：定时器
来源：http://igd.xinyue.icu

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hkf.hammf.cn

[U104] JS：防抖
来源：http://udg.jiagoushi.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zur.ctjpmb.com

[U105] JS：节流
来源：http://hrn.daxiang520.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nyp.shanyushiyangkeji.top

[U106] JS：日期格式化
来源：http://why.haohaochexian.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://agd.fanxiaobao.xyz

[U107] JS：数字千分位
来源：http://joa.yonumen.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yhx.fehbvm.com

[U108] JS：随机整数
来源：http://jun.guowangkeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://oju.c1oappe.top

[U109] JS：数组分组
来源：http://try.yj202588.top

Object.groupBy(arr, x => x.type)
来源：http://dmb.jqgufenzy.top

[U110] JS：数组分块
来源：http://hxd.meibo888.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ysh.zdbjq.cn

[U111] JS：对象转 Map
来源：http://wke.xuetiantiany.cn

new Map(Object.entries(obj))
来源：http://vet.yanxiufei.cn

[U112] JS：字符串补位
来源：http://pxk.jinqigfzy.top

"7".padStart(3, "0")
来源：http://jcn.shangyingyoupin.top

[U113] JS：正则替换全部
来源：http://sve.fehbvm.com

s.replaceAll("a", "b")
来源：http://brp.tian-w.cn

[U114] JS：JSON 深比较
来源：http://dvd.sjlbkw.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://uzs.shuidangran.top

[U115] JS：生成 UUID
来源：http://ppj.guowangkeji.top

crypto.randomUUID()
来源：http://mcm.yueranfly.top

[U116] JS：类型检查（JSDoc）
来源：http://fiu.gotoacloud.top

/** @param {string} name */ function f(name) {}
来源：http://kmd.zhijiandao.cn

[U117] JS：单元测试
来源：http://tpt.shanyushiyangtech.top

npm i -D vitest;  npx vitest
来源：http://vzj.yj20258888.top

[U118] JS：开发服务器
来源：http://nkj.yfazqb.com

npm i -D vite;  npx vite
来源：http://vil.yueranfly.top

[U119] JS：生产构建
来源：http://lhn.jqgfzy.top

npx vite build
来源：http://qcv.kuanghao11.cn

[U120] JS：读取环境变量（Vite）
来源：http://zvv.andypj.xyz

import.meta.env.VITE_API_URL
来源：http://njl.hnxiangtu.top

================================================================================
来源：http://pgh.feifeiyinyue.top

统计汇总
来源：http://upn.tanke756.top

================================================================================
来源：http://gvf.shuidangran.top

按语言统计（条）：
来源：http://vjg.316326.xyz

Python ......... 252
来源：http://vnb.gaohongyu789.top

PHP ............ 252
来源：http://myo.gaohongyu789.top

JavaScript ..... 252
来源：http://oyz.316326.xyz

TypeScript ..... 212
来源：http://mtd.aizwys.cn

Java ........... 212
来源：http://rxz.zycfv.cn

Go ............. 212
来源：http://rjm.yueranfly.top

Ruby ........... 212
来源：http://sab.gaohongyu789.top

C# ............. 212
来源：http://kfg.yvedp.cn

C .............. 30
来源：http://mgk.nanxuanxn.top

C++ ............ 30
来源：http://lzl.316326.xyz

SQL ............ 90
来源：http://jws.cdnleiting.top

Bash ........... 80
来源：http://byc.hysaishi.cn

Kotlin ......... 15
来源：http://clx.jqgufenzy.top

Swift .......... 15
来源：http://cep.svipenyu.cn

Lua ............ 10
来源：http://tye.vqdsnc.cn

Perl ........... 10
来源：http://adn.havefunace.top

Scala .......... 10
来源：http://tab.shangyingyoupin.top

------------------------------------
来源：http://nte.quarkkingdee.top

合计 ........... 2106 条
来源：http://uhd.zdbjq.cn

按章节统计：
来源：http://hrk.andypj.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xwv.xuanzx.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nkp.zdbjq.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kyo.kuanghao11.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://oce.jinqigfzy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ghg.yueranfly.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://apw.316326.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uhc.ivvv.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://csa.svipenyu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fik.ctjpmb.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xef.feifeiyinyue.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://okx.hysaishi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zgz.chenjidiqi.icu

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jrk.gotoacloud.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cdw.hywenlv.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zwl.pycfn.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cjm.jqgufenzy.top

Q SQL 专题                              90
来源：http://dxr.zhaomingkeji.xyz

R Bash 专题                             80
来源：http://ffq.hywenlv.cn

S C / C++ 专题                          60
来源：http://yms.chenzaomai.com

T 其他语言补充                          60
来源：http://zbd.ydzc1.top

U 高频实用片段                         120
来源：http://pth.yj20258.top

------------------------------------
来源：http://yqc.xingfuxueyuan.xyz

合计                                  2106 条
来源：http://eim.yuanzhike.top

--------------------------------------------------------------------------------
来源：http://oew.vehdjk.com

使用提醒
来源：http://jne.fzhhl.top

--------------------------------------------------------------------------------
来源：http://dvy.quarkkingdee.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dil.c1oappe.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tax.shzxlz.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://koy.cdnleiting.top

在旧版本上使用前请先确认语法支持情况。
来源：http://hnz.iojbl.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mwd.jinqigufen.top

—— 文件结束 ——
来源：http://pll.316326.xyz

================================================================================
来源：http://rqg.havefunace.top

程序语言常见例子速查手册（2024 版）
来源：http://kbv.yueranfly.top

Common Programming Examples Cheat Book
来源：http://qli.tanke756.top

================================================================================
来源：http://omk.redwolf501.top

【收录内容】
来源：http://hrk.dianchejie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://zwy.hongshengwenyu.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ykm.hywenlv.cn

SQL · Bash · C · C++
来源：http://akm.yj202588.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tuv.yangfankeji.com

【使用说明】
来源：http://uic.yonumen.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wwa.sxryk.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://abt.hongshengwenyu.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pck.fktsv.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gbk.xinyue.icu

Bash:  Shell         C:     C             C++:   C++
来源：http://zcg.yonumen.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qok.yuxming.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gay.xuetiantiany.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zhb.hfpthk.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://uaq.fengsongda.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://phc.yangfankeji.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ahe.ivvv.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ais.zhixingplan.top

【文件统计】
来源：http://ntg.316326.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://irt.c1oappe.top

--------------------------------------------------------------------------------
来源：http://koo.fengsongda.top

目  录
来源：http://jut.vehdjk.com

--------------------------------------------------------------------------------
来源：http://bdh.gaohongyu789.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dks.hcnkem.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ewi.zycfv.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://yzm.aibaodan.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hxt.svipenyu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nxn.cashguo.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://znx.xingfuxueyuan.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://alx.pengpengdd.cyou

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://lrb.hysaishi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kcv.pycfn.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://udo.zhoulong.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vli.bjfxy.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://oez.yongpay.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gqe.nanxuanxn.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vqr.iojbl.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lex.mhx1999.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xnx.haohaochexian.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ife.svipenyu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://lpx.hammf.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://nrs.iojbl.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cis.hongshengwenyu.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://bar.hfpthk.cn

================================================================================
来源：http://zkp.zhongyouzk.top

A. 基础语法与类型
来源：http://kdp.zhixingplan.top

================================================================================
来源：http://hpl.ybcxt.top

[A01] Hello World
来源：http://krz.yuxming.cn

Py:   print("Hello, World!")
来源：http://nuo.ydzc1.top

PHP:  echo "Hello, World!";
来源：http://mxa.hongshengwenyu.top

JS:   console.log("Hello, World!");
来源：http://rxz.xylfe.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qyo.fktsv.cn

Java: System.out.println("Hello, World!");
来源：http://aso.zhoulong.xyz

Go:   fmt.Println("Hello, World!")
来源：http://pyq.yuxming.cn

Ruby: puts "Hello, World!"
来源：http://pbe.hongshengwenyu.top

C#:   Console.WriteLine("Hello, World!");
来源：http://nml.pycfn.com

[A02] 变量声明与赋值
来源：http://thr.0kj1m.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jma.hammf.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://foq.daria6918.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ukd.bbcook.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vao.jianghu66.top

Java: String name = "Alex"; int age = 20;
来源：http://eyf.chenjidiqi.icu

Go:   name := "Alex"; age := 20
来源：http://ebc.vehdjk.com

Ruby: name = "Alex"; age = 20
来源：http://uix.vehdjk.com

C#:   string name = "Alex"; int age = 20;
来源：http://ysv.9152youxi.cn

[A03] 常量定义
来源：http://fhz.zhoulong.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://lic.jiagoushi.top

PHP:  const PI = 3.14159;
来源：http://tpd.hcnkem.com

JS:   const PI = 3.14159;
来源：http://ppb.hongshengwenyu.top

TS:   const PI: number = 3.14159;
来源：http://etn.hesvh.cn

Java: static final double PI = 3.14159;
来源：http://iix.pycfn.com

Go:   const PI = 3.14159
来源：http://azl.xuetiantiany.cn

Ruby: PI = 3.14159
来源：http://lsr.yfazqb.com

C#:   const double PI = 3.14159;
来源：http://dhn.jinqigfzy.top

[A04] 判断变量类型
来源：http://vfv.cheryme.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://wqe.jianghu66.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gkk.jianghu66.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hgo.shangyingyoupin.top

TS:   typeof x; x instanceof Date
来源：http://vok.quarkkingdee.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tny.tarul.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ygo.tanke756.top

Ruby: x.class; x.is_a?(Integer)
来源：http://khs.ppjwa.cn

C#:   x.GetType().Name; x is int
来源：http://shz.chenzaomai.com

[A05] 整数除法与取模
来源：http://ypg.vqdsnc.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://eqi.tarul.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://fth.hcnkem.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://stc.nwbrower.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://epv.chenjidiqi.icu


<!-- 参考信息 -->