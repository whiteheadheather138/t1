代发 wailian999

[U49] PHP：只读属性
来源：http://uld.dashuyun.cn

public readonly string $name
来源：http://ekt.jinqigufen.top

[U50] PHP：构造器属性提升
来源：http://ufn.wangshuangyany.cn

public function __construct(private int $id) {}
来源：http://mzs.daxiang520.top

[U51] PHP：数组解构
来源：http://pix.hongshengwenyu.top

[$a, $b] = $arr;
来源：http://grx.xziqi.cn

[U52] PHP：箭头函数
来源：http://dso.cdnleiting.top

$double = fn($x) => $x * 2;
来源：http://jnz.nwbrower.top

[U53] PHP：空合并运算符
来源：http://sno.sjlbkw.cn

$v = $a ?? $b ?? "default";
来源：http://htr.shzxlz.cn

[U54] PHP：空安全调用
来源：http://cpr.zhengqikj.top

$obj?->method()
来源：http://kzr.havefunace.top

[U55] PHP：match 表达式
来源：http://kun.xziqi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tgx.316326.xyz

[U56] PHP：命名参数
来源：http://uxw.yonumen.top

f(a: 1, b: 2)
来源：http://dfy.zhongyouzk.top

[U57] PHP：字符串插值
来源：http://xvh.9152youxi.cn

"值: {$a}"
来源：http://zjz.jyoumei.cn

[U58] PHP：数组三件套
来源：http://zhu.jinyuanbaomall.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ebo.fengsongda.top

[U59] PHP：自定义排序
来源：http://gmk.vehdjk.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qlt.wangshuangyany.cn

[U60] PHP：JSON 编解码
来源：http://paj.hfpthk.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pyr.birdmap.top

[U61] PHP：正则
来源：http://epc.zycfv.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vqy.ydjk.org.cn

[U62] PHP：日期对象
来源：http://azo.fengsongda.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bfd.hywenlv.cn

[U63] PHP：文件读写
来源：http://lmy.vqdsnc.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ilx.ehwqpu.com

[U64] PHP：目录遍历
来源：http://kae.vqdsnc.cn

glob("dir/*.php");  scandir("dir");
来源：http://wfa.jqgufenzy.top

[U65] PHP：会话
来源：http://xhb.xinyue.icu

session_start();  $_SESSION["uid"] = 1;
来源：http://swd.xuanzx.com

[U66] PHP：设置 Cookie
来源：http://djg.jinyuanbaomall.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kti.jlsjyb.cn

[U67] PHP：处理文件上传
来源：http://ojs.xziqi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ufp.snrcjt.cn

[U68] PHP：PDO 连接
来源：http://eys.tian-w.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://omu.0kj1m.cn

[U69] PHP：PDO 预处理
来源：http://con.pycfn.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://esj.dashuyun.cn

[U70] PHP：PDO 事务
来源：http://sqd.cashguo.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mbo.birdmap.top

[U71] PHP：抛出异常
来源：http://sep.yongpay.top

throw new RuntimeException("失败", 500);
来源：http://wfr.gaohongyu789.top

[U72] PHP：写错误日志
来源：http://udw.jinyuanbaomall.cn

error_log("失败: " . $e->getMessage());
来源：http://kik.ybcxt.top

[U73] PHP：读取 ini 配置
来源：http://inp.guowangkeji.top

parse_ini_file("config.ini", true)
来源：http://olm.xylfe.cn

[U74] PHP：读取环境变量
来源：http://rdc.ybcxt.top

getenv("APP_ENV") ?: "production"
来源：http://cbp.shuidangran.top

[U75] PHP：依赖注入
来源：http://wom.xziqi.cn

composer require psr/container
来源：http://vke.xylfe.cn

[U76] PHP：简单路由
来源：http://zpj.andypj.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zas.zdqjudy.top

[U77] PHP：模板渲染
来源：http://grd.nwbrower.top

composer require twig/twig
来源：http://vtz.hesvh.cn

[U78] PHP：单元测试
来源：http://mxy.xylfe.cn

composer require --dev phpunit/phpunit
来源：http://znf.zhijiandao.cn

[U79] PHP：静态分析
来源：http://fce.52xcode.cn

composer require --dev phpstan/phpstan
来源：http://tuw.zhoulong.xyz

[U80] PHP：代码规范修复
来源：http://zzp.jiagoushi.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://tkl.zdqjudy.top

[U81] JS：初始化项目
来源：http://txa.ctjpmb.com

npm init -y;  npm i express
来源：http://amp.birdmap.top

[U82] JS：package.json 脚本
来源：http://bgt.tian-w.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hpx.jlsjyb.cn

[U83] JS：ES Module 导入导出
来源：http://jld.iojbl.cn

export const a = 1;  import { a } from "./m.js";
来源：http://iij.andypj.xyz

[U84] JS：CommonJS 写法
来源：http://cax.dashuyun.cn

module.exports = { a };  const { a } = require("./m");
来源：http://vos.bbcook.cn

[U85] JS：可选链
来源：http://tzu.zdbjq.cn

a?.b?.c
来源：http://oms.shanyushiyangtech.top

[U86] JS：空值合并
来源：http://nxf.daria6918.cn

a ?? b
来源：http://uod.hnxiangtu.top

[U87] JS：解构默认值
来源：http://iel.smart0.xyz

const { a = 1, b = 2 } = obj;
来源：http://ajb.cucudq.cn

[U88] JS：对象展开合并
来源：http://yqh.fzhhl.top

{ ...a, ...b }
来源：http://epq.andypj.xyz

[U89] JS：数组去重
来源：http://yln.hywenlv.cn

[...new Set(arr)]
来源：http://nkp.tarul.cn

[U90] JS：数字数组排序
来源：http://ksq.tianlin.xyz

[...arr].sort((a, b) => a - b)
来源：http://xse.52xcode.cn

[U91] JS：对象键值遍历
来源：http://glm.0kj1m.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pdh.haohaochexian.top

[U92] JS：深拷贝
来源：http://ysg.jinqigfzy.top

structuredClone(obj)
来源：http://wvr.hesvh.cn

[U93] JS：模板字符串
来源：http://neb.9152youxi.cn

`共 ${n} 条`
来源：http://pov.pengpengdd.cyou

[U94] JS：箭头函数
来源：http://gnf.cashguo.top

const double = x => x * 2;
来源：http://txw.yongpay.top

[U95] JS：Promise 包装
来源：http://mkr.xziqi.cn

new Promise((resolve, reject) => {})
来源：http://nto.bjfxy.top

[U96] JS：async/await 与异常
来源：http://tbj.yfazqb.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://huy.uphjek.com

[U97] JS：并发请求
来源：http://hhj.hysaishi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://nlg.zhongyouzk.top

[U98] JS：fetch 带 JSON
来源：http://wva.feifeiyinyue.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ism.zhengqikj.top

[U99] JS：事件监听
来源：http://vtl.jinqigufen.top

el.addEventListener("click", e => {})
来源：http://igt.xuetiantiany.cn

[U100] JS：DOM 查询
来源：http://esw.haohaochexian.top

document.querySelector(".item")
来源：http://tjz.chenlongwang.top

[U101] JS：classList 操作
来源：http://liq.svipenyu.cn

el.classList.toggle("active")
来源：http://euh.fehbvm.com

[U102] JS：本地存储
来源：http://uuw.chenzaomai.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://exx.yonumen.top

[U103] JS：定时器
来源：http://dgv.xuetiantiany.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kfu.hnqzz.top

[U104] JS：防抖
来源：http://fmd.jinqigfzy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rdd.xingfuxueyuan.xyz

[U105] JS：节流
来源：http://vzh.kuanghao11.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://izt.tanke756.top

[U106] JS：日期格式化
来源：http://kqn.jyoumei.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pkd.yueranfly.top

[U107] JS：数字千分位
来源：http://crj.ehwqpu.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://big.fanxiaobao.xyz

[U108] JS：随机整数
来源：http://cpd.cdnleiting.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://aqh.xinyue.icu

[U109] JS：数组分组
来源：http://wzm.zdbjq.cn

Object.groupBy(arr, x => x.type)
来源：http://zzf.jqgufenzy.top

[U110] JS：数组分块
来源：http://wrb.xziqi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gzr.xuanzx.com

[U111] JS：对象转 Map
来源：http://xqo.xziqi.cn

new Map(Object.entries(obj))
来源：http://stf.yuxming.cn

[U112] JS：字符串补位
来源：http://zjw.yongpay.top

"7".padStart(3, "0")
来源：http://cqh.xinyue.icu

[U113] JS：正则替换全部
来源：http://dqm.feifeiyinyue.top

s.replaceAll("a", "b")
来源：http://mqp.tianlin.xyz

[U114] JS：JSON 深比较
来源：http://jzu.nanxuanxn.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ctp.tarul.cn

[U115] JS：生成 UUID
来源：http://iud.hfpthk.cn

crypto.randomUUID()
来源：http://wzw.9152youxi.cn

[U116] JS：类型检查（JSDoc）
来源：http://ija.pengpengdd.cyou

/** @param {string} name */ function f(name) {}
来源：http://izn.ydjk.org.cn

[U117] JS：单元测试
来源：http://npm.0kj1m.cn

npm i -D vitest;  npx vitest
来源：http://wnh.zhoulong.xyz

[U118] JS：开发服务器
来源：http://ooc.c1oappe.top

npm i -D vite;  npx vite
来源：http://xmt.jinqigfzy.top

[U119] JS：生产构建
来源：http://ueq.jinyuanbaomall.cn

npx vite build
来源：http://hlo.ehwqpu.com

[U120] JS：读取环境变量（Vite）
来源：http://bff.zhengqikj.top

import.meta.env.VITE_API_URL
来源：http://dzl.hnqzz.top

================================================================================
来源：http://jsn.yuanzhike.top

统计汇总
来源：http://tse.xuanzx.com

================================================================================
来源：http://njg.gotoacloud.top

按语言统计（条）：
来源：http://cbq.wangdashe.top

Python ......... 252
来源：http://lse.guannengcc.top

PHP ............ 252
来源：http://vij.hywenlv.cn

JavaScript ..... 252
来源：http://fog.bbcook.cn

TypeScript ..... 212
来源：http://plt.jqgufenzy.top

Java ........... 212
来源：http://itu.yuanzhike.top

Go ............. 212
来源：http://tpf.shangyingyoupin.top

Ruby ........... 212
来源：http://qkz.yangfankeji.com

C# ............. 212
来源：http://fze.daxiang520.top

C .............. 30
来源：http://dhv.shangyingyoupin.top

C++ ............ 30
来源：http://hoh.haohaochexian.top

SQL ............ 90
来源：http://dsn.ybcxt.top

Bash ........... 80
来源：http://ins.wangdashe.top

Kotlin ......... 15
来源：http://lhg.9152youxi.cn

Swift .......... 15
来源：http://jsl.ydzc1.top

Lua ............ 10
来源：http://mbb.shuidangran.top

Perl ........... 10
来源：http://qvp.shangyingyoupin.top

Scala .......... 10
来源：http://mkv.hongshengwenyu.top

------------------------------------
来源：http://cwk.aibaodan.cn

合计 ........... 2106 条
来源：http://ydi.shzxlz.cn

按章节统计：
来源：http://kiw.kuanghao11.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rwj.nwbrower.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ypp.sxryk.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://akr.sufxvd.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://det.hnxiangtu.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vqu.316326.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ved.zdqjudy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ajs.quarkkingdee.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dpp.jinqigfzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gvw.c1oappe.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rpg.hfpthk.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zkh.shanyushiyangtech.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jth.yj20258.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rdz.bjfxy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://aig.yfazqb.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fux.tanke756.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xla.havefunace.top

Q SQL 专题                              90
来源：http://cwu.vqdsnc.cn

R Bash 专题                             80
来源：http://kwq.hywenlv.cn

S C / C++ 专题                          60
来源：http://kce.hywenlv.cn

T 其他语言补充                          60
来源：http://yzs.xuetiantiany.cn

U 高频实用片段                         120
来源：http://brv.zhiwuduotai.top

------------------------------------
来源：http://dlp.zhiwuduotai.top

合计                                  2106 条
来源：http://nji.pycfn.com

--------------------------------------------------------------------------------
来源：http://jcq.redwolf501.top

使用提醒
来源：http://vxz.xylfe.cn

--------------------------------------------------------------------------------
来源：http://qws.hnxiangtu.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rcn.ivvv.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hfj.nanxuanxn.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mvv.cucudq.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ibs.0kj1m.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dhk.meibo888.top

—— 文件结束 ——
来源：http://jjo.ydzc1.top

================================================================================
来源：http://ipr.snrcjt.cn

程序语言常见例子速查手册（2024 版）
来源：http://zee.ivvv.top

Common Programming Examples Cheat Book
来源：http://mxb.zdbjq.cn

================================================================================
来源：http://wpa.zhiwuduotai.top

【收录内容】
来源：http://fyk.ppjwa.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vmm.shanyushiyangkeji.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wbs.316326.xyz

SQL · Bash · C · C++
来源：http://vmk.hnxiangtu.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://acs.ppjwa.cn

【使用说明】
来源：http://tod.yj20258.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://glm.zhixingplan.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ryk.yfazqb.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zyf.havefunace.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gjy.jiagoushi.top

Bash:  Shell         C:     C             C++:   C++
来源：http://ypc.jinyuanbaomall.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://okt.jiagoushi.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://dpk.zhoulong.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jyc.xziqi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hid.yuxming.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mnj.mhx1999.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hgp.zdbjq.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hde.chenlongwang.top

【文件统计】
来源：http://lvl.iojbl.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mzq.meibo888.top

--------------------------------------------------------------------------------
来源：http://qwt.yanxiufei.cn

目  录
来源：http://ezi.hnqzz.top

--------------------------------------------------------------------------------
来源：http://mmf.gaohongyu789.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vky.meibo888.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://asn.ctjpmb.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://txm.havefunace.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tvh.zdqjudy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tfi.yongpay.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://jiz.ehwqpu.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://trz.daria6918.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://uff.ctjpmb.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qpy.guowangkeji.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://uti.316326.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rzo.meibo888.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://trf.yvedp.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://bar.fktsv.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rtq.aizwys.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://uvv.yfazqb.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qti.guowangkeji.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vhn.cucudq.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://oud.andypj.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ylf.cashguo.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qsi.jinghuilouyu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xds.wangdashe.top

================================================================================
来源：http://fpv.fzhhl.top

A. 基础语法与类型
来源：http://kbc.fzhhl.top

================================================================================
来源：http://gkd.gzhubu.top

[A01] Hello World
来源：http://fyh.mhx1999.top

Py:   print("Hello, World!")
来源：http://epy.52xcode.cn

PHP:  echo "Hello, World!";
来源：http://ufe.hfpthk.cn

JS:   console.log("Hello, World!");
来源：http://izi.xingfuxueyuan.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hmc.ydjk.org.cn

Java: System.out.println("Hello, World!");
来源：http://gxj.sweek.top

Go:   fmt.Println("Hello, World!")
来源：http://iek.fanxiaobao.xyz

Ruby: puts "Hello, World!"
来源：http://qeq.nanxuanxn.top

C#:   Console.WriteLine("Hello, World!");
来源：http://hbd.jinqigufen.top

[A02] 变量声明与赋值
来源：http://kpf.smart0.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hul.dashuyun.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://oei.yj202588.top

JS:   let name = "Alex"; const age = 20;
来源：http://zba.havefunace.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fls.zhaomingkeji.xyz

Java: String name = "Alex"; int age = 20;
来源：http://esj.smart0.xyz

Go:   name := "Alex"; age := 20
来源：http://xsy.zhongyouzk.top

Ruby: name = "Alex"; age = 20
来源：http://siu.ybcxt.top

C#:   string name = "Alex"; int age = 20;
来源：http://jdv.zdbjq.cn

[A03] 常量定义
来源：http://wgc.xuanzx.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://aeb.meibo888.top

PHP:  const PI = 3.14159;
来源：http://wpq.zhijiandao.cn

JS:   const PI = 3.14159;
来源：http://cgv.tanke756.top

TS:   const PI: number = 3.14159;
来源：http://phj.jinqigufen.top

Java: static final double PI = 3.14159;
来源：http://yue.zhaomingkeji.xyz

Go:   const PI = 3.14159
来源：http://bdm.quarkkingdee.top

Ruby: PI = 3.14159
来源：http://hsl.meibo888.top

C#:   const double PI = 3.14159;
来源：http://wpl.jlsjyb.cn

[A04] 判断变量类型
来源：http://epv.jiagoushi.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://hux.tianlin.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://grr.quarkkingdee.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://eej.yanxiufei.cn

TS:   typeof x; x instanceof Date
来源：http://uzc.yj20258.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bta.fktsv.cn

Go:   reflect.TypeOf(x).Name()
来源：http://lgq.tarul.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://sdj.ppjwa.cn

C#:   x.GetType().Name; x is int
来源：http://zhc.zhiwuduotai.top

[A05] 整数除法与取模
来源：http://jco.yj20258.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fsy.zhoulong.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://odv.yj20258888.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bek.fehbvm.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://iwp.meibo888.top

Java: 7 / 2; 7 % 2
来源：http://utc.hnxiangtu.top

Go:   7 / 2; 7 % 2
来源：http://yya.chenjidiqi.icu

Ruby: 7 / 2; 7 % 2
来源：http://oyv.316326.xyz

C#:   7 / 2; 7 % 2
来源：http://hbn.haohaochexian.top

[A06] 字符串转数字
来源：http://kds.ehwqpu.com

Py:   int("42"); float("3.14")
来源：http://wat.ivvv.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://yzx.tianlin.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xes.xuanzx.com


<!-- 参考信息 -->