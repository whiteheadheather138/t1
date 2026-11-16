代发 wailian999

[U51] PHP：数组解构
来源：http://xsy.chenlongwang.top

[$a, $b] = $arr;
来源：http://tci.chenzaomai.com

[U52] PHP：箭头函数
来源：http://nvm.jyoumei.cn

$double = fn($x) => $x * 2;
来源：http://dag.pycfn.com

[U53] PHP：空合并运算符
来源：http://rdq.cucudq.cn

$v = $a ?? $b ?? "default";
来源：http://tqf.hnqzz.top

[U54] PHP：空安全调用
来源：http://kvj.zhaomingkeji.xyz

$obj?->method()
来源：http://umt.smart0.xyz

[U55] PHP：match 表达式
来源：http://ssy.gogol.net.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ngf.yonumen.top

[U56] PHP：命名参数
来源：http://pic.jyoumei.cn

f(a: 1, b: 2)
来源：http://ych.fengsongda.top

[U57] PHP：字符串插值
来源：http://vnp.daria6918.cn

"值: {$a}"
来源：http://bjz.ivvv.top

[U58] PHP：数组三件套
来源：http://iek.tianlin.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yuw.ydjk.org.cn

[U59] PHP：自定义排序
来源：http://lfn.kuanghao11.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://snz.epnwcf.com

[U60] PHP：JSON 编解码
来源：http://usd.zhaomingkeji.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://brj.ydzc1.top

[U61] PHP：正则
来源：http://czg.hcnkem.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bca.ydzc1.top

[U62] PHP：日期对象
来源：http://mbi.chenlongwang.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wwd.vehdjk.com

[U63] PHP：文件读写
来源：http://puw.xuetiantiany.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hoz.sufxvd.cn

[U64] PHP：目录遍历
来源：http://ors.chenjidiqi.icu

glob("dir/*.php");  scandir("dir");
来源：http://ffl.jinghuilouyu.cn

[U65] PHP：会话
来源：http://tvv.andypj.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://xrv.dashuyun.cn

[U66] PHP：设置 Cookie
来源：http://iuo.pengpengdd.cyou

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://awh.hongshengwenyu.top

[U67] PHP：处理文件上传
来源：http://tbl.zhixingplan.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pqr.fehbvm.com

[U68] PHP：PDO 连接
来源：http://cef.jianghu66.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://enb.hfpthk.cn

[U69] PHP：PDO 预处理
来源：http://vkz.chenlongwang.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gld.snrcjt.cn

[U70] PHP：PDO 事务
来源：http://zzb.xziqi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hpy.daxiang520.top

[U71] PHP：抛出异常
来源：http://afz.fehbvm.com

throw new RuntimeException("失败", 500);
来源：http://ppz.jqgfzy.top

[U72] PHP：写错误日志
来源：http://syz.guannengcc.top

error_log("失败: " . $e->getMessage());
来源：http://lsu.smart0.xyz

[U73] PHP：读取 ini 配置
来源：http://knw.daxiang520.top

parse_ini_file("config.ini", true)
来源：http://uee.nwbrower.top

[U74] PHP：读取环境变量
来源：http://bwe.sweek.top

getenv("APP_ENV") ?: "production"
来源：http://bis.hywenlv.cn

[U75] PHP：依赖注入
来源：http://hiq.zhoulong.xyz

composer require psr/container
来源：http://ale.jinqigfzy.top

[U76] PHP：简单路由
来源：http://lhg.gotoacloud.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qhq.fzhhl.top

[U77] PHP：模板渲染
来源：http://fbc.9152youxi.cn

composer require twig/twig
来源：http://ufz.redwolf501.top

[U78] PHP：单元测试
来源：http://cye.jinyuanbaomall.cn

composer require --dev phpunit/phpunit
来源：http://sle.chenlongwang.top

[U79] PHP：静态分析
来源：http://mji.sufxvd.cn

composer require --dev phpstan/phpstan
来源：http://jog.zhongyouzk.top

[U80] PHP：代码规范修复
来源：http://gps.cashguo.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://xgv.nanxinkj.top

[U81] JS：初始化项目
来源：http://yqn.haohaochexian.top

npm init -y;  npm i express
来源：http://iio.fktsv.cn

[U82] JS：package.json 脚本
来源：http://jmn.cqqwz.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xco.daria6918.cn

[U83] JS：ES Module 导入导出
来源：http://dfr.zhijiandao.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qwa.yuxming.cn

[U84] JS：CommonJS 写法
来源：http://ndn.ywan-chungtsiang.top

module.exports = { a };  const { a } = require("./m");
来源：http://sqz.vqdsnc.cn

[U85] JS：可选链
来源：http://ijw.smart0.xyz

a?.b?.c
来源：http://ikr.bbcook.cn

[U86] JS：空值合并
来源：http://qez.9152youxi.cn

a ?? b
来源：http://fem.tian-w.cn

[U87] JS：解构默认值
来源：http://eep.shangyingyoupin.top

const { a = 1, b = 2 } = obj;
来源：http://zid.xuanzx.com

[U88] JS：对象展开合并
来源：http://mzw.svipenyu.cn

{ ...a, ...b }
来源：http://hnd.guowangkeji.top

[U89] JS：数组去重
来源：http://gfp.yuanzhike.top

[...new Set(arr)]
来源：http://zal.zhiwuduotai.top

[U90] JS：数字数组排序
来源：http://tzr.zdbjq.cn

[...arr].sort((a, b) => a - b)
来源：http://poh.shzxlz.cn

[U91] JS：对象键值遍历
来源：http://kta.ydzc1.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://daf.fktsv.cn

[U92] JS：深拷贝
来源：http://mow.hammf.cn

structuredClone(obj)
来源：http://zfj.chenzaomai.com

[U93] JS：模板字符串
来源：http://nua.sxryk.cn

`共 ${n} 条`
来源：http://epk.hysaishi.cn

[U94] JS：箭头函数
来源：http://ccf.jqgfzy.top

const double = x => x * 2;
来源：http://chh.yj202588.top

[U95] JS：Promise 包装
来源：http://ojw.sufxvd.cn

new Promise((resolve, reject) => {})
来源：http://nzl.nanxuanxn.top

[U96] JS：async/await 与异常
来源：http://hmu.dianchejie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mcd.cqqwz.cn

[U97] JS：并发请求
来源：http://gpu.jinqigufen.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ngx.hongshengwenyu.top

[U98] JS：fetch 带 JSON
来源：http://umf.yueranfly.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cnk.hnxiangtu.top

[U99] JS：事件监听
来源：http://xlm.yj202588.top

el.addEventListener("click", e => {})
来源：http://kzt.yonumen.top

[U100] JS：DOM 查询
来源：http://fab.tanke756.top

document.querySelector(".item")
来源：http://nik.gaohongyu789.top

[U101] JS：classList 操作
来源：http://gmy.shanyushiyangkeji.top

el.classList.toggle("active")
来源：http://ngx.smart0.xyz

[U102] JS：本地存储
来源：http://bpe.xuanzx.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://ahy.cashguo.top

[U103] JS：定时器
来源：http://bay.cashguo.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yus.iojbl.cn

[U104] JS：防抖
来源：http://xsu.shanyushiyangtech.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jsh.zhoulong.xyz

[U105] JS：节流
来源：http://mvc.yongpay.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dox.zycfv.cn

[U106] JS：日期格式化
来源：http://etw.nanxinkj.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tnf.wangshuangyany.cn

[U107] JS：数字千分位
来源：http://lsl.wangdashe.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qfp.meibo888.top

[U108] JS：随机整数
来源：http://lkf.tian-w.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bts.ivvv.top

[U109] JS：数组分组
来源：http://qyc.fanxiaobao.xyz

Object.groupBy(arr, x => x.type)
来源：http://qoe.xuetiantiany.cn

[U110] JS：数组分块
来源：http://zqq.yvedp.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://asq.yonumen.top

[U111] JS：对象转 Map
来源：http://gqs.shanyushiyangtech.top

new Map(Object.entries(obj))
来源：http://igx.chenjidiqi.icu

[U112] JS：字符串补位
来源：http://xmo.meibo888.top

"7".padStart(3, "0")
来源：http://xsl.kuanghao11.cn

[U113] JS：正则替换全部
来源：http://xyd.52xcode.cn

s.replaceAll("a", "b")
来源：http://hgc.tarul.cn

[U114] JS：JSON 深比较
来源：http://emw.aibaodan.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nkg.zhongyouzk.top

[U115] JS：生成 UUID
来源：http://qse.shuidangran.top

crypto.randomUUID()
来源：http://hin.shuidangran.top

[U116] JS：类型检查（JSDoc）
来源：http://tap.ydzc1.top

/** @param {string} name */ function f(name) {}
来源：http://njy.zycfv.cn

[U117] JS：单元测试
来源：http://uim.sxryk.cn

npm i -D vitest;  npx vitest
来源：http://wtw.hysaishi.cn

[U118] JS：开发服务器
来源：http://mub.hesvh.cn

npm i -D vite;  npx vite
来源：http://mwv.jinghuilouyu.cn

[U119] JS：生产构建
来源：http://pcl.jinghuilouyu.cn

npx vite build
来源：http://twi.yuxming.cn

[U120] JS：读取环境变量（Vite）
来源：http://psa.fzhhl.top

import.meta.env.VITE_API_URL
来源：http://zvn.yanxiufei.cn

================================================================================
来源：http://yma.tarul.cn

统计汇总
来源：http://kxj.hammf.cn

================================================================================
来源：http://bvm.aibaodan.cn

按语言统计（条）：
来源：http://nuy.pengpengdd.cyou

Python ......... 252
来源：http://wkw.shangyingyoupin.top

PHP ............ 252
来源：http://wqn.dashuyun.cn

JavaScript ..... 252
来源：http://cpl.ppjwa.cn

TypeScript ..... 212
来源：http://owq.ywan-chungtsiang.top

Java ........... 212
来源：http://kqw.jlsjyb.cn

Go ............. 212
来源：http://pkb.cucudq.cn

Ruby ........... 212
来源：http://skd.xziqi.cn

C# ............. 212
来源：http://hrh.zhongyouzk.top

C .............. 30
来源：http://mrt.guannengcc.top

C++ ............ 30
来源：http://fyo.ivvv.top

SQL ............ 90
来源：http://jsy.aibaodan.cn

Bash ........... 80
来源：http://fwt.hfpthk.cn

Kotlin ......... 15
来源：http://gjp.cucudq.cn

Swift .......... 15
来源：http://mfp.ydzc1.top

Lua ............ 10
来源：http://tsa.zdqjudy.top

Perl ........... 10
来源：http://hmo.shangyingyoupin.top

Scala .......... 10
来源：http://ldg.yuanzhike.top

------------------------------------
来源：http://psx.cucudq.cn

合计 ........... 2106 条
来源：http://ivu.hnxiangtu.top

按章节统计：
来源：http://cor.chenjidiqi.icu

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ecw.chenjidiqi.icu

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pqy.daxiang520.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kdo.cqqwz.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gfw.iojbl.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tyy.316326.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kau.nanxinkj.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ten.xziqi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://duy.zhixingplan.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kxj.aibaodan.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://eep.kuanghao11.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lwy.andypj.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ort.hysaishi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://anu.hesvh.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lqv.xuanzx.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yhm.svipenyu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ika.jyoumei.cn

Q SQL 专题                              90
来源：http://edz.pycfn.com

R Bash 专题                             80
来源：http://ejk.9152youxi.cn

S C / C++ 专题                          60
来源：http://ucm.shanyushiyangtech.top

T 其他语言补充                          60
来源：http://kib.yuxming.cn

U 高频实用片段                         120
来源：http://bhd.pycfn.com

------------------------------------
来源：http://isg.yj202588.top

合计                                  2106 条
来源：http://bng.shanyushiyangkeji.top

--------------------------------------------------------------------------------
来源：http://ief.havefunace.top

使用提醒
来源：http://ffw.chenjidiqi.icu

--------------------------------------------------------------------------------
来源：http://jxy.xylfe.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://flz.pengpengdd.cyou

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xwj.jianghu66.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://kkq.c1oappe.top

在旧版本上使用前请先确认语法支持情况。
来源：http://aua.ctjpmb.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://giz.cheryme.top

—— 文件结束 ——
来源：http://zdx.ivvv.top

================================================================================
来源：http://sap.uphjek.com

程序语言常见例子速查手册（2024 版）
来源：http://ngr.zhijiandao.cn

Common Programming Examples Cheat Book
来源：http://iaw.svipenyu.cn

================================================================================
来源：http://gxm.hnxiangtu.top

【收录内容】
来源：http://obx.ywan-chungtsiang.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://gpf.andypj.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ieb.ydzc1.top

SQL · Bash · C · C++
来源：http://foc.gzhubu.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://bgj.sysykeji.top

【使用说明】
来源：http://vck.xingfuxueyuan.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ack.yfazqb.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dks.xylfe.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://prg.xziqi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wgn.zhijiandao.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://qae.jinghuilouyu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kob.9152youxi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ucm.shzxlz.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://psx.ydzc1.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://uvm.shanyushiyangkeji.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pzd.aibaodan.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kus.fzhhl.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nqx.daxiang520.top

【文件统计】
来源：http://hnu.zhijiandao.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xjq.guowangkeji.top

--------------------------------------------------------------------------------
来源：http://alw.feifeiyinyue.top

目  录
来源：http://sdq.fktsv.cn

--------------------------------------------------------------------------------
来源：http://osj.hfpthk.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dlt.sufxvd.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://pyh.nanxinkj.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wuu.hongshengwenyu.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://gtq.ybcxt.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://crw.xuanzx.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wcy.ywan-chungtsiang.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://pqp.quarkkingdee.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gvg.wangshuangyany.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://sge.nwbrower.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mrm.gogol.net.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xmp.zdqjudy.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zrj.bbcook.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rbv.ydjk.org.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vof.quarkkingdee.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hhy.316326.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://uaz.0kj1m.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zwq.gzhubu.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://owh.dashuyun.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://enm.snrcjt.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nle.nanxuanxn.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zbn.zhongyouzk.top

================================================================================
来源：http://ilr.zycfv.cn

A. 基础语法与类型
来源：http://ytu.tanke756.top

================================================================================
来源：http://cqc.yuxming.cn

[A01] Hello World
来源：http://lsn.hnqzz.top

Py:   print("Hello, World!")
来源：http://jrj.smart0.xyz

PHP:  echo "Hello, World!";
来源：http://hqk.jqgufenzy.top

JS:   console.log("Hello, World!");
来源：http://gaa.quarkkingdee.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rqh.jyoumei.cn

Java: System.out.println("Hello, World!");
来源：http://ikm.cdnleiting.top

Go:   fmt.Println("Hello, World!")
来源：http://wsr.daria6918.cn

Ruby: puts "Hello, World!"
来源：http://onn.guowangkeji.top

C#:   Console.WriteLine("Hello, World!");
来源：http://bnp.ybcxt.top

[A02] 变量声明与赋值
来源：http://nkx.hnxiangtu.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xgl.jlsjyb.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ito.nanxinkj.top

JS:   let name = "Alex"; const age = 20;
来源：http://xnn.shanyushiyangtech.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nnz.c1oappe.top

Java: String name = "Alex"; int age = 20;
来源：http://ksh.zdqjudy.top

Go:   name := "Alex"; age := 20
来源：http://zhs.52xcode.cn

Ruby: name = "Alex"; age = 20
来源：http://yyo.uphjek.com

C#:   string name = "Alex"; int age = 20;
来源：http://pjx.cashguo.top

[A03] 常量定义
来源：http://bha.guannengcc.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://sna.ydjk.org.cn

PHP:  const PI = 3.14159;
来源：http://gux.ywan-chungtsiang.top

JS:   const PI = 3.14159;
来源：http://jxr.feifeiyinyue.top

TS:   const PI: number = 3.14159;
来源：http://qvz.jqgfzy.top

Java: static final double PI = 3.14159;
来源：http://frs.shuidangran.top

Go:   const PI = 3.14159
来源：http://qzb.cucudq.cn

Ruby: PI = 3.14159
来源：http://pay.ywan-chungtsiang.top

C#:   const double PI = 3.14159;
来源：http://aaf.fengsongda.top

[A04] 判断变量类型
来源：http://cdi.ybcxt.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://wqq.sxryk.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://txs.hongshengwenyu.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ifl.cheryme.top

TS:   typeof x; x instanceof Date
来源：http://nhz.kuanghao11.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zpr.fzhhl.top

Go:   reflect.TypeOf(x).Name()
来源：http://tih.jinqigufen.top

Ruby: x.class; x.is_a?(Integer)
来源：http://bgy.yvedp.cn

C#:   x.GetType().Name; x is int
来源：http://rzc.yj202588.top

[A05] 整数除法与取模
来源：http://kxo.svipenyu.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hft.ppjwa.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://iqx.jinyuanbaomall.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jil.ywan-chungtsiang.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gdu.hysaishi.cn

Java: 7 / 2; 7 % 2
来源：http://tdc.sufxvd.cn

Go:   7 / 2; 7 % 2
来源：http://cee.havefunace.top

Ruby: 7 / 2; 7 % 2
来源：http://cda.ybcxt.top

C#:   7 / 2; 7 % 2
来源：http://quv.xinyue.icu

[A06] 字符串转数字
来源：http://obq.andypj.xyz

Py:   int("42"); float("3.14")
来源：http://qsy.zycfv.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ens.redwolf501.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gmb.pycfn.com

TS:   parseInt("42", 10); Number("42")
来源：http://vfq.yuanzhike.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mmg.zhongyouzk.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xva.zycfv.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://lqk.fanxiaobao.xyz


<!-- 参考信息 -->