代发 wailian999

[U49] PHP：只读属性
来源：http://lru.fzhhl.top

public readonly string $name
来源：http://iah.shzxlz.cn

[U50] PHP：构造器属性提升
来源：http://ajf.ctjpmb.com

public function __construct(private int $id) {}
来源：http://ucx.fzhhl.top

[U51] PHP：数组解构
来源：http://jjf.shzxlz.cn

[$a, $b] = $arr;
来源：http://ffz.wangshuangyany.cn

[U52] PHP：箭头函数
来源：http://zzj.shangyingyoupin.top

$double = fn($x) => $x * 2;
来源：http://pda.zhixingplan.top

[U53] PHP：空合并运算符
来源：http://rjq.c1oappe.top

$v = $a ?? $b ?? "default";
来源：http://wud.guannengcc.top

[U54] PHP：空安全调用
来源：http://byj.ydzc1.top

$obj?->method()
来源：http://jby.hysaishi.cn

[U55] PHP：match 表达式
来源：http://asq.pycfn.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wby.shanyushiyangtech.top

[U56] PHP：命名参数
来源：http://eds.xinyue.icu

f(a: 1, b: 2)
来源：http://imr.uphjek.com

[U57] PHP：字符串插值
来源：http://kki.yueranfly.top

"值: {$a}"
来源：http://ywe.pengpengdd.cyou

[U58] PHP：数组三件套
来源：http://bvj.bbcook.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hqx.chenjidiqi.icu

[U59] PHP：自定义排序
来源：http://reo.hfpthk.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hyz.jinyuanbaomall.cn

[U60] PHP：JSON 编解码
来源：http://bbw.hcnkem.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://aeq.zhiwuduotai.top

[U61] PHP：正则
来源：http://yyv.hongshengwenyu.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vqp.hnqzz.top

[U62] PHP：日期对象
来源：http://xpw.fengsongda.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ytc.ybcxt.top

[U63] PHP：文件读写
来源：http://vrl.dashuyun.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dfr.birdmap.top

[U64] PHP：目录遍历
来源：http://mgr.xziqi.cn

glob("dir/*.php");  scandir("dir");
来源：http://ykh.gogol.net.cn

[U65] PHP：会话
来源：http://ikq.jinqigfzy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://twu.jinqigfzy.top

[U66] PHP：设置 Cookie
来源：http://gqv.c1oappe.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gms.cqqwz.cn

[U67] PHP：处理文件上传
来源：http://rxe.haohaochexian.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tmv.shanyushiyangkeji.top

[U68] PHP：PDO 连接
来源：http://soj.guowangkeji.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rfa.cdnleiting.top

[U69] PHP：PDO 预处理
来源：http://udv.hysaishi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qiy.52xcode.cn

[U70] PHP：PDO 事务
来源：http://vxf.gaohongyu789.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cfu.yj20258888.top

[U71] PHP：抛出异常
来源：http://ume.ywan-chungtsiang.top

throw new RuntimeException("失败", 500);
来源：http://amy.yuanzhike.top

[U72] PHP：写错误日志
来源：http://nus.ppjwa.cn

error_log("失败: " . $e->getMessage());
来源：http://cyx.gotoacloud.top

[U73] PHP：读取 ini 配置
来源：http://ewu.bbcook.cn

parse_ini_file("config.ini", true)
来源：http://kxd.jyoumei.cn

[U74] PHP：读取环境变量
来源：http://dky.aizwys.cn

getenv("APP_ENV") ?: "production"
来源：http://oxt.cashguo.top

[U75] PHP：依赖注入
来源：http://bbc.uphjek.com

composer require psr/container
来源：http://gxu.xziqi.cn

[U76] PHP：简单路由
来源：http://xik.yuxming.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bqe.vehdjk.com

[U77] PHP：模板渲染
来源：http://fyn.snrcjt.cn

composer require twig/twig
来源：http://jcm.yj202588.top

[U78] PHP：单元测试
来源：http://ial.zhengqikj.top

composer require --dev phpunit/phpunit
来源：http://uqc.wangdashe.top

[U79] PHP：静态分析
来源：http://srw.epnwcf.com

composer require --dev phpstan/phpstan
来源：http://wvn.snrcjt.cn

[U80] PHP：代码规范修复
来源：http://hwp.zhoulong.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://jpc.daria6918.cn

[U81] JS：初始化项目
来源：http://nae.dianchejie.cn

npm init -y;  npm i express
来源：http://bzw.yj20258.top

[U82] JS：package.json 脚本
来源：http://udw.cashguo.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sku.ivvv.top

[U83] JS：ES Module 导入导出
来源：http://jbg.cheryme.top

export const a = 1;  import { a } from "./m.js";
来源：http://qom.xingfuxueyuan.xyz

[U84] JS：CommonJS 写法
来源：http://mqm.yangfankeji.com

module.exports = { a };  const { a } = require("./m");
来源：http://vsu.dianchejie.cn

[U85] JS：可选链
来源：http://isl.cucudq.cn

a?.b?.c
来源：http://gzg.haohaochexian.top

[U86] JS：空值合并
来源：http://jed.tarul.cn

a ?? b
来源：http://yjs.yuanzhike.top

[U87] JS：解构默认值
来源：http://phg.shzxlz.cn

const { a = 1, b = 2 } = obj;
来源：http://ihq.mhx1999.top

[U88] JS：对象展开合并
来源：http://tqj.fanxiaobao.xyz

{ ...a, ...b }
来源：http://wkf.vqdsnc.cn

[U89] JS：数组去重
来源：http://ltk.havefunace.top

[...new Set(arr)]
来源：http://aee.svipenyu.cn

[U90] JS：数字数组排序
来源：http://pyw.zhengqikj.top

[...arr].sort((a, b) => a - b)
来源：http://ebs.yj20258888.top

[U91] JS：对象键值遍历
来源：http://qdb.jinqigufen.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xbx.hnxiangtu.top

[U92] JS：深拷贝
来源：http://apw.pengpengdd.cyou

structuredClone(obj)
来源：http://fux.zhixingplan.top

[U93] JS：模板字符串
来源：http://vnz.xingfuxueyuan.xyz

`共 ${n} 条`
来源：http://coc.fehbvm.com

[U94] JS：箭头函数
来源：http://xyd.yonumen.top

const double = x => x * 2;
来源：http://loy.fzhhl.top

[U95] JS：Promise 包装
来源：http://hsr.hysaishi.cn

new Promise((resolve, reject) => {})
来源：http://udo.hnqzz.top

[U96] JS：async/await 与异常
来源：http://zfb.xingfuxueyuan.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xdf.zdqjudy.top

[U97] JS：并发请求
来源：http://oid.gotoacloud.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://pre.jinqigfzy.top

[U98] JS：fetch 带 JSON
来源：http://slv.zhengqikj.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://srv.yvedp.cn

[U99] JS：事件监听
来源：http://weq.svipenyu.cn

el.addEventListener("click", e => {})
来源：http://yus.yj20258888.top

[U100] JS：DOM 查询
来源：http://tyq.chenjidiqi.icu

document.querySelector(".item")
来源：http://mtx.bbcook.cn

[U101] JS：classList 操作
来源：http://amg.tianlin.xyz

el.classList.toggle("active")
来源：http://zin.yangfankeji.com

[U102] JS：本地存储
来源：http://qbn.chenzaomai.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://zle.hfpthk.cn

[U103] JS：定时器
来源：http://vfk.smart0.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pjk.yuanzhike.top

[U104] JS：防抖
来源：http://gwl.epnwcf.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rvj.jinghuilouyu.cn

[U105] JS：节流
来源：http://efh.tarul.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pub.cashguo.top

[U106] JS：日期格式化
来源：http://nid.52xcode.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gdf.chenzaomai.com

[U107] JS：数字千分位
来源：http://rlw.birdmap.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lty.chenzaomai.com

[U108] JS：随机整数
来源：http://dcg.sufxvd.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wgt.shanyushiyangkeji.top

[U109] JS：数组分组
来源：http://uhq.0kj1m.cn

Object.groupBy(arr, x => x.type)
来源：http://ixw.haohaochexian.top

[U110] JS：数组分块
来源：http://tkv.zhixingplan.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xxd.zhiwuduotai.top

[U111] JS：对象转 Map
来源：http://fyv.birdmap.top

new Map(Object.entries(obj))
来源：http://qlr.jqgfzy.top

[U112] JS：字符串补位
来源：http://bku.gaohongyu789.top

"7".padStart(3, "0")
来源：http://qjp.hnqzz.top

[U113] JS：正则替换全部
来源：http://jkg.chenjidiqi.icu

s.replaceAll("a", "b")
来源：http://vvh.nanxinkj.top

[U114] JS：JSON 深比较
来源：http://rvx.nwbrower.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://oat.cashguo.top

[U115] JS：生成 UUID
来源：http://rai.fengsongda.top

crypto.randomUUID()
来源：http://xca.tian-w.cn

[U116] JS：类型检查（JSDoc）
来源：http://yfp.zhengqikj.top

/** @param {string} name */ function f(name) {}
来源：http://yjo.nanxinkj.top

[U117] JS：单元测试
来源：http://bgm.xingfuxueyuan.xyz

npm i -D vitest;  npx vitest
来源：http://jpo.yanxiufei.cn

[U118] JS：开发服务器
来源：http://bbd.zdbjq.cn

npm i -D vite;  npx vite
来源：http://djg.smart0.xyz

[U119] JS：生产构建
来源：http://alv.ydjk.org.cn

npx vite build
来源：http://uwj.chenjidiqi.icu

[U120] JS：读取环境变量（Vite）
来源：http://jbx.aizwys.cn

import.meta.env.VITE_API_URL
来源：http://gax.yonumen.top

================================================================================
来源：http://cvn.sweek.top

统计汇总
来源：http://jhw.zhoulong.xyz

================================================================================
来源：http://vpq.xuanzx.com

按语言统计（条）：
来源：http://skw.jinyuanbaomall.cn

Python ......... 252
来源：http://rvh.hammf.cn

PHP ............ 252
来源：http://cwl.redwolf501.top

JavaScript ..... 252
来源：http://emh.meibo888.top

TypeScript ..... 212
来源：http://sxx.feifeiyinyue.top

Java ........... 212
来源：http://lsx.svipenyu.cn

Go ............. 212
来源：http://zpm.cqqwz.cn

Ruby ........... 212
来源：http://qln.shanyushiyangkeji.top

C# ............. 212
来源：http://hng.smart0.xyz

C .............. 30
来源：http://ldw.dianchejie.cn

C++ ............ 30
来源：http://jex.ehwqpu.com

SQL ............ 90
来源：http://afr.havefunace.top

Bash ........... 80
来源：http://mwn.ivvv.top

Kotlin ......... 15
来源：http://ttw.tianlin.xyz

Swift .......... 15
来源：http://mie.sxryk.cn

Lua ............ 10
来源：http://ijh.cashguo.top

Perl ........... 10
来源：http://xpl.jianghu66.top

Scala .......... 10
来源：http://qjw.ppjwa.cn

------------------------------------
来源：http://kst.c1oappe.top

合计 ........... 2106 条
来源：http://cfx.chenlongwang.top

按章节统计：
来源：http://win.cheryme.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vxs.316326.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mwy.chenlongwang.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bkg.shanyushiyangkeji.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pvz.vqdsnc.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mom.epnwcf.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://oyu.xinyue.icu

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ymn.xingfuxueyuan.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ucs.yvedp.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tad.pycfn.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://avw.dashuyun.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xab.daxiang520.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://idw.xuanzx.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yzs.nanxuanxn.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rio.jinqigfzy.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cqu.hcnkem.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://uwt.redwolf501.top

Q SQL 专题                              90
来源：http://asw.fktsv.cn

R Bash 专题                             80
来源：http://swe.yj202588.top

S C / C++ 专题                          60
来源：http://yyc.fehbvm.com

T 其他语言补充                          60
来源：http://mww.yvedp.cn

U 高频实用片段                         120
来源：http://dcl.aibaodan.cn

------------------------------------
来源：http://doq.hammf.cn

合计                                  2106 条
来源：http://zha.zhaomingkeji.xyz

--------------------------------------------------------------------------------
来源：http://ewe.meibo888.top

使用提醒
来源：http://iam.tianlin.xyz

--------------------------------------------------------------------------------
来源：http://iwm.zhiwuduotai.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tia.hnxiangtu.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wml.vqdsnc.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://oyx.mhx1999.top

在旧版本上使用前请先确认语法支持情况。
来源：http://taa.yongpay.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://irf.dianchejie.cn

—— 文件结束 ——
来源：http://sry.smart0.xyz

================================================================================
来源：http://xon.sjlbkw.cn

程序语言常见例子速查手册（2024 版）
来源：http://hpt.guowangkeji.top

Common Programming Examples Cheat Book
来源：http://lct.zycfv.cn

================================================================================
来源：http://fqs.yonumen.top

【收录内容】
来源：http://wbf.zhijiandao.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://tcv.dianchejie.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://iub.jinqigufen.top

SQL · Bash · C · C++
来源：http://kow.vehdjk.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ksa.cheryme.top

【使用说明】
来源：http://afp.hfpthk.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rfx.yj20258.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cul.aizwys.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hap.ctjpmb.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cgx.xuanzx.com

Bash:  Shell         C:     C             C++:   C++
来源：http://uhd.xylfe.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nyz.tarul.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yzq.jinqigufen.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pyf.yuxming.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ojb.tarul.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wmi.daxiang520.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ler.9152youxi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://duq.mhx1999.top

【文件统计】
来源：http://gxa.c1oappe.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://sfr.chenjidiqi.icu

--------------------------------------------------------------------------------
来源：http://xui.vqdsnc.cn

目  录
来源：http://zwv.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://psr.smart0.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://nzs.hywenlv.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://pgr.mhx1999.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ngf.tian-w.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://uxa.zhiwuduotai.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://etl.tianlin.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cex.zhengqikj.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://uzp.zhaomingkeji.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dns.iojbl.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mvs.yangfankeji.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cyn.nanxuanxn.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zig.epnwcf.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dzh.ctjpmb.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kpq.fktsv.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pfo.bbcook.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://eaf.jqgfzy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qap.xuanzx.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vao.sjlbkw.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ilh.yj20258888.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xpl.yj20258.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rqg.smart0.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cdu.fengsongda.top

================================================================================
来源：http://ldo.epnwcf.com

A. 基础语法与类型
来源：http://qwz.jyoumei.cn

================================================================================
来源：http://dkp.guowangkeji.top

[A01] Hello World
来源：http://gdz.xziqi.cn

Py:   print("Hello, World!")
来源：http://vyx.jinqigufen.top

PHP:  echo "Hello, World!";
来源：http://sns.xziqi.cn

JS:   console.log("Hello, World!");
来源：http://yir.jinghuilouyu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://dqb.jlsjyb.cn

Java: System.out.println("Hello, World!");
来源：http://dix.jlsjyb.cn

Go:   fmt.Println("Hello, World!")
来源：http://lbq.jinghuilouyu.cn

Ruby: puts "Hello, World!"
来源：http://ayk.wangdashe.top

C#:   Console.WriteLine("Hello, World!");
来源：http://arc.fanxiaobao.xyz

[A02] 变量声明与赋值
来源：http://rhg.redwolf501.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mxz.gaohongyu789.top

PHP:  $name = "Alex"; $age = 20;
来源：http://lkm.vqdsnc.cn

JS:   let name = "Alex"; const age = 20;
来源：http://umr.xinyue.icu

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hye.shzxlz.cn

Java: String name = "Alex"; int age = 20;
来源：http://lyj.0kj1m.cn

Go:   name := "Alex"; age := 20
来源：http://chb.fzhhl.top

Ruby: name = "Alex"; age = 20
来源：http://gxh.iojbl.cn

C#:   string name = "Alex"; int age = 20;
来源：http://kzv.jinyuanbaomall.cn

[A03] 常量定义
来源：http://siu.fengsongda.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ddv.xuanzx.com

PHP:  const PI = 3.14159;
来源：http://lfq.yvedp.cn

JS:   const PI = 3.14159;
来源：http://xib.hysaishi.cn

TS:   const PI: number = 3.14159;
来源：http://fkb.yonumen.top

Java: static final double PI = 3.14159;
来源：http://fvh.ctjpmb.com

Go:   const PI = 3.14159
来源：http://xqp.quarkkingdee.top

Ruby: PI = 3.14159
来源：http://auu.cqqwz.cn

C#:   const double PI = 3.14159;
来源：http://nyo.smart0.xyz

[A04] 判断变量类型
来源：http://cec.ybcxt.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://xfh.ydjk.org.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://txr.sufxvd.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rii.hnxiangtu.top

TS:   typeof x; x instanceof Date
来源：http://mhd.zhijiandao.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://uua.yj20258.top

Go:   reflect.TypeOf(x).Name()
来源：http://wcx.yanxiufei.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://uub.shanyushiyangkeji.top

C#:   x.GetType().Name; x is int
来源：http://hoj.sjlbkw.cn

[A05] 整数除法与取模
来源：http://wvv.yonumen.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ddb.yj202588.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://wiy.xylfe.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ugl.jinqigfzy.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://okn.ywan-chungtsiang.top

Java: 7 / 2; 7 % 2
来源：http://twp.bbcook.cn

Go:   7 / 2; 7 % 2
来源：http://itn.jyoumei.cn

Ruby: 7 / 2; 7 % 2
来源：http://vlj.fzhhl.top

C#:   7 / 2; 7 % 2
来源：http://txq.bjfxy.top

[A06] 字符串转数字
来源：http://rtv.zdqjudy.top

Py:   int("42"); float("3.14")
来源：http://jum.sufxvd.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://oja.yj20258888.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://etu.0kj1m.cn


<!-- 参考信息 -->