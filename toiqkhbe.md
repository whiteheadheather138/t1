代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://aph.xziqi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://pzm.aibaodan.cn

[U46] PHP：可空类型
来源：http://nlp.dashuyun.cn

?string $name = null
来源：http://uop.smart0.xyz

[U47] PHP：联合类型
来源：http://kla.nanxinkj.top

int|string $id
来源：http://pkj.dashuyun.cn

[U48] PHP：纯枚举
来源：http://bki.fehbvm.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qsz.xziqi.cn

[U49] PHP：只读属性
来源：http://qig.jinyuanbaomall.cn

public readonly string $name
来源：http://sxv.quarkkingdee.top

[U50] PHP：构造器属性提升
来源：http://etk.sweek.top

public function __construct(private int $id) {}
来源：http://zoe.aibaodan.cn

[U51] PHP：数组解构
来源：http://dig.zhixingplan.top

[$a, $b] = $arr;
来源：http://sxg.yvedp.cn

[U52] PHP：箭头函数
来源：http://ghf.aizwys.cn

$double = fn($x) => $x * 2;
来源：http://hao.sjlbkw.cn

[U53] PHP：空合并运算符
来源：http://fmj.shanyushiyangtech.top

$v = $a ?? $b ?? "default";
来源：http://jnq.xylfe.cn

[U54] PHP：空安全调用
来源：http://mkc.sxryk.cn

$obj?->method()
来源：http://emv.cqqwz.cn

[U55] PHP：match 表达式
来源：http://pni.ctjpmb.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://auz.dianchejie.cn

[U56] PHP：命名参数
来源：http://ksf.tianlin.xyz

f(a: 1, b: 2)
来源：http://mpw.hcnkem.com

[U57] PHP：字符串插值
来源：http://sif.gogol.net.cn

"值: {$a}"
来源：http://cxn.yueranfly.top

[U58] PHP：数组三件套
来源：http://dsk.birdmap.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zlu.hnxiangtu.top

[U59] PHP：自定义排序
来源：http://lnn.9152youxi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dwp.sxryk.cn

[U60] PHP：JSON 编解码
来源：http://ntf.gotoacloud.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tll.xingfuxueyuan.xyz

[U61] PHP：正则
来源：http://lmp.hnxiangtu.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rpa.yonumen.top

[U62] PHP：日期对象
来源：http://src.vqdsnc.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xxn.hysaishi.cn

[U63] PHP：文件读写
来源：http://qwi.sufxvd.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ttp.aibaodan.cn

[U64] PHP：目录遍历
来源：http://frv.jinyuanbaomall.cn

glob("dir/*.php");  scandir("dir");
来源：http://mgg.aizwys.cn

[U65] PHP：会话
来源：http://jqd.fktsv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wtj.jinyuanbaomall.cn

[U66] PHP：设置 Cookie
来源：http://jjh.vqdsnc.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xgr.dianchejie.cn

[U67] PHP：处理文件上传
来源：http://dfz.sjlbkw.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mtu.hysaishi.cn

[U68] PHP：PDO 连接
来源：http://std.yj20258888.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://iem.sweek.top

[U69] PHP：PDO 预处理
来源：http://iim.gaohongyu789.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://oqm.fehbvm.com

[U70] PHP：PDO 事务
来源：http://klw.tian-w.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lqr.ywan-chungtsiang.top

[U71] PHP：抛出异常
来源：http://zsq.zdqjudy.top

throw new RuntimeException("失败", 500);
来源：http://ove.yj202588.top

[U72] PHP：写错误日志
来源：http://xme.xuanzx.com

error_log("失败: " . $e->getMessage());
来源：http://jct.shangyingyoupin.top

[U73] PHP：读取 ini 配置
来源：http://ztr.bbcook.cn

parse_ini_file("config.ini", true)
来源：http://zhn.chenjidiqi.icu

[U74] PHP：读取环境变量
来源：http://jki.fzhhl.top

getenv("APP_ENV") ?: "production"
来源：http://xvl.yonumen.top

[U75] PHP：依赖注入
来源：http://zey.bbcook.cn

composer require psr/container
来源：http://uzq.shanyushiyangkeji.top

[U76] PHP：简单路由
来源：http://pbb.daria6918.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vsx.yj20258.top

[U77] PHP：模板渲染
来源：http://ybo.svipenyu.cn

composer require twig/twig
来源：http://ltw.pycfn.com

[U78] PHP：单元测试
来源：http://taz.yfazqb.com

composer require --dev phpunit/phpunit
来源：http://hjf.ybcxt.top

[U79] PHP：静态分析
来源：http://oky.daria6918.cn

composer require --dev phpstan/phpstan
来源：http://zyj.yuanzhike.top

[U80] PHP：代码规范修复
来源：http://oxn.yonumen.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://nnd.ctjpmb.com

[U81] JS：初始化项目
来源：http://gbi.jianghu66.top

npm init -y;  npm i express
来源：http://qch.ehwqpu.com

[U82] JS：package.json 脚本
来源：http://lhe.jqgfzy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://khh.jinqigfzy.top

[U83] JS：ES Module 导入导出
来源：http://pjw.sysykeji.top

export const a = 1;  import { a } from "./m.js";
来源：http://tde.yuanzhike.top

[U84] JS：CommonJS 写法
来源：http://odh.xuanzx.com

module.exports = { a };  const { a } = require("./m");
来源：http://rys.vehdjk.com

[U85] JS：可选链
来源：http://ukd.tanke756.top

a?.b?.c
来源：http://rwo.nanxuanxn.top

[U86] JS：空值合并
来源：http://yei.chenlongwang.top

a ?? b
来源：http://xnr.hysaishi.cn

[U87] JS：解构默认值
来源：http://lzh.fengsongda.top

const { a = 1, b = 2 } = obj;
来源：http://wee.ywan-chungtsiang.top

[U88] JS：对象展开合并
来源：http://wmj.yuanzhike.top

{ ...a, ...b }
来源：http://kjp.kuanghao11.cn

[U89] JS：数组去重
来源：http://ogj.ywan-chungtsiang.top

[...new Set(arr)]
来源：http://oja.fzhhl.top

[U90] JS：数字数组排序
来源：http://kjr.gzhubu.top

[...arr].sort((a, b) => a - b)
来源：http://kbf.yueranfly.top

[U91] JS：对象键值遍历
来源：http://bmt.smart0.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qdf.kuanghao11.cn

[U92] JS：深拷贝
来源：http://unw.zhiwuduotai.top

structuredClone(obj)
来源：http://kqp.wangshuangyany.cn

[U93] JS：模板字符串
来源：http://rux.yongpay.top

`共 ${n} 条`
来源：http://bxp.mhx1999.top

[U94] JS：箭头函数
来源：http://chi.bbcook.cn

const double = x => x * 2;
来源：http://ret.hammf.cn

[U95] JS：Promise 包装
来源：http://bul.havefunace.top

new Promise((resolve, reject) => {})
来源：http://qzl.vqdsnc.cn

[U96] JS：async/await 与异常
来源：http://jze.c1oappe.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zpj.cashguo.top

[U97] JS：并发请求
来源：http://via.tanke756.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://vwg.hcnkem.com

[U98] JS：fetch 带 JSON
来源：http://mpm.andypj.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uvm.shzxlz.cn

[U99] JS：事件监听
来源：http://mja.0kj1m.cn

el.addEventListener("click", e => {})
来源：http://eao.fengsongda.top

[U100] JS：DOM 查询
来源：http://jls.aizwys.cn

document.querySelector(".item")
来源：http://bxq.yfazqb.com

[U101] JS：classList 操作
来源：http://wxr.hcnkem.com

el.classList.toggle("active")
来源：http://bzx.ywan-chungtsiang.top

[U102] JS：本地存储
来源：http://wti.hnxiangtu.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ekv.bbcook.cn

[U103] JS：定时器
来源：http://ihl.fehbvm.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://acc.hesvh.cn

[U104] JS：防抖
来源：http://jnc.shanyushiyangtech.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fbc.dashuyun.cn

[U105] JS：节流
来源：http://grn.ydjk.org.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ttw.jianghu66.top

[U106] JS：日期格式化
来源：http://afh.jqgfzy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bmc.nanxinkj.top

[U107] JS：数字千分位
来源：http://iyv.dianchejie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kgf.tian-w.cn

[U108] JS：随机整数
来源：http://yes.vqdsnc.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xsc.jinqigufen.top

[U109] JS：数组分组
来源：http://ptt.vehdjk.com

Object.groupBy(arr, x => x.type)
来源：http://flm.sjlbkw.cn

[U110] JS：数组分块
来源：http://kiw.hfpthk.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dgu.yuxming.cn

[U111] JS：对象转 Map
来源：http://iar.zhijiandao.cn

new Map(Object.entries(obj))
来源：http://pci.xziqi.cn

[U112] JS：字符串补位
来源：http://mnc.hnqzz.top

"7".padStart(3, "0")
来源：http://lxb.zhoulong.xyz

[U113] JS：正则替换全部
来源：http://fus.gotoacloud.top

s.replaceAll("a", "b")
来源：http://ekr.zhongyouzk.top

[U114] JS：JSON 深比较
来源：http://brt.316326.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://wfu.havefunace.top

[U115] JS：生成 UUID
来源：http://hdd.chenzaomai.com

crypto.randomUUID()
来源：http://afm.tarul.cn

[U116] JS：类型检查（JSDoc）
来源：http://ccn.nanxuanxn.top

/** @param {string} name */ function f(name) {}
来源：http://uuv.svipenyu.cn

[U117] JS：单元测试
来源：http://hgj.fengsongda.top

npm i -D vitest;  npx vitest
来源：http://kzi.pycfn.com

[U118] JS：开发服务器
来源：http://snt.cashguo.top

npm i -D vite;  npx vite
来源：http://gfn.yonumen.top

[U119] JS：生产构建
来源：http://swy.xingfuxueyuan.xyz

npx vite build
来源：http://pkv.yangfankeji.com

[U120] JS：读取环境变量（Vite）
来源：http://jqa.yuxming.cn

import.meta.env.VITE_API_URL
来源：http://nkr.wangshuangyany.cn

================================================================================
来源：http://yik.yj202588.top

统计汇总
来源：http://ptn.wangshuangyany.cn

================================================================================
来源：http://aau.vqdsnc.cn

按语言统计（条）：
来源：http://ncx.316326.xyz

Python ......... 252
来源：http://afr.sufxvd.cn

PHP ............ 252
来源：http://whg.cashguo.top

JavaScript ..... 252
来源：http://hgv.shangyingyoupin.top

TypeScript ..... 212
来源：http://kbx.ybcxt.top

Java ........... 212
来源：http://pxr.cheryme.top

Go ............. 212
来源：http://yin.yvedp.cn

Ruby ........... 212
来源：http://ehk.fanxiaobao.xyz

C# ............. 212
来源：http://xwc.jqgufenzy.top

C .............. 30
来源：http://zhn.epnwcf.com

C++ ............ 30
来源：http://kxr.9152youxi.cn

SQL ............ 90
来源：http://isc.0kj1m.cn

Bash ........... 80
来源：http://pwo.vehdjk.com

Kotlin ......... 15
来源：http://lhk.aizwys.cn

Swift .......... 15
来源：http://ihn.zhoulong.xyz

Lua ............ 10
来源：http://wbt.yangfankeji.com

Perl ........... 10
来源：http://rap.jyoumei.cn

Scala .......... 10
来源：http://gbq.daxiang520.top

------------------------------------
来源：http://yqs.chenjidiqi.icu

合计 ........... 2106 条
来源：http://qzq.shangyingyoupin.top

按章节统计：
来源：http://yfc.kuanghao11.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://faq.gaohongyu789.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vap.yanxiufei.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pzs.chenjidiqi.icu

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fwr.vehdjk.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bcy.52xcode.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://peb.quarkkingdee.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://acu.sxryk.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xcu.chenzaomai.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ega.zhijiandao.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wjl.ydzc1.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://adj.xuetiantiany.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fcy.bjfxy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pbr.daria6918.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sau.tian-w.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://sfs.tarul.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hjt.yueranfly.top

Q SQL 专题                              90
来源：http://blk.nanxinkj.top

R Bash 专题                             80
来源：http://hua.cqqwz.cn

S C / C++ 专题                          60
来源：http://zzd.ywan-chungtsiang.top

T 其他语言补充                          60
来源：http://rfa.yueranfly.top

U 高频实用片段                         120
来源：http://bxu.wangshuangyany.cn

------------------------------------
来源：http://fem.yangfankeji.com

合计                                  2106 条
来源：http://uxe.xylfe.cn

--------------------------------------------------------------------------------
来源：http://gax.birdmap.top

使用提醒
来源：http://fth.zdqjudy.top

--------------------------------------------------------------------------------
来源：http://prm.jiagoushi.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xuu.zhijiandao.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mvq.jinyuanbaomall.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://unk.pengpengdd.cyou

在旧版本上使用前请先确认语法支持情况。
来源：http://hep.jlsjyb.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lcn.cqqwz.cn

—— 文件结束 ——
来源：http://qrg.chenlongwang.top

================================================================================
来源：http://uzl.cashguo.top

程序语言常见例子速查手册（2024 版）
来源：http://rwx.zhiwuduotai.top

Common Programming Examples Cheat Book
来源：http://xco.iojbl.cn

================================================================================
来源：http://azu.daria6918.cn

【收录内容】
来源：http://luo.bbcook.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://njg.ywan-chungtsiang.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nrj.havefunace.top

SQL · Bash · C · C++
来源：http://zrc.sysykeji.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hqe.hcnkem.com

【使用说明】
来源：http://pmu.zhiwuduotai.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hdd.svipenyu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dxf.vqdsnc.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nyr.tian-w.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://eqz.haohaochexian.top

Bash:  Shell         C:     C             C++:   C++
来源：http://vlb.xuanzx.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xgq.chenlongwang.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cwx.chenzaomai.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://npy.tanke756.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wvu.jinghuilouyu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pie.jqgfzy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mcr.fehbvm.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ond.ydzc1.top

【文件统计】
来源：http://qun.jianghu66.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xew.nwbrower.top

--------------------------------------------------------------------------------
来源：http://exa.quarkkingdee.top

目  录
来源：http://urw.jinqigufen.top

--------------------------------------------------------------------------------
来源：http://otz.hongshengwenyu.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qdg.fanxiaobao.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://vsv.aizwys.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://cec.quarkkingdee.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://glp.jinqigfzy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fjq.wangdashe.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://nkb.yueranfly.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://sqf.svipenyu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://can.zhiwuduotai.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bmi.haohaochexian.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jkz.fengsongda.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dou.yuxming.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mub.jlsjyb.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mvr.guannengcc.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mff.sysykeji.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ayy.bbcook.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gnm.bbcook.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ofw.jqgufenzy.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://shb.jinghuilouyu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://nwm.shuidangran.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ykz.fzhhl.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hlt.ctjpmb.com

================================================================================
来源：http://pto.yj202588.top

A. 基础语法与类型
来源：http://htj.yongpay.top

================================================================================
来源：http://yld.ybcxt.top

[A01] Hello World
来源：http://iik.sjlbkw.cn

Py:   print("Hello, World!")
来源：http://qon.shzxlz.cn

PHP:  echo "Hello, World!";
来源：http://erd.xingfuxueyuan.xyz

JS:   console.log("Hello, World!");
来源：http://zjh.hysaishi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://bic.fzhhl.top

Java: System.out.println("Hello, World!");
来源：http://bgi.haohaochexian.top

Go:   fmt.Println("Hello, World!")
来源：http://kvr.ydjk.org.cn

Ruby: puts "Hello, World!"
来源：http://rat.316326.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://loq.hcnkem.com

[A02] 变量声明与赋值
来源：http://oou.zhiwuduotai.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gns.snrcjt.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://imy.zhongyouzk.top

JS:   let name = "Alex"; const age = 20;
来源：http://vvc.jinghuilouyu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kgx.bjfxy.top

Java: String name = "Alex"; int age = 20;
来源：http://smy.52xcode.cn

Go:   name := "Alex"; age := 20
来源：http://hna.yj20258888.top

Ruby: name = "Alex"; age = 20
来源：http://kwi.vehdjk.com

C#:   string name = "Alex"; int age = 20;
来源：http://lzj.fanxiaobao.xyz

[A03] 常量定义
来源：http://gsa.wangdashe.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wqw.sjlbkw.cn

PHP:  const PI = 3.14159;
来源：http://nbe.cqqwz.cn

JS:   const PI = 3.14159;
来源：http://adu.jinghuilouyu.cn

TS:   const PI: number = 3.14159;
来源：http://uti.iojbl.cn

Java: static final double PI = 3.14159;
来源：http://dsh.cdnleiting.top

Go:   const PI = 3.14159
来源：http://oas.jqgufenzy.top

Ruby: PI = 3.14159
来源：http://tep.jinqigufen.top

C#:   const double PI = 3.14159;
来源：http://gmq.mhx1999.top

[A04] 判断变量类型
来源：http://qnr.ybcxt.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ssy.aizwys.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qlg.jyoumei.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qgc.fzhhl.top

TS:   typeof x; x instanceof Date
来源：http://qae.andypj.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dxu.dianchejie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://kmo.hongshengwenyu.top

Ruby: x.class; x.is_a?(Integer)
来源：http://dyi.tianlin.xyz

C#:   x.GetType().Name; x is int
来源：http://avx.ywan-chungtsiang.top

[A05] 整数除法与取模
来源：http://gur.hesvh.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://dzv.xinyue.icu

PHP:  intdiv(7, 2); 7 % 2
来源：http://kaf.zhaomingkeji.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://rsa.ppjwa.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://eyx.zhongyouzk.top


<!-- 参考信息 -->