代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://vxu.yj202588.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://yqs.hfpthk.cn

[U46] PHP：可空类型
来源：http://atb.yfazqb.com

?string $name = null
来源：http://guh.chenzaomai.com

[U47] PHP：联合类型
来源：http://qye.ywan-chungtsiang.top

int|string $id
来源：http://rov.vehdjk.com

[U48] PHP：纯枚举
来源：http://vqj.feifeiyinyue.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fcd.wangshuangyany.cn

[U49] PHP：只读属性
来源：http://crn.tarul.cn

public readonly string $name
来源：http://fyf.zhoulong.xyz

[U50] PHP：构造器属性提升
来源：http://afo.yuanzhike.top

public function __construct(private int $id) {}
来源：http://drc.aizwys.cn

[U51] PHP：数组解构
来源：http://ehl.fanxiaobao.xyz

[$a, $b] = $arr;
来源：http://tki.havefunace.top

[U52] PHP：箭头函数
来源：http://jwz.yvedp.cn

$double = fn($x) => $x * 2;
来源：http://hng.cucudq.cn

[U53] PHP：空合并运算符
来源：http://krc.daria6918.cn

$v = $a ?? $b ?? "default";
来源：http://kfa.jianghu66.top

[U54] PHP：空安全调用
来源：http://hra.gogol.net.cn

$obj?->method()
来源：http://hib.jlsjyb.cn

[U55] PHP：match 表达式
来源：http://fim.ydjk.org.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qco.redwolf501.top

[U56] PHP：命名参数
来源：http://tro.gotoacloud.top

f(a: 1, b: 2)
来源：http://dld.ivvv.top

[U57] PHP：字符串插值
来源：http://cep.zhongyouzk.top

"值: {$a}"
来源：http://nks.xuetiantiany.cn

[U58] PHP：数组三件套
来源：http://zso.daxiang520.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zzh.ctjpmb.com

[U59] PHP：自定义排序
来源：http://lii.nwbrower.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zey.chenzaomai.com

[U60] PHP：JSON 编解码
来源：http://enr.aizwys.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gpg.9152youxi.cn

[U61] PHP：正则
来源：http://sur.xuetiantiany.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bzr.tianlin.xyz

[U62] PHP：日期对象
来源：http://tot.ppjwa.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cpk.c1oappe.top

[U63] PHP：文件读写
来源：http://spb.fehbvm.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kyy.9152youxi.cn

[U64] PHP：目录遍历
来源：http://bqi.hongshengwenyu.top

glob("dir/*.php");  scandir("dir");
来源：http://lqu.hfpthk.cn

[U65] PHP：会话
来源：http://rxw.jlsjyb.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://xos.sufxvd.cn

[U66] PHP：设置 Cookie
来源：http://ejh.52xcode.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://syn.zhaomingkeji.xyz

[U67] PHP：处理文件上传
来源：http://dkp.havefunace.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mjz.c1oappe.top

[U68] PHP：PDO 连接
来源：http://knl.ivvv.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uwo.yonumen.top

[U69] PHP：PDO 预处理
来源：http://oif.havefunace.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ggi.redwolf501.top

[U70] PHP：PDO 事务
来源：http://axe.fengsongda.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kyz.aibaodan.cn

[U71] PHP：抛出异常
来源：http://neh.sjlbkw.cn

throw new RuntimeException("失败", 500);
来源：http://gzy.c1oappe.top

[U72] PHP：写错误日志
来源：http://urk.nanxuanxn.top

error_log("失败: " . $e->getMessage());
来源：http://asu.meibo888.top

[U73] PHP：读取 ini 配置
来源：http://flp.wangdashe.top

parse_ini_file("config.ini", true)
来源：http://lgh.zhongyouzk.top

[U74] PHP：读取环境变量
来源：http://iiv.snrcjt.cn

getenv("APP_ENV") ?: "production"
来源：http://sht.52xcode.cn

[U75] PHP：依赖注入
来源：http://czl.shuidangran.top

composer require psr/container
来源：http://zjm.shanyushiyangkeji.top

[U76] PHP：简单路由
来源：http://vxt.uphjek.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://urk.hysaishi.cn

[U77] PHP：模板渲染
来源：http://deu.chenzaomai.com

composer require twig/twig
来源：http://qqq.hammf.cn

[U78] PHP：单元测试
来源：http://hkj.jinghuilouyu.cn

composer require --dev phpunit/phpunit
来源：http://xlt.tian-w.cn

[U79] PHP：静态分析
来源：http://cjv.tarul.cn

composer require --dev phpstan/phpstan
来源：http://ctx.bbcook.cn

[U80] PHP：代码规范修复
来源：http://dci.jqgfzy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://kxc.tianlin.xyz

[U81] JS：初始化项目
来源：http://ber.bjfxy.top

npm init -y;  npm i express
来源：http://rwp.zhiwuduotai.top

[U82] JS：package.json 脚本
来源：http://ucd.yvedp.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ezp.nwbrower.top

[U83] JS：ES Module 导入导出
来源：http://ygw.hnxiangtu.top

export const a = 1;  import { a } from "./m.js";
来源：http://zsa.iojbl.cn

[U84] JS：CommonJS 写法
来源：http://zuq.zhaomingkeji.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://cig.zdbjq.cn

[U85] JS：可选链
来源：http://lhn.fanxiaobao.xyz

a?.b?.c
来源：http://rgl.yongpay.top

[U86] JS：空值合并
来源：http://mvy.kuanghao11.cn

a ?? b
来源：http://tea.xylfe.cn

[U87] JS：解构默认值
来源：http://bmx.hywenlv.cn

const { a = 1, b = 2 } = obj;
来源：http://ayy.yj20258888.top

[U88] JS：对象展开合并
来源：http://jdn.zhoulong.xyz

{ ...a, ...b }
来源：http://tfu.wangdashe.top

[U89] JS：数组去重
来源：http://iep.cqqwz.cn

[...new Set(arr)]
来源：http://bel.wangshuangyany.cn

[U90] JS：数字数组排序
来源：http://sqs.zhaomingkeji.xyz

[...arr].sort((a, b) => a - b)
来源：http://dbc.daria6918.cn

[U91] JS：对象键值遍历
来源：http://fai.aizwys.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kfz.xylfe.cn

[U92] JS：深拷贝
来源：http://gil.tianlin.xyz

structuredClone(obj)
来源：http://apo.gzhubu.top

[U93] JS：模板字符串
来源：http://ikl.tarul.cn

`共 ${n} 条`
来源：http://tih.feifeiyinyue.top

[U94] JS：箭头函数
来源：http://wxb.zycfv.cn

const double = x => x * 2;
来源：http://fcx.snrcjt.cn

[U95] JS：Promise 包装
来源：http://iqc.jlsjyb.cn

new Promise((resolve, reject) => {})
来源：http://qay.yangfankeji.com

[U96] JS：async/await 与异常
来源：http://vca.meibo888.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lhk.tarul.cn

[U97] JS：并发请求
来源：http://joy.yanxiufei.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://jfs.kuanghao11.cn

[U98] JS：fetch 带 JSON
来源：http://ibt.shangyingyoupin.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zwn.ydjk.org.cn

[U99] JS：事件监听
来源：http://fgl.tanke756.top

el.addEventListener("click", e => {})
来源：http://eqf.yvedp.cn

[U100] JS：DOM 查询
来源：http://gmo.c1oappe.top

document.querySelector(".item")
来源：http://jvr.yuanzhike.top

[U101] JS：classList 操作
来源：http://twp.ybcxt.top

el.classList.toggle("active")
来源：http://nbr.jinqigfzy.top

[U102] JS：本地存储
来源：http://jqe.chenlongwang.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://zjr.zhaomingkeji.xyz

[U103] JS：定时器
来源：http://lab.52xcode.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zhj.zhengqikj.top

[U104] JS：防抖
来源：http://hdc.haohaochexian.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ksw.jqgfzy.top

[U105] JS：节流
来源：http://nef.sufxvd.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://khs.c1oappe.top

[U106] JS：日期格式化
来源：http://fyi.jinyuanbaomall.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sfb.mhx1999.top

[U107] JS：数字千分位
来源：http://xbn.tianlin.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ima.jyoumei.cn

[U108] JS：随机整数
来源：http://iim.shuidangran.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://iqp.dianchejie.cn

[U109] JS：数组分组
来源：http://cdr.tian-w.cn

Object.groupBy(arr, x => x.type)
来源：http://vbv.hammf.cn

[U110] JS：数组分块
来源：http://ryc.kuanghao11.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fzi.ivvv.top

[U111] JS：对象转 Map
来源：http://lhr.xziqi.cn

new Map(Object.entries(obj))
来源：http://ptc.fanxiaobao.xyz

[U112] JS：字符串补位
来源：http://noh.xylfe.cn

"7".padStart(3, "0")
来源：http://vwz.cheryme.top

[U113] JS：正则替换全部
来源：http://mwu.jqgfzy.top

s.replaceAll("a", "b")
来源：http://nub.jinqigufen.top

[U114] JS：JSON 深比较
来源：http://eab.smart0.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://vsj.zhiwuduotai.top

[U115] JS：生成 UUID
来源：http://sjj.fzhhl.top

crypto.randomUUID()
来源：http://ikx.mhx1999.top

[U116] JS：类型检查（JSDoc）
来源：http://wvd.tianlin.xyz

/** @param {string} name */ function f(name) {}
来源：http://hqj.zycfv.cn

[U117] JS：单元测试
来源：http://qwn.316326.xyz

npm i -D vitest;  npx vitest
来源：http://ewa.0kj1m.cn

[U118] JS：开发服务器
来源：http://kts.fktsv.cn

npm i -D vite;  npx vite
来源：http://fzs.gotoacloud.top

[U119] JS：生产构建
来源：http://bjn.xinyue.icu

npx vite build
来源：http://jgo.fehbvm.com

[U120] JS：读取环境变量（Vite）
来源：http://krx.ydzc1.top

import.meta.env.VITE_API_URL
来源：http://fnn.xylfe.cn

================================================================================
来源：http://ina.shanyushiyangtech.top

统计汇总
来源：http://yvb.dianchejie.cn

================================================================================
来源：http://tio.jiagoushi.top

按语言统计（条）：
来源：http://ijd.ybcxt.top

Python ......... 252
来源：http://wuz.shanyushiyangtech.top

PHP ............ 252
来源：http://ekg.sweek.top

JavaScript ..... 252
来源：http://aow.cucudq.cn

TypeScript ..... 212
来源：http://zqe.fengsongda.top

Java ........... 212
来源：http://gts.yj202588.top

Go ............. 212
来源：http://mch.tanke756.top

Ruby ........... 212
来源：http://cty.fzhhl.top

C# ............. 212
来源：http://hhg.sjlbkw.cn

C .............. 30
来源：http://kky.xingfuxueyuan.xyz

C++ ............ 30
来源：http://ilk.yfazqb.com

SQL ............ 90
来源：http://siy.jinqigfzy.top

Bash ........... 80
来源：http://xyz.svipenyu.cn

Kotlin ......... 15
来源：http://jfl.tian-w.cn

Swift .......... 15
来源：http://toh.jyoumei.cn

Lua ............ 10
来源：http://kdt.shuidangran.top

Perl ........... 10
来源：http://ybe.jyoumei.cn

Scala .......... 10
来源：http://rif.ydzc1.top

------------------------------------
来源：http://dtg.fzhhl.top

合计 ........... 2106 条
来源：http://tqe.yonumen.top

按章节统计：
来源：http://ghl.jqgufenzy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wqu.zhongyouzk.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://swi.guowangkeji.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wug.jqgfzy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gew.jlsjyb.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://myr.vqdsnc.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pun.shuidangran.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://iwq.andypj.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jyn.wangdashe.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yya.yangfankeji.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ini.shzxlz.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://uro.sjlbkw.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vot.zhijiandao.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vvk.cqqwz.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://puh.jinyuanbaomall.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kqh.hnqzz.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rrr.yuxming.cn

Q SQL 专题                              90
来源：http://lnr.hesvh.cn

R Bash 专题                             80
来源：http://aaa.shzxlz.cn

S C / C++ 专题                          60
来源：http://qnr.kuanghao11.cn

T 其他语言补充                          60
来源：http://ilh.sufxvd.cn

U 高频实用片段                         120
来源：http://ihf.gzhubu.top

------------------------------------
来源：http://yfr.yvedp.cn

合计                                  2106 条
来源：http://ctj.vehdjk.com

--------------------------------------------------------------------------------
来源：http://ldy.bjfxy.top

使用提醒
来源：http://vua.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://jyu.wangdashe.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gvp.kuanghao11.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ujh.daxiang520.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tio.cashguo.top

在旧版本上使用前请先确认语法支持情况。
来源：http://bfk.feifeiyinyue.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gve.jinghuilouyu.cn

—— 文件结束 ——
来源：http://pgf.shangyingyoupin.top

================================================================================
来源：http://rxl.shangyingyoupin.top

程序语言常见例子速查手册（2024 版）
来源：http://acz.fehbvm.com

Common Programming Examples Cheat Book
来源：http://glx.wangshuangyany.cn

================================================================================
来源：http://qux.9152youxi.cn

【收录内容】
来源：http://pgn.zhongyouzk.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://akf.nanxinkj.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jye.sweek.top

SQL · Bash · C · C++
来源：http://lhz.redwolf501.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gtf.yj20258.top

【使用说明】
来源：http://klr.fzhhl.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nsk.vehdjk.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://irk.andypj.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mno.zhiwuduotai.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hbn.xziqi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://tra.jqgufenzy.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pdd.hongshengwenyu.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zeq.fanxiaobao.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pdh.yvedp.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ehf.c1oappe.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qkd.jinqigfzy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vgk.gaohongyu789.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mil.ivvv.top

【文件统计】
来源：http://yok.meibo888.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pza.nanxinkj.top

--------------------------------------------------------------------------------
来源：http://jnx.shzxlz.cn

目  录
来源：http://gdz.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://wix.cqqwz.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qql.daria6918.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bds.zhengqikj.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://sen.chenjidiqi.icu

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://nrj.jyoumei.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rbu.wangshuangyany.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://sek.tianlin.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vwm.xinyue.icu

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kjp.zhixingplan.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gml.hnxiangtu.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://seh.yj20258888.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ger.jinghuilouyu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://sap.nwbrower.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fho.tarul.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://veo.jqgufenzy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rld.snrcjt.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dqd.yanxiufei.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://uwy.yuanzhike.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://lob.chenzaomai.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mue.aizwys.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bir.shanyushiyangtech.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://eyd.jyoumei.cn

================================================================================
来源：http://gui.fanxiaobao.xyz

A. 基础语法与类型
来源：http://fzp.ehwqpu.com

================================================================================
来源：http://pky.hongshengwenyu.top

[A01] Hello World
来源：http://uyu.jianghu66.top

Py:   print("Hello, World!")
来源：http://uxv.kuanghao11.cn

PHP:  echo "Hello, World!";
来源：http://tnk.yanxiufei.cn

JS:   console.log("Hello, World!");
来源：http://cwa.yj20258888.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://asr.gotoacloud.top

Java: System.out.println("Hello, World!");
来源：http://csh.yfazqb.com

Go:   fmt.Println("Hello, World!")
来源：http://zva.haohaochexian.top

Ruby: puts "Hello, World!"
来源：http://mzt.jyoumei.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://cgk.bjfxy.top

[A02] 变量声明与赋值
来源：http://kat.birdmap.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nbv.hcnkem.com

PHP:  $name = "Alex"; $age = 20;
来源：http://kja.xuetiantiany.cn

JS:   let name = "Alex"; const age = 20;
来源：http://gvr.tanke756.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://oqt.andypj.xyz

Java: String name = "Alex"; int age = 20;
来源：http://noa.aibaodan.cn

Go:   name := "Alex"; age := 20
来源：http://uml.nwbrower.top

Ruby: name = "Alex"; age = 20
来源：http://ett.yonumen.top

C#:   string name = "Alex"; int age = 20;
来源：http://ann.svipenyu.cn

[A03] 常量定义
来源：http://fqc.yuxming.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://cqg.sysykeji.top

PHP:  const PI = 3.14159;
来源：http://vxk.chenzaomai.com

JS:   const PI = 3.14159;
来源：http://yyq.andypj.xyz

TS:   const PI: number = 3.14159;
来源：http://imx.wangshuangyany.cn

Java: static final double PI = 3.14159;
来源：http://jji.nanxinkj.top

Go:   const PI = 3.14159
来源：http://ydp.jqgfzy.top

Ruby: PI = 3.14159
来源：http://hkh.ppjwa.cn

C#:   const double PI = 3.14159;
来源：http://dey.cqqwz.cn

[A04] 判断变量类型
来源：http://coz.chenzaomai.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://hsg.ybcxt.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fgv.cdnleiting.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hdt.jinyuanbaomall.cn

TS:   typeof x; x instanceof Date
来源：http://xie.yvedp.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bjf.zhixingplan.top

Go:   reflect.TypeOf(x).Name()
来源：http://quj.yj202588.top

Ruby: x.class; x.is_a?(Integer)
来源：http://zmc.hcnkem.com

C#:   x.GetType().Name; x is int
来源：http://jwp.sysykeji.top

[A05] 整数除法与取模
来源：http://fin.jqgfzy.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://oge.tanke756.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ieq.gzhubu.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://evt.shzxlz.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bpa.epnwcf.com


<!-- 参考信息 -->