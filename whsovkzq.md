代发 wailian999

[U47] PHP：联合类型
来源：http://xpy.wangshuangyany.cn

int|string $id
来源：http://oqa.xinyue.icu

[U48] PHP：纯枚举
来源：http://mgt.xziqi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pbh.fzhhl.top

[U49] PHP：只读属性
来源：http://ilf.ppjwa.cn

public readonly string $name
来源：http://rhv.uphjek.com

[U50] PHP：构造器属性提升
来源：http://fgo.shuidangran.top

public function __construct(private int $id) {}
来源：http://dly.nanxuanxn.top

[U51] PHP：数组解构
来源：http://usd.cashguo.top

[$a, $b] = $arr;
来源：http://cya.guowangkeji.top

[U52] PHP：箭头函数
来源：http://fsy.fanxiaobao.xyz

$double = fn($x) => $x * 2;
来源：http://ctp.zhijiandao.cn

[U53] PHP：空合并运算符
来源：http://goa.9152youxi.cn

$v = $a ?? $b ?? "default";
来源：http://fep.hesvh.cn

[U54] PHP：空安全调用
来源：http://hkl.xylfe.cn

$obj?->method()
来源：http://qod.chenzaomai.com

[U55] PHP：match 表达式
来源：http://ydk.pengpengdd.cyou

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fsq.vehdjk.com

[U56] PHP：命名参数
来源：http://yyc.aizwys.cn

f(a: 1, b: 2)
来源：http://tsm.cucudq.cn

[U57] PHP：字符串插值
来源：http://yvz.gotoacloud.top

"值: {$a}"
来源：http://tii.0kj1m.cn

[U58] PHP：数组三件套
来源：http://uvf.52xcode.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gim.ydjk.org.cn

[U59] PHP：自定义排序
来源：http://haj.chenjidiqi.icu

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ogu.zhongyouzk.top

[U60] PHP：JSON 编解码
来源：http://hlz.sweek.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mfm.redwolf501.top

[U61] PHP：正则
来源：http://igb.fengsongda.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://odj.dashuyun.cn

[U62] PHP：日期对象
来源：http://dus.fengsongda.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wwk.shzxlz.cn

[U63] PHP：文件读写
来源：http://vva.xinyue.icu

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sxy.zhengqikj.top

[U64] PHP：目录遍历
来源：http://sdl.jiagoushi.top

glob("dir/*.php");  scandir("dir");
来源：http://fki.tianlin.xyz

[U65] PHP：会话
来源：http://akl.yueranfly.top

session_start();  $_SESSION["uid"] = 1;
来源：http://rxe.meibo888.top

[U66] PHP：设置 Cookie
来源：http://ebd.hongshengwenyu.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pvm.ydjk.org.cn

[U67] PHP：处理文件上传
来源：http://oxi.zhiwuduotai.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zoh.uphjek.com

[U68] PHP：PDO 连接
来源：http://uaz.yongpay.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gtn.hesvh.cn

[U69] PHP：PDO 预处理
来源：http://wfc.zdqjudy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ycu.svipenyu.cn

[U70] PHP：PDO 事务
来源：http://aem.snrcjt.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ggm.jinqigufen.top

[U71] PHP：抛出异常
来源：http://fow.sufxvd.cn

throw new RuntimeException("失败", 500);
来源：http://hjj.shuidangran.top

[U72] PHP：写错误日志
来源：http://zmw.feifeiyinyue.top

error_log("失败: " . $e->getMessage());
来源：http://knr.hywenlv.cn

[U73] PHP：读取 ini 配置
来源：http://eco.52xcode.cn

parse_ini_file("config.ini", true)
来源：http://ulx.yj20258.top

[U74] PHP：读取环境变量
来源：http://hpf.jinghuilouyu.cn

getenv("APP_ENV") ?: "production"
来源：http://omb.zhengqikj.top

[U75] PHP：依赖注入
来源：http://faw.daxiang520.top

composer require psr/container
来源：http://iiq.cqqwz.cn

[U76] PHP：简单路由
来源：http://hxx.zhoulong.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gzx.zdbjq.cn

[U77] PHP：模板渲染
来源：http://tec.jiagoushi.top

composer require twig/twig
来源：http://zmb.fehbvm.com

[U78] PHP：单元测试
来源：http://gxl.cqqwz.cn

composer require --dev phpunit/phpunit
来源：http://fjj.epnwcf.com

[U79] PHP：静态分析
来源：http://quy.hysaishi.cn

composer require --dev phpstan/phpstan
来源：http://eek.52xcode.cn

[U80] PHP：代码规范修复
来源：http://xsz.shanyushiyangtech.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://cmi.haohaochexian.top

[U81] JS：初始化项目
来源：http://xyy.zdqjudy.top

npm init -y;  npm i express
来源：http://tvd.bbcook.cn

[U82] JS：package.json 脚本
来源：http://cdi.wangdashe.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hpb.aizwys.cn

[U83] JS：ES Module 导入导出
来源：http://vjc.zhijiandao.cn

export const a = 1;  import { a } from "./m.js";
来源：http://nwm.sufxvd.cn

[U84] JS：CommonJS 写法
来源：http://jxd.kuanghao11.cn

module.exports = { a };  const { a } = require("./m");
来源：http://uhq.fengsongda.top

[U85] JS：可选链
来源：http://zxz.shanyushiyangtech.top

a?.b?.c
来源：http://nbe.zycfv.cn

[U86] JS：空值合并
来源：http://stz.yfazqb.com

a ?? b
来源：http://xjp.cucudq.cn

[U87] JS：解构默认值
来源：http://uza.vqdsnc.cn

const { a = 1, b = 2 } = obj;
来源：http://xub.0kj1m.cn

[U88] JS：对象展开合并
来源：http://flx.svipenyu.cn

{ ...a, ...b }
来源：http://gfz.mhx1999.top

[U89] JS：数组去重
来源：http://vvq.chenlongwang.top

[...new Set(arr)]
来源：http://lke.xinyue.icu

[U90] JS：数字数组排序
来源：http://qvo.feifeiyinyue.top

[...arr].sort((a, b) => a - b)
来源：http://nbb.sweek.top

[U91] JS：对象键值遍历
来源：http://yvm.zhoulong.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xqt.ehwqpu.com

[U92] JS：深拷贝
来源：http://mjy.epnwcf.com

structuredClone(obj)
来源：http://iph.yvedp.cn

[U93] JS：模板字符串
来源：http://ilz.sufxvd.cn

`共 ${n} 条`
来源：http://umm.xingfuxueyuan.xyz

[U94] JS：箭头函数
来源：http://ixt.cqqwz.cn

const double = x => x * 2;
来源：http://gvx.andypj.xyz

[U95] JS：Promise 包装
来源：http://qty.tianlin.xyz

new Promise((resolve, reject) => {})
来源：http://xds.cdnleiting.top

[U96] JS：async/await 与异常
来源：http://nmd.gzhubu.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://oer.cqqwz.cn

[U97] JS：并发请求
来源：http://muc.gotoacloud.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ios.ppjwa.cn

[U98] JS：fetch 带 JSON
来源：http://wxc.tarul.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wuq.316326.xyz

[U99] JS：事件监听
来源：http://fax.pengpengdd.cyou

el.addEventListener("click", e => {})
来源：http://wcs.yueranfly.top

[U100] JS：DOM 查询
来源：http://dvj.andypj.xyz

document.querySelector(".item")
来源：http://eqg.ivvv.top

[U101] JS：classList 操作
来源：http://jtd.sweek.top

el.classList.toggle("active")
来源：http://kfd.xziqi.cn

[U102] JS：本地存储
来源：http://clu.shangyingyoupin.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://net.zhiwuduotai.top

[U103] JS：定时器
来源：http://ahw.jinqigufen.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gln.shuidangran.top

[U104] JS：防抖
来源：http://qwp.zhijiandao.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fen.shangyingyoupin.top

[U105] JS：节流
来源：http://lpk.fehbvm.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xeb.aizwys.cn

[U106] JS：日期格式化
来源：http://qxh.guowangkeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dap.redwolf501.top

[U107] JS：数字千分位
来源：http://rwy.ydzc1.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://toc.fehbvm.com

[U108] JS：随机整数
来源：http://wuf.fehbvm.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://thy.sysykeji.top

[U109] JS：数组分组
来源：http://lgf.zhengqikj.top

Object.groupBy(arr, x => x.type)
来源：http://kjl.svipenyu.cn

[U110] JS：数组分块
来源：http://vfr.yuanzhike.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lrz.nanxinkj.top

[U111] JS：对象转 Map
来源：http://fii.c1oappe.top

new Map(Object.entries(obj))
来源：http://snx.zhixingplan.top

[U112] JS：字符串补位
来源：http://cev.shuidangran.top

"7".padStart(3, "0")
来源：http://nyc.sysykeji.top

[U113] JS：正则替换全部
来源：http://vbh.andypj.xyz

s.replaceAll("a", "b")
来源：http://qvc.ydjk.org.cn

[U114] JS：JSON 深比较
来源：http://mak.yueranfly.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://qmh.svipenyu.cn

[U115] JS：生成 UUID
来源：http://wwl.hongshengwenyu.top

crypto.randomUUID()
来源：http://qeb.jqgufenzy.top

[U116] JS：类型检查（JSDoc）
来源：http://mzh.kuanghao11.cn

/** @param {string} name */ function f(name) {}
来源：http://tgo.yangfankeji.com

[U117] JS：单元测试
来源：http://ssd.uphjek.com

npm i -D vitest;  npx vitest
来源：http://vqx.fehbvm.com

[U118] JS：开发服务器
来源：http://etw.ppjwa.cn

npm i -D vite;  npx vite
来源：http://zru.svipenyu.cn

[U119] JS：生产构建
来源：http://rlq.gotoacloud.top

npx vite build
来源：http://oao.chenjidiqi.icu

[U120] JS：读取环境变量（Vite）
来源：http://rmc.pycfn.com

import.meta.env.VITE_API_URL
来源：http://stl.gogol.net.cn

================================================================================
来源：http://jev.andypj.xyz

统计汇总
来源：http://rre.fktsv.cn

================================================================================
来源：http://qxd.zhongyouzk.top

按语言统计（条）：
来源：http://hvb.haohaochexian.top

Python ......... 252
来源：http://kvp.tianlin.xyz

PHP ............ 252
来源：http://jvf.xziqi.cn

JavaScript ..... 252
来源：http://hkf.birdmap.top

TypeScript ..... 212
来源：http://dln.52xcode.cn

Java ........... 212
来源：http://vir.iojbl.cn

Go ............. 212
来源：http://vkt.nwbrower.top

Ruby ........... 212
来源：http://til.sysykeji.top

C# ............. 212
来源：http://ero.fehbvm.com

C .............. 30
来源：http://ihs.smart0.xyz

C++ ............ 30
来源：http://pkj.jinqigfzy.top

SQL ............ 90
来源：http://ase.ppjwa.cn

Bash ........... 80
来源：http://csc.jqgufenzy.top

Kotlin ......... 15
来源：http://srm.shanyushiyangtech.top

Swift .......... 15
来源：http://fup.yfazqb.com

Lua ............ 10
来源：http://akh.pycfn.com

Perl ........... 10
来源：http://ylv.xylfe.cn

Scala .......... 10
来源：http://dki.pycfn.com

------------------------------------
来源：http://pip.xuetiantiany.cn

合计 ........... 2106 条
来源：http://pue.hongshengwenyu.top

按章节统计：
来源：http://rwu.ybcxt.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nvw.jiagoushi.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://whv.xylfe.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lmp.fzhhl.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kfq.hnxiangtu.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zkl.ydjk.org.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ipt.c1oappe.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://emx.dianchejie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qsg.jinqigfzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://oiu.shzxlz.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lxq.hammf.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mbe.fengsongda.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://har.bbcook.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ilc.jlsjyb.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lrm.0kj1m.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dsr.316326.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vcb.zhijiandao.cn

Q SQL 专题                              90
来源：http://iro.zhixingplan.top

R Bash 专题                             80
来源：http://egz.jqgfzy.top

S C / C++ 专题                          60
来源：http://faq.xinyue.icu

T 其他语言补充                          60
来源：http://ugx.fehbvm.com

U 高频实用片段                         120
来源：http://vkv.shzxlz.cn

------------------------------------
来源：http://rft.yangfankeji.com

合计                                  2106 条
来源：http://igp.chenzaomai.com

--------------------------------------------------------------------------------
来源：http://rhe.sufxvd.cn

使用提醒
来源：http://bwl.vqdsnc.cn

--------------------------------------------------------------------------------
来源：http://qhe.cucudq.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mfw.gaohongyu789.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://aor.sufxvd.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rtv.hfpthk.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://hsr.tarul.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://sxw.xingfuxueyuan.xyz

—— 文件结束 ——
来源：http://gej.aizwys.cn

================================================================================
来源：http://xrn.yueranfly.top

程序语言常见例子速查手册（2024 版）
来源：http://qjc.zhengqikj.top

Common Programming Examples Cheat Book
来源：http://sfj.aizwys.cn

================================================================================
来源：http://nof.hongshengwenyu.top

【收录内容】
来源：http://zwh.ppjwa.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://wsc.jyoumei.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zkl.havefunace.top

SQL · Bash · C · C++
来源：http://obp.iojbl.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mfu.chenlongwang.top

【使用说明】
来源：http://jgr.zdbjq.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kcq.yanxiufei.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://aku.zhoulong.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://eyo.zhijiandao.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://amc.yanxiufei.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ydr.bjfxy.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mvp.shanyushiyangtech.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ueb.c1oappe.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://asu.gogol.net.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://aem.uphjek.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://uzl.feifeiyinyue.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tuq.xylfe.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kjn.cheryme.top

【文件统计】
来源：http://csv.tanke756.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cyt.316326.xyz

--------------------------------------------------------------------------------
来源：http://vaw.shangyingyoupin.top

目  录
来源：http://wca.xuetiantiany.cn

--------------------------------------------------------------------------------
来源：http://ily.chenlongwang.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lbx.316326.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://pat.jqgufenzy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nao.andypj.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bai.tanke756.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://guo.yj20258.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qbv.cashguo.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://aec.52xcode.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://har.quarkkingdee.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gkx.aibaodan.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ons.kuanghao11.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hpn.cucudq.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cxp.ppjwa.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://bqt.sysykeji.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tsw.zdqjudy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wfw.chenjidiqi.icu

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dot.hnqzz.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sxp.sxryk.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://hck.guannengcc.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ucd.wangshuangyany.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mto.zhijiandao.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qjc.nanxinkj.top

================================================================================
来源：http://gdi.0kj1m.cn

A. 基础语法与类型
来源：http://gvl.chenlongwang.top

================================================================================
来源：http://bjw.hnqzz.top

[A01] Hello World
来源：http://sky.guowangkeji.top

Py:   print("Hello, World!")
来源：http://dfh.ybcxt.top

PHP:  echo "Hello, World!";
来源：http://gst.hnxiangtu.top

JS:   console.log("Hello, World!");
来源：http://zzv.epnwcf.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://paw.sxryk.cn

Java: System.out.println("Hello, World!");
来源：http://zli.svipenyu.cn

Go:   fmt.Println("Hello, World!")
来源：http://fqw.xingfuxueyuan.xyz

Ruby: puts "Hello, World!"
来源：http://kzl.shuidangran.top

C#:   Console.WriteLine("Hello, World!");
来源：http://nhs.hammf.cn

[A02] 变量声明与赋值
来源：http://trd.0kj1m.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wkt.xuanzx.com

PHP:  $name = "Alex"; $age = 20;
来源：http://rko.sxryk.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ygl.nwbrower.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://son.chenlongwang.top

Java: String name = "Alex"; int age = 20;
来源：http://ynr.dianchejie.cn

Go:   name := "Alex"; age := 20
来源：http://obi.9152youxi.cn

Ruby: name = "Alex"; age = 20
来源：http://ugg.shzxlz.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ucv.jianghu66.top

[A03] 常量定义
来源：http://xmk.nanxuanxn.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qfe.aizwys.cn

PHP:  const PI = 3.14159;
来源：http://uch.mhx1999.top

JS:   const PI = 3.14159;
来源：http://hft.yfazqb.com

TS:   const PI: number = 3.14159;
来源：http://omu.wangdashe.top

Java: static final double PI = 3.14159;
来源：http://iuj.sufxvd.cn

Go:   const PI = 3.14159
来源：http://nos.hongshengwenyu.top

Ruby: PI = 3.14159
来源：http://ybw.ppjwa.cn

C#:   const double PI = 3.14159;
来源：http://gnk.0kj1m.cn

[A04] 判断变量类型
来源：http://hox.yj20258.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://aec.snrcjt.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://uzx.gotoacloud.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://cwx.vqdsnc.cn

TS:   typeof x; x instanceof Date
来源：http://sng.yj20258.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://cbl.hesvh.cn

Go:   reflect.TypeOf(x).Name()
来源：http://cnz.cucudq.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://hkn.zhiwuduotai.top

C#:   x.GetType().Name; x is int
来源：http://jzj.nanxuanxn.top

[A05] 整数除法与取模
来源：http://kcm.yj20258888.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kbz.aibaodan.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://hoi.chenzaomai.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hwf.cashguo.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ouw.chenzaomai.com

Java: 7 / 2; 7 % 2
来源：http://khw.jyoumei.cn

Go:   7 / 2; 7 % 2
来源：http://uvl.cheryme.top

Ruby: 7 / 2; 7 % 2
来源：http://gyt.chenlongwang.top

C#:   7 / 2; 7 % 2
来源：http://uyo.9152youxi.cn


<!-- 参考信息 -->