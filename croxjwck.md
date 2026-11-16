代发 wailian999

[U49] PHP：只读属性
来源：http://sqe.jqgufenzy.top

public readonly string $name
来源：http://gnf.gotoacloud.top

[U50] PHP：构造器属性提升
来源：http://iyl.quarkkingdee.top

public function __construct(private int $id) {}
来源：http://kei.sxryk.cn

[U51] PHP：数组解构
来源：http://myu.smart0.xyz

[$a, $b] = $arr;
来源：http://fvs.snrcjt.cn

[U52] PHP：箭头函数
来源：http://qoh.jyoumei.cn

$double = fn($x) => $x * 2;
来源：http://iru.chenzaomai.com

[U53] PHP：空合并运算符
来源：http://spf.zhixingplan.top

$v = $a ?? $b ?? "default";
来源：http://pbz.hywenlv.cn

[U54] PHP：空安全调用
来源：http://qqg.zycfv.cn

$obj?->method()
来源：http://yda.jqgfzy.top

[U55] PHP：match 表达式
来源：http://omg.zycfv.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dxp.uphjek.com

[U56] PHP：命名参数
来源：http://gzz.jinghuilouyu.cn

f(a: 1, b: 2)
来源：http://dwv.aizwys.cn

[U57] PHP：字符串插值
来源：http://oii.aibaodan.cn

"值: {$a}"
来源：http://let.jinqigufen.top

[U58] PHP：数组三件套
来源：http://nxd.jinyuanbaomall.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gty.cashguo.top

[U59] PHP：自定义排序
来源：http://sfy.xuetiantiany.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fjk.jinqigfzy.top

[U60] PHP：JSON 编解码
来源：http://pnd.xylfe.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wcf.gaohongyu789.top

[U61] PHP：正则
来源：http://hsa.mhx1999.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gyp.hysaishi.cn

[U62] PHP：日期对象
来源：http://hpj.yj202588.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ohv.zhoulong.xyz

[U63] PHP：文件读写
来源：http://aqw.zhongyouzk.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wgd.yueranfly.top

[U64] PHP：目录遍历
来源：http://usf.meibo888.top

glob("dir/*.php");  scandir("dir");
来源：http://rod.chenlongwang.top

[U65] PHP：会话
来源：http://yub.jqgufenzy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ksj.yueranfly.top

[U66] PHP：设置 Cookie
来源：http://ajb.cheryme.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vbv.yongpay.top

[U67] PHP：处理文件上传
来源：http://ulq.cashguo.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ags.aibaodan.cn

[U68] PHP：PDO 连接
来源：http://qoc.vqdsnc.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jjr.zhijiandao.cn

[U69] PHP：PDO 预处理
来源：http://tod.gzhubu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ztg.dashuyun.cn

[U70] PHP：PDO 事务
来源：http://rdn.xingfuxueyuan.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wmb.chenjidiqi.icu

[U71] PHP：抛出异常
来源：http://rrv.ctjpmb.com

throw new RuntimeException("失败", 500);
来源：http://ksm.pengpengdd.cyou

[U72] PHP：写错误日志
来源：http://esf.jinqigfzy.top

error_log("失败: " . $e->getMessage());
来源：http://wbz.haohaochexian.top

[U73] PHP：读取 ini 配置
来源：http://fjs.ppjwa.cn

parse_ini_file("config.ini", true)
来源：http://wcf.daria6918.cn

[U74] PHP：读取环境变量
来源：http://sut.zhengqikj.top

getenv("APP_ENV") ?: "production"
来源：http://yrz.zhongyouzk.top

[U75] PHP：依赖注入
来源：http://kog.zhixingplan.top

composer require psr/container
来源：http://tta.aizwys.cn

[U76] PHP：简单路由
来源：http://bal.vehdjk.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jpz.aibaodan.cn

[U77] PHP：模板渲染
来源：http://yir.gaohongyu789.top

composer require twig/twig
来源：http://qze.ybcxt.top

[U78] PHP：单元测试
来源：http://zpr.jinqigufen.top

composer require --dev phpunit/phpunit
来源：http://smi.ybcxt.top

[U79] PHP：静态分析
来源：http://ajj.hcnkem.com

composer require --dev phpstan/phpstan
来源：http://gsd.aizwys.cn

[U80] PHP：代码规范修复
来源：http://xfq.sysykeji.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://dfd.sysykeji.top

[U81] JS：初始化项目
来源：http://zwu.xuetiantiany.cn

npm init -y;  npm i express
来源：http://sfu.haohaochexian.top

[U82] JS：package.json 脚本
来源：http://ojw.birdmap.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kok.jinqigufen.top

[U83] JS：ES Module 导入导出
来源：http://xnw.shanyushiyangtech.top

export const a = 1;  import { a } from "./m.js";
来源：http://suh.fzhhl.top

[U84] JS：CommonJS 写法
来源：http://nwv.yuanzhike.top

module.exports = { a };  const { a } = require("./m");
来源：http://ecg.svipenyu.cn

[U85] JS：可选链
来源：http://ilp.yj20258888.top

a?.b?.c
来源：http://nmd.jyoumei.cn

[U86] JS：空值合并
来源：http://skl.316326.xyz

a ?? b
来源：http://pbt.vehdjk.com

[U87] JS：解构默认值
来源：http://tnc.yuanzhike.top

const { a = 1, b = 2 } = obj;
来源：http://zlb.aibaodan.cn

[U88] JS：对象展开合并
来源：http://zsy.yueranfly.top

{ ...a, ...b }
来源：http://lhj.daria6918.cn

[U89] JS：数组去重
来源：http://gkd.ydjk.org.cn

[...new Set(arr)]
来源：http://kbf.andypj.xyz

[U90] JS：数字数组排序
来源：http://dbo.wangshuangyany.cn

[...arr].sort((a, b) => a - b)
来源：http://boa.havefunace.top

[U91] JS：对象键值遍历
来源：http://ssf.chenjidiqi.icu

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hxs.ppjwa.cn

[U92] JS：深拷贝
来源：http://yqn.uphjek.com

structuredClone(obj)
来源：http://sln.gzhubu.top

[U93] JS：模板字符串
来源：http://mco.fzhhl.top

`共 ${n} 条`
来源：http://xbs.meibo888.top

[U94] JS：箭头函数
来源：http://xhi.wangshuangyany.cn

const double = x => x * 2;
来源：http://klp.smart0.xyz

[U95] JS：Promise 包装
来源：http://iqs.zhaomingkeji.xyz

new Promise((resolve, reject) => {})
来源：http://mky.bbcook.cn

[U96] JS：async/await 与异常
来源：http://pqo.0kj1m.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uze.bbcook.cn

[U97] JS：并发请求
来源：http://exw.fehbvm.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://jyp.ppjwa.cn

[U98] JS：fetch 带 JSON
来源：http://rdd.ctjpmb.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zqi.hongshengwenyu.top

[U99] JS：事件监听
来源：http://ayn.jqgfzy.top

el.addEventListener("click", e => {})
来源：http://ftk.shzxlz.cn

[U100] JS：DOM 查询
来源：http://qto.yanxiufei.cn

document.querySelector(".item")
来源：http://osy.hesvh.cn

[U101] JS：classList 操作
来源：http://xxi.ppjwa.cn

el.classList.toggle("active")
来源：http://ubv.yj20258888.top

[U102] JS：本地存储
来源：http://mww.vehdjk.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://dqh.xuanzx.com

[U103] JS：定时器
来源：http://zdb.fengsongda.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jnm.hnxiangtu.top

[U104] JS：防抖
来源：http://xnf.xziqi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pri.nwbrower.top

[U105] JS：节流
来源：http://ndx.tian-w.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://euz.shanyushiyangtech.top

[U106] JS：日期格式化
来源：http://gda.hesvh.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zic.nwbrower.top

[U107] JS：数字千分位
来源：http://rnb.shuidangran.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xqx.ydzc1.top

[U108] JS：随机整数
来源：http://obu.nanxinkj.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pyn.fengsongda.top

[U109] JS：数组分组
来源：http://xyj.bjfxy.top

Object.groupBy(arr, x => x.type)
来源：http://cds.nanxuanxn.top

[U110] JS：数组分块
来源：http://jng.feifeiyinyue.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cdx.ydjk.org.cn

[U111] JS：对象转 Map
来源：http://any.yj202588.top

new Map(Object.entries(obj))
来源：http://bcy.xuetiantiany.cn

[U112] JS：字符串补位
来源：http://diz.jiagoushi.top

"7".padStart(3, "0")
来源：http://ygj.ydjk.org.cn

[U113] JS：正则替换全部
来源：http://jcw.jinyuanbaomall.cn

s.replaceAll("a", "b")
来源：http://bcg.dashuyun.cn

[U114] JS：JSON 深比较
来源：http://qrm.zhengqikj.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://rwu.0kj1m.cn

[U115] JS：生成 UUID
来源：http://alb.yuxming.cn

crypto.randomUUID()
来源：http://sdr.meibo888.top

[U116] JS：类型检查（JSDoc）
来源：http://vbj.guowangkeji.top

/** @param {string} name */ function f(name) {}
来源：http://yfu.cdnleiting.top

[U117] JS：单元测试
来源：http://jcp.0kj1m.cn

npm i -D vitest;  npx vitest
来源：http://dne.jqgufenzy.top

[U118] JS：开发服务器
来源：http://wfp.daria6918.cn

npm i -D vite;  npx vite
来源：http://nbw.jinqigfzy.top

[U119] JS：生产构建
来源：http://yhh.yangfankeji.com

npx vite build
来源：http://pzn.yueranfly.top

[U120] JS：读取环境变量（Vite）
来源：http://qjg.gotoacloud.top

import.meta.env.VITE_API_URL
来源：http://gmy.hnqzz.top

================================================================================
来源：http://ekt.zhixingplan.top

统计汇总
来源：http://ftf.ppjwa.cn

================================================================================
来源：http://dff.smart0.xyz

按语言统计（条）：
来源：http://xto.wangshuangyany.cn

Python ......... 252
来源：http://twu.vqdsnc.cn

PHP ............ 252
来源：http://bfr.iojbl.cn

JavaScript ..... 252
来源：http://fxl.ywan-chungtsiang.top

TypeScript ..... 212
来源：http://wtt.guowangkeji.top

Java ........... 212
来源：http://tjg.xziqi.cn

Go ............. 212
来源：http://aqi.tianlin.xyz

Ruby ........... 212
来源：http://tfl.jqgfzy.top

C# ............. 212
来源：http://gnn.jianghu66.top

C .............. 30
来源：http://ivb.gzhubu.top

C++ ............ 30
来源：http://nhu.sxryk.cn

SQL ............ 90
来源：http://fxu.xuetiantiany.cn

Bash ........... 80
来源：http://vyz.yangfankeji.com

Kotlin ......... 15
来源：http://akb.xingfuxueyuan.xyz

Swift .......... 15
来源：http://ylh.xingfuxueyuan.xyz

Lua ............ 10
来源：http://zbd.shanyushiyangtech.top

Perl ........... 10
来源：http://awd.hnqzz.top

Scala .......... 10
来源：http://lhr.jinyuanbaomall.cn

------------------------------------
来源：http://ujk.chenlongwang.top

合计 ........... 2106 条
来源：http://ftm.epnwcf.com

按章节统计：
来源：http://hkr.havefunace.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fgd.0kj1m.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fuh.ivvv.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vlx.52xcode.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kzg.yongpay.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://iyg.cqqwz.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rsh.hfpthk.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zuk.0kj1m.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zyq.meibo888.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ykc.xuetiantiany.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lyb.jyoumei.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://eoo.xziqi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dkz.yj202588.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hjs.daxiang520.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://guo.havefunace.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kzy.bbcook.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xau.xylfe.cn

Q SQL 专题                              90
来源：http://jja.birdmap.top

R Bash 专题                             80
来源：http://ttv.hesvh.cn

S C / C++ 专题                          60
来源：http://igj.gaohongyu789.top

T 其他语言补充                          60
来源：http://yfc.jinyuanbaomall.cn

U 高频实用片段                         120
来源：http://bvb.xingfuxueyuan.xyz

------------------------------------
来源：http://kdw.ydjk.org.cn

合计                                  2106 条
来源：http://vvr.hnqzz.top

--------------------------------------------------------------------------------
来源：http://fgu.svipenyu.cn

使用提醒
来源：http://guz.tarul.cn

--------------------------------------------------------------------------------
来源：http://nxf.yongpay.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vrz.jqgufenzy.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bmz.hnxiangtu.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xia.chenjidiqi.icu

在旧版本上使用前请先确认语法支持情况。
来源：http://cmt.hongshengwenyu.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hwp.316326.xyz

—— 文件结束 ——
来源：http://cfd.yangfankeji.com

================================================================================
来源：http://qxp.jinqigufen.top

程序语言常见例子速查手册（2024 版）
来源：http://azh.jlsjyb.cn

Common Programming Examples Cheat Book
来源：http://hpd.yanxiufei.cn

================================================================================
来源：http://air.cashguo.top

【收录内容】
来源：http://fco.andypj.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://kul.redwolf501.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wxa.yongpay.top

SQL · Bash · C · C++
来源：http://cjg.jyoumei.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ayx.jinqigufen.top

【使用说明】
来源：http://ncc.cqqwz.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://doi.wangdashe.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vlx.jlsjyb.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qhu.zdqjudy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wum.tianlin.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://mts.316326.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dyj.52xcode.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://esq.svipenyu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ifg.yj20258.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ipw.bbcook.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wsl.dianchejie.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://oey.cqqwz.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nrz.andypj.xyz

【文件统计】
来源：http://zky.jqgufenzy.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lke.tarul.cn

--------------------------------------------------------------------------------
来源：http://gve.ydjk.org.cn

目  录
来源：http://yfs.aibaodan.cn

--------------------------------------------------------------------------------
来源：http://kuh.nwbrower.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dji.shanyushiyangkeji.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://oes.0kj1m.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ptx.tanke756.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qzd.yuxming.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ymm.aizwys.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://iai.quarkkingdee.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://reu.mhx1999.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nem.svipenyu.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tlk.guowangkeji.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xez.zhaomingkeji.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://lld.smart0.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zzg.bbcook.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fer.316326.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hnd.zycfv.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://yzu.jinqigufen.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bgx.guannengcc.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ymo.feifeiyinyue.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://yiv.jinqigufen.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lmj.hfpthk.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vlb.kuanghao11.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://buf.cdnleiting.top

================================================================================
来源：http://sjp.meibo888.top

A. 基础语法与类型
来源：http://qfy.jianghu66.top

================================================================================
来源：http://vff.guannengcc.top

[A01] Hello World
来源：http://efb.yfazqb.com

Py:   print("Hello, World!")
来源：http://bel.jqgfzy.top

PHP:  echo "Hello, World!";
来源：http://zfp.ehwqpu.com

JS:   console.log("Hello, World!");
来源：http://pjz.hnqzz.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jqk.vqdsnc.cn

Java: System.out.println("Hello, World!");
来源：http://iyz.yfazqb.com

Go:   fmt.Println("Hello, World!")
来源：http://wst.nanxinkj.top

Ruby: puts "Hello, World!"
来源：http://rlu.ywan-chungtsiang.top

C#:   Console.WriteLine("Hello, World!");
来源：http://cjr.52xcode.cn

[A02] 变量声明与赋值
来源：http://iau.vehdjk.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://igu.chenlongwang.top

PHP:  $name = "Alex"; $age = 20;
来源：http://mmb.shangyingyoupin.top

JS:   let name = "Alex"; const age = 20;
来源：http://oif.fzhhl.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://cze.meibo888.top

Java: String name = "Alex"; int age = 20;
来源：http://xbf.zhengqikj.top

Go:   name := "Alex"; age := 20
来源：http://qxy.daxiang520.top

Ruby: name = "Alex"; age = 20
来源：http://kal.pycfn.com

C#:   string name = "Alex"; int age = 20;
来源：http://zto.zhixingplan.top

[A03] 常量定义
来源：http://dzi.mhx1999.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://slj.zhoulong.xyz

PHP:  const PI = 3.14159;
来源：http://thw.haohaochexian.top

JS:   const PI = 3.14159;
来源：http://jnr.jqgufenzy.top

TS:   const PI: number = 3.14159;
来源：http://yyo.yanxiufei.cn

Java: static final double PI = 3.14159;
来源：http://kxf.gotoacloud.top

Go:   const PI = 3.14159
来源：http://fuy.cdnleiting.top

Ruby: PI = 3.14159
来源：http://xxk.feifeiyinyue.top

C#:   const double PI = 3.14159;
来源：http://jyd.tarul.cn

[A04] 判断变量类型
来源：http://eja.xylfe.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://hnf.ppjwa.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://aec.smart0.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jnr.birdmap.top

TS:   typeof x; x instanceof Date
来源：http://imt.fanxiaobao.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wrg.sweek.top

Go:   reflect.TypeOf(x).Name()
来源：http://esc.tarul.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://dml.chenzaomai.com

C#:   x.GetType().Name; x is int
来源：http://lkh.gogol.net.cn

[A05] 整数除法与取模
来源：http://jij.daxiang520.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yxq.yangfankeji.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://fqo.redwolf501.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lpw.gaohongyu789.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rna.yonumen.top

Java: 7 / 2; 7 % 2
来源：http://pkz.ehwqpu.com

Go:   7 / 2; 7 % 2
来源：http://yay.zdqjudy.top

Ruby: 7 / 2; 7 % 2
来源：http://oxf.yj20258888.top

C#:   7 / 2; 7 % 2
来源：http://jdb.yangfankeji.com

[A06] 字符串转数字
来源：http://ubr.hnxiangtu.top

Py:   int("42"); float("3.14")
来源：http://lsy.havefunace.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jmt.uphjek.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://iqv.havefunace.top


<!-- 参考信息 -->