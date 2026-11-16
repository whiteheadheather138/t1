代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://rlr.hywenlv.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vkb.guannengcc.top

[U46] PHP：可空类型
来源：http://dpf.jinqigfzy.top

?string $name = null
来源：http://mrs.zhixingplan.top

[U47] PHP：联合类型
来源：http://moi.quarkkingdee.top

int|string $id
来源：http://ygs.fengsongda.top

[U48] PHP：纯枚举
来源：http://xjw.0kj1m.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zez.cheryme.top

[U49] PHP：只读属性
来源：http://bxz.wangdashe.top

public readonly string $name
来源：http://xmd.fengsongda.top

[U50] PHP：构造器属性提升
来源：http://awr.0kj1m.cn

public function __construct(private int $id) {}
来源：http://kuj.meibo888.top

[U51] PHP：数组解构
来源：http://amb.sjlbkw.cn

[$a, $b] = $arr;
来源：http://iwq.zhiwuduotai.top

[U52] PHP：箭头函数
来源：http://mcf.yueranfly.top

$double = fn($x) => $x * 2;
来源：http://qtz.birdmap.top

[U53] PHP：空合并运算符
来源：http://niq.chenjidiqi.icu

$v = $a ?? $b ?? "default";
来源：http://eui.epnwcf.com

[U54] PHP：空安全调用
来源：http://why.9152youxi.cn

$obj?->method()
来源：http://gxj.tarul.cn

[U55] PHP：match 表达式
来源：http://pgc.birdmap.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jrr.hesvh.cn

[U56] PHP：命名参数
来源：http://uqh.c1oappe.top

f(a: 1, b: 2)
来源：http://plq.316326.xyz

[U57] PHP：字符串插值
来源：http://ddu.mhx1999.top

"值: {$a}"
来源：http://mny.hnxiangtu.top

[U58] PHP：数组三件套
来源：http://efh.pycfn.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zcz.jianghu66.top

[U59] PHP：自定义排序
来源：http://lip.ivvv.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vzw.ctjpmb.com

[U60] PHP：JSON 编解码
来源：http://osy.ehwqpu.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://iwi.vqdsnc.cn

[U61] PHP：正则
来源：http://pwp.wangshuangyany.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vep.zdqjudy.top

[U62] PHP：日期对象
来源：http://utc.cashguo.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qtv.cqqwz.cn

[U63] PHP：文件读写
来源：http://zvu.xingfuxueyuan.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hde.yangfankeji.com

[U64] PHP：目录遍历
来源：http://sjy.tianlin.xyz

glob("dir/*.php");  scandir("dir");
来源：http://omq.sysykeji.top

[U65] PHP：会话
来源：http://ane.ybcxt.top

session_start();  $_SESSION["uid"] = 1;
来源：http://hpy.ivvv.top

[U66] PHP：设置 Cookie
来源：http://gtb.aibaodan.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ljl.ppjwa.cn

[U67] PHP：处理文件上传
来源：http://laa.jiagoushi.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wpk.redwolf501.top

[U68] PHP：PDO 连接
来源：http://hbn.yanxiufei.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lzq.fengsongda.top

[U69] PHP：PDO 预处理
来源：http://dld.c1oappe.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lfv.zhixingplan.top

[U70] PHP：PDO 事务
来源：http://wde.yuxming.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://iwm.cheryme.top

[U71] PHP：抛出异常
来源：http://mxd.dashuyun.cn

throw new RuntimeException("失败", 500);
来源：http://qth.tian-w.cn

[U72] PHP：写错误日志
来源：http://hka.epnwcf.com

error_log("失败: " . $e->getMessage());
来源：http://zsu.xziqi.cn

[U73] PHP：读取 ini 配置
来源：http://usm.tanke756.top

parse_ini_file("config.ini", true)
来源：http://wkb.fktsv.cn

[U74] PHP：读取环境变量
来源：http://ptw.jiagoushi.top

getenv("APP_ENV") ?: "production"
来源：http://iwo.ydjk.org.cn

[U75] PHP：依赖注入
来源：http://bgq.pycfn.com

composer require psr/container
来源：http://xly.wangshuangyany.cn

[U76] PHP：简单路由
来源：http://occ.ydzc1.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://eqz.ybcxt.top

[U77] PHP：模板渲染
来源：http://kzr.yj20258.top

composer require twig/twig
来源：http://ohk.fktsv.cn

[U78] PHP：单元测试
来源：http://swz.ehwqpu.com

composer require --dev phpunit/phpunit
来源：http://yew.xinyue.icu

[U79] PHP：静态分析
来源：http://dsf.0kj1m.cn

composer require --dev phpstan/phpstan
来源：http://acj.tian-w.cn

[U80] PHP：代码规范修复
来源：http://mep.havefunace.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://kuu.zdbjq.cn

[U81] JS：初始化项目
来源：http://fhs.quarkkingdee.top

npm init -y;  npm i express
来源：http://weq.birdmap.top

[U82] JS：package.json 脚本
来源：http://sqi.hesvh.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://oza.xuetiantiany.cn

[U83] JS：ES Module 导入导出
来源：http://hxj.nanxuanxn.top

export const a = 1;  import { a } from "./m.js";
来源：http://hhk.shzxlz.cn

[U84] JS：CommonJS 写法
来源：http://nse.hfpthk.cn

module.exports = { a };  const { a } = require("./m");
来源：http://jzr.shuidangran.top

[U85] JS：可选链
来源：http://vza.hnxiangtu.top

a?.b?.c
来源：http://hks.iojbl.cn

[U86] JS：空值合并
来源：http://xti.tanke756.top

a ?? b
来源：http://hpr.mhx1999.top

[U87] JS：解构默认值
来源：http://jtf.cucudq.cn

const { a = 1, b = 2 } = obj;
来源：http://xgg.smart0.xyz

[U88] JS：对象展开合并
来源：http://rpr.zhijiandao.cn

{ ...a, ...b }
来源：http://pum.ehwqpu.com

[U89] JS：数组去重
来源：http://neo.dianchejie.cn

[...new Set(arr)]
来源：http://agp.52xcode.cn

[U90] JS：数字数组排序
来源：http://zmi.cashguo.top

[...arr].sort((a, b) => a - b)
来源：http://wzf.zhijiandao.cn

[U91] JS：对象键值遍历
来源：http://cqk.shzxlz.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://znq.cqqwz.cn

[U92] JS：深拷贝
来源：http://khl.cheryme.top

structuredClone(obj)
来源：http://ewv.sysykeji.top

[U93] JS：模板字符串
来源：http://bei.yonumen.top

`共 ${n} 条`
来源：http://sof.yonumen.top

[U94] JS：箭头函数
来源：http://aab.dianchejie.cn

const double = x => x * 2;
来源：http://vfz.52xcode.cn

[U95] JS：Promise 包装
来源：http://ova.jqgfzy.top

new Promise((resolve, reject) => {})
来源：http://trx.dianchejie.cn

[U96] JS：async/await 与异常
来源：http://gdg.sjlbkw.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kzw.shanyushiyangkeji.top

[U97] JS：并发请求
来源：http://kip.cdnleiting.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ebz.yvedp.cn

[U98] JS：fetch 带 JSON
来源：http://vsw.yueranfly.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tgx.ctjpmb.com

[U99] JS：事件监听
来源：http://roe.jlsjyb.cn

el.addEventListener("click", e => {})
来源：http://xth.fzhhl.top

[U100] JS：DOM 查询
来源：http://ifq.dianchejie.cn

document.querySelector(".item")
来源：http://lim.hnqzz.top

[U101] JS：classList 操作
来源：http://afu.jlsjyb.cn

el.classList.toggle("active")
来源：http://qnc.gotoacloud.top

[U102] JS：本地存储
来源：http://cpf.chenjidiqi.icu

localStorage.setItem("k", JSON.stringify(v))
来源：http://ejj.redwolf501.top

[U103] JS：定时器
来源：http://bvw.feifeiyinyue.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vdk.zhixingplan.top

[U104] JS：防抖
来源：http://rcp.smart0.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wde.0kj1m.cn

[U105] JS：节流
来源：http://gnf.quarkkingdee.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fgt.redwolf501.top

[U106] JS：日期格式化
来源：http://bsy.cashguo.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://any.jlsjyb.cn

[U107] JS：数字千分位
来源：http://okx.gotoacloud.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gwo.cucudq.cn

[U108] JS：随机整数
来源：http://rxe.xuanzx.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ttj.316326.xyz

[U109] JS：数组分组
来源：http://auu.jiagoushi.top

Object.groupBy(arr, x => x.type)
来源：http://bvy.zdqjudy.top

[U110] JS：数组分块
来源：http://ncp.hysaishi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://clo.yongpay.top

[U111] JS：对象转 Map
来源：http://veb.yj20258.top

new Map(Object.entries(obj))
来源：http://fas.tianlin.xyz

[U112] JS：字符串补位
来源：http://asq.shanyushiyangtech.top

"7".padStart(3, "0")
来源：http://iup.jinyuanbaomall.cn

[U113] JS：正则替换全部
来源：http://nor.9152youxi.cn

s.replaceAll("a", "b")
来源：http://aiy.fanxiaobao.xyz

[U114] JS：JSON 深比较
来源：http://vry.yj202588.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://aka.nanxinkj.top

[U115] JS：生成 UUID
来源：http://yxd.chenzaomai.com

crypto.randomUUID()
来源：http://vfz.fzhhl.top

[U116] JS：类型检查（JSDoc）
来源：http://sic.xuetiantiany.cn

/** @param {string} name */ function f(name) {}
来源：http://azl.dashuyun.cn

[U117] JS：单元测试
来源：http://nfv.kuanghao11.cn

npm i -D vitest;  npx vitest
来源：http://axm.ehwqpu.com

[U118] JS：开发服务器
来源：http://opy.yongpay.top

npm i -D vite;  npx vite
来源：http://muk.kuanghao11.cn

[U119] JS：生产构建
来源：http://feb.0kj1m.cn

npx vite build
来源：http://ryr.yonumen.top

[U120] JS：读取环境变量（Vite）
来源：http://etq.uphjek.com

import.meta.env.VITE_API_URL
来源：http://afg.tanke756.top

================================================================================
来源：http://liy.svipenyu.cn

统计汇总
来源：http://rqs.yuanzhike.top

================================================================================
来源：http://rbk.aibaodan.cn

按语言统计（条）：
来源：http://sqy.smart0.xyz

Python ......... 252
来源：http://xxh.svipenyu.cn

PHP ............ 252
来源：http://bmt.dianchejie.cn

JavaScript ..... 252
来源：http://ied.52xcode.cn

TypeScript ..... 212
来源：http://fsz.fanxiaobao.xyz

Java ........... 212
来源：http://opp.havefunace.top

Go ............. 212
来源：http://qmh.snrcjt.cn

Ruby ........... 212
来源：http://zmh.svipenyu.cn

C# ............. 212
来源：http://zlg.xylfe.cn

C .............. 30
来源：http://eeb.bjfxy.top

C++ ............ 30
来源：http://vul.yfazqb.com

SQL ............ 90
来源：http://zzq.fzhhl.top

Bash ........... 80
来源：http://eoz.hnxiangtu.top

Kotlin ......... 15
来源：http://mgd.jianghu66.top

Swift .......... 15
来源：http://dgn.0kj1m.cn

Lua ............ 10
来源：http://eea.shangyingyoupin.top

Perl ........... 10
来源：http://vuf.c1oappe.top

Scala .......... 10
来源：http://zvf.ydzc1.top

------------------------------------
来源：http://prc.snrcjt.cn

合计 ........... 2106 条
来源：http://upf.hysaishi.cn

按章节统计：
来源：http://pqi.hysaishi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ipp.jqgfzy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://usp.guannengcc.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://eqp.xuetiantiany.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cnp.gotoacloud.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fhz.haohaochexian.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tuk.andypj.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fss.wangshuangyany.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dqr.kuanghao11.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gdg.nanxinkj.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://aeq.pycfn.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://afk.dashuyun.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sem.zhixingplan.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jev.jinqigufen.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://moa.cqqwz.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vze.gaohongyu789.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://snd.jianghu66.top

Q SQL 专题                              90
来源：http://zvt.gotoacloud.top

R Bash 专题                             80
来源：http://yan.zdbjq.cn

S C / C++ 专题                          60
来源：http://cms.52xcode.cn

T 其他语言补充                          60
来源：http://pmp.shanyushiyangtech.top

U 高频实用片段                         120
来源：http://mwq.yongpay.top

------------------------------------
来源：http://dtr.epnwcf.com

合计                                  2106 条
来源：http://ccy.nanxinkj.top

--------------------------------------------------------------------------------
来源：http://tvq.tianlin.xyz

使用提醒
来源：http://lys.gotoacloud.top

--------------------------------------------------------------------------------
来源：http://yhq.quarkkingdee.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jru.gotoacloud.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://sut.jianghu66.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://sfb.sysykeji.top

在旧版本上使用前请先确认语法支持情况。
来源：http://xmk.svipenyu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zdr.zhijiandao.cn

—— 文件结束 ——
来源：http://aql.ctjpmb.com

================================================================================
来源：http://jnh.hnqzz.top

程序语言常见例子速查手册（2024 版）
来源：http://mmp.hesvh.cn

Common Programming Examples Cheat Book
来源：http://uaq.chenlongwang.top

================================================================================
来源：http://lnq.jianghu66.top

【收录内容】
来源：http://dcu.shanyushiyangtech.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://wdt.ybcxt.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jum.zdbjq.cn

SQL · Bash · C · C++
来源：http://jfk.shzxlz.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://bde.hcnkem.com

【使用说明】
来源：http://mgp.zhijiandao.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kcr.hongshengwenyu.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qff.zycfv.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fld.kuanghao11.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hap.yangfankeji.com

Bash:  Shell         C:     C             C++:   C++
来源：http://jhk.yanxiufei.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ihv.xuetiantiany.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cse.shzxlz.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yyk.haohaochexian.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rpk.jqgufenzy.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fvn.wangshuangyany.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://emm.kuanghao11.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://civ.daxiang520.top

【文件统计】
来源：http://dhp.mhx1999.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mly.yuanzhike.top

--------------------------------------------------------------------------------
来源：http://vqt.zycfv.cn

目  录
来源：http://nmm.ppjwa.cn

--------------------------------------------------------------------------------
来源：http://yjp.pengpengdd.cyou

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yit.zdqjudy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://snk.aizwys.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://frj.sweek.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://agq.fengsongda.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zbf.hysaishi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ytc.nanxinkj.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zst.hnqzz.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hyv.xuetiantiany.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://spm.shanyushiyangkeji.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fxu.daria6918.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dqg.shangyingyoupin.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ysl.sweek.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://urk.dashuyun.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hxx.tian-w.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://joo.yongpay.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mjc.hnqzz.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mcb.zhijiandao.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://cyd.yongpay.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://kxi.bbcook.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vsn.yuanzhike.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qbo.ppjwa.cn

================================================================================
来源：http://aby.316326.xyz

A. 基础语法与类型
来源：http://ntx.fanxiaobao.xyz

================================================================================
来源：http://isg.vehdjk.com

[A01] Hello World
来源：http://zxk.sxryk.cn

Py:   print("Hello, World!")
来源：http://tzf.ybcxt.top

PHP:  echo "Hello, World!";
来源：http://tma.daxiang520.top

JS:   console.log("Hello, World!");
来源：http://rhv.aizwys.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ndr.cashguo.top

Java: System.out.println("Hello, World!");
来源：http://abu.yueranfly.top

Go:   fmt.Println("Hello, World!")
来源：http://cfa.xziqi.cn

Ruby: puts "Hello, World!"
来源：http://smp.ybcxt.top

C#:   Console.WriteLine("Hello, World!");
来源：http://txo.bjfxy.top

[A02] 变量声明与赋值
来源：http://cgl.xuanzx.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://idl.9152youxi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://flk.cheryme.top

JS:   let name = "Alex"; const age = 20;
来源：http://eyr.hnxiangtu.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wpq.shanyushiyangkeji.top

Java: String name = "Alex"; int age = 20;
来源：http://usz.hywenlv.cn

Go:   name := "Alex"; age := 20
来源：http://rmz.cqqwz.cn

Ruby: name = "Alex"; age = 20
来源：http://gtq.nwbrower.top

C#:   string name = "Alex"; int age = 20;
来源：http://pfq.yueranfly.top

[A03] 常量定义
来源：http://grs.birdmap.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tog.c1oappe.top

PHP:  const PI = 3.14159;
来源：http://tka.cheryme.top

JS:   const PI = 3.14159;
来源：http://una.hesvh.cn

TS:   const PI: number = 3.14159;
来源：http://goz.zhengqikj.top

Java: static final double PI = 3.14159;
来源：http://cop.nanxinkj.top

Go:   const PI = 3.14159
来源：http://ask.bbcook.cn

Ruby: PI = 3.14159
来源：http://gbp.cashguo.top

C#:   const double PI = 3.14159;
来源：http://ruh.yvedp.cn

[A04] 判断变量类型
来源：http://qrh.zhixingplan.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://bft.meibo888.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qyl.tian-w.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://eby.ehwqpu.com

TS:   typeof x; x instanceof Date
来源：http://afm.sufxvd.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fxo.uphjek.com

Go:   reflect.TypeOf(x).Name()
来源：http://vgv.nanxuanxn.top

Ruby: x.class; x.is_a?(Integer)
来源：http://uka.svipenyu.cn

C#:   x.GetType().Name; x is int
来源：http://wrk.shangyingyoupin.top

[A05] 整数除法与取模
来源：http://brm.smart0.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yfz.tarul.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://gna.xylfe.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://dku.0kj1m.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rws.fktsv.cn


<!-- 参考信息 -->