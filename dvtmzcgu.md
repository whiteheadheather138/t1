代发 wailian999

[U49] PHP：只读属性
来源：http://lns.chenzaomai.com

public readonly string $name
来源：http://sde.svipenyu.cn

[U50] PHP：构造器属性提升
来源：http://avb.jinqigfzy.top

public function __construct(private int $id) {}
来源：http://uqy.shanyushiyangkeji.top

[U51] PHP：数组解构
来源：http://vay.jinyuanbaomall.cn

[$a, $b] = $arr;
来源：http://apb.fzhhl.top

[U52] PHP：箭头函数
来源：http://yci.epnwcf.com

$double = fn($x) => $x * 2;
来源：http://daz.yj20258.top

[U53] PHP：空合并运算符
来源：http://bcn.gogol.net.cn

$v = $a ?? $b ?? "default";
来源：http://cnx.svipenyu.cn

[U54] PHP：空安全调用
来源：http://jlc.c1oappe.top

$obj?->method()
来源：http://ppo.xuanzx.com

[U55] PHP：match 表达式
来源：http://tld.cheryme.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uuz.cdnleiting.top

[U56] PHP：命名参数
来源：http://ite.tarul.cn

f(a: 1, b: 2)
来源：http://yoz.guannengcc.top

[U57] PHP：字符串插值
来源：http://jcr.jyoumei.cn

"值: {$a}"
来源：http://suw.vehdjk.com

[U58] PHP：数组三件套
来源：http://ugh.9152youxi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fbq.yj20258888.top

[U59] PHP：自定义排序
来源：http://ngh.shuidangran.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xyy.ybcxt.top

[U60] PHP：JSON 编解码
来源：http://qvj.zhoulong.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hna.kuanghao11.cn

[U61] PHP：正则
来源：http://stn.nanxinkj.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rtt.ctjpmb.com

[U62] PHP：日期对象
来源：http://nnz.gotoacloud.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hnr.yongpay.top

[U63] PHP：文件读写
来源：http://lrl.sxryk.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://doq.hnqzz.top

[U64] PHP：目录遍历
来源：http://hwk.daria6918.cn

glob("dir/*.php");  scandir("dir");
来源：http://rvd.chenlongwang.top

[U65] PHP：会话
来源：http://ebr.aizwys.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://aiz.smart0.xyz

[U66] PHP：设置 Cookie
来源：http://djt.hcnkem.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://frk.xingfuxueyuan.xyz

[U67] PHP：处理文件上传
来源：http://wlz.meibo888.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cia.tanke756.top

[U68] PHP：PDO 连接
来源：http://lpm.snrcjt.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zot.fehbvm.com

[U69] PHP：PDO 预处理
来源：http://twg.hongshengwenyu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hbg.gotoacloud.top

[U70] PHP：PDO 事务
来源：http://als.yonumen.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mwg.yangfankeji.com

[U71] PHP：抛出异常
来源：http://vsz.shanyushiyangkeji.top

throw new RuntimeException("失败", 500);
来源：http://kme.wangshuangyany.cn

[U72] PHP：写错误日志
来源：http://ouv.bbcook.cn

error_log("失败: " . $e->getMessage());
来源：http://xkk.tian-w.cn

[U73] PHP：读取 ini 配置
来源：http://exr.ivvv.top

parse_ini_file("config.ini", true)
来源：http://laq.ppjwa.cn

[U74] PHP：读取环境变量
来源：http://ove.ybcxt.top

getenv("APP_ENV") ?: "production"
来源：http://rte.9152youxi.cn

[U75] PHP：依赖注入
来源：http://gse.sysykeji.top

composer require psr/container
来源：http://wnf.ctjpmb.com

[U76] PHP：简单路由
来源：http://wfi.yfazqb.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://otc.jyoumei.cn

[U77] PHP：模板渲染
来源：http://awg.zycfv.cn

composer require twig/twig
来源：http://hxr.zdqjudy.top

[U78] PHP：单元测试
来源：http://fye.ydjk.org.cn

composer require --dev phpunit/phpunit
来源：http://jud.xinyue.icu

[U79] PHP：静态分析
来源：http://niq.xylfe.cn

composer require --dev phpstan/phpstan
来源：http://mfk.zhongyouzk.top

[U80] PHP：代码规范修复
来源：http://gta.0kj1m.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://isr.bjfxy.top

[U81] JS：初始化项目
来源：http://egv.zhixingplan.top

npm init -y;  npm i express
来源：http://tof.fanxiaobao.xyz

[U82] JS：package.json 脚本
来源：http://kho.tian-w.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nmq.xylfe.cn

[U83] JS：ES Module 导入导出
来源：http://ymj.daria6918.cn

export const a = 1;  import { a } from "./m.js";
来源：http://odl.zycfv.cn

[U84] JS：CommonJS 写法
来源：http://ssn.shanyushiyangkeji.top

module.exports = { a };  const { a } = require("./m");
来源：http://khd.xinyue.icu

[U85] JS：可选链
来源：http://fmd.wangshuangyany.cn

a?.b?.c
来源：http://qmd.cheryme.top

[U86] JS：空值合并
来源：http://tsr.gotoacloud.top

a ?? b
来源：http://aum.redwolf501.top

[U87] JS：解构默认值
来源：http://uvm.jinqigfzy.top

const { a = 1, b = 2 } = obj;
来源：http://pwq.ydzc1.top

[U88] JS：对象展开合并
来源：http://fza.cqqwz.cn

{ ...a, ...b }
来源：http://nke.guowangkeji.top

[U89] JS：数组去重
来源：http://jia.nwbrower.top

[...new Set(arr)]
来源：http://hwf.iojbl.cn

[U90] JS：数字数组排序
来源：http://phg.haohaochexian.top

[...arr].sort((a, b) => a - b)
来源：http://kvi.snrcjt.cn

[U91] JS：对象键值遍历
来源：http://utg.tianlin.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hts.gzhubu.top

[U92] JS：深拷贝
来源：http://dau.zhiwuduotai.top

structuredClone(obj)
来源：http://xzy.chenlongwang.top

[U93] JS：模板字符串
来源：http://wvi.tanke756.top

`共 ${n} 条`
来源：http://nxs.vqdsnc.cn

[U94] JS：箭头函数
来源：http://fmp.zycfv.cn

const double = x => x * 2;
来源：http://tej.yj20258888.top

[U95] JS：Promise 包装
来源：http://wiy.yj202588.top

new Promise((resolve, reject) => {})
来源：http://ogg.sweek.top

[U96] JS：async/await 与异常
来源：http://kgc.yfazqb.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://crm.fanxiaobao.xyz

[U97] JS：并发请求
来源：http://czg.shanyushiyangtech.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://bkb.ydzc1.top

[U98] JS：fetch 带 JSON
来源：http://aze.birdmap.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jnv.cdnleiting.top

[U99] JS：事件监听
来源：http://qjd.birdmap.top

el.addEventListener("click", e => {})
来源：http://bfp.zhixingplan.top

[U100] JS：DOM 查询
来源：http://kbl.yj202588.top

document.querySelector(".item")
来源：http://lwf.jyoumei.cn

[U101] JS：classList 操作
来源：http://xic.epnwcf.com

el.classList.toggle("active")
来源：http://zdj.0kj1m.cn

[U102] JS：本地存储
来源：http://zyu.ywan-chungtsiang.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://xkj.hesvh.cn

[U103] JS：定时器
来源：http://nxl.yfazqb.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gfz.jyoumei.cn

[U104] JS：防抖
来源：http://lkx.quarkkingdee.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qdm.shuidangran.top

[U105] JS：节流
来源：http://uic.xylfe.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lwi.zhongyouzk.top

[U106] JS：日期格式化
来源：http://rms.jqgfzy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ewp.ywan-chungtsiang.top

[U107] JS：数字千分位
来源：http://orc.cdnleiting.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rbs.hysaishi.cn

[U108] JS：随机整数
来源：http://nyq.cucudq.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fxm.fengsongda.top

[U109] JS：数组分组
来源：http://vfn.jqgufenzy.top

Object.groupBy(arr, x => x.type)
来源：http://lvp.feifeiyinyue.top

[U110] JS：数组分块
来源：http://rol.ydzc1.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gvh.52xcode.cn

[U111] JS：对象转 Map
来源：http://cyo.xinyue.icu

new Map(Object.entries(obj))
来源：http://usv.jianghu66.top

[U112] JS：字符串补位
来源：http://hfm.cucudq.cn

"7".padStart(3, "0")
来源：http://tca.cucudq.cn

[U113] JS：正则替换全部
来源：http://wdw.shzxlz.cn

s.replaceAll("a", "b")
来源：http://zdu.gogol.net.cn

[U114] JS：JSON 深比较
来源：http://wzt.zhixingplan.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://hcj.jqgfzy.top

[U115] JS：生成 UUID
来源：http://tyb.cashguo.top

crypto.randomUUID()
来源：http://mzg.wangdashe.top

[U116] JS：类型检查（JSDoc）
来源：http://plh.nanxuanxn.top

/** @param {string} name */ function f(name) {}
来源：http://wac.yueranfly.top

[U117] JS：单元测试
来源：http://zbn.fanxiaobao.xyz

npm i -D vitest;  npx vitest
来源：http://app.andypj.xyz

[U118] JS：开发服务器
来源：http://vhb.haohaochexian.top

npm i -D vite;  npx vite
来源：http://ugp.tanke756.top

[U119] JS：生产构建
来源：http://wvh.zhoulong.xyz

npx vite build
来源：http://idk.chenjidiqi.icu

[U120] JS：读取环境变量（Vite）
来源：http://qlo.dashuyun.cn

import.meta.env.VITE_API_URL
来源：http://pjy.chenlongwang.top

================================================================================
来源：http://ufy.vqdsnc.cn

统计汇总
来源：http://cmb.hcnkem.com

================================================================================
来源：http://nhj.sjlbkw.cn

按语言统计（条）：
来源：http://xsa.guowangkeji.top

Python ......... 252
来源：http://idl.bbcook.cn

PHP ............ 252
来源：http://nxo.guannengcc.top

JavaScript ..... 252
来源：http://gfd.chenlongwang.top

TypeScript ..... 212
来源：http://lgv.jinqigfzy.top

Java ........... 212
来源：http://ihf.fehbvm.com

Go ............. 212
来源：http://nms.chenzaomai.com

Ruby ........... 212
来源：http://rqw.jqgufenzy.top

C# ............. 212
来源：http://qlg.quarkkingdee.top

C .............. 30
来源：http://gnb.0kj1m.cn

C++ ............ 30
来源：http://btz.ybcxt.top

SQL ............ 90
来源：http://jql.dianchejie.cn

Bash ........... 80
来源：http://cda.tanke756.top

Kotlin ......... 15
来源：http://jbf.wangdashe.top

Swift .......... 15
来源：http://etp.xuanzx.com

Lua ............ 10
来源：http://bbe.daria6918.cn

Perl ........... 10
来源：http://yys.smart0.xyz

Scala .......... 10
来源：http://fgs.shzxlz.cn

------------------------------------
来源：http://lqx.gogol.net.cn

合计 ........... 2106 条
来源：http://rui.316326.xyz

按章节统计：
来源：http://gib.chenjidiqi.icu

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://glc.yj20258.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mko.yueranfly.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ntd.chenzaomai.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kir.hysaishi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dkg.vehdjk.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sga.vqdsnc.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ktx.zhaomingkeji.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gpo.aibaodan.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://oed.zhengqikj.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qnj.xinyue.icu

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://iab.wangshuangyany.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mqc.ywan-chungtsiang.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ptv.hcnkem.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rpb.fktsv.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://uke.ppjwa.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ppx.daxiang520.top

Q SQL 专题                              90
来源：http://meg.shangyingyoupin.top

R Bash 专题                             80
来源：http://nxm.cdnleiting.top

S C / C++ 专题                          60
来源：http://xvp.jlsjyb.cn

T 其他语言补充                          60
来源：http://fye.cdnleiting.top

U 高频实用片段                         120
来源：http://wob.yuxming.cn

------------------------------------
来源：http://wrn.havefunace.top

合计                                  2106 条
来源：http://ntn.uphjek.com

--------------------------------------------------------------------------------
来源：http://srb.chenzaomai.com

使用提醒
来源：http://qty.yuanzhike.top

--------------------------------------------------------------------------------
来源：http://zzi.nanxuanxn.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://oxy.fktsv.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xtx.zhoulong.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://sqk.xinyue.icu

在旧版本上使用前请先确认语法支持情况。
来源：http://hrm.vehdjk.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wwn.fktsv.cn

—— 文件结束 ——
来源：http://tji.cashguo.top

================================================================================
来源：http://vdv.fzhhl.top

程序语言常见例子速查手册（2024 版）
来源：http://wwi.nanxinkj.top

Common Programming Examples Cheat Book
来源：http://thk.bbcook.cn

================================================================================
来源：http://cxt.cdnleiting.top

【收录内容】
来源：http://rej.ydjk.org.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://zju.yj202588.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vif.vehdjk.com

SQL · Bash · C · C++
来源：http://vky.tarul.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kou.gotoacloud.top

【使用说明】
来源：http://mag.vqdsnc.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ogr.yueranfly.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mvu.fktsv.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jla.ydjk.org.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://pqx.tanke756.top

Bash:  Shell         C:     C             C++:   C++
来源：http://gia.xinyue.icu

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dvw.zhoulong.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://sip.shanyushiyangkeji.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lmu.wangdashe.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ctg.yj20258888.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://kgq.ehwqpu.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://evb.dianchejie.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://elp.ppjwa.cn

【文件统计】
来源：http://dsu.hongshengwenyu.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cni.jyoumei.cn

--------------------------------------------------------------------------------
来源：http://lrs.chenzaomai.com

目  录
来源：http://ftc.jqgufenzy.top

--------------------------------------------------------------------------------
来源：http://dih.316326.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rbr.chenlongwang.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://csl.xuanzx.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://lki.jinyuanbaomall.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qik.jinqigfzy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://pyf.wangshuangyany.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zkn.zhoulong.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qki.zhiwuduotai.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://sny.shanyushiyangtech.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jhe.quarkkingdee.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cmq.jinqigfzy.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nxm.hfpthk.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ick.havefunace.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hvs.jqgufenzy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mxt.yuxming.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://tvm.ywan-chungtsiang.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://uqp.zdqjudy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wdo.hesvh.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://obo.yvedp.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://iot.nwbrower.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://koy.zdqjudy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pzs.hongshengwenyu.top

================================================================================
来源：http://vqx.c1oappe.top

A. 基础语法与类型
来源：http://nej.jlsjyb.cn

================================================================================
来源：http://oop.vehdjk.com

[A01] Hello World
来源：http://txp.ybcxt.top

Py:   print("Hello, World!")
来源：http://niz.uphjek.com

PHP:  echo "Hello, World!";
来源：http://gui.hammf.cn

JS:   console.log("Hello, World!");
来源：http://poh.xuetiantiany.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cuz.9152youxi.cn

Java: System.out.println("Hello, World!");
来源：http://tiw.cheryme.top

Go:   fmt.Println("Hello, World!")
来源：http://pmh.dianchejie.cn

Ruby: puts "Hello, World!"
来源：http://lcz.jinqigfzy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://mvq.chenzaomai.com

[A02] 变量声明与赋值
来源：http://ufh.zhaomingkeji.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jlh.yfazqb.com

PHP:  $name = "Alex"; $age = 20;
来源：http://aqa.zhongyouzk.top

JS:   let name = "Alex"; const age = 20;
来源：http://myo.chenzaomai.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://erv.ydzc1.top

Java: String name = "Alex"; int age = 20;
来源：http://zmf.yanxiufei.cn

Go:   name := "Alex"; age := 20
来源：http://ryx.daria6918.cn

Ruby: name = "Alex"; age = 20
来源：http://mtn.yj20258.top

C#:   string name = "Alex"; int age = 20;
来源：http://epo.cdnleiting.top

[A03] 常量定义
来源：http://ycr.yfazqb.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tcj.chenzaomai.com

PHP:  const PI = 3.14159;
来源：http://jux.jiagoushi.top

JS:   const PI = 3.14159;
来源：http://ufo.snrcjt.cn

TS:   const PI: number = 3.14159;
来源：http://hzp.ywan-chungtsiang.top

Java: static final double PI = 3.14159;
来源：http://dvb.jinqigufen.top

Go:   const PI = 3.14159
来源：http://jwz.ybcxt.top

Ruby: PI = 3.14159
来源：http://zsa.snrcjt.cn

C#:   const double PI = 3.14159;
来源：http://fyg.hnqzz.top

[A04] 判断变量类型
来源：http://ifd.chenjidiqi.icu

Py:   type(x).__name__; isinstance(x, int)
来源：http://klm.cucudq.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jai.hfpthk.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://yfz.mhx1999.top

TS:   typeof x; x instanceof Date
来源：http://fzl.guowangkeji.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gfc.gaohongyu789.top

Go:   reflect.TypeOf(x).Name()
来源：http://tqr.gogol.net.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://dhk.fengsongda.top

C#:   x.GetType().Name; x is int
来源：http://fbu.cdnleiting.top

[A05] 整数除法与取模
来源：http://kpa.redwolf501.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mpj.guannengcc.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://qcf.ywan-chungtsiang.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jhk.tanke756.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ska.cashguo.top

Java: 7 / 2; 7 % 2
来源：http://xua.zhongyouzk.top

Go:   7 / 2; 7 % 2
来源：http://xev.gaohongyu789.top

Ruby: 7 / 2; 7 % 2
来源：http://rtm.smart0.xyz

C#:   7 / 2; 7 % 2
来源：http://pkp.yj202588.top

[A06] 字符串转数字
来源：http://hog.hnxiangtu.top

Py:   int("42"); float("3.14")
来源：http://mex.quarkkingdee.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ctv.aizwys.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hto.sxryk.cn


<!-- 参考信息 -->