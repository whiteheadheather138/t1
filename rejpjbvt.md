代发 wailian999

[U59] PHP：自定义排序
来源：http://bnu.ydjk.org.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kbe.tanke756.top

[U60] PHP：JSON 编解码
来源：http://oln.hfpthk.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://aqc.sysykeji.top

[U61] PHP：正则
来源：http://ver.cashguo.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mng.daria6918.cn

[U62] PHP：日期对象
来源：http://lsr.wangdashe.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ozy.zhengqikj.top

[U63] PHP：文件读写
来源：http://aib.pengpengdd.cyou

file_get_contents($f);  file_put_contents($f, $data);
来源：http://asy.jlsjyb.cn

[U64] PHP：目录遍历
来源：http://gic.ppjwa.cn

glob("dir/*.php");  scandir("dir");
来源：http://olr.ppjwa.cn

[U65] PHP：会话
来源：http://fqw.fanxiaobao.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://gwj.jlsjyb.cn

[U66] PHP：设置 Cookie
来源：http://xwz.9152youxi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wrr.sxryk.cn

[U67] PHP：处理文件上传
来源：http://trc.zhijiandao.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qyy.yuanzhike.top

[U68] PHP：PDO 连接
来源：http://smw.bjfxy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mru.xinyue.icu

[U69] PHP：PDO 预处理
来源：http://opo.fengsongda.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zle.yfazqb.com

[U70] PHP：PDO 事务
来源：http://lqn.fanxiaobao.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kbr.cucudq.cn

[U71] PHP：抛出异常
来源：http://pum.hysaishi.cn

throw new RuntimeException("失败", 500);
来源：http://rgl.cqqwz.cn

[U72] PHP：写错误日志
来源：http://wws.vehdjk.com

error_log("失败: " . $e->getMessage());
来源：http://uvc.c1oappe.top

[U73] PHP：读取 ini 配置
来源：http://lsy.xinyue.icu

parse_ini_file("config.ini", true)
来源：http://bsc.ppjwa.cn

[U74] PHP：读取环境变量
来源：http://ekc.zhaomingkeji.xyz

getenv("APP_ENV") ?: "production"
来源：http://cws.bbcook.cn

[U75] PHP：依赖注入
来源：http://jyk.xingfuxueyuan.xyz

composer require psr/container
来源：http://cso.yj20258888.top

[U76] PHP：简单路由
来源：http://mir.hnqzz.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ijn.shzxlz.cn

[U77] PHP：模板渲染
来源：http://rhc.hnqzz.top

composer require twig/twig
来源：http://pjq.quarkkingdee.top

[U78] PHP：单元测试
来源：http://aev.wangdashe.top

composer require --dev phpunit/phpunit
来源：http://kjb.ppjwa.cn

[U79] PHP：静态分析
来源：http://lgd.pengpengdd.cyou

composer require --dev phpstan/phpstan
来源：http://sme.fanxiaobao.xyz

[U80] PHP：代码规范修复
来源：http://lgo.sxryk.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://vny.sjlbkw.cn

[U81] JS：初始化项目
来源：http://yzz.hongshengwenyu.top

npm init -y;  npm i express
来源：http://hmk.cashguo.top

[U82] JS：package.json 脚本
来源：http://ibr.vehdjk.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xta.ywan-chungtsiang.top

[U83] JS：ES Module 导入导出
来源：http://dax.iojbl.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lgs.nanxuanxn.top

[U84] JS：CommonJS 写法
来源：http://kbk.zhiwuduotai.top

module.exports = { a };  const { a } = require("./m");
来源：http://yhp.gotoacloud.top

[U85] JS：可选链
来源：http://vwn.hesvh.cn

a?.b?.c
来源：http://vvd.xinyue.icu

[U86] JS：空值合并
来源：http://vyo.jyoumei.cn

a ?? b
来源：http://xud.c1oappe.top

[U87] JS：解构默认值
来源：http://tdr.aibaodan.cn

const { a = 1, b = 2 } = obj;
来源：http://kqi.xziqi.cn

[U88] JS：对象展开合并
来源：http://wee.hongshengwenyu.top

{ ...a, ...b }
来源：http://dak.aizwys.cn

[U89] JS：数组去重
来源：http://zbb.bbcook.cn

[...new Set(arr)]
来源：http://dbf.bjfxy.top

[U90] JS：数字数组排序
来源：http://zcz.cucudq.cn

[...arr].sort((a, b) => a - b)
来源：http://vjp.sjlbkw.cn

[U91] JS：对象键值遍历
来源：http://dnl.iojbl.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vhf.cheryme.top

[U92] JS：深拷贝
来源：http://une.gaohongyu789.top

structuredClone(obj)
来源：http://fuq.wangdashe.top

[U93] JS：模板字符串
来源：http://prt.hfpthk.cn

`共 ${n} 条`
来源：http://rma.jianghu66.top

[U94] JS：箭头函数
来源：http://uip.ydzc1.top

const double = x => x * 2;
来源：http://liw.xuanzx.com

[U95] JS：Promise 包装
来源：http://jgy.yongpay.top

new Promise((resolve, reject) => {})
来源：http://tlx.wangdashe.top

[U96] JS：async/await 与异常
来源：http://oxg.nanxuanxn.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ttk.xuanzx.com

[U97] JS：并发请求
来源：http://kbr.gzhubu.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://nzp.fktsv.cn

[U98] JS：fetch 带 JSON
来源：http://ywo.epnwcf.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hqx.bjfxy.top

[U99] JS：事件监听
来源：http://yvx.zhengqikj.top

el.addEventListener("click", e => {})
来源：http://isi.birdmap.top

[U100] JS：DOM 查询
来源：http://zfz.cheryme.top

document.querySelector(".item")
来源：http://tac.shangyingyoupin.top

[U101] JS：classList 操作
来源：http://hel.yonumen.top

el.classList.toggle("active")
来源：http://oia.ivvv.top

[U102] JS：本地存储
来源：http://qdh.chenzaomai.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://xfa.xuetiantiany.cn

[U103] JS：定时器
来源：http://mom.nanxuanxn.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kgl.cucudq.cn

[U104] JS：防抖
来源：http://nyn.havefunace.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dgy.kuanghao11.cn

[U105] JS：节流
来源：http://ykn.chenlongwang.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ubp.smart0.xyz

[U106] JS：日期格式化
来源：http://wtm.ybcxt.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hgc.jianghu66.top

[U107] JS：数字千分位
来源：http://nkc.fengsongda.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://est.aizwys.cn

[U108] JS：随机整数
来源：http://pzt.52xcode.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://str.hongshengwenyu.top

[U109] JS：数组分组
来源：http://mhk.tianlin.xyz

Object.groupBy(arr, x => x.type)
来源：http://oin.316326.xyz

[U110] JS：数组分块
来源：http://znd.yangfankeji.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ckv.jinqigfzy.top

[U111] JS：对象转 Map
来源：http://pej.tanke756.top

new Map(Object.entries(obj))
来源：http://fpj.sjlbkw.cn

[U112] JS：字符串补位
来源：http://uco.shangyingyoupin.top

"7".padStart(3, "0")
来源：http://vyh.ctjpmb.com

[U113] JS：正则替换全部
来源：http://jet.tarul.cn

s.replaceAll("a", "b")
来源：http://vqp.zhongyouzk.top

[U114] JS：JSON 深比较
来源：http://fty.guannengcc.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://lqt.316326.xyz

[U115] JS：生成 UUID
来源：http://zca.jinyuanbaomall.cn

crypto.randomUUID()
来源：http://hoh.yongpay.top

[U116] JS：类型检查（JSDoc）
来源：http://fai.jiagoushi.top

/** @param {string} name */ function f(name) {}
来源：http://yom.yuxming.cn

[U117] JS：单元测试
来源：http://jzj.fanxiaobao.xyz

npm i -D vitest;  npx vitest
来源：http://oxz.xziqi.cn

[U118] JS：开发服务器
来源：http://iwq.gogol.net.cn

npm i -D vite;  npx vite
来源：http://ugm.zdbjq.cn

[U119] JS：生产构建
来源：http://wim.zycfv.cn

npx vite build
来源：http://kqu.xingfuxueyuan.xyz

[U120] JS：读取环境变量（Vite）
来源：http://drb.jlsjyb.cn

import.meta.env.VITE_API_URL
来源：http://cny.ydzc1.top

================================================================================
来源：http://ofx.hnqzz.top

统计汇总
来源：http://epw.aibaodan.cn

================================================================================
来源：http://fcs.bjfxy.top

按语言统计（条）：
来源：http://ljl.hysaishi.cn

Python ......... 252
来源：http://qar.dashuyun.cn

PHP ............ 252
来源：http://tut.havefunace.top

JavaScript ..... 252
来源：http://tru.nanxinkj.top

TypeScript ..... 212
来源：http://lqt.daria6918.cn

Java ........... 212
来源：http://kbu.c1oappe.top

Go ............. 212
来源：http://cxk.0kj1m.cn

Ruby ........... 212
来源：http://liz.yj202588.top

C# ............. 212
来源：http://vis.svipenyu.cn

C .............. 30
来源：http://qcd.jinqigufen.top

C++ ............ 30
来源：http://cjo.ivvv.top

SQL ............ 90
来源：http://dji.jinqigfzy.top

Bash ........... 80
来源：http://fgk.gotoacloud.top

Kotlin ......... 15
来源：http://ywb.andypj.xyz

Swift .......... 15
来源：http://zmd.havefunace.top

Lua ............ 10
来源：http://tdy.yanxiufei.cn

Perl ........... 10
来源：http://eep.xziqi.cn

Scala .......... 10
来源：http://nty.andypj.xyz

------------------------------------
来源：http://wfk.zdbjq.cn

合计 ........... 2106 条
来源：http://tej.vehdjk.com

按章节统计：
来源：http://nzk.cdnleiting.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dhz.dianchejie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://amn.cqqwz.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nad.zhoulong.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qdh.sysykeji.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dkh.wangdashe.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gil.xuetiantiany.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://eji.feifeiyinyue.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qzt.havefunace.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dgx.havefunace.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dvf.cdnleiting.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hek.kuanghao11.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nbx.yuanzhike.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kgs.ydjk.org.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hwi.tianlin.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://quu.ydjk.org.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://igq.ydzc1.top

Q SQL 专题                              90
来源：http://aae.ybcxt.top

R Bash 专题                             80
来源：http://lpj.ehwqpu.com

S C / C++ 专题                          60
来源：http://edg.guannengcc.top

T 其他语言补充                          60
来源：http://jyn.cucudq.cn

U 高频实用片段                         120
来源：http://xmc.ehwqpu.com

------------------------------------
来源：http://ehc.dashuyun.cn

合计                                  2106 条
来源：http://qnz.zycfv.cn

--------------------------------------------------------------------------------
来源：http://zbp.sweek.top

使用提醒
来源：http://swr.jinghuilouyu.cn

--------------------------------------------------------------------------------
来源：http://qjm.yj20258.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tqa.guannengcc.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://myt.sysykeji.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://iri.jqgufenzy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://dkm.cheryme.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://syq.xylfe.cn

—— 文件结束 ——
来源：http://wje.ywan-chungtsiang.top

================================================================================
来源：http://uvb.bbcook.cn

程序语言常见例子速查手册（2024 版）
来源：http://ilh.chenzaomai.com

Common Programming Examples Cheat Book
来源：http://adt.hywenlv.cn

================================================================================
来源：http://mfx.pengpengdd.cyou

【收录内容】
来源：http://duo.jinyuanbaomall.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vmt.snrcjt.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fzd.jyoumei.cn

SQL · Bash · C · C++
来源：http://lyt.aibaodan.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tle.zdqjudy.top

【使用说明】
来源：http://zox.tian-w.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rox.epnwcf.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ncm.zhijiandao.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mrr.yuanzhike.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hxa.cqqwz.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://txy.c1oappe.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gad.zdbjq.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lbv.havefunace.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://btz.yfazqb.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://epf.feifeiyinyue.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://cvl.shanyushiyangtech.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wmu.jyoumei.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ggv.hcnkem.com

【文件统计】
来源：http://xwh.jinqigfzy.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://bnp.sxryk.cn

--------------------------------------------------------------------------------
来源：http://lrw.xingfuxueyuan.xyz

目  录
来源：http://ice.yfazqb.com

--------------------------------------------------------------------------------
来源：http://cvn.haohaochexian.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kdc.gogol.net.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xfo.sxryk.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ixw.zhengqikj.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pco.yfazqb.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ljb.sufxvd.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ero.meibo888.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vcq.ydjk.org.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://slo.nanxuanxn.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kav.nanxinkj.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://zxu.jyoumei.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ruq.bbcook.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xvs.yuxming.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lxt.tarul.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kij.hnxiangtu.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xml.fktsv.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://chv.9152youxi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pxn.fehbvm.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://dkg.316326.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hkj.pycfn.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yzy.zdqjudy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ejo.snrcjt.cn

================================================================================
来源：http://cqr.9152youxi.cn

A. 基础语法与类型
来源：http://xgv.ydzc1.top

================================================================================
来源：http://lpn.gogol.net.cn

[A01] Hello World
来源：http://rag.fengsongda.top

Py:   print("Hello, World!")
来源：http://tar.xuanzx.com

PHP:  echo "Hello, World!";
来源：http://weq.ydzc1.top

JS:   console.log("Hello, World!");
来源：http://rvb.shangyingyoupin.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wuz.ywan-chungtsiang.top

Java: System.out.println("Hello, World!");
来源：http://frt.chenjidiqi.icu

Go:   fmt.Println("Hello, World!")
来源：http://tun.vqdsnc.cn

Ruby: puts "Hello, World!"
来源：http://jix.cashguo.top

C#:   Console.WriteLine("Hello, World!");
来源：http://srf.0kj1m.cn

[A02] 变量声明与赋值
来源：http://rxh.zhengqikj.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zhl.aizwys.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://lpe.cashguo.top

JS:   let name = "Alex"; const age = 20;
来源：http://fkd.jinyuanbaomall.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hni.fanxiaobao.xyz

Java: String name = "Alex"; int age = 20;
来源：http://fxf.fehbvm.com

Go:   name := "Alex"; age := 20
来源：http://sdg.kuanghao11.cn

Ruby: name = "Alex"; age = 20
来源：http://fpr.guannengcc.top

C#:   string name = "Alex"; int age = 20;
来源：http://zny.hysaishi.cn

[A03] 常量定义
来源：http://fkb.sweek.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://njp.jyoumei.cn

PHP:  const PI = 3.14159;
来源：http://pnr.zdqjudy.top

JS:   const PI = 3.14159;
来源：http://ode.yuanzhike.top

TS:   const PI: number = 3.14159;
来源：http://jji.yj202588.top

Java: static final double PI = 3.14159;
来源：http://foq.iojbl.cn

Go:   const PI = 3.14159
来源：http://ndy.pengpengdd.cyou

Ruby: PI = 3.14159
来源：http://trq.0kj1m.cn

C#:   const double PI = 3.14159;
来源：http://fuj.xingfuxueyuan.xyz

[A04] 判断变量类型
来源：http://jur.feifeiyinyue.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://enl.tianlin.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hgm.ctjpmb.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ueq.fengsongda.top

TS:   typeof x; x instanceof Date
来源：http://aax.9152youxi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hgg.9152youxi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://tsc.zhongyouzk.top

Ruby: x.class; x.is_a?(Integer)
来源：http://dhm.andypj.xyz

C#:   x.GetType().Name; x is int
来源：http://lfg.yj20258888.top

[A05] 整数除法与取模
来源：http://qip.zdqjudy.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://giu.haohaochexian.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://tcv.epnwcf.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ptd.yj20258.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://brf.52xcode.cn

Java: 7 / 2; 7 % 2
来源：http://awq.aibaodan.cn

Go:   7 / 2; 7 % 2
来源：http://zgs.wangshuangyany.cn

Ruby: 7 / 2; 7 % 2
来源：http://jme.snrcjt.cn

C#:   7 / 2; 7 % 2
来源：http://rng.zhengqikj.top

[A06] 字符串转数字
来源：http://scd.xingfuxueyuan.xyz

Py:   int("42"); float("3.14")
来源：http://kml.yj20258.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nip.quarkkingdee.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://rwy.birdmap.top

TS:   parseInt("42", 10); Number("42")
来源：http://dqb.wangdashe.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://urm.c1oappe.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blj.hnxiangtu.top

Ruby: "42".to_i; "3.14".to_f
来源：http://vje.nanxuanxn.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jzr.snrcjt.cn

[A07] 数字转字符串
来源：http://aud.andypj.xyz

Py:   str(42)
来源：http://adc.jianghu66.top

PHP:  (string) 42; strval(42)
来源：http://nlv.jinghuilouyu.cn

JS:   String(42); (42).toString()
来源：http://vsv.gotoacloud.top

TS:   String(42)
来源：http://rhg.aizwys.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://nxs.ydzc1.top

Go:   strconv.Itoa(42)
来源：http://zky.0kj1m.cn

Ruby: 42.to_s
来源：http://bum.yuxming.cn

C#:   42.ToString()
来源：http://xdv.yueranfly.top

[A08] 取整与四舍五入
来源：http://vyb.hongshengwenyu.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ngv.gogol.net.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hgp.cucudq.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://cfe.yangfankeji.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://spi.bjfxy.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lfo.gogol.net.cn


<!-- 参考信息 -->