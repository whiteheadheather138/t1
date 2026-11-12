代发 wailian999

[U47] PHP：联合类型
来源：http://efe.chenlongwang.top

int|string $id
来源：http://pxh.andypj.xyz

[U48] PHP：纯枚举
来源：http://hrm.fehbvm.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://arc.zhongyouzk.top

[U49] PHP：只读属性
来源：http://zva.ywan-chungtsiang.top

public readonly string $name
来源：http://qks.guannengcc.top

[U50] PHP：构造器属性提升
来源：http://knr.ydzc1.top

public function __construct(private int $id) {}
来源：http://nlk.zhongyouzk.top

[U51] PHP：数组解构
来源：http://kpz.cdnleiting.top

[$a, $b] = $arr;
来源：http://byr.yuxming.cn

[U52] PHP：箭头函数
来源：http://umw.wangdashe.top

$double = fn($x) => $x * 2;
来源：http://vjt.fanxiaobao.xyz

[U53] PHP：空合并运算符
来源：http://kxf.sysykeji.top

$v = $a ?? $b ?? "default";
来源：http://lym.birdmap.top

[U54] PHP：空安全调用
来源：http://jnn.yuxming.cn

$obj?->method()
来源：http://mdq.zhengqikj.top

[U55] PHP：match 表达式
来源：http://zcp.xziqi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vrq.kuanghao11.cn

[U56] PHP：命名参数
来源：http://ljt.daxiang520.top

f(a: 1, b: 2)
来源：http://xdx.cdnleiting.top

[U57] PHP：字符串插值
来源：http://gwf.fehbvm.com

"值: {$a}"
来源：http://gvp.fktsv.cn

[U58] PHP：数组三件套
来源：http://rvf.zhoulong.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vwj.0kj1m.cn

[U59] PHP：自定义排序
来源：http://abp.zhongyouzk.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ron.yueranfly.top

[U60] PHP：JSON 编解码
来源：http://det.nanxuanxn.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dyh.tianlin.xyz

[U61] PHP：正则
来源：http://opz.sufxvd.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://drd.zycfv.cn

[U62] PHP：日期对象
来源：http://ymr.zhengqikj.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dbs.zycfv.cn

[U63] PHP：文件读写
来源：http://xtb.aizwys.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bgr.hywenlv.cn

[U64] PHP：目录遍历
来源：http://yvr.nanxinkj.top

glob("dir/*.php");  scandir("dir");
来源：http://gnw.zhijiandao.cn

[U65] PHP：会话
来源：http://tgi.yueranfly.top

session_start();  $_SESSION["uid"] = 1;
来源：http://qoh.yuanzhike.top

[U66] PHP：设置 Cookie
来源：http://qbt.jqgufenzy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wff.pengpengdd.cyou

[U67] PHP：处理文件上传
来源：http://dqh.yueranfly.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://luz.kuanghao11.cn

[U68] PHP：PDO 连接
来源：http://xrr.zhiwuduotai.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vfq.nanxinkj.top

[U69] PHP：PDO 预处理
来源：http://lbs.fanxiaobao.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tgl.ctjpmb.com

[U70] PHP：PDO 事务
来源：http://cjo.sysykeji.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wdj.jyoumei.cn

[U71] PHP：抛出异常
来源：http://znt.52xcode.cn

throw new RuntimeException("失败", 500);
来源：http://als.birdmap.top

[U72] PHP：写错误日志
来源：http://frz.chenlongwang.top

error_log("失败: " . $e->getMessage());
来源：http://yev.ydzc1.top

[U73] PHP：读取 ini 配置
来源：http://ych.yueranfly.top

parse_ini_file("config.ini", true)
来源：http://mmp.zhijiandao.cn

[U74] PHP：读取环境变量
来源：http://jby.tarul.cn

getenv("APP_ENV") ?: "production"
来源：http://mrq.aibaodan.cn

[U75] PHP：依赖注入
来源：http://ctz.xuetiantiany.cn

composer require psr/container
来源：http://pnw.shangyingyoupin.top

[U76] PHP：简单路由
来源：http://wnw.yonumen.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://whm.sufxvd.cn

[U77] PHP：模板渲染
来源：http://ksf.shanyushiyangtech.top

composer require twig/twig
来源：http://zkp.yanxiufei.cn

[U78] PHP：单元测试
来源：http://fdc.fanxiaobao.xyz

composer require --dev phpunit/phpunit
来源：http://dks.c1oappe.top

[U79] PHP：静态分析
来源：http://mcr.xziqi.cn

composer require --dev phpstan/phpstan
来源：http://dbq.xylfe.cn

[U80] PHP：代码规范修复
来源：http://htj.jqgufenzy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://rcr.pycfn.com

[U81] JS：初始化项目
来源：http://lkc.yfazqb.com

npm init -y;  npm i express
来源：http://huv.xingfuxueyuan.xyz

[U82] JS：package.json 脚本
来源：http://fnh.hnqzz.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://iti.jinyuanbaomall.cn

[U83] JS：ES Module 导入导出
来源：http://xxe.ydjk.org.cn

export const a = 1;  import { a } from "./m.js";
来源：http://tff.nwbrower.top

[U84] JS：CommonJS 写法
来源：http://nco.chenzaomai.com

module.exports = { a };  const { a } = require("./m");
来源：http://ijm.jinqigufen.top

[U85] JS：可选链
来源：http://mhs.guowangkeji.top

a?.b?.c
来源：http://dtd.shanyushiyangkeji.top

[U86] JS：空值合并
来源：http://meg.shuidangran.top

a ?? b
来源：http://oqy.fzhhl.top

[U87] JS：解构默认值
来源：http://wxx.hcnkem.com

const { a = 1, b = 2 } = obj;
来源：http://azc.cucudq.cn

[U88] JS：对象展开合并
来源：http://rae.smart0.xyz

{ ...a, ...b }
来源：http://oib.ivvv.top

[U89] JS：数组去重
来源：http://ghu.jiagoushi.top

[...new Set(arr)]
来源：http://ldn.zycfv.cn

[U90] JS：数字数组排序
来源：http://iqv.jlsjyb.cn

[...arr].sort((a, b) => a - b)
来源：http://qdr.chenzaomai.com

[U91] JS：对象键值遍历
来源：http://vjb.chenzaomai.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zkr.hesvh.cn

[U92] JS：深拷贝
来源：http://ugm.zhongyouzk.top

structuredClone(obj)
来源：http://mzf.zhengqikj.top

[U93] JS：模板字符串
来源：http://cpc.0kj1m.cn

`共 ${n} 条`
来源：http://cok.nanxuanxn.top

[U94] JS：箭头函数
来源：http://xww.zdbjq.cn

const double = x => x * 2;
来源：http://zhs.xinyue.icu

[U95] JS：Promise 包装
来源：http://vmp.ehwqpu.com

new Promise((resolve, reject) => {})
来源：http://lpj.wangshuangyany.cn

[U96] JS：async/await 与异常
来源：http://dlb.hesvh.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dhj.jlsjyb.cn

[U97] JS：并发请求
来源：http://gou.hnxiangtu.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ebf.yonumen.top

[U98] JS：fetch 带 JSON
来源：http://lfg.cashguo.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tac.zhixingplan.top

[U99] JS：事件监听
来源：http://ntp.guowangkeji.top

el.addEventListener("click", e => {})
来源：http://ybr.fzhhl.top

[U100] JS：DOM 查询
来源：http://kni.zhengqikj.top

document.querySelector(".item")
来源：http://zly.hysaishi.cn

[U101] JS：classList 操作
来源：http://mbv.pycfn.com

el.classList.toggle("active")
来源：http://mqu.uphjek.com

[U102] JS：本地存储
来源：http://gsi.ywan-chungtsiang.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://otf.fehbvm.com

[U103] JS：定时器
来源：http://oul.zhongyouzk.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dtc.epnwcf.com

[U104] JS：防抖
来源：http://vez.sweek.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pbx.xuetiantiany.cn

[U105] JS：节流
来源：http://tdn.zhaomingkeji.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ftt.sysykeji.top

[U106] JS：日期格式化
来源：http://tke.jinyuanbaomall.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://exz.tanke756.top

[U107] JS：数字千分位
来源：http://hna.chenzaomai.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wcn.yangfankeji.com

[U108] JS：随机整数
来源：http://nsx.meibo888.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zsg.jiagoushi.top

[U109] JS：数组分组
来源：http://gdg.jinqigufen.top

Object.groupBy(arr, x => x.type)
来源：http://kof.hysaishi.cn

[U110] JS：数组分块
来源：http://uai.nanxinkj.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lwj.zhengqikj.top

[U111] JS：对象转 Map
来源：http://oyq.0kj1m.cn

new Map(Object.entries(obj))
来源：http://eeq.yueranfly.top

[U112] JS：字符串补位
来源：http://zal.smart0.xyz

"7".padStart(3, "0")
来源：http://pps.yfazqb.com

[U113] JS：正则替换全部
来源：http://ptb.shuidangran.top

s.replaceAll("a", "b")
来源：http://qab.jiagoushi.top

[U114] JS：JSON 深比较
来源：http://vay.snrcjt.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://rfu.mhx1999.top

[U115] JS：生成 UUID
来源：http://kmt.guannengcc.top

crypto.randomUUID()
来源：http://zvv.nwbrower.top

[U116] JS：类型检查（JSDoc）
来源：http://kws.chenzaomai.com

/** @param {string} name */ function f(name) {}
来源：http://foh.ivvv.top

[U117] JS：单元测试
来源：http://msz.xuetiantiany.cn

npm i -D vitest;  npx vitest
来源：http://abm.daria6918.cn

[U118] JS：开发服务器
来源：http://ghz.zhijiandao.cn

npm i -D vite;  npx vite
来源：http://qny.xylfe.cn

[U119] JS：生产构建
来源：http://jlw.epnwcf.com

npx vite build
来源：http://uab.tian-w.cn

[U120] JS：读取环境变量（Vite）
来源：http://ydf.9152youxi.cn

import.meta.env.VITE_API_URL
来源：http://ruo.316326.xyz

================================================================================
来源：http://pyf.cashguo.top

统计汇总
来源：http://dhy.xuetiantiany.cn

================================================================================
来源：http://jrp.nanxuanxn.top

按语言统计（条）：
来源：http://vly.316326.xyz

Python ......... 252
来源：http://xvq.nanxinkj.top

PHP ............ 252
来源：http://iai.yuxming.cn

JavaScript ..... 252
来源：http://fpx.bjfxy.top

TypeScript ..... 212
来源：http://ltf.jinqigufen.top

Java ........... 212
来源：http://rdq.hongshengwenyu.top

Go ............. 212
来源：http://wgl.meibo888.top

Ruby ........... 212
来源：http://rpp.ydjk.org.cn

C# ............. 212
来源：http://glo.birdmap.top

C .............. 30
来源：http://ufu.hysaishi.cn

C++ ............ 30
来源：http://jby.aizwys.cn

SQL ............ 90
来源：http://ycw.316326.xyz

Bash ........... 80
来源：http://hyg.hongshengwenyu.top

Kotlin ......... 15
来源：http://fkx.vqdsnc.cn

Swift .......... 15
来源：http://mdz.gotoacloud.top

Lua ............ 10
来源：http://miy.52xcode.cn

Perl ........... 10
来源：http://utn.vehdjk.com

Scala .......... 10
来源：http://lme.cdnleiting.top

------------------------------------
来源：http://lbq.bbcook.cn

合计 ........... 2106 条
来源：http://khs.yonumen.top

按章节统计：
来源：http://gdq.quarkkingdee.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://apy.jinqigufen.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nbh.gaohongyu789.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://juu.hysaishi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pgs.smart0.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ahd.dashuyun.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vux.dashuyun.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ima.aibaodan.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ocz.chenzaomai.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://cou.xziqi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qsm.fzhhl.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zwm.0kj1m.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gbt.fehbvm.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tfw.hysaishi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qjq.ppjwa.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rcq.yj20258888.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gmw.zhixingplan.top

Q SQL 专题                              90
来源：http://jih.jqgufenzy.top

R Bash 专题                             80
来源：http://wlv.ppjwa.cn

S C / C++ 专题                          60
来源：http://ieg.52xcode.cn

T 其他语言补充                          60
来源：http://jzv.zdbjq.cn

U 高频实用片段                         120
来源：http://akh.shuidangran.top

------------------------------------
来源：http://hhh.hnxiangtu.top

合计                                  2106 条
来源：http://wvn.316326.xyz

--------------------------------------------------------------------------------
来源：http://ysu.sjlbkw.cn

使用提醒
来源：http://khw.haohaochexian.top

--------------------------------------------------------------------------------
来源：http://jqn.shangyingyoupin.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fhv.tian-w.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://adl.yuanzhike.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zfx.zhiwuduotai.top

在旧版本上使用前请先确认语法支持情况。
来源：http://nzz.ywan-chungtsiang.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://drn.fengsongda.top

—— 文件结束 ——
来源：http://ztx.zdqjudy.top

================================================================================
来源：http://dzo.ydzc1.top

程序语言常见例子速查手册（2024 版）
来源：http://fuu.jinqigufen.top

Common Programming Examples Cheat Book
来源：http://bie.hnqzz.top

================================================================================
来源：http://iej.fzhhl.top

【收录内容】
来源：http://ogs.sweek.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://itz.birdmap.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://sny.pycfn.com

SQL · Bash · C · C++
来源：http://coq.hcnkem.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wmd.zhengqikj.top

【使用说明】
来源：http://ipg.shuidangran.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://iqt.jinyuanbaomall.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kpu.wangdashe.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ddg.hysaishi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xjw.jiagoushi.top

Bash:  Shell         C:     C             C++:   C++
来源：http://mej.uphjek.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://epy.xziqi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kfy.zhoulong.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nmk.jinqigfzy.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://sxx.hnxiangtu.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nss.jqgfzy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vec.shuidangran.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://lfm.bjfxy.top

【文件统计】
来源：http://uxa.gzhubu.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://llr.dianchejie.cn

--------------------------------------------------------------------------------
来源：http://awx.bbcook.cn

目  录
来源：http://wys.birdmap.top

--------------------------------------------------------------------------------
来源：http://dao.hcnkem.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rmn.dashuyun.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mds.pycfn.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hcp.kuanghao11.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://neq.dashuyun.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vzp.jqgufenzy.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fss.xuetiantiany.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fzi.shangyingyoupin.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pwv.jlsjyb.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://cdn.iojbl.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://kqi.ybcxt.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://flg.xinyue.icu

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gnm.xuetiantiany.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hxs.dianchejie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://nnz.yfazqb.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hwm.yj202588.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://pmk.mhx1999.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zfr.xziqi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://prv.guannengcc.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://gts.hywenlv.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lln.havefunace.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ujc.jinyuanbaomall.cn

================================================================================
来源：http://bey.yj20258.top

A. 基础语法与类型
来源：http://ebw.ctjpmb.com

================================================================================
来源：http://xab.sysykeji.top

[A01] Hello World
来源：http://gdg.jinqigfzy.top

Py:   print("Hello, World!")
来源：http://len.yongpay.top

PHP:  echo "Hello, World!";
来源：http://lqw.zhixingplan.top

JS:   console.log("Hello, World!");
来源：http://cok.guowangkeji.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fec.hammf.cn

Java: System.out.println("Hello, World!");
来源：http://vzc.shuidangran.top

Go:   fmt.Println("Hello, World!")
来源：http://gyo.iojbl.cn

Ruby: puts "Hello, World!"
来源：http://hnc.ehwqpu.com

C#:   Console.WriteLine("Hello, World!");
来源：http://ahu.daxiang520.top

[A02] 变量声明与赋值
来源：http://kyh.hfpthk.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tjx.zhijiandao.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://rqx.wangshuangyany.cn

JS:   let name = "Alex"; const age = 20;
来源：http://fwz.gaohongyu789.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qjw.tianlin.xyz

Java: String name = "Alex"; int age = 20;
来源：http://iiz.xingfuxueyuan.xyz

Go:   name := "Alex"; age := 20
来源：http://kpk.snrcjt.cn

Ruby: name = "Alex"; age = 20
来源：http://hhm.zhoulong.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://nmt.zdqjudy.top

[A03] 常量定义
来源：http://qtg.fzhhl.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://cxi.pycfn.com

PHP:  const PI = 3.14159;
来源：http://oyu.ehwqpu.com

JS:   const PI = 3.14159;
来源：http://anw.tanke756.top

TS:   const PI: number = 3.14159;
来源：http://cic.zhongyouzk.top

Java: static final double PI = 3.14159;
来源：http://hvi.jianghu66.top

Go:   const PI = 3.14159
来源：http://ajs.bjfxy.top

Ruby: PI = 3.14159
来源：http://snj.tarul.cn

C#:   const double PI = 3.14159;
来源：http://qqv.redwolf501.top

[A04] 判断变量类型
来源：http://fwr.cdnleiting.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://hid.zhoulong.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xzw.sufxvd.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gpk.ppjwa.cn

TS:   typeof x; x instanceof Date
来源：http://wxm.xuanzx.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ufm.vehdjk.com

Go:   reflect.TypeOf(x).Name()
来源：http://qwl.zdqjudy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://vkv.ivvv.top

C#:   x.GetType().Name; x is int
来源：http://rhz.316326.xyz

[A05] 整数除法与取模
来源：http://wqu.dashuyun.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rxz.jqgufenzy.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ooz.daria6918.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://rnq.jinqigfzy.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ozd.ydzc1.top

Java: 7 / 2; 7 % 2
来源：http://rpi.nwbrower.top

Go:   7 / 2; 7 % 2
来源：http://bcr.jyoumei.cn

Ruby: 7 / 2; 7 % 2
来源：http://ywv.dianchejie.cn

C#:   7 / 2; 7 % 2
来源：http://kgp.chenlongwang.top


<!-- 参考信息 -->