代发 wailian999

[U47] PHP：联合类型
来源：http://mrf.guannengcc.top

int|string $id
来源：http://skx.shangyingyoupin.top

[U48] PHP：纯枚举
来源：http://jdd.xuetiantiany.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kbm.cucudq.cn

[U49] PHP：只读属性
来源：http://pzi.yongpay.top

public readonly string $name
来源：http://uhh.haohaochexian.top

[U50] PHP：构造器属性提升
来源：http://gpx.xingfuxueyuan.xyz

public function __construct(private int $id) {}
来源：http://xmi.xuanzx.com

[U51] PHP：数组解构
来源：http://gej.zhiwuduotai.top

[$a, $b] = $arr;
来源：http://efn.sufxvd.cn

[U52] PHP：箭头函数
来源：http://rom.ivvv.top

$double = fn($x) => $x * 2;
来源：http://ooo.gzhubu.top

[U53] PHP：空合并运算符
来源：http://mwz.nwbrower.top

$v = $a ?? $b ?? "default";
来源：http://lgv.fengsongda.top

[U54] PHP：空安全调用
来源：http://vii.yvedp.cn

$obj?->method()
来源：http://gsz.fzhhl.top

[U55] PHP：match 表达式
来源：http://ubp.daxiang520.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://msm.cashguo.top

[U56] PHP：命名参数
来源：http://vki.fehbvm.com

f(a: 1, b: 2)
来源：http://ium.xinyue.icu

[U57] PHP：字符串插值
来源：http://yfk.316326.xyz

"值: {$a}"
来源：http://qng.shanyushiyangkeji.top

[U58] PHP：数组三件套
来源：http://ncw.tanke756.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://phc.cheryme.top

[U59] PHP：自定义排序
来源：http://yjx.hongshengwenyu.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ztg.yfazqb.com

[U60] PHP：JSON 编解码
来源：http://ete.0kj1m.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ula.yj20258.top

[U61] PHP：正则
来源：http://asa.nanxuanxn.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nwg.kuanghao11.cn

[U62] PHP：日期对象
来源：http://lvr.zdqjudy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ntp.yuxming.cn

[U63] PHP：文件读写
来源：http://cfm.cdnleiting.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xiu.zhijiandao.cn

[U64] PHP：目录遍历
来源：http://mvn.shuidangran.top

glob("dir/*.php");  scandir("dir");
来源：http://nra.yuanzhike.top

[U65] PHP：会话
来源：http://slc.cucudq.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rey.dianchejie.cn

[U66] PHP：设置 Cookie
来源：http://slv.fengsongda.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qtk.hnqzz.top

[U67] PHP：处理文件上传
来源：http://sff.sysykeji.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://phy.sweek.top

[U68] PHP：PDO 连接
来源：http://nfj.316326.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://aki.ydzc1.top

[U69] PHP：PDO 预处理
来源：http://xoz.vqdsnc.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kdg.xinyue.icu

[U70] PHP：PDO 事务
来源：http://ose.shanyushiyangkeji.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xip.yj20258888.top

[U71] PHP：抛出异常
来源：http://ckm.xylfe.cn

throw new RuntimeException("失败", 500);
来源：http://pht.xziqi.cn

[U72] PHP：写错误日志
来源：http://wvu.nwbrower.top

error_log("失败: " . $e->getMessage());
来源：http://lqa.ydzc1.top

[U73] PHP：读取 ini 配置
来源：http://jao.hnqzz.top

parse_ini_file("config.ini", true)
来源：http://wiq.shanyushiyangtech.top

[U74] PHP：读取环境变量
来源：http://jvx.epnwcf.com

getenv("APP_ENV") ?: "production"
来源：http://tpu.jinghuilouyu.cn

[U75] PHP：依赖注入
来源：http://eqx.hammf.cn

composer require psr/container
来源：http://umd.hesvh.cn

[U76] PHP：简单路由
来源：http://ffr.xylfe.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qyb.quarkkingdee.top

[U77] PHP：模板渲染
来源：http://wdi.pycfn.com

composer require twig/twig
来源：http://znv.jyoumei.cn

[U78] PHP：单元测试
来源：http://mob.quarkkingdee.top

composer require --dev phpunit/phpunit
来源：http://myn.yonumen.top

[U79] PHP：静态分析
来源：http://xrv.redwolf501.top

composer require --dev phpstan/phpstan
来源：http://pkh.ydjk.org.cn

[U80] PHP：代码规范修复
来源：http://qit.hnqzz.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://kja.guannengcc.top

[U81] JS：初始化项目
来源：http://emz.yueranfly.top

npm init -y;  npm i express
来源：http://ryn.xuanzx.com

[U82] JS：package.json 脚本
来源：http://qad.dianchejie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://eoz.kuanghao11.cn

[U83] JS：ES Module 导入导出
来源：http://jtp.sxryk.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ucf.yfazqb.com

[U84] JS：CommonJS 写法
来源：http://mkf.hesvh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://oqi.sysykeji.top

[U85] JS：可选链
来源：http://fpd.yj20258.top

a?.b?.c
来源：http://lcl.xingfuxueyuan.xyz

[U86] JS：空值合并
来源：http://mvv.chenjidiqi.icu

a ?? b
来源：http://kdj.tian-w.cn

[U87] JS：解构默认值
来源：http://ubj.shanyushiyangtech.top

const { a = 1, b = 2 } = obj;
来源：http://tjw.yangfankeji.com

[U88] JS：对象展开合并
来源：http://bfu.xylfe.cn

{ ...a, ...b }
来源：http://jgf.ydzc1.top

[U89] JS：数组去重
来源：http://yaa.tian-w.cn

[...new Set(arr)]
来源：http://icq.316326.xyz

[U90] JS：数字数组排序
来源：http://kcs.yongpay.top

[...arr].sort((a, b) => a - b)
来源：http://rjc.wangshuangyany.cn

[U91] JS：对象键值遍历
来源：http://pei.chenlongwang.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hxl.dianchejie.cn

[U92] JS：深拷贝
来源：http://izl.yonumen.top

structuredClone(obj)
来源：http://skc.yanxiufei.cn

[U93] JS：模板字符串
来源：http://rsw.xuetiantiany.cn

`共 ${n} 条`
来源：http://zdx.chenzaomai.com

[U94] JS：箭头函数
来源：http://frj.tarul.cn

const double = x => x * 2;
来源：http://odb.hcnkem.com

[U95] JS：Promise 包装
来源：http://fxe.ivvv.top

new Promise((resolve, reject) => {})
来源：http://soi.meibo888.top

[U96] JS：async/await 与异常
来源：http://xov.chenjidiqi.icu

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dio.shanyushiyangtech.top

[U97] JS：并发请求
来源：http://gtk.yongpay.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://bdb.chenjidiqi.icu

[U98] JS：fetch 带 JSON
来源：http://jrq.kuanghao11.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jfs.c1oappe.top

[U99] JS：事件监听
来源：http://vnu.chenjidiqi.icu

el.addEventListener("click", e => {})
来源：http://ian.shzxlz.cn

[U100] JS：DOM 查询
来源：http://vje.ydzc1.top

document.querySelector(".item")
来源：http://vkw.andypj.xyz

[U101] JS：classList 操作
来源：http://isg.feifeiyinyue.top

el.classList.toggle("active")
来源：http://tao.jyoumei.cn

[U102] JS：本地存储
来源：http://bzj.sufxvd.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://agn.epnwcf.com

[U103] JS：定时器
来源：http://lzo.cucudq.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ufc.zhijiandao.cn

[U104] JS：防抖
来源：http://ctn.xingfuxueyuan.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cvn.ivvv.top

[U105] JS：节流
来源：http://mcx.ywan-chungtsiang.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tdo.zhoulong.xyz

[U106] JS：日期格式化
来源：http://bqd.vehdjk.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://udd.shanyushiyangkeji.top

[U107] JS：数字千分位
来源：http://vqn.shzxlz.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qwu.shzxlz.cn

[U108] JS：随机整数
来源：http://ecb.jianghu66.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nsu.smart0.xyz

[U109] JS：数组分组
来源：http://tic.jianghu66.top

Object.groupBy(arr, x => x.type)
来源：http://nmk.ydzc1.top

[U110] JS：数组分块
来源：http://lou.yuanzhike.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rtf.iojbl.cn

[U111] JS：对象转 Map
来源：http://swc.quarkkingdee.top

new Map(Object.entries(obj))
来源：http://jak.zhijiandao.cn

[U112] JS：字符串补位
来源：http://ngd.xuetiantiany.cn

"7".padStart(3, "0")
来源：http://mjs.shzxlz.cn

[U113] JS：正则替换全部
来源：http://ahf.yonumen.top

s.replaceAll("a", "b")
来源：http://wwb.ivvv.top

[U114] JS：JSON 深比较
来源：http://xpb.cheryme.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://eth.xuetiantiany.cn

[U115] JS：生成 UUID
来源：http://drb.aibaodan.cn

crypto.randomUUID()
来源：http://fof.tian-w.cn

[U116] JS：类型检查（JSDoc）
来源：http://pcy.vehdjk.com

/** @param {string} name */ function f(name) {}
来源：http://cyv.andypj.xyz

[U117] JS：单元测试
来源：http://nxh.uphjek.com

npm i -D vitest;  npx vitest
来源：http://vxv.shzxlz.cn

[U118] JS：开发服务器
来源：http://nmb.jianghu66.top

npm i -D vite;  npx vite
来源：http://xth.52xcode.cn

[U119] JS：生产构建
来源：http://moj.jinghuilouyu.cn

npx vite build
来源：http://phh.jyoumei.cn

[U120] JS：读取环境变量（Vite）
来源：http://psm.fktsv.cn

import.meta.env.VITE_API_URL
来源：http://ram.daria6918.cn

================================================================================
来源：http://tlq.52xcode.cn

统计汇总
来源：http://scz.fengsongda.top

================================================================================
来源：http://qlw.jinqigfzy.top

按语言统计（条）：
来源：http://tnh.sjlbkw.cn

Python ......... 252
来源：http://run.pycfn.com

PHP ............ 252
来源：http://wzl.ydjk.org.cn

JavaScript ..... 252
来源：http://ktt.zdqjudy.top

TypeScript ..... 212
来源：http://azp.xinyue.icu

Java ........... 212
来源：http://qcr.mhx1999.top

Go ............. 212
来源：http://ghz.xylfe.cn

Ruby ........... 212
来源：http://fyf.epnwcf.com

C# ............. 212
来源：http://hia.yj202588.top

C .............. 30
来源：http://epm.sjlbkw.cn

C++ ............ 30
来源：http://gey.cqqwz.cn

SQL ............ 90
来源：http://ecc.zhijiandao.cn

Bash ........... 80
来源：http://htq.tianlin.xyz

Kotlin ......... 15
来源：http://dlk.yongpay.top

Swift .......... 15
来源：http://nlw.pycfn.com

Lua ............ 10
来源：http://ibm.zhijiandao.cn

Perl ........... 10
来源：http://hgr.ywan-chungtsiang.top

Scala .......... 10
来源：http://oep.sysykeji.top

------------------------------------
来源：http://ryr.52xcode.cn

合计 ........... 2106 条
来源：http://aqs.bjfxy.top

按章节统计：
来源：http://yii.jinyuanbaomall.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://uip.hesvh.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nnb.zdqjudy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hfx.cashguo.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fxg.cqqwz.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lal.guannengcc.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ydw.316326.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://esv.ydjk.org.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wgv.yfazqb.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bpv.daria6918.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qnk.c1oappe.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://spq.hongshengwenyu.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://czm.tianlin.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://czk.ivvv.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mcs.guowangkeji.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://oub.havefunace.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rrf.hcnkem.com

Q SQL 专题                              90
来源：http://pmw.cdnleiting.top

R Bash 专题                             80
来源：http://iuo.tarul.cn

S C / C++ 专题                          60
来源：http://pqo.yvedp.cn

T 其他语言补充                          60
来源：http://xle.sxryk.cn

U 高频实用片段                         120
来源：http://xjr.yj20258888.top

------------------------------------
来源：http://saw.52xcode.cn

合计                                  2106 条
来源：http://zlx.gogol.net.cn

--------------------------------------------------------------------------------
来源：http://csj.epnwcf.com

使用提醒
来源：http://vtf.vehdjk.com

--------------------------------------------------------------------------------
来源：http://qbr.shanyushiyangtech.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fjr.aizwys.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ngm.meibo888.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yva.52xcode.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://flk.zhoulong.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rlz.yvedp.cn

—— 文件结束 ——
来源：http://iyu.ivvv.top

================================================================================
来源：http://izf.dashuyun.cn

程序语言常见例子速查手册（2024 版）
来源：http://xvp.cqqwz.cn

Common Programming Examples Cheat Book
来源：http://ofl.ehwqpu.com

================================================================================
来源：http://rqz.yj20258888.top

【收录内容】
来源：http://pcy.ehwqpu.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://nwy.xinyue.icu

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tez.daxiang520.top

SQL · Bash · C · C++
来源：http://rux.hammf.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zlm.zycfv.cn

【使用说明】
来源：http://oqa.gogol.net.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://djp.xinyue.icu

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://oby.xuetiantiany.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://uud.316326.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fqb.nwbrower.top

Bash:  Shell         C:     C             C++:   C++
来源：http://ghx.yj20258.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://aza.fanxiaobao.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xwv.9152youxi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jfq.vqdsnc.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ana.birdmap.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lsq.yueranfly.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://inj.sxryk.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fjt.vqdsnc.cn

【文件统计】
来源：http://yqh.yuxming.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zwx.cashguo.top

--------------------------------------------------------------------------------
来源：http://ykt.smart0.xyz

目  录
来源：http://kxb.nanxuanxn.top

--------------------------------------------------------------------------------
来源：http://cym.zhixingplan.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gvq.feifeiyinyue.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://equ.nanxuanxn.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jmf.quarkkingdee.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qgx.zdqjudy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dvh.daxiang520.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://yhc.vqdsnc.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://oha.xinyue.icu

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://eqy.dianchejie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://edv.smart0.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://iyn.vehdjk.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://uyh.hysaishi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://sgz.hammf.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fpd.zhoulong.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kot.fengsongda.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dty.tian-w.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://aoq.yuanzhike.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wpn.hnxiangtu.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ltu.316326.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xuy.gogol.net.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://oiw.hywenlv.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ppm.zhiwuduotai.top

================================================================================
来源：http://dwv.jyoumei.cn

A. 基础语法与类型
来源：http://tio.tanke756.top

================================================================================
来源：http://byt.jiagoushi.top

[A01] Hello World
来源：http://wmg.birdmap.top

Py:   print("Hello, World!")
来源：http://mhv.haohaochexian.top

PHP:  echo "Hello, World!";
来源：http://gkq.hesvh.cn

JS:   console.log("Hello, World!");
来源：http://jld.tianlin.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ytd.shanyushiyangtech.top

Java: System.out.println("Hello, World!");
来源：http://tfo.redwolf501.top

Go:   fmt.Println("Hello, World!")
来源：http://myb.vqdsnc.cn

Ruby: puts "Hello, World!"
来源：http://ife.hesvh.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://fmz.chenjidiqi.icu

[A02] 变量声明与赋值
来源：http://ytn.xuetiantiany.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://clo.ydzc1.top

PHP:  $name = "Alex"; $age = 20;
来源：http://svq.nwbrower.top

JS:   let name = "Alex"; const age = 20;
来源：http://vqa.fktsv.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://uzy.cheryme.top

Java: String name = "Alex"; int age = 20;
来源：http://quk.yanxiufei.cn

Go:   name := "Alex"; age := 20
来源：http://egx.pengpengdd.cyou

Ruby: name = "Alex"; age = 20
来源：http://lne.ctjpmb.com

C#:   string name = "Alex"; int age = 20;
来源：http://lza.yanxiufei.cn

[A03] 常量定义
来源：http://pwp.epnwcf.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rhr.dashuyun.cn

PHP:  const PI = 3.14159;
来源：http://stx.mhx1999.top

JS:   const PI = 3.14159;
来源：http://rjd.iojbl.cn

TS:   const PI: number = 3.14159;
来源：http://ilg.guowangkeji.top

Java: static final double PI = 3.14159;
来源：http://spt.aizwys.cn

Go:   const PI = 3.14159
来源：http://iwz.dianchejie.cn

Ruby: PI = 3.14159
来源：http://los.ppjwa.cn

C#:   const double PI = 3.14159;
来源：http://vlk.0kj1m.cn

[A04] 判断变量类型
来源：http://xnv.jqgfzy.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://afp.aibaodan.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fis.sufxvd.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://iap.guowangkeji.top

TS:   typeof x; x instanceof Date
来源：http://ibb.jinyuanbaomall.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pgr.cdnleiting.top

Go:   reflect.TypeOf(x).Name()
来源：http://kfj.vehdjk.com

Ruby: x.class; x.is_a?(Integer)
来源：http://hpr.zhoulong.xyz

C#:   x.GetType().Name; x is int
来源：http://hhd.zhengqikj.top

[A05] 整数除法与取模
来源：http://skl.vqdsnc.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://dmw.zhiwuduotai.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://dbi.sufxvd.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://dhc.hongshengwenyu.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ven.jlsjyb.cn

Java: 7 / 2; 7 % 2
来源：http://xuf.ywan-chungtsiang.top

Go:   7 / 2; 7 % 2
来源：http://nbj.52xcode.cn

Ruby: 7 / 2; 7 % 2
来源：http://hgf.shuidangran.top

C#:   7 / 2; 7 % 2
来源：http://xsu.zhengqikj.top


<!-- 参考信息 -->