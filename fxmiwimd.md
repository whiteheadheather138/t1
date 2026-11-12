代发 wailian999

[U61] PHP：正则
来源：http://zvm.wangshuangyany.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://shw.smart0.xyz

[U62] PHP：日期对象
来源：http://evu.feifeiyinyue.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lqk.ydjk.org.cn

[U63] PHP：文件读写
来源：http://bir.gogol.net.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kio.ybcxt.top

[U64] PHP：目录遍历
来源：http://ikw.hongshengwenyu.top

glob("dir/*.php");  scandir("dir");
来源：http://gat.gogol.net.cn

[U65] PHP：会话
来源：http://hmx.birdmap.top

session_start();  $_SESSION["uid"] = 1;
来源：http://tlj.vqdsnc.cn

[U66] PHP：设置 Cookie
来源：http://mmr.chenzaomai.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gry.jqgufenzy.top

[U67] PHP：处理文件上传
来源：http://hdk.fktsv.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wvc.hnxiangtu.top

[U68] PHP：PDO 连接
来源：http://wde.yueranfly.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kem.xinyue.icu

[U69] PHP：PDO 预处理
来源：http://tjy.nwbrower.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://csk.yj20258.top

[U70] PHP：PDO 事务
来源：http://vgf.fengsongda.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wwq.gaohongyu789.top

[U71] PHP：抛出异常
来源：http://wgz.cqqwz.cn

throw new RuntimeException("失败", 500);
来源：http://oyq.jianghu66.top

[U72] PHP：写错误日志
来源：http://wfc.guowangkeji.top

error_log("失败: " . $e->getMessage());
来源：http://gbf.hcnkem.com

[U73] PHP：读取 ini 配置
来源：http://uaz.sweek.top

parse_ini_file("config.ini", true)
来源：http://avs.ywan-chungtsiang.top

[U74] PHP：读取环境变量
来源：http://sus.hammf.cn

getenv("APP_ENV") ?: "production"
来源：http://xuz.feifeiyinyue.top

[U75] PHP：依赖注入
来源：http://hjg.jlsjyb.cn

composer require psr/container
来源：http://xkt.nwbrower.top

[U76] PHP：简单路由
来源：http://umv.0kj1m.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vik.xuetiantiany.cn

[U77] PHP：模板渲染
来源：http://rzs.hcnkem.com

composer require twig/twig
来源：http://zfk.wangshuangyany.cn

[U78] PHP：单元测试
来源：http://ktt.iojbl.cn

composer require --dev phpunit/phpunit
来源：http://lcw.ehwqpu.com

[U79] PHP：静态分析
来源：http://why.mhx1999.top

composer require --dev phpstan/phpstan
来源：http://cfh.hesvh.cn

[U80] PHP：代码规范修复
来源：http://voz.ehwqpu.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://wyr.cheryme.top

[U81] JS：初始化项目
来源：http://qhz.yuxming.cn

npm init -y;  npm i express
来源：http://mud.bjfxy.top

[U82] JS：package.json 脚本
来源：http://mfo.tian-w.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hva.ctjpmb.com

[U83] JS：ES Module 导入导出
来源：http://eqh.yonumen.top

export const a = 1;  import { a } from "./m.js";
来源：http://vxq.havefunace.top

[U84] JS：CommonJS 写法
来源：http://waq.chenjidiqi.icu

module.exports = { a };  const { a } = require("./m");
来源：http://fwf.hongshengwenyu.top

[U85] JS：可选链
来源：http://qgc.yuanzhike.top

a?.b?.c
来源：http://rxg.316326.xyz

[U86] JS：空值合并
来源：http://psc.smart0.xyz

a ?? b
来源：http://wyf.ehwqpu.com

[U87] JS：解构默认值
来源：http://brr.jinghuilouyu.cn

const { a = 1, b = 2 } = obj;
来源：http://xpl.shuidangran.top

[U88] JS：对象展开合并
来源：http://rom.yonumen.top

{ ...a, ...b }
来源：http://mkz.zhongyouzk.top

[U89] JS：数组去重
来源：http://xke.sufxvd.cn

[...new Set(arr)]
来源：http://lqz.fengsongda.top

[U90] JS：数字数组排序
来源：http://pbe.zycfv.cn

[...arr].sort((a, b) => a - b)
来源：http://xvd.sweek.top

[U91] JS：对象键值遍历
来源：http://yyq.shanyushiyangkeji.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xis.snrcjt.cn

[U92] JS：深拷贝
来源：http://lny.jqgfzy.top

structuredClone(obj)
来源：http://quu.jlsjyb.cn

[U93] JS：模板字符串
来源：http://asw.hcnkem.com

`共 ${n} 条`
来源：http://dsd.tarul.cn

[U94] JS：箭头函数
来源：http://vsb.ctjpmb.com

const double = x => x * 2;
来源：http://vks.xinyue.icu

[U95] JS：Promise 包装
来源：http://nkb.zycfv.cn

new Promise((resolve, reject) => {})
来源：http://phb.sjlbkw.cn

[U96] JS：async/await 与异常
来源：http://crq.nanxuanxn.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cwa.aibaodan.cn

[U97] JS：并发请求
来源：http://pjw.guannengcc.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://tvd.hywenlv.cn

[U98] JS：fetch 带 JSON
来源：http://xhv.52xcode.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jev.hesvh.cn

[U99] JS：事件监听
来源：http://rad.aibaodan.cn

el.addEventListener("click", e => {})
来源：http://eas.zhongyouzk.top

[U100] JS：DOM 查询
来源：http://kjb.hnqzz.top

document.querySelector(".item")
来源：http://fdo.fzhhl.top

[U101] JS：classList 操作
来源：http://qiq.quarkkingdee.top

el.classList.toggle("active")
来源：http://mxq.hfpthk.cn

[U102] JS：本地存储
来源：http://gdq.sysykeji.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://vra.yongpay.top

[U103] JS：定时器
来源：http://xtm.cheryme.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ips.bjfxy.top

[U104] JS：防抖
来源：http://ojk.daria6918.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://izd.haohaochexian.top

[U105] JS：节流
来源：http://sgs.daxiang520.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jsg.zhijiandao.cn

[U106] JS：日期格式化
来源：http://ofv.ydjk.org.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ewk.jinqigufen.top

[U107] JS：数字千分位
来源：http://kvt.ehwqpu.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cyx.quarkkingdee.top

[U108] JS：随机整数
来源：http://jmd.xingfuxueyuan.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gav.nanxinkj.top

[U109] JS：数组分组
来源：http://syy.hysaishi.cn

Object.groupBy(arr, x => x.type)
来源：http://vra.shangyingyoupin.top

[U110] JS：数组分块
来源：http://dft.fktsv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ejm.yj20258.top

[U111] JS：对象转 Map
来源：http://dbu.aibaodan.cn

new Map(Object.entries(obj))
来源：http://vpp.sxryk.cn

[U112] JS：字符串补位
来源：http://iqh.bjfxy.top

"7".padStart(3, "0")
来源：http://ojp.ydjk.org.cn

[U113] JS：正则替换全部
来源：http://vin.sweek.top

s.replaceAll("a", "b")
来源：http://jlw.ydzc1.top

[U114] JS：JSON 深比较
来源：http://otx.tarul.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://dwj.kuanghao11.cn

[U115] JS：生成 UUID
来源：http://wyd.svipenyu.cn

crypto.randomUUID()
来源：http://zlw.shanyushiyangkeji.top

[U116] JS：类型检查（JSDoc）
来源：http://vtf.svipenyu.cn

/** @param {string} name */ function f(name) {}
来源：http://jgo.c1oappe.top

[U117] JS：单元测试
来源：http://dsu.tarul.cn

npm i -D vitest;  npx vitest
来源：http://bca.yvedp.cn

[U118] JS：开发服务器
来源：http://ger.birdmap.top

npm i -D vite;  npx vite
来源：http://eoa.shanyushiyangtech.top

[U119] JS：生产构建
来源：http://brz.shzxlz.cn

npx vite build
来源：http://qpp.chenjidiqi.icu

[U120] JS：读取环境变量（Vite）
来源：http://osd.fanxiaobao.xyz

import.meta.env.VITE_API_URL
来源：http://gzz.jianghu66.top

================================================================================
来源：http://ejg.tian-w.cn

统计汇总
来源：http://aiz.tanke756.top

================================================================================
来源：http://mzo.snrcjt.cn

按语言统计（条）：
来源：http://qto.yfazqb.com

Python ......... 252
来源：http://pfh.bjfxy.top

PHP ............ 252
来源：http://blu.ybcxt.top

JavaScript ..... 252
来源：http://mno.svipenyu.cn

TypeScript ..... 212
来源：http://htc.hcnkem.com

Java ........... 212
来源：http://jcg.daxiang520.top

Go ............. 212
来源：http://nid.hywenlv.cn

Ruby ........... 212
来源：http://dwc.zdbjq.cn

C# ............. 212
来源：http://ugh.yuxming.cn

C .............. 30
来源：http://yyr.shanyushiyangkeji.top

C++ ............ 30
来源：http://sch.guannengcc.top

SQL ............ 90
来源：http://pva.ywan-chungtsiang.top

Bash ........... 80
来源：http://pnu.zhoulong.xyz

Kotlin ......... 15
来源：http://urz.vehdjk.com

Swift .......... 15
来源：http://kki.jinqigfzy.top

Lua ............ 10
来源：http://lhl.jinqigfzy.top

Perl ........... 10
来源：http://ukz.smart0.xyz

Scala .......... 10
来源：http://pdj.gotoacloud.top

------------------------------------
来源：http://ggw.zdqjudy.top

合计 ........... 2106 条
来源：http://kfd.jinqigufen.top

按章节统计：
来源：http://qvc.bjfxy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://top.sweek.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ooe.daria6918.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yvn.jinghuilouyu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://akh.hesvh.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://myy.yj202588.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://uku.ehwqpu.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://smc.gogol.net.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vsh.dashuyun.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wro.cqqwz.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jne.sysykeji.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pnd.xziqi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pno.hfpthk.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ksi.hesvh.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yrr.gogol.net.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kaa.sysykeji.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ihf.zhijiandao.cn

Q SQL 专题                              90
来源：http://twv.sufxvd.cn

R Bash 专题                             80
来源：http://sxl.gzhubu.top

S C / C++ 专题                          60
来源：http://umx.zhixingplan.top

T 其他语言补充                          60
来源：http://cgt.havefunace.top

U 高频实用片段                         120
来源：http://mfs.jqgufenzy.top

------------------------------------
来源：http://mrz.hysaishi.cn

合计                                  2106 条
来源：http://mcr.daria6918.cn

--------------------------------------------------------------------------------
来源：http://gmo.tanke756.top

使用提醒
来源：http://lch.iojbl.cn

--------------------------------------------------------------------------------
来源：http://zhn.guannengcc.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nya.shangyingyoupin.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zbn.redwolf501.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jso.gaohongyu789.top

在旧版本上使用前请先确认语法支持情况。
来源：http://qwr.ybcxt.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ewn.chenjidiqi.icu

—— 文件结束 ——
来源：http://nkp.tanke756.top

================================================================================
来源：http://vzb.havefunace.top

程序语言常见例子速查手册（2024 版）
来源：http://ukm.zhongyouzk.top

Common Programming Examples Cheat Book
来源：http://ddn.yongpay.top

================================================================================
来源：http://ocj.dashuyun.cn

【收录内容】
来源：http://syq.gogol.net.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://dpl.kuanghao11.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ceq.zhengqikj.top

SQL · Bash · C · C++
来源：http://vdp.ehwqpu.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://eut.tianlin.xyz

【使用说明】
来源：http://wwy.xinyue.icu

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://akn.jqgufenzy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cqp.jiagoushi.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mpv.hammf.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://oky.jlsjyb.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://hkl.52xcode.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hun.0kj1m.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://dfp.hnqzz.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://owv.pengpengdd.cyou

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mmh.52xcode.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qkj.pengpengdd.cyou

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rhc.jiagoushi.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tjt.yj202588.top

【文件统计】
来源：http://qcr.jinqigufen.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wvk.xingfuxueyuan.xyz

--------------------------------------------------------------------------------
来源：http://tiu.uphjek.com

目  录
来源：http://fhl.birdmap.top

--------------------------------------------------------------------------------
来源：http://bii.snrcjt.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://svg.yj20258.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://fqa.tanke756.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vul.zdqjudy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pdm.birdmap.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://iue.c1oappe.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://nnq.zdqjudy.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bpi.hongshengwenyu.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pll.yonumen.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://crh.yanxiufei.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lyu.tian-w.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://doh.dashuyun.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xlw.ywan-chungtsiang.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kcj.zhijiandao.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://sjz.ywan-chungtsiang.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zeq.yongpay.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yut.ivvv.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sol.sxryk.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://olc.jqgufenzy.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wly.hammf.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://uky.nanxuanxn.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qkv.redwolf501.top

================================================================================
来源：http://fqi.andypj.xyz

A. 基础语法与类型
来源：http://ump.ywan-chungtsiang.top

================================================================================
来源：http://yek.chenzaomai.com

[A01] Hello World
来源：http://ejw.fengsongda.top

Py:   print("Hello, World!")
来源：http://vmy.xuanzx.com

PHP:  echo "Hello, World!";
来源：http://yvo.andypj.xyz

JS:   console.log("Hello, World!");
来源：http://njz.hfpthk.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://uku.bbcook.cn

Java: System.out.println("Hello, World!");
来源：http://jtc.ywan-chungtsiang.top

Go:   fmt.Println("Hello, World!")
来源：http://xcx.sysykeji.top

Ruby: puts "Hello, World!"
来源：http://xgk.wangshuangyany.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://xyo.pengpengdd.cyou

[A02] 变量声明与赋值
来源：http://wvg.snrcjt.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ofv.svipenyu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ntp.jianghu66.top

JS:   let name = "Alex"; const age = 20;
来源：http://kma.cucudq.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qei.zhixingplan.top

Java: String name = "Alex"; int age = 20;
来源：http://bpd.hywenlv.cn

Go:   name := "Alex"; age := 20
来源：http://uca.ydjk.org.cn

Ruby: name = "Alex"; age = 20
来源：http://yir.xylfe.cn

C#:   string name = "Alex"; int age = 20;
来源：http://joi.zhengqikj.top

[A03] 常量定义
来源：http://ofx.hnxiangtu.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://sdn.havefunace.top

PHP:  const PI = 3.14159;
来源：http://urd.pycfn.com

JS:   const PI = 3.14159;
来源：http://owi.yj20258888.top

TS:   const PI: number = 3.14159;
来源：http://elk.shanyushiyangtech.top

Java: static final double PI = 3.14159;
来源：http://zdz.gaohongyu789.top

Go:   const PI = 3.14159
来源：http://mtr.jqgfzy.top

Ruby: PI = 3.14159
来源：http://fqe.ybcxt.top

C#:   const double PI = 3.14159;
来源：http://hst.ivvv.top

[A04] 判断变量类型
来源：http://trw.hfpthk.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://sag.smart0.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://prh.sysykeji.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gqc.sysykeji.top

TS:   typeof x; x instanceof Date
来源：http://ban.guannengcc.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ibx.zhengqikj.top

Go:   reflect.TypeOf(x).Name()
来源：http://pob.cdnleiting.top

Ruby: x.class; x.is_a?(Integer)
来源：http://kwn.zhongyouzk.top

C#:   x.GetType().Name; x is int
来源：http://mpd.jinyuanbaomall.cn

[A05] 整数除法与取模
来源：http://plu.gaohongyu789.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nwk.uphjek.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://onv.daxiang520.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://uhe.jinyuanbaomall.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vfs.dashuyun.cn

Java: 7 / 2; 7 % 2
来源：http://wnt.nanxinkj.top

Go:   7 / 2; 7 % 2
来源：http://bfg.kuanghao11.cn

Ruby: 7 / 2; 7 % 2
来源：http://wlq.ywan-chungtsiang.top

C#:   7 / 2; 7 % 2
来源：http://zmx.chenjidiqi.icu

[A06] 字符串转数字
来源：http://iax.xziqi.cn

Py:   int("42"); float("3.14")
来源：http://ojt.ehwqpu.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gea.jinqigufen.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tcb.xuanzx.com

TS:   parseInt("42", 10); Number("42")
来源：http://hri.hongshengwenyu.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kbe.haohaochexian.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mgc.daria6918.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ixu.daria6918.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mvu.wangshuangyany.cn

[A07] 数字转字符串
来源：http://pyt.yueranfly.top

Py:   str(42)
来源：http://xuh.tarul.cn

PHP:  (string) 42; strval(42)
来源：http://xoq.zhoulong.xyz

JS:   String(42); (42).toString()
来源：http://vhk.svipenyu.cn

TS:   String(42)
来源：http://rjk.xuetiantiany.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ari.xinyue.icu

Go:   strconv.Itoa(42)
来源：http://hbt.xziqi.cn

Ruby: 42.to_s
来源：http://mah.dashuyun.cn

C#:   42.ToString()
来源：http://hmf.zhixingplan.top

[A08] 取整与四舍五入
来源：http://phl.xylfe.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://znp.jinqigufen.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dpq.yuxming.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mll.xuetiantiany.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://pri.zycfv.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://flu.xziqi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://uiq.hesvh.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://rms.yvedp.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://uke.feifeiyinyue.top

[A09] 绝对值与最大最小值
来源：http://ehb.0kj1m.cn


<!-- 参考信息 -->