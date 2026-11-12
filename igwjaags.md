代发 wailian999

[U49] PHP：只读属性
来源：http://lme.ivvv.top

public readonly string $name
来源：http://wnb.hammf.cn

[U50] PHP：构造器属性提升
来源：http://kdf.jqgufenzy.top

public function __construct(private int $id) {}
来源：http://its.ehwqpu.com

[U51] PHP：数组解构
来源：http://fgi.cheryme.top

[$a, $b] = $arr;
来源：http://knn.yvedp.cn

[U52] PHP：箭头函数
来源：http://zgy.haohaochexian.top

$double = fn($x) => $x * 2;
来源：http://lyz.hcnkem.com

[U53] PHP：空合并运算符
来源：http://hfm.xylfe.cn

$v = $a ?? $b ?? "default";
来源：http://vhz.uphjek.com

[U54] PHP：空安全调用
来源：http://gce.zdbjq.cn

$obj?->method()
来源：http://evp.uphjek.com

[U55] PHP：match 表达式
来源：http://ujq.cqqwz.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yrd.vqdsnc.cn

[U56] PHP：命名参数
来源：http://mia.andypj.xyz

f(a: 1, b: 2)
来源：http://cqc.ivvv.top

[U57] PHP：字符串插值
来源：http://zws.zycfv.cn

"值: {$a}"
来源：http://qna.sxryk.cn

[U58] PHP：数组三件套
来源：http://qao.yonumen.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qiq.havefunace.top

[U59] PHP：自定义排序
来源：http://uut.gaohongyu789.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://axm.xziqi.cn

[U60] PHP：JSON 编解码
来源：http://owh.zhiwuduotai.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ebd.gogol.net.cn

[U61] PHP：正则
来源：http://igc.zdbjq.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wjf.jinghuilouyu.cn

[U62] PHP：日期对象
来源：http://man.gzhubu.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bfc.gotoacloud.top

[U63] PHP：文件读写
来源：http://itl.ybcxt.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pgs.jinqigufen.top

[U64] PHP：目录遍历
来源：http://hvd.jianghu66.top

glob("dir/*.php");  scandir("dir");
来源：http://xnq.yuxming.cn

[U65] PHP：会话
来源：http://aac.hywenlv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wmr.fanxiaobao.xyz

[U66] PHP：设置 Cookie
来源：http://ysr.iojbl.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gsg.0kj1m.cn

[U67] PHP：处理文件上传
来源：http://uax.hammf.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://osk.aibaodan.cn

[U68] PHP：PDO 连接
来源：http://bnj.wangshuangyany.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://shy.aibaodan.cn

[U69] PHP：PDO 预处理
来源：http://bvo.c1oappe.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hyd.cqqwz.cn

[U70] PHP：PDO 事务
来源：http://gof.snrcjt.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xvk.vqdsnc.cn

[U71] PHP：抛出异常
来源：http://ebz.tarul.cn

throw new RuntimeException("失败", 500);
来源：http://yko.cashguo.top

[U72] PHP：写错误日志
来源：http://vfs.kuanghao11.cn

error_log("失败: " . $e->getMessage());
来源：http://pya.mhx1999.top

[U73] PHP：读取 ini 配置
来源：http://nap.shanyushiyangkeji.top

parse_ini_file("config.ini", true)
来源：http://nyc.jinyuanbaomall.cn

[U74] PHP：读取环境变量
来源：http://zth.yj202588.top

getenv("APP_ENV") ?: "production"
来源：http://hja.jiagoushi.top

[U75] PHP：依赖注入
来源：http://scw.0kj1m.cn

composer require psr/container
来源：http://svp.hywenlv.cn

[U76] PHP：简单路由
来源：http://ohn.mhx1999.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fht.yongpay.top

[U77] PHP：模板渲染
来源：http://iwh.ybcxt.top

composer require twig/twig
来源：http://yam.yuxming.cn

[U78] PHP：单元测试
来源：http://uon.zhijiandao.cn

composer require --dev phpunit/phpunit
来源：http://ptl.ybcxt.top

[U79] PHP：静态分析
来源：http://zxh.nwbrower.top

composer require --dev phpstan/phpstan
来源：http://nxk.sxryk.cn

[U80] PHP：代码规范修复
来源：http://bvc.hnxiangtu.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://cut.yuxming.cn

[U81] JS：初始化项目
来源：http://xdn.shanyushiyangkeji.top

npm init -y;  npm i express
来源：http://zgk.iojbl.cn

[U82] JS：package.json 脚本
来源：http://aqt.chenjidiqi.icu

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ifh.0kj1m.cn

[U83] JS：ES Module 导入导出
来源：http://iro.gogol.net.cn

export const a = 1;  import { a } from "./m.js";
来源：http://tpv.fengsongda.top

[U84] JS：CommonJS 写法
来源：http://tmr.hammf.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wqg.jinqigufen.top

[U85] JS：可选链
来源：http://cqv.yangfankeji.com

a?.b?.c
来源：http://fta.chenzaomai.com

[U86] JS：空值合并
来源：http://ufk.ywan-chungtsiang.top

a ?? b
来源：http://ocu.ydzc1.top

[U87] JS：解构默认值
来源：http://rzl.havefunace.top

const { a = 1, b = 2 } = obj;
来源：http://xnc.gaohongyu789.top

[U88] JS：对象展开合并
来源：http://avy.sweek.top

{ ...a, ...b }
来源：http://qaz.redwolf501.top

[U89] JS：数组去重
来源：http://vii.ehwqpu.com

[...new Set(arr)]
来源：http://wiy.cucudq.cn

[U90] JS：数字数组排序
来源：http://rcb.zhaomingkeji.xyz

[...arr].sort((a, b) => a - b)
来源：http://hiu.daria6918.cn

[U91] JS：对象键值遍历
来源：http://efa.ydzc1.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wsc.316326.xyz

[U92] JS：深拷贝
来源：http://ckx.ydjk.org.cn

structuredClone(obj)
来源：http://zko.hywenlv.cn

[U93] JS：模板字符串
来源：http://gwa.xuanzx.com

`共 ${n} 条`
来源：http://clr.kuanghao11.cn

[U94] JS：箭头函数
来源：http://nxw.ctjpmb.com

const double = x => x * 2;
来源：http://mms.daria6918.cn

[U95] JS：Promise 包装
来源：http://mqn.c1oappe.top

new Promise((resolve, reject) => {})
来源：http://wlv.316326.xyz

[U96] JS：async/await 与异常
来源：http://etx.dashuyun.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qsq.havefunace.top

[U97] JS：并发请求
来源：http://yma.fktsv.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://txv.jinghuilouyu.cn

[U98] JS：fetch 带 JSON
来源：http://zij.snrcjt.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sqv.jlsjyb.cn

[U99] JS：事件监听
来源：http://xiz.hcnkem.com

el.addEventListener("click", e => {})
来源：http://bzl.zdbjq.cn

[U100] JS：DOM 查询
来源：http://mke.cdnleiting.top

document.querySelector(".item")
来源：http://wds.gaohongyu789.top

[U101] JS：classList 操作
来源：http://wsh.zycfv.cn

el.classList.toggle("active")
来源：http://mff.shanyushiyangkeji.top

[U102] JS：本地存储
来源：http://hlc.bbcook.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://tbr.smart0.xyz

[U103] JS：定时器
来源：http://hme.zhixingplan.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sun.quarkkingdee.top

[U104] JS：防抖
来源：http://kbn.fengsongda.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jjf.ehwqpu.com

[U105] JS：节流
来源：http://dil.guannengcc.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pok.zdbjq.cn

[U106] JS：日期格式化
来源：http://qsq.uphjek.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://uqj.havefunace.top

[U107] JS：数字千分位
来源：http://hcg.316326.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wnw.bbcook.cn

[U108] JS：随机整数
来源：http://ect.yfazqb.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uwb.wangshuangyany.cn

[U109] JS：数组分组
来源：http://dxr.sjlbkw.cn

Object.groupBy(arr, x => x.type)
来源：http://onq.yuxming.cn

[U110] JS：数组分块
来源：http://fte.gzhubu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://slc.shzxlz.cn

[U111] JS：对象转 Map
来源：http://ehj.ivvv.top

new Map(Object.entries(obj))
来源：http://ayw.hfpthk.cn

[U112] JS：字符串补位
来源：http://gov.zdqjudy.top

"7".padStart(3, "0")
来源：http://fvw.fzhhl.top

[U113] JS：正则替换全部
来源：http://eaw.cqqwz.cn

s.replaceAll("a", "b")
来源：http://knk.chenzaomai.com

[U114] JS：JSON 深比较
来源：http://kvu.sxryk.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ocm.sysykeji.top

[U115] JS：生成 UUID
来源：http://cdk.0kj1m.cn

crypto.randomUUID()
来源：http://toc.yj20258.top

[U116] JS：类型检查（JSDoc）
来源：http://lcb.yanxiufei.cn

/** @param {string} name */ function f(name) {}
来源：http://ntw.xuanzx.com

[U117] JS：单元测试
来源：http://fjw.hcnkem.com

npm i -D vitest;  npx vitest
来源：http://sln.yueranfly.top

[U118] JS：开发服务器
来源：http://clz.hnqzz.top

npm i -D vite;  npx vite
来源：http://vjh.ivvv.top

[U119] JS：生产构建
来源：http://rbq.guowangkeji.top

npx vite build
来源：http://lrj.jinghuilouyu.cn

[U120] JS：读取环境变量（Vite）
来源：http://oes.c1oappe.top

import.meta.env.VITE_API_URL
来源：http://ngk.ctjpmb.com

================================================================================
来源：http://rec.c1oappe.top

统计汇总
来源：http://cus.meibo888.top

================================================================================
来源：http://uwi.haohaochexian.top

按语言统计（条）：
来源：http://yqt.yongpay.top

Python ......... 252
来源：http://qvn.jyoumei.cn

PHP ............ 252
来源：http://cfp.xziqi.cn

JavaScript ..... 252
来源：http://tin.guowangkeji.top

TypeScript ..... 212
来源：http://gja.wangdashe.top

Java ........... 212
来源：http://jcc.smart0.xyz

Go ............. 212
来源：http://muo.hywenlv.cn

Ruby ........... 212
来源：http://gac.yj20258888.top

C# ............. 212
来源：http://ivp.chenjidiqi.icu

C .............. 30
来源：http://ynn.dashuyun.cn

C++ ............ 30
来源：http://ijl.jianghu66.top

SQL ............ 90
来源：http://dil.hnqzz.top

Bash ........... 80
来源：http://vbd.c1oappe.top

Kotlin ......... 15
来源：http://kea.yvedp.cn

Swift .......... 15
来源：http://ixe.fzhhl.top

Lua ............ 10
来源：http://mqe.ppjwa.cn

Perl ........... 10
来源：http://czq.jinghuilouyu.cn

Scala .......... 10
来源：http://lkn.xuetiantiany.cn

------------------------------------
来源：http://kta.feifeiyinyue.top

合计 ........... 2106 条
来源：http://mzw.fengsongda.top

按章节统计：
来源：http://uaq.havefunace.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://obb.zhiwuduotai.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bbh.chenzaomai.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ydi.shanyushiyangtech.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lvf.sjlbkw.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cms.gzhubu.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zsa.sxryk.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ffx.ehwqpu.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jtn.hnxiangtu.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fkr.shanyushiyangtech.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://unn.ppjwa.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hkn.ehwqpu.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://uqa.zhongyouzk.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://orh.ydjk.org.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://oaa.shanyushiyangkeji.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zcl.guowangkeji.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xfh.hnxiangtu.top

Q SQL 专题                              90
来源：http://oxp.daxiang520.top

R Bash 专题                             80
来源：http://iiy.mhx1999.top

S C / C++ 专题                          60
来源：http://hqh.hnxiangtu.top

T 其他语言补充                          60
来源：http://jnl.pengpengdd.cyou

U 高频实用片段                         120
来源：http://dcn.yj202588.top

------------------------------------
来源：http://afl.snrcjt.cn

合计                                  2106 条
来源：http://tlx.yueranfly.top

--------------------------------------------------------------------------------
来源：http://xal.yj20258888.top

使用提醒
来源：http://ztx.yuxming.cn

--------------------------------------------------------------------------------
来源：http://tyg.jinqigfzy.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lpg.wangdashe.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vas.jinqigfzy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dvv.zhoulong.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://ehf.hongshengwenyu.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hyn.sufxvd.cn

—— 文件结束 ——
来源：http://vcz.gotoacloud.top

================================================================================
来源：http://ees.bbcook.cn

程序语言常见例子速查手册（2024 版）
来源：http://fif.hnxiangtu.top

Common Programming Examples Cheat Book
来源：http://jum.hnqzz.top

================================================================================
来源：http://zdv.hammf.cn

【收录内容】
来源：http://rkn.ppjwa.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://dgc.epnwcf.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://lle.snrcjt.cn

SQL · Bash · C · C++
来源：http://uun.iojbl.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://sfr.cheryme.top

【使用说明】
来源：http://tsd.jyoumei.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gxe.yueranfly.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mdx.cucudq.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hcy.c1oappe.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qyl.ivvv.top

Bash:  Shell         C:     C             C++:   C++
来源：http://sat.yj20258888.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baa.hcnkem.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qug.chenzaomai.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pux.svipenyu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qic.hfpthk.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rma.aizwys.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://svp.nanxinkj.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vlm.zhoulong.xyz

【文件统计】
来源：http://wku.tian-w.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mov.hnxiangtu.top

--------------------------------------------------------------------------------
来源：http://jrk.yvedp.cn

目  录
来源：http://rei.fehbvm.com

--------------------------------------------------------------------------------
来源：http://mlz.jinyuanbaomall.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://eie.birdmap.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://fpr.zhiwuduotai.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://amg.shanyushiyangtech.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mjd.jinyuanbaomall.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lgq.haohaochexian.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://end.yanxiufei.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://odf.jlsjyb.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rkn.guannengcc.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://caw.ydjk.org.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yzf.316326.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wmo.nwbrower.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gjw.bbcook.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ttg.sweek.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zqm.xuanzx.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://nxp.316326.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://nuj.sxryk.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://oyy.yfazqb.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://gnm.cashguo.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://aun.yfazqb.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://aoo.nanxinkj.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nrx.hysaishi.cn

================================================================================
来源：http://bon.nanxuanxn.top

A. 基础语法与类型
来源：http://zwe.tarul.cn

================================================================================
来源：http://gxo.cdnleiting.top

[A01] Hello World
来源：http://czy.bbcook.cn

Py:   print("Hello, World!")
来源：http://uie.cqqwz.cn

PHP:  echo "Hello, World!";
来源：http://qeh.feifeiyinyue.top

JS:   console.log("Hello, World!");
来源：http://ise.chenlongwang.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://add.guowangkeji.top

Java: System.out.println("Hello, World!");
来源：http://ivy.hfpthk.cn

Go:   fmt.Println("Hello, World!")
来源：http://hco.yuanzhike.top

Ruby: puts "Hello, World!"
来源：http://qic.hfpthk.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://bys.hywenlv.cn

[A02] 变量声明与赋值
来源：http://dox.nanxinkj.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yjc.pycfn.com

PHP:  $name = "Alex"; $age = 20;
来源：http://vps.dianchejie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://pra.jiagoushi.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://tjm.yfazqb.com

Java: String name = "Alex"; int age = 20;
来源：http://ezh.9152youxi.cn

Go:   name := "Alex"; age := 20
来源：http://lsp.ctjpmb.com

Ruby: name = "Alex"; age = 20
来源：http://ihm.ppjwa.cn

C#:   string name = "Alex"; int age = 20;
来源：http://rex.yvedp.cn

[A03] 常量定义
来源：http://gpa.chenlongwang.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hds.sufxvd.cn

PHP:  const PI = 3.14159;
来源：http://vpg.tianlin.xyz

JS:   const PI = 3.14159;
来源：http://gkg.yfazqb.com

TS:   const PI: number = 3.14159;
来源：http://jfg.bjfxy.top

Java: static final double PI = 3.14159;
来源：http://stq.svipenyu.cn

Go:   const PI = 3.14159
来源：http://mnx.chenlongwang.top

Ruby: PI = 3.14159
来源：http://jnc.daria6918.cn

C#:   const double PI = 3.14159;
来源：http://evz.wangdashe.top

[A04] 判断变量类型
来源：http://nqf.redwolf501.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://vca.yonumen.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://etf.cqqwz.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://abo.fktsv.cn

TS:   typeof x; x instanceof Date
来源：http://zea.shzxlz.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xvy.sxryk.cn

Go:   reflect.TypeOf(x).Name()
来源：http://fdz.hfpthk.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://nmu.hnqzz.top

C#:   x.GetType().Name; x is int
来源：http://fqq.zhixingplan.top

[A05] 整数除法与取模
来源：http://cpt.uphjek.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ibw.shzxlz.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://qpd.xuanzx.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jls.vqdsnc.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://euv.ywan-chungtsiang.top

Java: 7 / 2; 7 % 2
来源：http://vtx.c1oappe.top

Go:   7 / 2; 7 % 2
来源：http://zjg.ehwqpu.com

Ruby: 7 / 2; 7 % 2
来源：http://gvl.andypj.xyz

C#:   7 / 2; 7 % 2
来源：http://aqk.sjlbkw.cn

[A06] 字符串转数字
来源：http://rnp.nanxinkj.top

Py:   int("42"); float("3.14")
来源：http://zzc.sjlbkw.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fgv.yangfankeji.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jpn.kuanghao11.cn


<!-- 参考信息 -->