代发 wailian999

[U53] PHP：空合并运算符
来源：http://jam.aibaodan.cn

$v = $a ?? $b ?? "default";
来源：http://jsf.cheryme.top

[U54] PHP：空安全调用
来源：http://job.vehdjk.com

$obj?->method()
来源：http://kxd.jqgufenzy.top

[U55] PHP：match 表达式
来源：http://psv.xziqi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zgp.xuanzx.com

[U56] PHP：命名参数
来源：http://qcv.fengsongda.top

f(a: 1, b: 2)
来源：http://wip.jinqigufen.top

[U57] PHP：字符串插值
来源：http://opf.yuanzhike.top

"值: {$a}"
来源：http://awv.redwolf501.top

[U58] PHP：数组三件套
来源：http://oes.mhx1999.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jce.jqgfzy.top

[U59] PHP：自定义排序
来源：http://wfw.shanyushiyangtech.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kdn.jinqigufen.top

[U60] PHP：JSON 编解码
来源：http://yuw.wangdashe.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vdh.xinyue.icu

[U61] PHP：正则
来源：http://clz.wangdashe.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fop.wangshuangyany.cn

[U62] PHP：日期对象
来源：http://aiy.gzhubu.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pfx.9152youxi.cn

[U63] PHP：文件读写
来源：http://nhd.52xcode.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://osr.epnwcf.com

[U64] PHP：目录遍历
来源：http://yob.yvedp.cn

glob("dir/*.php");  scandir("dir");
来源：http://rha.fanxiaobao.xyz

[U65] PHP：会话
来源：http://dwk.jlsjyb.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://soj.haohaochexian.top

[U66] PHP：设置 Cookie
来源：http://uva.c1oappe.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nmd.hysaishi.cn

[U67] PHP：处理文件上传
来源：http://diz.zdqjudy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://adj.hesvh.cn

[U68] PHP：PDO 连接
来源：http://onx.daria6918.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://paz.chenlongwang.top

[U69] PHP：PDO 预处理
来源：http://nkb.hfpthk.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://umu.jinyuanbaomall.cn

[U70] PHP：PDO 事务
来源：http://sbz.guannengcc.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://aeo.hnxiangtu.top

[U71] PHP：抛出异常
来源：http://wqq.ivvv.top

throw new RuntimeException("失败", 500);
来源：http://ezn.zhengqikj.top

[U72] PHP：写错误日志
来源：http://ewc.ctjpmb.com

error_log("失败: " . $e->getMessage());
来源：http://pfy.gzhubu.top

[U73] PHP：读取 ini 配置
来源：http://qnx.yvedp.cn

parse_ini_file("config.ini", true)
来源：http://uww.sufxvd.cn

[U74] PHP：读取环境变量
来源：http://byt.havefunace.top

getenv("APP_ENV") ?: "production"
来源：http://nol.jiagoushi.top

[U75] PHP：依赖注入
来源：http://fhm.uphjek.com

composer require psr/container
来源：http://nwu.uphjek.com

[U76] PHP：简单路由
来源：http://ubq.yj202588.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fvz.ydzc1.top

[U77] PHP：模板渲染
来源：http://hsq.ehwqpu.com

composer require twig/twig
来源：http://dqq.52xcode.cn

[U78] PHP：单元测试
来源：http://fjm.yj202588.top

composer require --dev phpunit/phpunit
来源：http://msy.hnxiangtu.top

[U79] PHP：静态分析
来源：http://xky.ybcxt.top

composer require --dev phpstan/phpstan
来源：http://wli.jinqigfzy.top

[U80] PHP：代码规范修复
来源：http://rbc.birdmap.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ckg.ehwqpu.com

[U81] JS：初始化项目
来源：http://mjn.wangshuangyany.cn

npm init -y;  npm i express
来源：http://cnu.jinyuanbaomall.cn

[U82] JS：package.json 脚本
来源：http://hpd.tian-w.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bvt.fanxiaobao.xyz

[U83] JS：ES Module 导入导出
来源：http://upr.havefunace.top

export const a = 1;  import { a } from "./m.js";
来源：http://jkt.yfazqb.com

[U84] JS：CommonJS 写法
来源：http://nyb.shangyingyoupin.top

module.exports = { a };  const { a } = require("./m");
来源：http://blj.cqqwz.cn

[U85] JS：可选链
来源：http://ypr.aizwys.cn

a?.b?.c
来源：http://mrg.vqdsnc.cn

[U86] JS：空值合并
来源：http://fhz.uphjek.com

a ?? b
来源：http://vzn.havefunace.top

[U87] JS：解构默认值
来源：http://cdz.ybcxt.top

const { a = 1, b = 2 } = obj;
来源：http://xuk.cdnleiting.top

[U88] JS：对象展开合并
来源：http://ibn.nwbrower.top

{ ...a, ...b }
来源：http://biv.fktsv.cn

[U89] JS：数组去重
来源：http://mij.dashuyun.cn

[...new Set(arr)]
来源：http://ztm.cqqwz.cn

[U90] JS：数字数组排序
来源：http://pma.shuidangran.top

[...arr].sort((a, b) => a - b)
来源：http://vil.shangyingyoupin.top

[U91] JS：对象键值遍历
来源：http://qfy.xylfe.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://luc.yvedp.cn

[U92] JS：深拷贝
来源：http://aye.smart0.xyz

structuredClone(obj)
来源：http://mzj.fanxiaobao.xyz

[U93] JS：模板字符串
来源：http://myf.jqgfzy.top

`共 ${n} 条`
来源：http://fca.jiagoushi.top

[U94] JS：箭头函数
来源：http://xjn.gotoacloud.top

const double = x => x * 2;
来源：http://yqv.xziqi.cn

[U95] JS：Promise 包装
来源：http://jfw.zhijiandao.cn

new Promise((resolve, reject) => {})
来源：http://ncz.snrcjt.cn

[U96] JS：async/await 与异常
来源：http://mnb.yfazqb.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gtc.aizwys.cn

[U97] JS：并发请求
来源：http://ivw.meibo888.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ebx.0kj1m.cn

[U98] JS：fetch 带 JSON
来源：http://vnx.chenlongwang.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://amg.hywenlv.cn

[U99] JS：事件监听
来源：http://hxo.yueranfly.top

el.addEventListener("click", e => {})
来源：http://gdn.cdnleiting.top

[U100] JS：DOM 查询
来源：http://fmu.tanke756.top

document.querySelector(".item")
来源：http://tzm.xziqi.cn

[U101] JS：classList 操作
来源：http://djz.ywan-chungtsiang.top

el.classList.toggle("active")
来源：http://aza.cucudq.cn

[U102] JS：本地存储
来源：http://ubd.hnqzz.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://yqd.nanxuanxn.top

[U103] JS：定时器
来源：http://bon.jinghuilouyu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nks.hfpthk.cn

[U104] JS：防抖
来源：http://doe.zhongyouzk.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dga.zhaomingkeji.xyz

[U105] JS：节流
来源：http://gys.ybcxt.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://url.hcnkem.com

[U106] JS：日期格式化
来源：http://wzn.chenjidiqi.icu

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://myr.snrcjt.cn

[U107] JS：数字千分位
来源：http://obu.chenzaomai.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://egi.aibaodan.cn

[U108] JS：随机整数
来源：http://jby.yj202588.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zna.cdnleiting.top

[U109] JS：数组分组
来源：http://uyq.aizwys.cn

Object.groupBy(arr, x => x.type)
来源：http://lej.kuanghao11.cn

[U110] JS：数组分块
来源：http://wsb.jyoumei.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rxm.jqgfzy.top

[U111] JS：对象转 Map
来源：http://jee.jinqigufen.top

new Map(Object.entries(obj))
来源：http://bhh.sweek.top

[U112] JS：字符串补位
来源：http://wqm.fehbvm.com

"7".padStart(3, "0")
来源：http://vbd.yanxiufei.cn

[U113] JS：正则替换全部
来源：http://jno.daxiang520.top

s.replaceAll("a", "b")
来源：http://yog.shanyushiyangkeji.top

[U114] JS：JSON 深比较
来源：http://dib.ehwqpu.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://kpa.jianghu66.top

[U115] JS：生成 UUID
来源：http://hrx.jyoumei.cn

crypto.randomUUID()
来源：http://qlw.xziqi.cn

[U116] JS：类型检查（JSDoc）
来源：http://kju.shuidangran.top

/** @param {string} name */ function f(name) {}
来源：http://pix.nanxinkj.top

[U117] JS：单元测试
来源：http://dkw.quarkkingdee.top

npm i -D vitest;  npx vitest
来源：http://efi.chenzaomai.com

[U118] JS：开发服务器
来源：http://bre.ehwqpu.com

npm i -D vite;  npx vite
来源：http://lqd.aizwys.cn

[U119] JS：生产构建
来源：http://pvs.tian-w.cn

npx vite build
来源：http://stx.yuanzhike.top

[U120] JS：读取环境变量（Vite）
来源：http://reo.gotoacloud.top

import.meta.env.VITE_API_URL
来源：http://srv.jianghu66.top

================================================================================
来源：http://svy.jinyuanbaomall.cn

统计汇总
来源：http://otm.kuanghao11.cn

================================================================================
来源：http://rfd.zhongyouzk.top

按语言统计（条）：
来源：http://rhl.cashguo.top

Python ......... 252
来源：http://itf.zycfv.cn

PHP ............ 252
来源：http://nbq.aibaodan.cn

JavaScript ..... 252
来源：http://npf.svipenyu.cn

TypeScript ..... 212
来源：http://fkp.jinqigufen.top

Java ........... 212
来源：http://ktx.zycfv.cn

Go ............. 212
来源：http://epm.gogol.net.cn

Ruby ........... 212
来源：http://tze.shanyushiyangtech.top

C# ............. 212
来源：http://meh.sufxvd.cn

C .............. 30
来源：http://mfj.shanyushiyangtech.top

C++ ............ 30
来源：http://pjl.aizwys.cn

SQL ............ 90
来源：http://ear.hnxiangtu.top

Bash ........... 80
来源：http://tik.xziqi.cn

Kotlin ......... 15
来源：http://ldq.jiagoushi.top

Swift .......... 15
来源：http://tqn.jqgufenzy.top

Lua ............ 10
来源：http://csq.tanke756.top

Perl ........... 10
来源：http://cej.jinqigufen.top

Scala .......... 10
来源：http://bgo.shuidangran.top

------------------------------------
来源：http://kcf.jiagoushi.top

合计 ........... 2106 条
来源：http://knw.dashuyun.cn

按章节统计：
来源：http://juj.zycfv.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://efl.fengsongda.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rjz.9152youxi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sxr.snrcjt.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://orw.vqdsnc.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gbw.zhongyouzk.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vqo.chenjidiqi.icu

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mna.tanke756.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://saj.epnwcf.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qyt.ybcxt.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kcg.kuanghao11.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://evl.xylfe.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nlf.vehdjk.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xst.fzhhl.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mvr.zhaomingkeji.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ivi.ehwqpu.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wrm.pycfn.com

Q SQL 专题                              90
来源：http://gds.zhijiandao.cn

R Bash 专题                             80
来源：http://tyc.ehwqpu.com

S C / C++ 专题                          60
来源：http://rel.cucudq.cn

T 其他语言补充                          60
来源：http://tup.yuxming.cn

U 高频实用片段                         120
来源：http://xex.dianchejie.cn

------------------------------------
来源：http://ldi.tianlin.xyz

合计                                  2106 条
来源：http://deb.kuanghao11.cn

--------------------------------------------------------------------------------
来源：http://kts.hesvh.cn

使用提醒
来源：http://xkw.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://vwq.hnxiangtu.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bhp.hcnkem.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://sqc.zhijiandao.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qak.jinqigufen.top

在旧版本上使用前请先确认语法支持情况。
来源：http://wcq.hongshengwenyu.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hxu.daria6918.cn

—— 文件结束 ——
来源：http://mko.yuxming.cn

================================================================================
来源：http://cmm.shanyushiyangkeji.top

程序语言常见例子速查手册（2024 版）
来源：http://cut.gotoacloud.top

Common Programming Examples Cheat Book
来源：http://sdt.aizwys.cn

================================================================================
来源：http://qtl.tianlin.xyz

【收录内容】
来源：http://ssq.9152youxi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://lrk.quarkkingdee.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hoi.jqgufenzy.top

SQL · Bash · C · C++
来源：http://eot.yangfankeji.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://seb.cashguo.top

【使用说明】
来源：http://cff.yanxiufei.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lup.cucudq.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://stb.gzhubu.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zoz.xingfuxueyuan.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://utm.daria6918.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://jrm.tanke756.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ixt.cashguo.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qps.hnqzz.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mrf.hongshengwenyu.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tbd.yj202588.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tlk.fktsv.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lrn.jqgufenzy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qzn.guannengcc.top

【文件统计】
来源：http://plz.tanke756.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://unx.xingfuxueyuan.xyz

--------------------------------------------------------------------------------
来源：http://xzh.ywan-chungtsiang.top

目  录
来源：http://wka.jinghuilouyu.cn

--------------------------------------------------------------------------------
来源：http://brt.ywan-chungtsiang.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pty.jinqigufen.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ynj.fehbvm.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wtx.cdnleiting.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://uop.shanyushiyangtech.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://pow.xuetiantiany.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vry.shuidangran.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zuy.zhiwuduotai.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://cmo.0kj1m.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://twm.shanyushiyangkeji.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://oxp.zhongyouzk.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mej.yangfankeji.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://noh.hnqzz.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vvd.smart0.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://sew.sufxvd.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qfg.mhx1999.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zqu.epnwcf.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ocg.zycfv.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://gqj.daria6918.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ohy.iojbl.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vlu.0kj1m.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fzj.hammf.cn

================================================================================
来源：http://ppx.zhijiandao.cn

A. 基础语法与类型
来源：http://sda.xuetiantiany.cn

================================================================================
来源：http://btu.jlsjyb.cn

[A01] Hello World
来源：http://qfr.epnwcf.com

Py:   print("Hello, World!")
来源：http://xaz.epnwcf.com

PHP:  echo "Hello, World!";
来源：http://vng.nanxuanxn.top

JS:   console.log("Hello, World!");
来源：http://mhb.dashuyun.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ttp.ydjk.org.cn

Java: System.out.println("Hello, World!");
来源：http://pqa.sjlbkw.cn

Go:   fmt.Println("Hello, World!")
来源：http://zro.xylfe.cn

Ruby: puts "Hello, World!"
来源：http://bjb.zhongyouzk.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ijk.xuetiantiany.cn

[A02] 变量声明与赋值
来源：http://hnt.ppjwa.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wqz.sufxvd.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://afo.daria6918.cn

JS:   let name = "Alex"; const age = 20;
来源：http://uxb.sjlbkw.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mvz.smart0.xyz

Java: String name = "Alex"; int age = 20;
来源：http://zra.sjlbkw.cn

Go:   name := "Alex"; age := 20
来源：http://zvz.cheryme.top

Ruby: name = "Alex"; age = 20
来源：http://jaq.jinghuilouyu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://csz.jianghu66.top

[A03] 常量定义
来源：http://xwm.zdqjudy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yus.zhixingplan.top

PHP:  const PI = 3.14159;
来源：http://zse.zhongyouzk.top

JS:   const PI = 3.14159;
来源：http://dhw.smart0.xyz

TS:   const PI: number = 3.14159;
来源：http://hkc.hongshengwenyu.top

Java: static final double PI = 3.14159;
来源：http://ssf.daxiang520.top

Go:   const PI = 3.14159
来源：http://lyk.yj20258888.top

Ruby: PI = 3.14159
来源：http://yvf.dianchejie.cn

C#:   const double PI = 3.14159;
来源：http://lnh.hnqzz.top

[A04] 判断变量类型
来源：http://trw.birdmap.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://vte.guowangkeji.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://sut.daxiang520.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pvk.aibaodan.cn

TS:   typeof x; x instanceof Date
来源：http://wmq.ybcxt.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ggh.hfpthk.cn

Go:   reflect.TypeOf(x).Name()
来源：http://cpe.hongshengwenyu.top

Ruby: x.class; x.is_a?(Integer)
来源：http://tlz.gogol.net.cn

C#:   x.GetType().Name; x is int
来源：http://nqr.ydzc1.top

[A05] 整数除法与取模
来源：http://nkk.xuanzx.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kfb.yj20258888.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://wbo.sysykeji.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vii.yangfankeji.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://inv.ppjwa.cn

Java: 7 / 2; 7 % 2
来源：http://xvh.9152youxi.cn

Go:   7 / 2; 7 % 2
来源：http://ifv.cheryme.top

Ruby: 7 / 2; 7 % 2
来源：http://uyp.daxiang520.top

C#:   7 / 2; 7 % 2
来源：http://ivs.cashguo.top

[A06] 字符串转数字
来源：http://dyv.gogol.net.cn

Py:   int("42"); float("3.14")
来源：http://muu.xinyue.icu

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kqf.zycfv.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jib.yvedp.cn

TS:   parseInt("42", 10); Number("42")
来源：http://wtq.jqgufenzy.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qcz.hywenlv.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ipl.chenjidiqi.icu

Ruby: "42".to_i; "3.14".to_f
来源：http://ymb.ppjwa.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://bbm.vehdjk.com

[A07] 数字转字符串
来源：http://fop.ppjwa.cn

Py:   str(42)
来源：http://sqa.wangdashe.top

PHP:  (string) 42; strval(42)
来源：http://dns.cdnleiting.top


<!-- 参考信息 -->