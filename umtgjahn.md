代发 wailian999

[U49] PHP：只读属性
来源：http://kzm.cashguo.top

public readonly string $name
来源：http://iym.hywenlv.cn

[U50] PHP：构造器属性提升
来源：http://yao.zhiwuduotai.top

public function __construct(private int $id) {}
来源：http://xjt.shzxlz.cn

[U51] PHP：数组解构
来源：http://pvm.hammf.cn

[$a, $b] = $arr;
来源：http://btq.yj20258888.top

[U52] PHP：箭头函数
来源：http://iov.hywenlv.cn

$double = fn($x) => $x * 2;
来源：http://wzy.shanyushiyangtech.top

[U53] PHP：空合并运算符
来源：http://dug.yuxming.cn

$v = $a ?? $b ?? "default";
来源：http://ymp.xuanzx.com

[U54] PHP：空安全调用
来源：http://par.uphjek.com

$obj?->method()
来源：http://iiu.birdmap.top

[U55] PHP：match 表达式
来源：http://akk.zhengqikj.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://odk.yuxming.cn

[U56] PHP：命名参数
来源：http://wvk.ydjk.org.cn

f(a: 1, b: 2)
来源：http://web.guowangkeji.top

[U57] PHP：字符串插值
来源：http://cuv.zycfv.cn

"值: {$a}"
来源：http://vdx.jyoumei.cn

[U58] PHP：数组三件套
来源：http://sar.xinyue.icu

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cdm.nwbrower.top

[U59] PHP：自定义排序
来源：http://son.andypj.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tkf.zdbjq.cn

[U60] PHP：JSON 编解码
来源：http://aqs.jiagoushi.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://poh.jqgfzy.top

[U61] PHP：正则
来源：http://eqt.yanxiufei.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://olm.xuetiantiany.cn

[U62] PHP：日期对象
来源：http://omv.nwbrower.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ijy.c1oappe.top

[U63] PHP：文件读写
来源：http://fdz.hcnkem.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mqv.hcnkem.com

[U64] PHP：目录遍历
来源：http://tmk.daria6918.cn

glob("dir/*.php");  scandir("dir");
来源：http://hoq.smart0.xyz

[U65] PHP：会话
来源：http://wav.xuetiantiany.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ptn.shuidangran.top

[U66] PHP：设置 Cookie
来源：http://aqx.fehbvm.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hib.zdqjudy.top

[U67] PHP：处理文件上传
来源：http://drp.hongshengwenyu.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zgm.hfpthk.cn

[U68] PHP：PDO 连接
来源：http://lmi.jqgfzy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vdk.shangyingyoupin.top

[U69] PHP：PDO 预处理
来源：http://hpg.yfazqb.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sty.birdmap.top

[U70] PHP：PDO 事务
来源：http://aap.kuanghao11.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://avg.jiagoushi.top

[U71] PHP：抛出异常
来源：http://ncz.shuidangran.top

throw new RuntimeException("失败", 500);
来源：http://pwp.zhixingplan.top

[U72] PHP：写错误日志
来源：http://tvi.guannengcc.top

error_log("失败: " . $e->getMessage());
来源：http://nzn.nanxinkj.top

[U73] PHP：读取 ini 配置
来源：http://xgu.jqgfzy.top

parse_ini_file("config.ini", true)
来源：http://hfz.c1oappe.top

[U74] PHP：读取环境变量
来源：http://pvz.ppjwa.cn

getenv("APP_ENV") ?: "production"
来源：http://htz.cdnleiting.top

[U75] PHP：依赖注入
来源：http://bki.ivvv.top

composer require psr/container
来源：http://rbz.haohaochexian.top

[U76] PHP：简单路由
来源：http://nla.yanxiufei.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pnr.shzxlz.cn

[U77] PHP：模板渲染
来源：http://nwc.ybcxt.top

composer require twig/twig
来源：http://egt.quarkkingdee.top

[U78] PHP：单元测试
来源：http://dxf.nanxinkj.top

composer require --dev phpunit/phpunit
来源：http://jaj.ydzc1.top

[U79] PHP：静态分析
来源：http://pff.zhengqikj.top

composer require --dev phpstan/phpstan
来源：http://feh.52xcode.cn

[U80] PHP：代码规范修复
来源：http://spn.fanxiaobao.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://cux.hysaishi.cn

[U81] JS：初始化项目
来源：http://utx.havefunace.top

npm init -y;  npm i express
来源：http://gex.vehdjk.com

[U82] JS：package.json 脚本
来源：http://efj.sysykeji.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tmj.shanyushiyangtech.top

[U83] JS：ES Module 导入导出
来源：http://iyw.daria6918.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zbv.zycfv.cn

[U84] JS：CommonJS 写法
来源：http://qsj.sweek.top

module.exports = { a };  const { a } = require("./m");
来源：http://grq.nanxuanxn.top

[U85] JS：可选链
来源：http://end.kuanghao11.cn

a?.b?.c
来源：http://kwd.yfazqb.com

[U86] JS：空值合并
来源：http://trp.ctjpmb.com

a ?? b
来源：http://vxc.ydjk.org.cn

[U87] JS：解构默认值
来源：http://usz.yongpay.top

const { a = 1, b = 2 } = obj;
来源：http://esb.xinyue.icu

[U88] JS：对象展开合并
来源：http://qxj.ydzc1.top

{ ...a, ...b }
来源：http://iys.tianlin.xyz

[U89] JS：数组去重
来源：http://rji.yanxiufei.cn

[...new Set(arr)]
来源：http://mse.shzxlz.cn

[U90] JS：数字数组排序
来源：http://tqf.cashguo.top

[...arr].sort((a, b) => a - b)
来源：http://rhy.yj20258888.top

[U91] JS：对象键值遍历
来源：http://vjt.hammf.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hxd.ydzc1.top

[U92] JS：深拷贝
来源：http://ndt.chenjidiqi.icu

structuredClone(obj)
来源：http://ffb.sysykeji.top

[U93] JS：模板字符串
来源：http://srr.svipenyu.cn

`共 ${n} 条`
来源：http://vtz.shzxlz.cn

[U94] JS：箭头函数
来源：http://nqb.xylfe.cn

const double = x => x * 2;
来源：http://jpc.xinyue.icu

[U95] JS：Promise 包装
来源：http://cvr.tarul.cn

new Promise((resolve, reject) => {})
来源：http://vqi.aizwys.cn

[U96] JS：async/await 与异常
来源：http://ogv.gzhubu.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lkv.jqgfzy.top

[U97] JS：并发请求
来源：http://nlz.cucudq.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vnj.tarul.cn

[U98] JS：fetch 带 JSON
来源：http://kzq.daria6918.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fev.dashuyun.cn

[U99] JS：事件监听
来源：http://krv.iojbl.cn

el.addEventListener("click", e => {})
来源：http://gcj.smart0.xyz

[U100] JS：DOM 查询
来源：http://esn.bbcook.cn

document.querySelector(".item")
来源：http://bhh.aibaodan.cn

[U101] JS：classList 操作
来源：http://nsi.zycfv.cn

el.classList.toggle("active")
来源：http://rnr.gaohongyu789.top

[U102] JS：本地存储
来源：http://yjp.smart0.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://wnb.epnwcf.com

[U103] JS：定时器
来源：http://tkj.jinghuilouyu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dlm.gzhubu.top

[U104] JS：防抖
来源：http://hze.chenzaomai.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://idp.sufxvd.cn

[U105] JS：节流
来源：http://coz.shanyushiyangkeji.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yyi.birdmap.top

[U106] JS：日期格式化
来源：http://edp.zhengqikj.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gpv.c1oappe.top

[U107] JS：数字千分位
来源：http://ghh.yvedp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://guu.yuxming.cn

[U108] JS：随机整数
来源：http://djt.nwbrower.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jac.daxiang520.top

[U109] JS：数组分组
来源：http://gku.jinqigufen.top

Object.groupBy(arr, x => x.type)
来源：http://knp.jinqigufen.top

[U110] JS：数组分块
来源：http://kct.tanke756.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qyt.hysaishi.cn

[U111] JS：对象转 Map
来源：http://sgm.daria6918.cn

new Map(Object.entries(obj))
来源：http://nwa.pycfn.com

[U112] JS：字符串补位
来源：http://ugh.ybcxt.top

"7".padStart(3, "0")
来源：http://ils.feifeiyinyue.top

[U113] JS：正则替换全部
来源：http://zvn.zhixingplan.top

s.replaceAll("a", "b")
来源：http://rwe.vqdsnc.cn

[U114] JS：JSON 深比较
来源：http://njr.ppjwa.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://bwo.52xcode.cn

[U115] JS：生成 UUID
来源：http://ybk.9152youxi.cn

crypto.randomUUID()
来源：http://caj.cucudq.cn

[U116] JS：类型检查（JSDoc）
来源：http://ias.c1oappe.top

/** @param {string} name */ function f(name) {}
来源：http://hvi.yonumen.top

[U117] JS：单元测试
来源：http://jha.chenzaomai.com

npm i -D vitest;  npx vitest
来源：http://bmj.hcnkem.com

[U118] JS：开发服务器
来源：http://lyf.fengsongda.top

npm i -D vite;  npx vite
来源：http://dbf.sxryk.cn

[U119] JS：生产构建
来源：http://ilm.xziqi.cn

npx vite build
来源：http://hko.hesvh.cn

[U120] JS：读取环境变量（Vite）
来源：http://mov.cqqwz.cn

import.meta.env.VITE_API_URL
来源：http://wal.yangfankeji.com

================================================================================
来源：http://stx.zdbjq.cn

统计汇总
来源：http://brt.jianghu66.top

================================================================================
来源：http://bsd.0kj1m.cn

按语言统计（条）：
来源：http://rxe.zhiwuduotai.top

Python ......... 252
来源：http://qcv.52xcode.cn

PHP ............ 252
来源：http://fwu.daxiang520.top

JavaScript ..... 252
来源：http://irr.jyoumei.cn

TypeScript ..... 212
来源：http://ecm.yuanzhike.top

Java ........... 212
来源：http://wzx.jyoumei.cn

Go ............. 212
来源：http://fzc.ywan-chungtsiang.top

Ruby ........... 212
来源：http://jkn.0kj1m.cn

C# ............. 212
来源：http://zfl.chenzaomai.com

C .............. 30
来源：http://gke.sufxvd.cn

C++ ............ 30
来源：http://pdn.hongshengwenyu.top

SQL ............ 90
来源：http://arm.redwolf501.top

Bash ........... 80
来源：http://gan.jqgufenzy.top

Kotlin ......... 15
来源：http://yen.birdmap.top

Swift .......... 15
来源：http://kjv.yj20258888.top

Lua ............ 10
来源：http://obx.yj202588.top

Perl ........... 10
来源：http://mwb.shanyushiyangkeji.top

Scala .......... 10
来源：http://iqk.smart0.xyz

------------------------------------
来源：http://vxp.shuidangran.top

合计 ........... 2106 条
来源：http://fvx.dianchejie.cn

按章节统计：
来源：http://ewk.hongshengwenyu.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://azf.hnxiangtu.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wtj.zycfv.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jms.zhoulong.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://eid.cucudq.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cje.yj20258.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jfa.zhengqikj.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kvj.gaohongyu789.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nua.hammf.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mtl.uphjek.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://waz.shuidangran.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mxu.hfpthk.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cmt.jinqigfzy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jdp.zhoulong.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dzq.xylfe.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kgv.feifeiyinyue.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vqy.sufxvd.cn

Q SQL 专题                              90
来源：http://yao.xylfe.cn

R Bash 专题                             80
来源：http://ohg.sweek.top

S C / C++ 专题                          60
来源：http://kmr.tianlin.xyz

T 其他语言补充                          60
来源：http://ojq.andypj.xyz

U 高频实用片段                         120
来源：http://hww.haohaochexian.top

------------------------------------
来源：http://orz.pengpengdd.cyou

合计                                  2106 条
来源：http://jgw.shuidangran.top

--------------------------------------------------------------------------------
来源：http://lxj.nanxuanxn.top

使用提醒
来源：http://fmh.xuetiantiany.cn

--------------------------------------------------------------------------------
来源：http://fll.zhijiandao.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rlg.quarkkingdee.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://otw.tanke756.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://caz.ydzc1.top

在旧版本上使用前请先确认语法支持情况。
来源：http://uff.vqdsnc.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jks.ydjk.org.cn

—— 文件结束 ——
来源：http://avv.zycfv.cn

================================================================================
来源：http://jhc.shanyushiyangtech.top

程序语言常见例子速查手册（2024 版）
来源：http://hoz.jlsjyb.cn

Common Programming Examples Cheat Book
来源：http://rdu.shuidangran.top

================================================================================
来源：http://imc.jyoumei.cn

【收录内容】
来源：http://vpd.fanxiaobao.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://zar.shanyushiyangtech.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rqc.feifeiyinyue.top

SQL · Bash · C · C++
来源：http://mpw.ywan-chungtsiang.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://izl.guannengcc.top

【使用说明】
来源：http://mki.gotoacloud.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kkz.yj20258888.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bay.daxiang520.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zhh.zhijiandao.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ngf.zhengqikj.top

Bash:  Shell         C:     C             C++:   C++
来源：http://gwv.zhongyouzk.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://crm.zdqjudy.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nks.hywenlv.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dzc.pycfn.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yzq.svipenyu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ugm.ivvv.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qsp.tanke756.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jhd.sufxvd.cn

【文件统计】
来源：http://uga.redwolf501.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rnc.ybcxt.top

--------------------------------------------------------------------------------
来源：http://mvh.tanke756.top

目  录
来源：http://flq.chenlongwang.top

--------------------------------------------------------------------------------
来源：http://skb.smart0.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kwq.jiagoushi.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://pcs.tarul.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wij.epnwcf.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vpb.shangyingyoupin.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jsm.fengsongda.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pwv.hongshengwenyu.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gmq.jqgfzy.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ewk.yongpay.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rfx.shanyushiyangkeji.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mfh.gotoacloud.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://eap.vqdsnc.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bwt.9152youxi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wuz.jyoumei.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pdk.aizwys.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rbd.zhongyouzk.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ury.shuidangran.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tvj.zdbjq.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://dhw.ivvv.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vwk.jqgfzy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qgd.dianchejie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://glj.yanxiufei.cn

================================================================================
来源：http://wvf.ybcxt.top

A. 基础语法与类型
来源：http://uym.ywan-chungtsiang.top

================================================================================
来源：http://sjg.yj20258888.top

[A01] Hello World
来源：http://aii.gotoacloud.top

Py:   print("Hello, World!")
来源：http://uln.zhaomingkeji.xyz

PHP:  echo "Hello, World!";
来源：http://hmd.shzxlz.cn

JS:   console.log("Hello, World!");
来源：http://vmx.epnwcf.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://iah.316326.xyz

Java: System.out.println("Hello, World!");
来源：http://ojm.52xcode.cn

Go:   fmt.Println("Hello, World!")
来源：http://abv.shzxlz.cn

Ruby: puts "Hello, World!"
来源：http://bck.yfazqb.com

C#:   Console.WriteLine("Hello, World!");
来源：http://smy.sweek.top

[A02] 变量声明与赋值
来源：http://azc.hnqzz.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dbe.sxryk.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://fvy.sxryk.cn

JS:   let name = "Alex"; const age = 20;
来源：http://vof.pengpengdd.cyou

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ozb.redwolf501.top

Java: String name = "Alex"; int age = 20;
来源：http://ssq.316326.xyz

Go:   name := "Alex"; age := 20
来源：http://qya.ydzc1.top

Ruby: name = "Alex"; age = 20
来源：http://jbe.wangshuangyany.cn

C#:   string name = "Alex"; int age = 20;
来源：http://pdc.snrcjt.cn

[A03] 常量定义
来源：http://zys.hongshengwenyu.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mun.gaohongyu789.top

PHP:  const PI = 3.14159;
来源：http://cfd.cdnleiting.top

JS:   const PI = 3.14159;
来源：http://nig.feifeiyinyue.top

TS:   const PI: number = 3.14159;
来源：http://dhz.vehdjk.com

Java: static final double PI = 3.14159;
来源：http://zfq.daria6918.cn

Go:   const PI = 3.14159
来源：http://dyb.chenlongwang.top

Ruby: PI = 3.14159
来源：http://sya.chenlongwang.top

C#:   const double PI = 3.14159;
来源：http://bah.dashuyun.cn

[A04] 判断变量类型
来源：http://gcd.jinghuilouyu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://vwt.jqgfzy.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mul.zhixingplan.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vav.yongpay.top

TS:   typeof x; x instanceof Date
来源：http://kkg.yj20258888.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wfx.hammf.cn

Go:   reflect.TypeOf(x).Name()
来源：http://amv.zycfv.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://era.52xcode.cn

C#:   x.GetType().Name; x is int
来源：http://zjx.sxryk.cn

[A05] 整数除法与取模
来源：http://dmb.c1oappe.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ehx.hongshengwenyu.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://eve.zhoulong.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://uax.zhixingplan.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://shr.zhoulong.xyz

Java: 7 / 2; 7 % 2
来源：http://isi.yj202588.top

Go:   7 / 2; 7 % 2
来源：http://rzd.meibo888.top

Ruby: 7 / 2; 7 % 2
来源：http://gum.xuetiantiany.cn

C#:   7 / 2; 7 % 2
来源：http://dgg.cqqwz.cn

[A06] 字符串转数字
来源：http://kgk.jinqigfzy.top

Py:   int("42"); float("3.14")
来源：http://arc.gotoacloud.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://avh.jqgfzy.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ykr.fanxiaobao.xyz


<!-- 参考信息 -->