代发 wailian999

[U49] PHP：只读属性
来源：http://ohj.sjlbkw.cn

public readonly string $name
来源：http://ozx.hcnkem.com

[U50] PHP：构造器属性提升
来源：http://xyq.pycfn.com

public function __construct(private int $id) {}
来源：http://hvn.sufxvd.cn

[U51] PHP：数组解构
来源：http://qzt.zhaomingkeji.xyz

[$a, $b] = $arr;
来源：http://xww.yj20258.top

[U52] PHP：箭头函数
来源：http://hit.haohaochexian.top

$double = fn($x) => $x * 2;
来源：http://utj.haohaochexian.top

[U53] PHP：空合并运算符
来源：http://wqt.iojbl.cn

$v = $a ?? $b ?? "default";
来源：http://rmm.ehwqpu.com

[U54] PHP：空安全调用
来源：http://ahf.shanyushiyangkeji.top

$obj?->method()
来源：http://raf.nwbrower.top

[U55] PHP：match 表达式
来源：http://ync.cheryme.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://env.jinqigfzy.top

[U56] PHP：命名参数
来源：http://wpc.ppjwa.cn

f(a: 1, b: 2)
来源：http://snu.wangdashe.top

[U57] PHP：字符串插值
来源：http://zos.yueranfly.top

"值: {$a}"
来源：http://dhc.xinyue.icu

[U58] PHP：数组三件套
来源：http://jva.hywenlv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jbp.xinyue.icu

[U59] PHP：自定义排序
来源：http://zel.tian-w.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cnl.tian-w.cn

[U60] PHP：JSON 编解码
来源：http://suh.smart0.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mms.zhijiandao.cn

[U61] PHP：正则
来源：http://jfl.yueranfly.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ckk.haohaochexian.top

[U62] PHP：日期对象
来源：http://bje.birdmap.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uek.tanke756.top

[U63] PHP：文件读写
来源：http://eod.ybcxt.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gtm.zhixingplan.top

[U64] PHP：目录遍历
来源：http://ojk.xingfuxueyuan.xyz

glob("dir/*.php");  scandir("dir");
来源：http://cuw.zhongyouzk.top

[U65] PHP：会话
来源：http://hbi.fktsv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://knh.jqgfzy.top

[U66] PHP：设置 Cookie
来源：http://xqb.haohaochexian.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pkj.yfazqb.com

[U67] PHP：处理文件上传
来源：http://sfa.ivvv.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jls.sweek.top

[U68] PHP：PDO 连接
来源：http://hez.jinghuilouyu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qvp.daxiang520.top

[U69] PHP：PDO 预处理
来源：http://pyg.feifeiyinyue.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zqb.yuanzhike.top

[U70] PHP：PDO 事务
来源：http://qcy.tian-w.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ias.jinqigfzy.top

[U71] PHP：抛出异常
来源：http://qjt.fanxiaobao.xyz

throw new RuntimeException("失败", 500);
来源：http://gkg.ywan-chungtsiang.top

[U72] PHP：写错误日志
来源：http://nfj.ywan-chungtsiang.top

error_log("失败: " . $e->getMessage());
来源：http://spx.pengpengdd.cyou

[U73] PHP：读取 ini 配置
来源：http://gtd.uphjek.com

parse_ini_file("config.ini", true)
来源：http://tsh.shangyingyoupin.top

[U74] PHP：读取环境变量
来源：http://jql.uphjek.com

getenv("APP_ENV") ?: "production"
来源：http://ipd.zhixingplan.top

[U75] PHP：依赖注入
来源：http://cmq.sufxvd.cn

composer require psr/container
来源：http://afu.gzhubu.top

[U76] PHP：简单路由
来源：http://pcc.xingfuxueyuan.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nbr.sweek.top

[U77] PHP：模板渲染
来源：http://gmk.jinghuilouyu.cn

composer require twig/twig
来源：http://diu.sufxvd.cn

[U78] PHP：单元测试
来源：http://qfs.yangfankeji.com

composer require --dev phpunit/phpunit
来源：http://uis.hnxiangtu.top

[U79] PHP：静态分析
来源：http://rdw.redwolf501.top

composer require --dev phpstan/phpstan
来源：http://grv.nwbrower.top

[U80] PHP：代码规范修复
来源：http://eog.hysaishi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://fbp.daxiang520.top

[U81] JS：初始化项目
来源：http://fjx.zhengqikj.top

npm init -y;  npm i express
来源：http://url.yfazqb.com

[U82] JS：package.json 脚本
来源：http://rif.bjfxy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wib.jiagoushi.top

[U83] JS：ES Module 导入导出
来源：http://dme.cheryme.top

export const a = 1;  import { a } from "./m.js";
来源：http://wyw.tianlin.xyz

[U84] JS：CommonJS 写法
来源：http://bph.jqgufenzy.top

module.exports = { a };  const { a } = require("./m");
来源：http://rrz.aizwys.cn

[U85] JS：可选链
来源：http://bii.zhongyouzk.top

a?.b?.c
来源：http://aje.hysaishi.cn

[U86] JS：空值合并
来源：http://vaf.zhaomingkeji.xyz

a ?? b
来源：http://gzc.cheryme.top

[U87] JS：解构默认值
来源：http://awz.quarkkingdee.top

const { a = 1, b = 2 } = obj;
来源：http://jhq.c1oappe.top

[U88] JS：对象展开合并
来源：http://uin.gotoacloud.top

{ ...a, ...b }
来源：http://oxp.shangyingyoupin.top

[U89] JS：数组去重
来源：http://vta.jiagoushi.top

[...new Set(arr)]
来源：http://bia.smart0.xyz

[U90] JS：数字数组排序
来源：http://gyg.guowangkeji.top

[...arr].sort((a, b) => a - b)
来源：http://xip.hesvh.cn

[U91] JS：对象键值遍历
来源：http://kaj.jinqigfzy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gtl.pycfn.com

[U92] JS：深拷贝
来源：http://yst.kuanghao11.cn

structuredClone(obj)
来源：http://zyq.jiagoushi.top

[U93] JS：模板字符串
来源：http://uqt.ydjk.org.cn

`共 ${n} 条`
来源：http://ogg.hammf.cn

[U94] JS：箭头函数
来源：http://msu.cdnleiting.top

const double = x => x * 2;
来源：http://wll.0kj1m.cn

[U95] JS：Promise 包装
来源：http://vha.hammf.cn

new Promise((resolve, reject) => {})
来源：http://oke.shanyushiyangtech.top

[U96] JS：async/await 与异常
来源：http://tcp.ivvv.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ojj.xuanzx.com

[U97] JS：并发请求
来源：http://unf.gotoacloud.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://faw.xuetiantiany.cn

[U98] JS：fetch 带 JSON
来源：http://lao.hnqzz.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uue.jianghu66.top

[U99] JS：事件监听
来源：http://oic.c1oappe.top

el.addEventListener("click", e => {})
来源：http://kvf.cqqwz.cn

[U100] JS：DOM 查询
来源：http://rlj.tianlin.xyz

document.querySelector(".item")
来源：http://riu.daxiang520.top

[U101] JS：classList 操作
来源：http://sls.daria6918.cn

el.classList.toggle("active")
来源：http://phk.xuanzx.com

[U102] JS：本地存储
来源：http://avi.jqgufenzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ewa.c1oappe.top

[U103] JS：定时器
来源：http://ylh.aizwys.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ngf.meibo888.top

[U104] JS：防抖
来源：http://zti.hesvh.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uyp.kuanghao11.cn

[U105] JS：节流
来源：http://mvv.hammf.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://asj.nwbrower.top

[U106] JS：日期格式化
来源：http://hmh.xylfe.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pxt.yuanzhike.top

[U107] JS：数字千分位
来源：http://xwl.jlsjyb.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bcb.hammf.cn

[U108] JS：随机整数
来源：http://kzq.tanke756.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://typ.pycfn.com

[U109] JS：数组分组
来源：http://tlw.xuanzx.com

Object.groupBy(arr, x => x.type)
来源：http://mjn.gogol.net.cn

[U110] JS：数组分块
来源：http://dsa.redwolf501.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gfm.shangyingyoupin.top

[U111] JS：对象转 Map
来源：http://kuq.yj202588.top

new Map(Object.entries(obj))
来源：http://uhu.haohaochexian.top

[U112] JS：字符串补位
来源：http://wfr.cashguo.top

"7".padStart(3, "0")
来源：http://seb.dianchejie.cn

[U113] JS：正则替换全部
来源：http://yio.havefunace.top

s.replaceAll("a", "b")
来源：http://hsz.shuidangran.top

[U114] JS：JSON 深比较
来源：http://lvy.dashuyun.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qaj.svipenyu.cn

[U115] JS：生成 UUID
来源：http://irl.shzxlz.cn

crypto.randomUUID()
来源：http://ijq.chenlongwang.top

[U116] JS：类型检查（JSDoc）
来源：http://myp.cashguo.top

/** @param {string} name */ function f(name) {}
来源：http://okh.jinqigufen.top

[U117] JS：单元测试
来源：http://bbe.jianghu66.top

npm i -D vitest;  npx vitest
来源：http://vpz.shangyingyoupin.top

[U118] JS：开发服务器
来源：http://erc.daria6918.cn

npm i -D vite;  npx vite
来源：http://xlv.pengpengdd.cyou

[U119] JS：生产构建
来源：http://jvv.zdbjq.cn

npx vite build
来源：http://oen.tianlin.xyz

[U120] JS：读取环境变量（Vite）
来源：http://jkl.hfpthk.cn

import.meta.env.VITE_API_URL
来源：http://tec.zycfv.cn

================================================================================
来源：http://fqv.yanxiufei.cn

统计汇总
来源：http://kmt.sysykeji.top

================================================================================
来源：http://fyg.aizwys.cn

按语言统计（条）：
来源：http://yno.jinqigufen.top

Python ......... 252
来源：http://efz.jinqigufen.top

PHP ............ 252
来源：http://vix.nwbrower.top

JavaScript ..... 252
来源：http://npo.9152youxi.cn

TypeScript ..... 212
来源：http://myc.ybcxt.top

Java ........... 212
来源：http://ksb.cucudq.cn

Go ............. 212
来源：http://eab.zhixingplan.top

Ruby ........... 212
来源：http://srh.nwbrower.top

C# ............. 212
来源：http://qrg.yonumen.top

C .............. 30
来源：http://lgs.pycfn.com

C++ ............ 30
来源：http://whm.zhengqikj.top

SQL ............ 90
来源：http://hak.hywenlv.cn

Bash ........... 80
来源：http://tgk.fanxiaobao.xyz

Kotlin ......... 15
来源：http://ydl.jqgufenzy.top

Swift .......... 15
来源：http://vor.uphjek.com

Lua ............ 10
来源：http://xkr.shuidangran.top

Perl ........... 10
来源：http://yny.gogol.net.cn

Scala .......... 10
来源：http://gsm.zycfv.cn

------------------------------------
来源：http://eyf.pengpengdd.cyou

合计 ........... 2106 条
来源：http://zur.andypj.xyz

按章节统计：
来源：http://qyq.vqdsnc.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pav.aibaodan.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cht.jiagoushi.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gfq.fengsongda.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://svx.meibo888.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hli.zdbjq.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tqg.sufxvd.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bct.gzhubu.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ets.guowangkeji.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kdk.jiagoushi.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rba.daria6918.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qbv.meibo888.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://shi.quarkkingdee.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hke.xziqi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wue.pengpengdd.cyou

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wtz.hysaishi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jck.havefunace.top

Q SQL 专题                              90
来源：http://sfe.yonumen.top

R Bash 专题                             80
来源：http://hfm.pengpengdd.cyou

S C / C++ 专题                          60
来源：http://yqf.andypj.xyz

T 其他语言补充                          60
来源：http://wpq.zdbjq.cn

U 高频实用片段                         120
来源：http://ivl.chenjidiqi.icu

------------------------------------
来源：http://zth.9152youxi.cn

合计                                  2106 条
来源：http://gcm.cdnleiting.top

--------------------------------------------------------------------------------
来源：http://plz.redwolf501.top

使用提醒
来源：http://sfa.zhiwuduotai.top

--------------------------------------------------------------------------------
来源：http://jnd.gotoacloud.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hax.shzxlz.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dvt.cashguo.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dxu.yuanzhike.top

在旧版本上使用前请先确认语法支持情况。
来源：http://iki.chenzaomai.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gwk.daria6918.cn

—— 文件结束 ——
来源：http://lal.mhx1999.top

================================================================================
来源：http://xsz.shanyushiyangtech.top

程序语言常见例子速查手册（2024 版）
来源：http://rfb.jiagoushi.top

Common Programming Examples Cheat Book
来源：http://vin.chenlongwang.top

================================================================================
来源：http://vbv.zhoulong.xyz

【收录内容】
来源：http://hgr.yuxming.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://acq.ydjk.org.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://odj.shangyingyoupin.top

SQL · Bash · C · C++
来源：http://pdi.c1oappe.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://bpl.jianghu66.top

【使用说明】
来源：http://dfn.xylfe.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kon.jinyuanbaomall.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vkb.vehdjk.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nil.bbcook.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jqe.chenlongwang.top

Bash:  Shell         C:     C             C++:   C++
来源：http://yeo.shanyushiyangkeji.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://cqw.vqdsnc.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zzm.tarul.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://sxg.dashuyun.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jnu.sxryk.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dld.snrcjt.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://oej.xinyue.icu

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pih.xinyue.icu

【文件统计】
来源：http://sgu.xylfe.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://bbb.hfpthk.cn

--------------------------------------------------------------------------------
来源：http://xwj.aibaodan.cn

目  录
来源：http://zks.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://gzn.zhaomingkeji.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xpl.zhijiandao.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://spy.yvedp.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ktc.yj20258.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ocw.xingfuxueyuan.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://eeo.haohaochexian.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hkn.ybcxt.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yva.hnqzz.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mfg.feifeiyinyue.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ugl.smart0.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://umd.hcnkem.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jjv.iojbl.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zvu.gaohongyu789.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vwr.andypj.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://sgx.zdbjq.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wjj.svipenyu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://pua.hywenlv.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ypx.sufxvd.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wyj.jinqigufen.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ook.jinqigufen.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fxo.chenlongwang.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://uwm.ivvv.top

================================================================================
来源：http://kva.cqqwz.cn

A. 基础语法与类型
来源：http://yah.sjlbkw.cn

================================================================================
来源：http://nhm.yj20258.top

[A01] Hello World
来源：http://zrt.fehbvm.com

Py:   print("Hello, World!")
来源：http://byg.yuxming.cn

PHP:  echo "Hello, World!";
来源：http://lfi.zhengqikj.top

JS:   console.log("Hello, World!");
来源：http://pgx.9152youxi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://isu.redwolf501.top

Java: System.out.println("Hello, World!");
来源：http://ebu.fengsongda.top

Go:   fmt.Println("Hello, World!")
来源：http://xam.chenjidiqi.icu

Ruby: puts "Hello, World!"
来源：http://udz.ctjpmb.com

C#:   Console.WriteLine("Hello, World!");
来源：http://vix.ywan-chungtsiang.top

[A02] 变量声明与赋值
来源：http://yge.0kj1m.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://lwr.zdqjudy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://jpl.hcnkem.com

JS:   let name = "Alex"; const age = 20;
来源：http://klr.nwbrower.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://oto.feifeiyinyue.top

Java: String name = "Alex"; int age = 20;
来源：http://kfr.shanyushiyangtech.top

Go:   name := "Alex"; age := 20
来源：http://mlv.vqdsnc.cn

Ruby: name = "Alex"; age = 20
来源：http://kyb.uphjek.com

C#:   string name = "Alex"; int age = 20;
来源：http://gkp.birdmap.top

[A03] 常量定义
来源：http://idg.zdqjudy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wlc.jinyuanbaomall.cn

PHP:  const PI = 3.14159;
来源：http://lsk.jianghu66.top

JS:   const PI = 3.14159;
来源：http://nin.fehbvm.com

TS:   const PI: number = 3.14159;
来源：http://prj.birdmap.top

Java: static final double PI = 3.14159;
来源：http://cfo.aibaodan.cn

Go:   const PI = 3.14159
来源：http://qae.uphjek.com

Ruby: PI = 3.14159
来源：http://qme.chenlongwang.top

C#:   const double PI = 3.14159;
来源：http://mdn.cdnleiting.top

[A04] 判断变量类型
来源：http://vnx.cdnleiting.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://exx.xingfuxueyuan.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://iss.birdmap.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://emr.zhongyouzk.top

TS:   typeof x; x instanceof Date
来源：http://mdv.bbcook.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://eme.chenzaomai.com

Go:   reflect.TypeOf(x).Name()
来源：http://lyv.hywenlv.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://mkw.yvedp.cn

C#:   x.GetType().Name; x is int
来源：http://inl.uphjek.com

[A05] 整数除法与取模
来源：http://fdz.fehbvm.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://uxh.shanyushiyangtech.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://fre.vehdjk.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qqf.jiagoushi.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xzf.yvedp.cn

Java: 7 / 2; 7 % 2
来源：http://iyx.mhx1999.top

Go:   7 / 2; 7 % 2
来源：http://tvb.9152youxi.cn

Ruby: 7 / 2; 7 % 2
来源：http://dze.hnqzz.top

C#:   7 / 2; 7 % 2
来源：http://rvi.fanxiaobao.xyz

[A06] 字符串转数字
来源：http://zmi.xylfe.cn

Py:   int("42"); float("3.14")
来源：http://qfx.jinyuanbaomall.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wpl.mhx1999.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vpt.xuanzx.com


<!-- 参考信息 -->