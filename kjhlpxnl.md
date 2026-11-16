代发 wailian999

[U53] PHP：空合并运算符
来源：http://zah.316326.xyz

$v = $a ?? $b ?? "default";
来源：http://xag.zhongyouzk.top

[U54] PHP：空安全调用
来源：http://cwd.guannengcc.top

$obj?->method()
来源：http://frr.cashguo.top

[U55] PHP：match 表达式
来源：http://vfb.quarkkingdee.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ogl.guannengcc.top

[U56] PHP：命名参数
来源：http://jex.zhijiandao.cn

f(a: 1, b: 2)
来源：http://qkr.yanxiufei.cn

[U57] PHP：字符串插值
来源：http://zio.hcnkem.com

"值: {$a}"
来源：http://npj.jiagoushi.top

[U58] PHP：数组三件套
来源：http://jwj.shanyushiyangkeji.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bhl.guowangkeji.top

[U59] PHP：自定义排序
来源：http://hht.sweek.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jgr.zhiwuduotai.top

[U60] PHP：JSON 编解码
来源：http://zbk.cdnleiting.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gff.havefunace.top

[U61] PHP：正则
来源：http://asl.redwolf501.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jfh.feifeiyinyue.top

[U62] PHP：日期对象
来源：http://aah.jqgfzy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wvj.jqgfzy.top

[U63] PHP：文件读写
来源：http://urr.cheryme.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://aab.yj202588.top

[U64] PHP：目录遍历
来源：http://xyn.yuxming.cn

glob("dir/*.php");  scandir("dir");
来源：http://lok.fehbvm.com

[U65] PHP：会话
来源：http://ytm.yongpay.top

session_start();  $_SESSION["uid"] = 1;
来源：http://baw.dashuyun.cn

[U66] PHP：设置 Cookie
来源：http://xdc.fktsv.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dmw.yongpay.top

[U67] PHP：处理文件上传
来源：http://ssr.guannengcc.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qfa.feifeiyinyue.top

[U68] PHP：PDO 连接
来源：http://vqm.hnxiangtu.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vyh.hysaishi.cn

[U69] PHP：PDO 预处理
来源：http://yjj.0kj1m.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hdv.aibaodan.cn

[U70] PHP：PDO 事务
来源：http://abu.hnqzz.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qbu.chenzaomai.com

[U71] PHP：抛出异常
来源：http://sin.uphjek.com

throw new RuntimeException("失败", 500);
来源：http://klz.xingfuxueyuan.xyz

[U72] PHP：写错误日志
来源：http://gaw.zhongyouzk.top

error_log("失败: " . $e->getMessage());
来源：http://eac.cashguo.top

[U73] PHP：读取 ini 配置
来源：http://xzk.tian-w.cn

parse_ini_file("config.ini", true)
来源：http://lcf.vehdjk.com

[U74] PHP：读取环境变量
来源：http://qmy.shzxlz.cn

getenv("APP_ENV") ?: "production"
来源：http://ggw.jqgufenzy.top

[U75] PHP：依赖注入
来源：http://jzb.fktsv.cn

composer require psr/container
来源：http://yzm.yueranfly.top

[U76] PHP：简单路由
来源：http://jlz.bjfxy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bqn.snrcjt.cn

[U77] PHP：模板渲染
来源：http://abn.guannengcc.top

composer require twig/twig
来源：http://zak.wangshuangyany.cn

[U78] PHP：单元测试
来源：http://tlu.zhaomingkeji.xyz

composer require --dev phpunit/phpunit
来源：http://ajh.vehdjk.com

[U79] PHP：静态分析
来源：http://qyo.hongshengwenyu.top

composer require --dev phpstan/phpstan
来源：http://jao.cqqwz.cn

[U80] PHP：代码规范修复
来源：http://ayp.nanxuanxn.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://dye.svipenyu.cn

[U81] JS：初始化项目
来源：http://aeh.shzxlz.cn

npm init -y;  npm i express
来源：http://kql.zdqjudy.top

[U82] JS：package.json 脚本
来源：http://ngl.jianghu66.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ion.andypj.xyz

[U83] JS：ES Module 导入导出
来源：http://eea.yuxming.cn

export const a = 1;  import { a } from "./m.js";
来源：http://pga.nwbrower.top

[U84] JS：CommonJS 写法
来源：http://bmq.chenjidiqi.icu

module.exports = { a };  const { a } = require("./m");
来源：http://eix.ydzc1.top

[U85] JS：可选链
来源：http://prt.zdbjq.cn

a?.b?.c
来源：http://htu.cheryme.top

[U86] JS：空值合并
来源：http://uah.bbcook.cn

a ?? b
来源：http://qzc.vqdsnc.cn

[U87] JS：解构默认值
来源：http://lxn.jianghu66.top

const { a = 1, b = 2 } = obj;
来源：http://qqd.gogol.net.cn

[U88] JS：对象展开合并
来源：http://eri.jqgufenzy.top

{ ...a, ...b }
来源：http://zoj.fehbvm.com

[U89] JS：数组去重
来源：http://bob.mhx1999.top

[...new Set(arr)]
来源：http://ibh.svipenyu.cn

[U90] JS：数字数组排序
来源：http://vqa.smart0.xyz

[...arr].sort((a, b) => a - b)
来源：http://kli.feifeiyinyue.top

[U91] JS：对象键值遍历
来源：http://hze.ydjk.org.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://scg.cucudq.cn

[U92] JS：深拷贝
来源：http://djs.jinqigfzy.top

structuredClone(obj)
来源：http://mih.jinyuanbaomall.cn

[U93] JS：模板字符串
来源：http://awf.shanyushiyangkeji.top

`共 ${n} 条`
来源：http://ile.c1oappe.top

[U94] JS：箭头函数
来源：http://kmk.meibo888.top

const double = x => x * 2;
来源：http://eme.316326.xyz

[U95] JS：Promise 包装
来源：http://niu.chenjidiqi.icu

new Promise((resolve, reject) => {})
来源：http://uta.hesvh.cn

[U96] JS：async/await 与异常
来源：http://poc.yfazqb.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cnk.gaohongyu789.top

[U97] JS：并发请求
来源：http://fvg.shangyingyoupin.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://owh.hfpthk.cn

[U98] JS：fetch 带 JSON
来源：http://fib.xuanzx.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ase.316326.xyz

[U99] JS：事件监听
来源：http://fhm.nanxuanxn.top

el.addEventListener("click", e => {})
来源：http://app.gotoacloud.top

[U100] JS：DOM 查询
来源：http://wla.hesvh.cn

document.querySelector(".item")
来源：http://pym.sufxvd.cn

[U101] JS：classList 操作
来源：http://lmp.hammf.cn

el.classList.toggle("active")
来源：http://wmf.nanxuanxn.top

[U102] JS：本地存储
来源：http://lel.c1oappe.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://suf.yuxming.cn

[U103] JS：定时器
来源：http://uep.zhixingplan.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sog.hysaishi.cn

[U104] JS：防抖
来源：http://eqe.316326.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tyu.jianghu66.top

[U105] JS：节流
来源：http://ffy.hcnkem.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qmq.xylfe.cn

[U106] JS：日期格式化
来源：http://qwm.wangshuangyany.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bsi.hnxiangtu.top

[U107] JS：数字千分位
来源：http://tjk.zdqjudy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ttm.ppjwa.cn

[U108] JS：随机整数
来源：http://cnr.shanyushiyangkeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://aws.kuanghao11.cn

[U109] JS：数组分组
来源：http://kws.ydzc1.top

Object.groupBy(arr, x => x.type)
来源：http://nyj.hywenlv.cn

[U110] JS：数组分块
来源：http://uti.sxryk.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sbk.ybcxt.top

[U111] JS：对象转 Map
来源：http://bde.quarkkingdee.top

new Map(Object.entries(obj))
来源：http://xtp.ctjpmb.com

[U112] JS：字符串补位
来源：http://fgx.zhaomingkeji.xyz

"7".padStart(3, "0")
来源：http://fix.zhaomingkeji.xyz

[U113] JS：正则替换全部
来源：http://sgz.zhaomingkeji.xyz

s.replaceAll("a", "b")
来源：http://rnj.xuanzx.com

[U114] JS：JSON 深比较
来源：http://voo.yuxming.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://srv.0kj1m.cn

[U115] JS：生成 UUID
来源：http://kjo.havefunace.top

crypto.randomUUID()
来源：http://ptc.epnwcf.com

[U116] JS：类型检查（JSDoc）
来源：http://uea.pengpengdd.cyou

/** @param {string} name */ function f(name) {}
来源：http://qul.aizwys.cn

[U117] JS：单元测试
来源：http://isy.pycfn.com

npm i -D vitest;  npx vitest
来源：http://vvz.zhixingplan.top

[U118] JS：开发服务器
来源：http://xxi.cheryme.top

npm i -D vite;  npx vite
来源：http://lmn.cqqwz.cn

[U119] JS：生产构建
来源：http://nxl.snrcjt.cn

npx vite build
来源：http://ljv.jqgfzy.top

[U120] JS：读取环境变量（Vite）
来源：http://mmm.jiagoushi.top

import.meta.env.VITE_API_URL
来源：http://vvi.xuanzx.com

================================================================================
来源：http://oen.ppjwa.cn

统计汇总
来源：http://fxi.ctjpmb.com

================================================================================
来源：http://jul.dashuyun.cn

按语言统计（条）：
来源：http://vir.jinyuanbaomall.cn

Python ......... 252
来源：http://noc.xylfe.cn

PHP ............ 252
来源：http://guj.cheryme.top

JavaScript ..... 252
来源：http://mbf.fzhhl.top

TypeScript ..... 212
来源：http://zoc.ppjwa.cn

Java ........... 212
来源：http://vtr.xingfuxueyuan.xyz

Go ............. 212
来源：http://azk.sysykeji.top

Ruby ........... 212
来源：http://csm.fanxiaobao.xyz

C# ............. 212
来源：http://usv.fanxiaobao.xyz

C .............. 30
来源：http://rqx.yuanzhike.top

C++ ............ 30
来源：http://hvg.nanxuanxn.top

SQL ............ 90
来源：http://cbo.tarul.cn

Bash ........... 80
来源：http://tet.sxryk.cn

Kotlin ......... 15
来源：http://ifz.shzxlz.cn

Swift .......... 15
来源：http://vfz.jiagoushi.top

Lua ............ 10
来源：http://zor.gaohongyu789.top

Perl ........... 10
来源：http://ygu.zdqjudy.top

Scala .......... 10
来源：http://xjg.ctjpmb.com

------------------------------------
来源：http://evv.bjfxy.top

合计 ........... 2106 条
来源：http://kmi.wangshuangyany.cn

按章节统计：
来源：http://khh.jyoumei.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://frd.zycfv.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jpn.0kj1m.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ilx.hnxiangtu.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://iil.xinyue.icu

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zhb.svipenyu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://skh.svipenyu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gpq.hywenlv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://spw.xuanzx.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pqn.hongshengwenyu.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ccm.yj20258.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hwk.tarul.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://bnt.shanyushiyangtech.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kyr.meibo888.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fau.shanyushiyangkeji.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://whz.jinqigfzy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://aos.jlsjyb.cn

Q SQL 专题                              90
来源：http://abz.yanxiufei.cn

R Bash 专题                             80
来源：http://gwe.ivvv.top

S C / C++ 专题                          60
来源：http://hss.jyoumei.cn

T 其他语言补充                          60
来源：http://igi.yonumen.top

U 高频实用片段                         120
来源：http://toc.zhijiandao.cn

------------------------------------
来源：http://dkk.cheryme.top

合计                                  2106 条
来源：http://czw.hammf.cn

--------------------------------------------------------------------------------
来源：http://wfk.birdmap.top

使用提醒
来源：http://oor.yvedp.cn

--------------------------------------------------------------------------------
来源：http://suq.hywenlv.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://izg.ivvv.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rbh.yj20258.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mju.birdmap.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ltc.jinqigufen.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nwj.quarkkingdee.top

—— 文件结束 ——
来源：http://yue.pengpengdd.cyou

================================================================================
来源：http://psb.sjlbkw.cn

程序语言常见例子速查手册（2024 版）
来源：http://rgo.nwbrower.top

Common Programming Examples Cheat Book
来源：http://vae.aibaodan.cn

================================================================================
来源：http://kjd.jinyuanbaomall.cn

【收录内容】
来源：http://ann.redwolf501.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ozf.chenzaomai.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://llv.ivvv.top

SQL · Bash · C · C++
来源：http://gfo.epnwcf.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://twv.tanke756.top

【使用说明】
来源：http://zok.snrcjt.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://oay.nanxuanxn.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qve.zhengqikj.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://cvw.feifeiyinyue.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vaj.pengpengdd.cyou

Bash:  Shell         C:     C             C++:   C++
来源：http://cgi.hywenlv.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xad.shangyingyoupin.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ylh.cdnleiting.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rsr.jinyuanbaomall.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wsi.nwbrower.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nsi.yuxming.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dep.sweek.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ukw.zdqjudy.top

【文件统计】
来源：http://xjg.shanyushiyangkeji.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vbq.svipenyu.cn

--------------------------------------------------------------------------------
来源：http://cel.cqqwz.cn

目  录
来源：http://uwl.yj20258.top

--------------------------------------------------------------------------------
来源：http://qkx.tian-w.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hwx.feifeiyinyue.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://uww.fanxiaobao.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zas.zdqjudy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://icj.pycfn.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ilr.yj202588.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://srh.hysaishi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hbf.zhengqikj.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qnr.tarul.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://efh.hammf.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://spl.cheryme.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://lhr.bbcook.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ltb.haohaochexian.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://avn.c1oappe.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://oxc.tarul.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fmw.ctjpmb.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://isd.ydzc1.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://egj.hcnkem.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://msp.xziqi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hjf.wangdashe.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://sns.zhaomingkeji.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rfr.ehwqpu.com

================================================================================
来源：http://dfi.iojbl.cn

A. 基础语法与类型
来源：http://szs.wangdashe.top

================================================================================
来源：http://qzi.zhaomingkeji.xyz

[A01] Hello World
来源：http://cju.zhiwuduotai.top

Py:   print("Hello, World!")
来源：http://rii.9152youxi.cn

PHP:  echo "Hello, World!";
来源：http://xfb.sufxvd.cn

JS:   console.log("Hello, World!");
来源：http://rio.yuanzhike.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vbf.jinqigfzy.top

Java: System.out.println("Hello, World!");
来源：http://dci.tanke756.top

Go:   fmt.Println("Hello, World!")
来源：http://mdu.gotoacloud.top

Ruby: puts "Hello, World!"
来源：http://ofu.cheryme.top

C#:   Console.WriteLine("Hello, World!");
来源：http://wxr.yvedp.cn

[A02] 变量声明与赋值
来源：http://sdv.shuidangran.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jgx.zhiwuduotai.top

PHP:  $name = "Alex"; $age = 20;
来源：http://cyq.tianlin.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://lyy.aibaodan.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xpw.yj20258.top

Java: String name = "Alex"; int age = 20;
来源：http://gpt.snrcjt.cn

Go:   name := "Alex"; age := 20
来源：http://lac.tian-w.cn

Ruby: name = "Alex"; age = 20
来源：http://sud.nwbrower.top

C#:   string name = "Alex"; int age = 20;
来源：http://flv.zhixingplan.top

[A03] 常量定义
来源：http://bwz.jqgfzy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kpj.ydzc1.top

PHP:  const PI = 3.14159;
来源：http://qdw.cqqwz.cn

JS:   const PI = 3.14159;
来源：http://bey.mhx1999.top

TS:   const PI: number = 3.14159;
来源：http://qzg.jqgfzy.top

Java: static final double PI = 3.14159;
来源：http://rht.cqqwz.cn

Go:   const PI = 3.14159
来源：http://ijq.hcnkem.com

Ruby: PI = 3.14159
来源：http://upa.jinyuanbaomall.cn

C#:   const double PI = 3.14159;
来源：http://fzj.hesvh.cn

[A04] 判断变量类型
来源：http://glr.shanyushiyangtech.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://sjf.sysykeji.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://cjz.pycfn.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tmt.tian-w.cn

TS:   typeof x; x instanceof Date
来源：http://myt.c1oappe.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://nph.52xcode.cn

Go:   reflect.TypeOf(x).Name()
来源：http://guk.c1oappe.top

Ruby: x.class; x.is_a?(Integer)
来源：http://qej.birdmap.top

C#:   x.GetType().Name; x is int
来源：http://kep.shanyushiyangkeji.top

[A05] 整数除法与取模
来源：http://slx.shuidangran.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ywr.jiagoushi.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://dpe.ctjpmb.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nwr.jinqigufen.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ffh.hammf.cn

Java: 7 / 2; 7 % 2
来源：http://tmw.haohaochexian.top

Go:   7 / 2; 7 % 2
来源：http://ysb.zhiwuduotai.top

Ruby: 7 / 2; 7 % 2
来源：http://tto.smart0.xyz

C#:   7 / 2; 7 % 2
来源：http://gpo.sysykeji.top

[A06] 字符串转数字
来源：http://rgg.daxiang520.top

Py:   int("42"); float("3.14")
来源：http://uuc.guannengcc.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://cgy.hywenlv.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hwv.jqgfzy.top

TS:   parseInt("42", 10); Number("42")
来源：http://dhy.gogol.net.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tls.dashuyun.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://oki.gotoacloud.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ivv.zhongyouzk.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://idw.kuanghao11.cn

[A07] 数字转字符串
来源：http://asb.zdqjudy.top

Py:   str(42)
来源：http://zev.iojbl.cn

PHP:  (string) 42; strval(42)
来源：http://isw.yj20258888.top


<!-- 参考信息 -->