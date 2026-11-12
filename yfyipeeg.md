代发 wailian999

[U49] PHP：只读属性
来源：http://wyh.kuanghao11.cn

public readonly string $name
来源：http://rpf.yonumen.top

[U50] PHP：构造器属性提升
来源：http://uwv.cqqwz.cn

public function __construct(private int $id) {}
来源：http://tat.smart0.xyz

[U51] PHP：数组解构
来源：http://zcz.hammf.cn

[$a, $b] = $arr;
来源：http://hzm.sjlbkw.cn

[U52] PHP：箭头函数
来源：http://lnw.jyoumei.cn

$double = fn($x) => $x * 2;
来源：http://kec.daxiang520.top

[U53] PHP：空合并运算符
来源：http://hdg.yj20258.top

$v = $a ?? $b ?? "default";
来源：http://xan.shangyingyoupin.top

[U54] PHP：空安全调用
来源：http://npd.smart0.xyz

$obj?->method()
来源：http://xak.shzxlz.cn

[U55] PHP：match 表达式
来源：http://osb.hammf.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qie.yj20258.top

[U56] PHP：命名参数
来源：http://vpm.nanxinkj.top

f(a: 1, b: 2)
来源：http://wed.hnxiangtu.top

[U57] PHP：字符串插值
来源：http://rra.pengpengdd.cyou

"值: {$a}"
来源：http://eib.gaohongyu789.top

[U58] PHP：数组三件套
来源：http://ike.zhixingplan.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ajy.pengpengdd.cyou

[U59] PHP：自定义排序
来源：http://apd.316326.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aqw.gotoacloud.top

[U60] PHP：JSON 编解码
来源：http://exv.haohaochexian.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bgf.yanxiufei.cn

[U61] PHP：正则
来源：http://raj.yuxming.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qbh.yj20258.top

[U62] PHP：日期对象
来源：http://fsb.yuxming.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yyt.yj20258888.top

[U63] PHP：文件读写
来源：http://pye.gzhubu.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://edp.zhiwuduotai.top

[U64] PHP：目录遍历
来源：http://tjf.shanyushiyangkeji.top

glob("dir/*.php");  scandir("dir");
来源：http://epl.gaohongyu789.top

[U65] PHP：会话
来源：http://hft.shzxlz.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://tuf.daria6918.cn

[U66] PHP：设置 Cookie
来源：http://klj.ivvv.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tcd.chenlongwang.top

[U67] PHP：处理文件上传
来源：http://gtl.yueranfly.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fut.mhx1999.top

[U68] PHP：PDO 连接
来源：http://fvx.sjlbkw.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://leg.yongpay.top

[U69] PHP：PDO 预处理
来源：http://vlk.yj202588.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kzt.xuetiantiany.cn

[U70] PHP：PDO 事务
来源：http://xay.birdmap.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cfu.fktsv.cn

[U71] PHP：抛出异常
来源：http://dgu.yanxiufei.cn

throw new RuntimeException("失败", 500);
来源：http://jwv.0kj1m.cn

[U72] PHP：写错误日志
来源：http://ohp.fktsv.cn

error_log("失败: " . $e->getMessage());
来源：http://woh.cdnleiting.top

[U73] PHP：读取 ini 配置
来源：http://lmc.jinqigfzy.top

parse_ini_file("config.ini", true)
来源：http://umt.shuidangran.top

[U74] PHP：读取环境变量
来源：http://spe.gogol.net.cn

getenv("APP_ENV") ?: "production"
来源：http://woj.jinghuilouyu.cn

[U75] PHP：依赖注入
来源：http://exc.snrcjt.cn

composer require psr/container
来源：http://dmz.xinyue.icu

[U76] PHP：简单路由
来源：http://exr.9152youxi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ubr.fehbvm.com

[U77] PHP：模板渲染
来源：http://qrf.ywan-chungtsiang.top

composer require twig/twig
来源：http://cxs.yj20258.top

[U78] PHP：单元测试
来源：http://xug.hfpthk.cn

composer require --dev phpunit/phpunit
来源：http://aqz.snrcjt.cn

[U79] PHP：静态分析
来源：http://zqw.yangfankeji.com

composer require --dev phpstan/phpstan
来源：http://idp.jinghuilouyu.cn

[U80] PHP：代码规范修复
来源：http://cwf.fehbvm.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://hbd.sjlbkw.cn

[U81] JS：初始化项目
来源：http://ewp.52xcode.cn

npm init -y;  npm i express
来源：http://tkp.zycfv.cn

[U82] JS：package.json 脚本
来源：http://fbe.guowangkeji.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hbr.shanyushiyangkeji.top

[U83] JS：ES Module 导入导出
来源：http://ldk.xuetiantiany.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xtn.jiagoushi.top

[U84] JS：CommonJS 写法
来源：http://xey.havefunace.top

module.exports = { a };  const { a } = require("./m");
来源：http://ciz.meibo888.top

[U85] JS：可选链
来源：http://fih.9152youxi.cn

a?.b?.c
来源：http://ayd.jiagoushi.top

[U86] JS：空值合并
来源：http://oxj.cucudq.cn

a ?? b
来源：http://kwn.fzhhl.top

[U87] JS：解构默认值
来源：http://odj.hongshengwenyu.top

const { a = 1, b = 2 } = obj;
来源：http://ypt.mhx1999.top

[U88] JS：对象展开合并
来源：http://tkf.redwolf501.top

{ ...a, ...b }
来源：http://oxg.ctjpmb.com

[U89] JS：数组去重
来源：http://bzk.fktsv.cn

[...new Set(arr)]
来源：http://zjp.nwbrower.top

[U90] JS：数字数组排序
来源：http://unt.xuetiantiany.cn

[...arr].sort((a, b) => a - b)
来源：http://oma.vehdjk.com

[U91] JS：对象键值遍历
来源：http://eyj.havefunace.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://civ.fanxiaobao.xyz

[U92] JS：深拷贝
来源：http://nlf.tianlin.xyz

structuredClone(obj)
来源：http://bau.jqgufenzy.top

[U93] JS：模板字符串
来源：http://lfa.aibaodan.cn

`共 ${n} 条`
来源：http://xwd.snrcjt.cn

[U94] JS：箭头函数
来源：http://age.hammf.cn

const double = x => x * 2;
来源：http://zks.birdmap.top

[U95] JS：Promise 包装
来源：http://usf.zhoulong.xyz

new Promise((resolve, reject) => {})
来源：http://gun.yuxming.cn

[U96] JS：async/await 与异常
来源：http://jgu.ppjwa.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nhf.guannengcc.top

[U97] JS：并发请求
来源：http://jty.nwbrower.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ybw.chenjidiqi.icu

[U98] JS：fetch 带 JSON
来源：http://ube.hesvh.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cgl.tanke756.top

[U99] JS：事件监听
来源：http://bzy.jinqigfzy.top

el.addEventListener("click", e => {})
来源：http://ftt.yuanzhike.top

[U100] JS：DOM 查询
来源：http://lxq.yuxming.cn

document.querySelector(".item")
来源：http://nco.hammf.cn

[U101] JS：classList 操作
来源：http://otg.meibo888.top

el.classList.toggle("active")
来源：http://dlt.ctjpmb.com

[U102] JS：本地存储
来源：http://ryk.snrcjt.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://mmj.ppjwa.cn

[U103] JS：定时器
来源：http://wgi.jianghu66.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lpj.fzhhl.top

[U104] JS：防抖
来源：http://caq.hnxiangtu.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wtl.shanyushiyangtech.top

[U105] JS：节流
来源：http://gut.meibo888.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mcn.jiagoushi.top

[U106] JS：日期格式化
来源：http://anc.jinghuilouyu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://isy.aizwys.cn

[U107] JS：数字千分位
来源：http://ptz.0kj1m.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baa.epnwcf.com

[U108] JS：随机整数
来源：http://hir.yuxming.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://azm.ywan-chungtsiang.top

[U109] JS：数组分组
来源：http://wdc.zdqjudy.top

Object.groupBy(arr, x => x.type)
来源：http://hmi.pengpengdd.cyou

[U110] JS：数组分块
来源：http://xaf.52xcode.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://klw.ehwqpu.com

[U111] JS：对象转 Map
来源：http://yoe.jinghuilouyu.cn

new Map(Object.entries(obj))
来源：http://mjc.mhx1999.top

[U112] JS：字符串补位
来源：http://zql.tianlin.xyz

"7".padStart(3, "0")
来源：http://tzo.sysykeji.top

[U113] JS：正则替换全部
来源：http://tud.fehbvm.com

s.replaceAll("a", "b")
来源：http://uod.yuxming.cn

[U114] JS：JSON 深比较
来源：http://lah.tanke756.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://egb.svipenyu.cn

[U115] JS：生成 UUID
来源：http://pmr.yj20258.top

crypto.randomUUID()
来源：http://vnq.tianlin.xyz

[U116] JS：类型检查（JSDoc）
来源：http://mht.jqgufenzy.top

/** @param {string} name */ function f(name) {}
来源：http://xbz.feifeiyinyue.top

[U117] JS：单元测试
来源：http://kel.shangyingyoupin.top

npm i -D vitest;  npx vitest
来源：http://osq.hnxiangtu.top

[U118] JS：开发服务器
来源：http://wck.meibo888.top

npm i -D vite;  npx vite
来源：http://jct.quarkkingdee.top

[U119] JS：生产构建
来源：http://vuw.chenlongwang.top

npx vite build
来源：http://enk.iojbl.cn

[U120] JS：读取环境变量（Vite）
来源：http://rhe.jqgufenzy.top

import.meta.env.VITE_API_URL
来源：http://icm.fehbvm.com

================================================================================
来源：http://omv.fengsongda.top

统计汇总
来源：http://voc.yonumen.top

================================================================================
来源：http://cyd.tanke756.top

按语言统计（条）：
来源：http://ktp.hcnkem.com

Python ......... 252
来源：http://mnl.tarul.cn

PHP ............ 252
来源：http://jqi.cqqwz.cn

JavaScript ..... 252
来源：http://ivk.ydzc1.top

TypeScript ..... 212
来源：http://zff.ivvv.top

Java ........... 212
来源：http://vox.fktsv.cn

Go ............. 212
来源：http://lyd.yongpay.top

Ruby ........... 212
来源：http://mho.svipenyu.cn

C# ............. 212
来源：http://rix.jiagoushi.top

C .............. 30
来源：http://wns.bbcook.cn

C++ ............ 30
来源：http://mbm.hysaishi.cn

SQL ............ 90
来源：http://fvj.zhijiandao.cn

Bash ........... 80
来源：http://iuk.jyoumei.cn

Kotlin ......... 15
来源：http://rxi.daria6918.cn

Swift .......... 15
来源：http://quu.jinqigfzy.top

Lua ............ 10
来源：http://zjt.daria6918.cn

Perl ........... 10
来源：http://msn.hnqzz.top

Scala .......... 10
来源：http://mhy.zdbjq.cn

------------------------------------
来源：http://duy.xylfe.cn

合计 ........... 2106 条
来源：http://lfg.guannengcc.top

按章节统计：
来源：http://cuz.jlsjyb.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gio.nanxinkj.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sya.chenzaomai.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://iwz.zhongyouzk.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://euq.dianchejie.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xkk.quarkkingdee.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ycx.jinghuilouyu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ept.havefunace.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ops.zhaomingkeji.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vgm.tanke756.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://drc.zhoulong.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fsd.epnwcf.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zsr.fehbvm.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hcy.tarul.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://iov.cheryme.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://oip.snrcjt.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://idf.quarkkingdee.top

Q SQL 专题                              90
来源：http://tds.xingfuxueyuan.xyz

R Bash 专题                             80
来源：http://hio.cucudq.cn

S C / C++ 专题                          60
来源：http://wxj.daria6918.cn

T 其他语言补充                          60
来源：http://rrb.cheryme.top

U 高频实用片段                         120
来源：http://tis.jinghuilouyu.cn

------------------------------------
来源：http://thh.zhaomingkeji.xyz

合计                                  2106 条
来源：http://ihg.gzhubu.top

--------------------------------------------------------------------------------
来源：http://gmp.nanxinkj.top

使用提醒
来源：http://jam.yj20258888.top

--------------------------------------------------------------------------------
来源：http://pcw.yj20258888.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vmc.fzhhl.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://axi.yonumen.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lod.quarkkingdee.top

在旧版本上使用前请先确认语法支持情况。
来源：http://flj.jinghuilouyu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rfx.yueranfly.top

—— 文件结束 ——
来源：http://dsw.ctjpmb.com

================================================================================
来源：http://sqb.yuanzhike.top

程序语言常见例子速查手册（2024 版）
来源：http://xwj.shanyushiyangtech.top

Common Programming Examples Cheat Book
来源：http://gig.pycfn.com

================================================================================
来源：http://exl.epnwcf.com

【收录内容】
来源：http://vuq.jqgfzy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ind.aibaodan.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://uhn.ybcxt.top

SQL · Bash · C · C++
来源：http://uoy.jlsjyb.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ask.bjfxy.top

【使用说明】
来源：http://xsl.ctjpmb.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ybs.bbcook.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bkz.zdbjq.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://udu.yongpay.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cjg.xuanzx.com

Bash:  Shell         C:     C             C++:   C++
来源：http://qfj.smart0.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://eor.hnxiangtu.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gnx.hnqzz.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fmr.sysykeji.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pbn.pycfn.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gtq.cheryme.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://akt.kuanghao11.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kyp.xylfe.cn

【文件统计】
来源：http://moe.nanxuanxn.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://chy.yuanzhike.top

--------------------------------------------------------------------------------
来源：http://fwp.zhongyouzk.top

目  录
来源：http://wri.cqqwz.cn

--------------------------------------------------------------------------------
来源：http://nwb.fzhhl.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qrt.tarul.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://pmf.meibo888.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://orp.bbcook.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qws.xinyue.icu

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mse.daxiang520.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://dkr.vqdsnc.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://oca.yanxiufei.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zpf.chenlongwang.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://axz.sweek.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rje.hammf.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ofw.havefunace.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hkk.c1oappe.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lql.ywan-chungtsiang.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://nuc.fehbvm.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://yhh.jinghuilouyu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://esi.yangfankeji.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jge.sxryk.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://nhu.yj202588.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jgi.xuanzx.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gse.zhoulong.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.yonumen.top

================================================================================
来源：http://rxx.gzhubu.top

A. 基础语法与类型
来源：http://xiv.ctjpmb.com

================================================================================
来源：http://oxe.52xcode.cn

[A01] Hello World
来源：http://eje.sufxvd.cn

Py:   print("Hello, World!")
来源：http://rqg.shanyushiyangtech.top

PHP:  echo "Hello, World!";
来源：http://qqp.jqgufenzy.top

JS:   console.log("Hello, World!");
来源：http://ajw.cucudq.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yxp.gogol.net.cn

Java: System.out.println("Hello, World!");
来源：http://uys.hammf.cn

Go:   fmt.Println("Hello, World!")
来源：http://wwp.jinyuanbaomall.cn

Ruby: puts "Hello, World!"
来源：http://bxq.yuxming.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://smr.wangshuangyany.cn

[A02] 变量声明与赋值
来源：http://kqh.xuanzx.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gtu.tian-w.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://bkb.yj20258888.top

JS:   let name = "Alex"; const age = 20;
来源：http://bye.ydzc1.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://afi.jinqigfzy.top

Java: String name = "Alex"; int age = 20;
来源：http://msd.wangdashe.top

Go:   name := "Alex"; age := 20
来源：http://wbs.yuanzhike.top

Ruby: name = "Alex"; age = 20
来源：http://ecj.bbcook.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ckj.fktsv.cn

[A03] 常量定义
来源：http://hku.yuanzhike.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gjz.cdnleiting.top

PHP:  const PI = 3.14159;
来源：http://pod.yvedp.cn

JS:   const PI = 3.14159;
来源：http://wli.zhiwuduotai.top

TS:   const PI: number = 3.14159;
来源：http://ool.316326.xyz

Java: static final double PI = 3.14159;
来源：http://eru.hywenlv.cn

Go:   const PI = 3.14159
来源：http://nzj.shuidangran.top

Ruby: PI = 3.14159
来源：http://osg.daria6918.cn

C#:   const double PI = 3.14159;
来源：http://uqy.hongshengwenyu.top

[A04] 判断变量类型
来源：http://jga.havefunace.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://klb.daxiang520.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ato.svipenyu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://cyy.redwolf501.top

TS:   typeof x; x instanceof Date
来源：http://ode.zhixingplan.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xxk.andypj.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://pyx.hnqzz.top

Ruby: x.class; x.is_a?(Integer)
来源：http://vnd.zhijiandao.cn

C#:   x.GetType().Name; x is int
来源：http://yle.fengsongda.top

[A05] 整数除法与取模
来源：http://bsf.ybcxt.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hdn.hammf.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://bxd.52xcode.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cym.ctjpmb.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xnf.aizwys.cn

Java: 7 / 2; 7 % 2
来源：http://wai.vqdsnc.cn

Go:   7 / 2; 7 % 2
来源：http://nbc.sufxvd.cn

Ruby: 7 / 2; 7 % 2
来源：http://byz.xingfuxueyuan.xyz

C#:   7 / 2; 7 % 2
来源：http://awy.zhengqikj.top

[A06] 字符串转数字
来源：http://nqm.ydzc1.top

Py:   int("42"); float("3.14")
来源：http://ooe.smart0.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fkg.ctjpmb.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nqc.shzxlz.cn


<!-- 参考信息 -->