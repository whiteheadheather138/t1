代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://hnd.tianlin.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://met.nwbrower.top

[U46] PHP：可空类型
来源：http://xog.ivvv.top

?string $name = null
来源：http://ehf.fzhhl.top

[U47] PHP：联合类型
来源：http://keu.yuxming.cn

int|string $id
来源：http://xfr.ydjk.org.cn

[U48] PHP：纯枚举
来源：http://ufl.52xcode.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://njf.cashguo.top

[U49] PHP：只读属性
来源：http://xmr.hammf.cn

public readonly string $name
来源：http://ptp.gaohongyu789.top

[U50] PHP：构造器属性提升
来源：http://fak.zhengqikj.top

public function __construct(private int $id) {}
来源：http://rlu.zhongyouzk.top

[U51] PHP：数组解构
来源：http://pfk.jiagoushi.top

[$a, $b] = $arr;
来源：http://gpz.vehdjk.com

[U52] PHP：箭头函数
来源：http://nnl.cucudq.cn

$double = fn($x) => $x * 2;
来源：http://hoq.cqqwz.cn

[U53] PHP：空合并运算符
来源：http://scv.cdnleiting.top

$v = $a ?? $b ?? "default";
来源：http://jhk.sweek.top

[U54] PHP：空安全调用
来源：http://cgf.smart0.xyz

$obj?->method()
来源：http://rcn.zhijiandao.cn

[U55] PHP：match 表达式
来源：http://nfb.gotoacloud.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rpe.zycfv.cn

[U56] PHP：命名参数
来源：http://hig.ydjk.org.cn

f(a: 1, b: 2)
来源：http://ehv.ctjpmb.com

[U57] PHP：字符串插值
来源：http://hlv.fktsv.cn

"值: {$a}"
来源：http://aun.nanxuanxn.top

[U58] PHP：数组三件套
来源：http://uoh.jyoumei.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ivh.zhaomingkeji.xyz

[U59] PHP：自定义排序
来源：http://pjm.ppjwa.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://skp.yueranfly.top

[U60] PHP：JSON 编解码
来源：http://ncl.xuetiantiany.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://apd.hongshengwenyu.top

[U61] PHP：正则
来源：http://glc.iojbl.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mwu.tianlin.xyz

[U62] PHP：日期对象
来源：http://dna.fzhhl.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yir.kuanghao11.cn

[U63] PHP：文件读写
来源：http://fdv.daria6918.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xkp.sysykeji.top

[U64] PHP：目录遍历
来源：http://yjm.jqgfzy.top

glob("dir/*.php");  scandir("dir");
来源：http://zgi.shuidangran.top

[U65] PHP：会话
来源：http://xzh.jyoumei.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://sxw.yuxming.cn

[U66] PHP：设置 Cookie
来源：http://bhi.cucudq.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bku.jlsjyb.cn

[U67] PHP：处理文件上传
来源：http://smg.sufxvd.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bcn.hammf.cn

[U68] PHP：PDO 连接
来源：http://uvs.gaohongyu789.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hty.ppjwa.cn

[U69] PHP：PDO 预处理
来源：http://zrn.ctjpmb.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lwa.nwbrower.top

[U70] PHP：PDO 事务
来源：http://vac.yj202588.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://opy.zhaomingkeji.xyz

[U71] PHP：抛出异常
来源：http://pib.shzxlz.cn

throw new RuntimeException("失败", 500);
来源：http://upp.ydjk.org.cn

[U72] PHP：写错误日志
来源：http://krq.jqgfzy.top

error_log("失败: " . $e->getMessage());
来源：http://hic.vqdsnc.cn

[U73] PHP：读取 ini 配置
来源：http://nmq.xuetiantiany.cn

parse_ini_file("config.ini", true)
来源：http://csd.yueranfly.top

[U74] PHP：读取环境变量
来源：http://wgh.hywenlv.cn

getenv("APP_ENV") ?: "production"
来源：http://iie.gaohongyu789.top

[U75] PHP：依赖注入
来源：http://rir.yonumen.top

composer require psr/container
来源：http://noa.chenzaomai.com

[U76] PHP：简单路由
来源：http://mgh.9152youxi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://luk.ywan-chungtsiang.top

[U77] PHP：模板渲染
来源：http://sma.aizwys.cn

composer require twig/twig
来源：http://fei.xuanzx.com

[U78] PHP：单元测试
来源：http://mzl.xuetiantiany.cn

composer require --dev phpunit/phpunit
来源：http://rav.hcnkem.com

[U79] PHP：静态分析
来源：http://kix.cqqwz.cn

composer require --dev phpstan/phpstan
来源：http://eaf.hfpthk.cn

[U80] PHP：代码规范修复
来源：http://bwq.bjfxy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://zyf.andypj.xyz

[U81] JS：初始化项目
来源：http://kim.hnqzz.top

npm init -y;  npm i express
来源：http://npt.sysykeji.top

[U82] JS：package.json 脚本
来源：http://brx.smart0.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vpa.xinyue.icu

[U83] JS：ES Module 导入导出
来源：http://kku.jinghuilouyu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://esc.vehdjk.com

[U84] JS：CommonJS 写法
来源：http://pfm.yueranfly.top

module.exports = { a };  const { a } = require("./m");
来源：http://xlb.chenjidiqi.icu

[U85] JS：可选链
来源：http://zuc.cashguo.top

a?.b?.c
来源：http://izk.svipenyu.cn

[U86] JS：空值合并
来源：http://qio.hongshengwenyu.top

a ?? b
来源：http://mxl.yonumen.top

[U87] JS：解构默认值
来源：http://ghd.ydzc1.top

const { a = 1, b = 2 } = obj;
来源：http://fcs.ybcxt.top

[U88] JS：对象展开合并
来源：http://ery.tarul.cn

{ ...a, ...b }
来源：http://upz.gotoacloud.top

[U89] JS：数组去重
来源：http://frf.hnqzz.top

[...new Set(arr)]
来源：http://cjh.redwolf501.top

[U90] JS：数字数组排序
来源：http://tly.birdmap.top

[...arr].sort((a, b) => a - b)
来源：http://mdj.aibaodan.cn

[U91] JS：对象键值遍历
来源：http://drp.jqgfzy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lov.andypj.xyz

[U92] JS：深拷贝
来源：http://mnf.gaohongyu789.top

structuredClone(obj)
来源：http://zvg.hysaishi.cn

[U93] JS：模板字符串
来源：http://yqd.hywenlv.cn

`共 ${n} 条`
来源：http://qew.316326.xyz

[U94] JS：箭头函数
来源：http://egi.kuanghao11.cn

const double = x => x * 2;
来源：http://whj.0kj1m.cn

[U95] JS：Promise 包装
来源：http://ffi.pengpengdd.cyou

new Promise((resolve, reject) => {})
来源：http://pxa.0kj1m.cn

[U96] JS：async/await 与异常
来源：http://meo.gaohongyu789.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ixj.xuetiantiany.cn

[U97] JS：并发请求
来源：http://uee.jqgufenzy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://jpr.cqqwz.cn

[U98] JS：fetch 带 JSON
来源：http://cgt.fehbvm.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dnu.fzhhl.top

[U99] JS：事件监听
来源：http://srq.gaohongyu789.top

el.addEventListener("click", e => {})
来源：http://lkk.shangyingyoupin.top

[U100] JS：DOM 查询
来源：http://nwj.sjlbkw.cn

document.querySelector(".item")
来源：http://oef.snrcjt.cn

[U101] JS：classList 操作
来源：http://rzq.nanxuanxn.top

el.classList.toggle("active")
来源：http://kfa.wangshuangyany.cn

[U102] JS：本地存储
来源：http://lyd.hammf.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://quy.mhx1999.top

[U103] JS：定时器
来源：http://wka.hysaishi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dbm.aibaodan.cn

[U104] JS：防抖
来源：http://ogc.wangdashe.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fxu.shanyushiyangkeji.top

[U105] JS：节流
来源：http://etr.zdbjq.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lux.jyoumei.cn

[U106] JS：日期格式化
来源：http://lxr.shanyushiyangtech.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dxq.gaohongyu789.top

[U107] JS：数字千分位
来源：http://ofk.epnwcf.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gtn.ybcxt.top

[U108] JS：随机整数
来源：http://wso.daria6918.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ysq.mhx1999.top

[U109] JS：数组分组
来源：http://rvc.pycfn.com

Object.groupBy(arr, x => x.type)
来源：http://zno.xinyue.icu

[U110] JS：数组分块
来源：http://ixz.wangdashe.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uqn.nanxuanxn.top

[U111] JS：对象转 Map
来源：http://lpd.yangfankeji.com

new Map(Object.entries(obj))
来源：http://qzk.xinyue.icu

[U112] JS：字符串补位
来源：http://bky.dashuyun.cn

"7".padStart(3, "0")
来源：http://reo.mhx1999.top

[U113] JS：正则替换全部
来源：http://ocg.wangshuangyany.cn

s.replaceAll("a", "b")
来源：http://qxh.aizwys.cn

[U114] JS：JSON 深比较
来源：http://chs.tianlin.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://isj.jiagoushi.top

[U115] JS：生成 UUID
来源：http://wzv.shzxlz.cn

crypto.randomUUID()
来源：http://olu.xingfuxueyuan.xyz

[U116] JS：类型检查（JSDoc）
来源：http://jvd.tarul.cn

/** @param {string} name */ function f(name) {}
来源：http://xmi.feifeiyinyue.top

[U117] JS：单元测试
来源：http://pwr.316326.xyz

npm i -D vitest;  npx vitest
来源：http://pvy.sysykeji.top

[U118] JS：开发服务器
来源：http://uvm.hongshengwenyu.top

npm i -D vite;  npx vite
来源：http://vfk.zhoulong.xyz

[U119] JS：生产构建
来源：http://vbg.shuidangran.top

npx vite build
来源：http://kcq.hnxiangtu.top

[U120] JS：读取环境变量（Vite）
来源：http://mfy.yvedp.cn

import.meta.env.VITE_API_URL
来源：http://ciq.uphjek.com

================================================================================
来源：http://vix.jinghuilouyu.cn

统计汇总
来源：http://txz.xuetiantiany.cn

================================================================================
来源：http://hcb.jqgufenzy.top

按语言统计（条）：
来源：http://hfb.nanxinkj.top

Python ......... 252
来源：http://myb.guannengcc.top

PHP ............ 252
来源：http://ixf.xuetiantiany.cn

JavaScript ..... 252
来源：http://kyf.chenzaomai.com

TypeScript ..... 212
来源：http://fex.uphjek.com

Java ........... 212
来源：http://tao.jlsjyb.cn

Go ............. 212
来源：http://kco.fktsv.cn

Ruby ........... 212
来源：http://uoj.nwbrower.top

C# ............. 212
来源：http://vmx.shanyushiyangkeji.top

C .............. 30
来源：http://bqs.ydjk.org.cn

C++ ............ 30
来源：http://aap.ywan-chungtsiang.top

SQL ............ 90
来源：http://unv.nanxuanxn.top

Bash ........... 80
来源：http://tzc.ppjwa.cn

Kotlin ......... 15
来源：http://brk.chenzaomai.com

Swift .......... 15
来源：http://odw.nwbrower.top

Lua ............ 10
来源：http://jpk.sxryk.cn

Perl ........... 10
来源：http://ygv.c1oappe.top

Scala .......... 10
来源：http://tjg.yueranfly.top

------------------------------------
来源：http://eeh.xylfe.cn

合计 ........... 2106 条
来源：http://pxx.jinqigfzy.top

按章节统计：
来源：http://hka.cucudq.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://war.jinyuanbaomall.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hfe.xziqi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ktw.jinyuanbaomall.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://owo.jlsjyb.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zuc.yuxming.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://avi.fehbvm.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://heb.haohaochexian.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://end.0kj1m.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yya.sufxvd.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bzt.xziqi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://njj.epnwcf.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://haq.jinyuanbaomall.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cez.jianghu66.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://euz.daria6918.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zjh.yj20258.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yur.chenjidiqi.icu

Q SQL 专题                              90
来源：http://dlq.ppjwa.cn

R Bash 专题                             80
来源：http://owh.zdqjudy.top

S C / C++ 专题                          60
来源：http://uxm.yj20258.top

T 其他语言补充                          60
来源：http://oii.yonumen.top

U 高频实用片段                         120
来源：http://aqg.tian-w.cn

------------------------------------
来源：http://xrj.nanxinkj.top

合计                                  2106 条
来源：http://yxv.havefunace.top

--------------------------------------------------------------------------------
来源：http://iwv.sufxvd.cn

使用提醒
来源：http://nlc.tian-w.cn

--------------------------------------------------------------------------------
来源：http://szc.zhongyouzk.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://afs.svipenyu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://btz.jinghuilouyu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jhy.cucudq.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://diy.wangshuangyany.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://knl.feifeiyinyue.top

—— 文件结束 ——
来源：http://efc.chenjidiqi.icu

================================================================================
来源：http://joe.gotoacloud.top

程序语言常见例子速查手册（2024 版）
来源：http://fmo.yj202588.top

Common Programming Examples Cheat Book
来源：http://hjd.guannengcc.top

================================================================================
来源：http://cim.ppjwa.cn

【收录内容】
来源：http://lzf.zhixingplan.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://slt.aizwys.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nxp.cashguo.top

SQL · Bash · C · C++
来源：http://hiu.zhengqikj.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ied.jinghuilouyu.cn

【使用说明】
来源：http://hch.jinqigfzy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kgq.ehwqpu.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://gmp.jlsjyb.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kls.uphjek.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://myw.aizwys.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://fjw.ywan-chungtsiang.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kek.xingfuxueyuan.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cfd.xziqi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pbv.daria6918.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rbm.9152youxi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fwo.52xcode.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jvn.zhongyouzk.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kjr.guowangkeji.top

【文件统计】
来源：http://isl.cucudq.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vnl.tarul.cn

--------------------------------------------------------------------------------
来源：http://cqw.wangshuangyany.cn

目  录
来源：http://xmi.xinyue.icu

--------------------------------------------------------------------------------
来源：http://hhb.mhx1999.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fem.epnwcf.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xcd.xziqi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kns.jqgufenzy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ukg.aibaodan.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fhw.fanxiaobao.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wkr.nanxinkj.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://six.52xcode.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rcf.jinqigufen.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ldk.shzxlz.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rmy.316326.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://lim.zhongyouzk.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://nxo.gotoacloud.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ckz.xinyue.icu

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ssu.tanke756.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cay.xingfuxueyuan.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://min.smart0.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qgq.uphjek.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://ktk.andypj.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://grr.smart0.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gpy.yj20258888.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nki.nanxinkj.top

================================================================================
来源：http://luk.hywenlv.cn

A. 基础语法与类型
来源：http://bfm.shzxlz.cn

================================================================================
来源：http://ogk.gaohongyu789.top

[A01] Hello World
来源：http://bts.yongpay.top

Py:   print("Hello, World!")
来源：http://krc.jinyuanbaomall.cn

PHP:  echo "Hello, World!";
来源：http://fwk.haohaochexian.top

JS:   console.log("Hello, World!");
来源：http://sqn.vqdsnc.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nyy.mhx1999.top

Java: System.out.println("Hello, World!");
来源：http://oor.jqgfzy.top

Go:   fmt.Println("Hello, World!")
来源：http://evd.hammf.cn

Ruby: puts "Hello, World!"
来源：http://faw.cqqwz.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://gwe.xziqi.cn

[A02] 变量声明与赋值
来源：http://vvu.chenjidiqi.icu

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://umt.chenlongwang.top

PHP:  $name = "Alex"; $age = 20;
来源：http://uxc.birdmap.top

JS:   let name = "Alex"; const age = 20;
来源：http://jrl.jlsjyb.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bki.jinghuilouyu.cn

Java: String name = "Alex"; int age = 20;
来源：http://lui.gogol.net.cn

Go:   name := "Alex"; age := 20
来源：http://tfv.zycfv.cn

Ruby: name = "Alex"; age = 20
来源：http://qvf.xinyue.icu

C#:   string name = "Alex"; int age = 20;
来源：http://lht.gogol.net.cn

[A03] 常量定义
来源：http://fpn.ctjpmb.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://waf.0kj1m.cn

PHP:  const PI = 3.14159;
来源：http://vtu.chenzaomai.com

JS:   const PI = 3.14159;
来源：http://hnd.redwolf501.top

TS:   const PI: number = 3.14159;
来源：http://msr.yongpay.top

Java: static final double PI = 3.14159;
来源：http://zxs.wangdashe.top

Go:   const PI = 3.14159
来源：http://isp.fzhhl.top

Ruby: PI = 3.14159
来源：http://bzd.zycfv.cn

C#:   const double PI = 3.14159;
来源：http://skx.ivvv.top

[A04] 判断变量类型
来源：http://geq.52xcode.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://umt.cdnleiting.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://uch.chenjidiqi.icu

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://unu.shangyingyoupin.top

TS:   typeof x; x instanceof Date
来源：http://npy.xylfe.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pup.yj20258888.top

Go:   reflect.TypeOf(x).Name()
来源：http://jkw.bjfxy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://beq.yuanzhike.top

C#:   x.GetType().Name; x is int
来源：http://mhm.smart0.xyz

[A05] 整数除法与取模
来源：http://jra.sufxvd.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yak.tian-w.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://pdb.xuanzx.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://inh.hysaishi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cqh.birdmap.top


<!-- 参考信息 -->