代发 wailian999

[U59] PHP：自定义排序
来源：http://gkt.tian-w.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zzv.chenzaomai.com

[U60] PHP：JSON 编解码
来源：http://lsm.meibo888.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yru.sjlbkw.cn

[U61] PHP：正则
来源：http://mom.hnqzz.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://azm.zhaomingkeji.xyz

[U62] PHP：日期对象
来源：http://qap.wangshuangyany.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zcb.gotoacloud.top

[U63] PHP：文件读写
来源：http://fmb.fanxiaobao.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mgt.ybcxt.top

[U64] PHP：目录遍历
来源：http://zpb.cqqwz.cn

glob("dir/*.php");  scandir("dir");
来源：http://rcw.snrcjt.cn

[U65] PHP：会话
来源：http://gda.zhixingplan.top

session_start();  $_SESSION["uid"] = 1;
来源：http://rgi.uphjek.com

[U66] PHP：设置 Cookie
来源：http://tzn.zhiwuduotai.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hhf.hysaishi.cn

[U67] PHP：处理文件上传
来源：http://tpk.fzhhl.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cpn.gotoacloud.top

[U68] PHP：PDO 连接
来源：http://nap.jlsjyb.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vva.ydzc1.top

[U69] PHP：PDO 预处理
来源：http://qpl.nanxinkj.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dvh.zhongyouzk.top

[U70] PHP：PDO 事务
来源：http://ltc.redwolf501.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gcu.cucudq.cn

[U71] PHP：抛出异常
来源：http://yil.nwbrower.top

throw new RuntimeException("失败", 500);
来源：http://sfr.andypj.xyz

[U72] PHP：写错误日志
来源：http://afw.yangfankeji.com

error_log("失败: " . $e->getMessage());
来源：http://ubs.jiagoushi.top

[U73] PHP：读取 ini 配置
来源：http://ukl.shanyushiyangtech.top

parse_ini_file("config.ini", true)
来源：http://qsd.gotoacloud.top

[U74] PHP：读取环境变量
来源：http://ikk.zhoulong.xyz

getenv("APP_ENV") ?: "production"
来源：http://vuc.yanxiufei.cn

[U75] PHP：依赖注入
来源：http://omy.epnwcf.com

composer require psr/container
来源：http://ryp.svipenyu.cn

[U76] PHP：简单路由
来源：http://spw.yfazqb.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hrg.daria6918.cn

[U77] PHP：模板渲染
来源：http://xdp.yvedp.cn

composer require twig/twig
来源：http://wvk.jinyuanbaomall.cn

[U78] PHP：单元测试
来源：http://mhs.cdnleiting.top

composer require --dev phpunit/phpunit
来源：http://rlw.aibaodan.cn

[U79] PHP：静态分析
来源：http://dyf.yanxiufei.cn

composer require --dev phpstan/phpstan
来源：http://qrb.9152youxi.cn

[U80] PHP：代码规范修复
来源：http://xlc.quarkkingdee.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://uev.cqqwz.cn

[U81] JS：初始化项目
来源：http://xvc.ydzc1.top

npm init -y;  npm i express
来源：http://xgt.shangyingyoupin.top

[U82] JS：package.json 脚本
来源：http://qgt.gzhubu.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nig.sjlbkw.cn

[U83] JS：ES Module 导入导出
来源：http://pcw.xylfe.cn

export const a = 1;  import { a } from "./m.js";
来源：http://rzb.bjfxy.top

[U84] JS：CommonJS 写法
来源：http://yjj.sysykeji.top

module.exports = { a };  const { a } = require("./m");
来源：http://pow.dashuyun.cn

[U85] JS：可选链
来源：http://jib.ctjpmb.com

a?.b?.c
来源：http://uoj.uphjek.com

[U86] JS：空值合并
来源：http://tri.ybcxt.top

a ?? b
来源：http://wvy.9152youxi.cn

[U87] JS：解构默认值
来源：http://evr.tanke756.top

const { a = 1, b = 2 } = obj;
来源：http://hyi.ywan-chungtsiang.top

[U88] JS：对象展开合并
来源：http://ilf.uphjek.com

{ ...a, ...b }
来源：http://leg.haohaochexian.top

[U89] JS：数组去重
来源：http://jnc.cqqwz.cn

[...new Set(arr)]
来源：http://kfy.yueranfly.top

[U90] JS：数字数组排序
来源：http://xae.birdmap.top

[...arr].sort((a, b) => a - b)
来源：http://glr.zhiwuduotai.top

[U91] JS：对象键值遍历
来源：http://jfa.pengpengdd.cyou

Object.entries(obj).forEach(([k, v]) => {});
来源：http://epj.gaohongyu789.top

[U92] JS：深拷贝
来源：http://lzz.316326.xyz

structuredClone(obj)
来源：http://sqt.hywenlv.cn

[U93] JS：模板字符串
来源：http://vjp.dashuyun.cn

`共 ${n} 条`
来源：http://dqq.snrcjt.cn

[U94] JS：箭头函数
来源：http://nfn.fehbvm.com

const double = x => x * 2;
来源：http://pwt.andypj.xyz

[U95] JS：Promise 包装
来源：http://yje.316326.xyz

new Promise((resolve, reject) => {})
来源：http://ugo.gotoacloud.top

[U96] JS：async/await 与异常
来源：http://hxz.wangdashe.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qwx.zhijiandao.cn

[U97] JS：并发请求
来源：http://wat.yueranfly.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://edi.9152youxi.cn

[U98] JS：fetch 带 JSON
来源：http://jhq.bjfxy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dgx.snrcjt.cn

[U99] JS：事件监听
来源：http://hvk.ydzc1.top

el.addEventListener("click", e => {})
来源：http://gte.hesvh.cn

[U100] JS：DOM 查询
来源：http://ebk.epnwcf.com

document.querySelector(".item")
来源：http://jhz.tianlin.xyz

[U101] JS：classList 操作
来源：http://kpa.hesvh.cn

el.classList.toggle("active")
来源：http://tjl.epnwcf.com

[U102] JS：本地存储
来源：http://hkz.9152youxi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://hib.ehwqpu.com

[U103] JS：定时器
来源：http://mno.redwolf501.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://obh.yueranfly.top

[U104] JS：防抖
来源：http://uim.zhoulong.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bkp.andypj.xyz

[U105] JS：节流
来源：http://hly.chenlongwang.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://diq.jinqigfzy.top

[U106] JS：日期格式化
来源：http://vat.sweek.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ivf.jiagoushi.top

[U107] JS：数字千分位
来源：http://poq.haohaochexian.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xau.cdnleiting.top

[U108] JS：随机整数
来源：http://lkx.gzhubu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mls.redwolf501.top

[U109] JS：数组分组
来源：http://lhu.dashuyun.cn

Object.groupBy(arr, x => x.type)
来源：http://oyo.cashguo.top

[U110] JS：数组分块
来源：http://rln.guowangkeji.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://oqz.zhoulong.xyz

[U111] JS：对象转 Map
来源：http://dyv.gaohongyu789.top

new Map(Object.entries(obj))
来源：http://ktp.hcnkem.com

[U112] JS：字符串补位
来源：http://rnb.hnqzz.top

"7".padStart(3, "0")
来源：http://dkq.aizwys.cn

[U113] JS：正则替换全部
来源：http://utr.aizwys.cn

s.replaceAll("a", "b")
来源：http://mfa.haohaochexian.top

[U114] JS：JSON 深比较
来源：http://lrf.dashuyun.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://kwp.9152youxi.cn

[U115] JS：生成 UUID
来源：http://neo.havefunace.top

crypto.randomUUID()
来源：http://cza.yj20258888.top

[U116] JS：类型检查（JSDoc）
来源：http://ofr.zhongyouzk.top

/** @param {string} name */ function f(name) {}
来源：http://iol.epnwcf.com

[U117] JS：单元测试
来源：http://wdc.ctjpmb.com

npm i -D vitest;  npx vitest
来源：http://dku.yueranfly.top

[U118] JS：开发服务器
来源：http://pky.chenjidiqi.icu

npm i -D vite;  npx vite
来源：http://zbm.316326.xyz

[U119] JS：生产构建
来源：http://wob.yj20258.top

npx vite build
来源：http://rfc.shanyushiyangtech.top

[U120] JS：读取环境变量（Vite）
来源：http://kca.chenlongwang.top

import.meta.env.VITE_API_URL
来源：http://dcr.chenzaomai.com

================================================================================
来源：http://jxy.tarul.cn

统计汇总
来源：http://zvc.zhaomingkeji.xyz

================================================================================
来源：http://gqg.hysaishi.cn

按语言统计（条）：
来源：http://ujo.pengpengdd.cyou

Python ......... 252
来源：http://ldt.hnxiangtu.top

PHP ............ 252
来源：http://bli.fktsv.cn

JavaScript ..... 252
来源：http://agz.svipenyu.cn

TypeScript ..... 212
来源：http://gdc.fktsv.cn

Java ........... 212
来源：http://yei.nwbrower.top

Go ............. 212
来源：http://eaj.sjlbkw.cn

Ruby ........... 212
来源：http://civ.ydjk.org.cn

C# ............. 212
来源：http://hti.xuetiantiany.cn

C .............. 30
来源：http://bzr.daria6918.cn

C++ ............ 30
来源：http://reb.shzxlz.cn

SQL ............ 90
来源：http://xtp.ehwqpu.com

Bash ........... 80
来源：http://wek.jinqigufen.top

Kotlin ......... 15
来源：http://jts.dashuyun.cn

Swift .......... 15
来源：http://utj.meibo888.top

Lua ............ 10
来源：http://vtq.daxiang520.top

Perl ........... 10
来源：http://uie.hysaishi.cn

Scala .......... 10
来源：http://zbm.fengsongda.top

------------------------------------
来源：http://omp.vqdsnc.cn

合计 ........... 2106 条
来源：http://ixb.fengsongda.top

按章节统计：
来源：http://fpj.jinghuilouyu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yhp.guowangkeji.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xzr.guannengcc.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wau.redwolf501.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nwg.aibaodan.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hqs.gogol.net.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rlm.chenlongwang.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tif.nwbrower.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lhl.gogol.net.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gbo.ctjpmb.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://aug.tian-w.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bhu.zhongyouzk.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://eii.iojbl.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://geg.zhijiandao.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dph.shuidangran.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://sin.xuetiantiany.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tbm.dashuyun.cn

Q SQL 专题                              90
来源：http://qwa.cqqwz.cn

R Bash 专题                             80
来源：http://lnp.havefunace.top

S C / C++ 专题                          60
来源：http://wok.yongpay.top

T 其他语言补充                          60
来源：http://duf.svipenyu.cn

U 高频实用片段                         120
来源：http://ccb.ydzc1.top

------------------------------------
来源：http://kks.gotoacloud.top

合计                                  2106 条
来源：http://ezq.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://crf.jqgfzy.top

使用提醒
来源：http://sqg.gotoacloud.top

--------------------------------------------------------------------------------
来源：http://lco.epnwcf.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xmv.meibo888.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fwq.shuidangran.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yot.ydjk.org.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://sfd.hnxiangtu.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fii.yuanzhike.top

—— 文件结束 ——
来源：http://ijk.yueranfly.top

================================================================================
来源：http://qaq.hnqzz.top

程序语言常见例子速查手册（2024 版）
来源：http://ryn.ivvv.top

Common Programming Examples Cheat Book
来源：http://ckc.haohaochexian.top

================================================================================
来源：http://mdk.gaohongyu789.top

【收录内容】
来源：http://apv.0kj1m.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ynq.yfazqb.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dey.shanyushiyangtech.top

SQL · Bash · C · C++
来源：http://mur.zhiwuduotai.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rpv.ehwqpu.com

【使用说明】
来源：http://zah.jiagoushi.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://iui.xziqi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zwa.svipenyu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lma.xziqi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ccf.andypj.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://xxc.guannengcc.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tcy.shanyushiyangkeji.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ofu.zhoulong.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://asq.yongpay.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hia.sweek.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zrr.ydjk.org.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://iwr.yvedp.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hej.cheryme.top

【文件统计】
来源：http://mng.xinyue.icu

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yye.pengpengdd.cyou

--------------------------------------------------------------------------------
来源：http://fbu.jqgfzy.top

目  录
来源：http://fsi.sysykeji.top

--------------------------------------------------------------------------------
来源：http://jbo.shanyushiyangtech.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bwj.316326.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tsr.zdqjudy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dof.zhaomingkeji.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jcg.tanke756.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://pvu.wangshuangyany.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://shj.zdqjudy.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://tbk.daxiang520.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ehx.jinyuanbaomall.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lvk.yonumen.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yan.bbcook.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://whr.andypj.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://luf.wangdashe.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://noh.xingfuxueyuan.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://apj.ywan-chungtsiang.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ruz.jyoumei.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qkm.tianlin.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wcu.andypj.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://vkq.316326.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jgy.ppjwa.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://uxe.cdnleiting.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wvm.hesvh.cn

================================================================================
来源：http://aoz.xuetiantiany.cn

A. 基础语法与类型
来源：http://jup.epnwcf.com

================================================================================
来源：http://ity.aibaodan.cn

[A01] Hello World
来源：http://mnk.xuanzx.com

Py:   print("Hello, World!")
来源：http://bvd.9152youxi.cn

PHP:  echo "Hello, World!";
来源：http://thk.xylfe.cn

JS:   console.log("Hello, World!");
来源：http://mfr.jinyuanbaomall.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://plb.cdnleiting.top

Java: System.out.println("Hello, World!");
来源：http://pql.shzxlz.cn

Go:   fmt.Println("Hello, World!")
来源：http://qof.zdbjq.cn

Ruby: puts "Hello, World!"
来源：http://sko.quarkkingdee.top

C#:   Console.WriteLine("Hello, World!");
来源：http://hcs.cdnleiting.top

[A02] 变量声明与赋值
来源：http://hfa.zhoulong.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://plz.hysaishi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://pqf.9152youxi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://dmy.havefunace.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nse.cqqwz.cn

Java: String name = "Alex"; int age = 20;
来源：http://hya.hcnkem.com

Go:   name := "Alex"; age := 20
来源：http://nvb.52xcode.cn

Ruby: name = "Alex"; age = 20
来源：http://vcp.pengpengdd.cyou

C#:   string name = "Alex"; int age = 20;
来源：http://hsv.nwbrower.top

[A03] 常量定义
来源：http://ptz.aibaodan.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qjd.ivvv.top

PHP:  const PI = 3.14159;
来源：http://luc.snrcjt.cn

JS:   const PI = 3.14159;
来源：http://lcs.birdmap.top

TS:   const PI: number = 3.14159;
来源：http://dgb.dashuyun.cn

Java: static final double PI = 3.14159;
来源：http://dcd.pycfn.com

Go:   const PI = 3.14159
来源：http://czy.zhijiandao.cn

Ruby: PI = 3.14159
来源：http://qlz.jlsjyb.cn

C#:   const double PI = 3.14159;
来源：http://kyy.shanyushiyangtech.top

[A04] 判断变量类型
来源：http://cyn.zdqjudy.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://bed.tian-w.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wzm.dashuyun.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bne.yfazqb.com

TS:   typeof x; x instanceof Date
来源：http://rsw.daria6918.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://esb.xingfuxueyuan.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://uru.zhaomingkeji.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://qeq.xuetiantiany.cn

C#:   x.GetType().Name; x is int
来源：http://qbn.aibaodan.cn

[A05] 整数除法与取模
来源：http://bpb.yuanzhike.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hvm.nanxinkj.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://jiw.xziqi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tma.dianchejie.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fdf.kuanghao11.cn

Java: 7 / 2; 7 % 2
来源：http://dzt.gaohongyu789.top

Go:   7 / 2; 7 % 2
来源：http://eby.guannengcc.top

Ruby: 7 / 2; 7 % 2
来源：http://edk.epnwcf.com

C#:   7 / 2; 7 % 2
来源：http://kjl.daria6918.cn

[A06] 字符串转数字
来源：http://atq.zdqjudy.top

Py:   int("42"); float("3.14")
来源：http://tsx.birdmap.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zev.cheryme.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lxv.yangfankeji.com

TS:   parseInt("42", 10); Number("42")
来源：http://fzx.hysaishi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fyl.ppjwa.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://okp.jinqigfzy.top

Ruby: "42".to_i; "3.14".to_f
来源：http://brr.ybcxt.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ueq.shangyingyoupin.top

[A07] 数字转字符串
来源：http://jll.hfpthk.cn

Py:   str(42)
来源：http://tij.redwolf501.top

PHP:  (string) 42; strval(42)
来源：http://rqk.52xcode.cn

JS:   String(42); (42).toString()
来源：http://sgh.jinqigfzy.top

TS:   String(42)
来源：http://mdp.andypj.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://jcw.hcnkem.com

Go:   strconv.Itoa(42)
来源：http://vbf.gogol.net.cn

Ruby: 42.to_s
来源：http://gqj.9152youxi.cn

C#:   42.ToString()
来源：http://eik.hongshengwenyu.top

[A08] 取整与四舍五入
来源：http://wpo.fktsv.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ftw.guannengcc.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ztf.iojbl.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mlw.yonumen.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://eja.jlsjyb.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lxb.yvedp.cn


<!-- 参考信息 -->