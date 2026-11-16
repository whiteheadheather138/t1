代发 wailian999

[U55] PHP：match 表达式
来源：http://gze.xuetiantiany.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tti.jiagoushi.top

[U56] PHP：命名参数
来源：http://tbw.tanke756.top

f(a: 1, b: 2)
来源：http://cxj.xuanzx.com

[U57] PHP：字符串插值
来源：http://gsc.mhx1999.top

"值: {$a}"
来源：http://lwn.cashguo.top

[U58] PHP：数组三件套
来源：http://uut.316326.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nfx.hfpthk.cn

[U59] PHP：自定义排序
来源：http://kem.zhongyouzk.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rsn.fehbvm.com

[U60] PHP：JSON 编解码
来源：http://gep.jinghuilouyu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sly.quarkkingdee.top

[U61] PHP：正则
来源：http://via.yj20258.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cja.snrcjt.cn

[U62] PHP：日期对象
来源：http://xzd.birdmap.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nfy.hnxiangtu.top

[U63] PHP：文件读写
来源：http://hsw.nanxinkj.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qjb.aizwys.cn

[U64] PHP：目录遍历
来源：http://rmq.hysaishi.cn

glob("dir/*.php");  scandir("dir");
来源：http://ibj.yj202588.top

[U65] PHP：会话
来源：http://ppc.nwbrower.top

session_start();  $_SESSION["uid"] = 1;
来源：http://shk.jlsjyb.cn

[U66] PHP：设置 Cookie
来源：http://ahv.yuanzhike.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://twk.daxiang520.top

[U67] PHP：处理文件上传
来源：http://pfk.cashguo.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xpm.yonumen.top

[U68] PHP：PDO 连接
来源：http://ged.bjfxy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xzq.havefunace.top

[U69] PHP：PDO 预处理
来源：http://cao.jiagoushi.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://msh.nwbrower.top

[U70] PHP：PDO 事务
来源：http://lgt.tian-w.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bjy.fzhhl.top

[U71] PHP：抛出异常
来源：http://arx.shuidangran.top

throw new RuntimeException("失败", 500);
来源：http://ard.yj20258888.top

[U72] PHP：写错误日志
来源：http://bkf.bbcook.cn

error_log("失败: " . $e->getMessage());
来源：http://aan.ctjpmb.com

[U73] PHP：读取 ini 配置
来源：http://rmj.fktsv.cn

parse_ini_file("config.ini", true)
来源：http://fiy.guannengcc.top

[U74] PHP：读取环境变量
来源：http://xxf.zdbjq.cn

getenv("APP_ENV") ?: "production"
来源：http://nbg.zhengqikj.top

[U75] PHP：依赖注入
来源：http://ndw.jiagoushi.top

composer require psr/container
来源：http://jeq.jqgfzy.top

[U76] PHP：简单路由
来源：http://jhq.52xcode.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ibo.xziqi.cn

[U77] PHP：模板渲染
来源：http://wsd.guowangkeji.top

composer require twig/twig
来源：http://rsz.sxryk.cn

[U78] PHP：单元测试
来源：http://iav.wangdashe.top

composer require --dev phpunit/phpunit
来源：http://yts.xylfe.cn

[U79] PHP：静态分析
来源：http://ucj.vehdjk.com

composer require --dev phpstan/phpstan
来源：http://zlf.aibaodan.cn

[U80] PHP：代码规范修复
来源：http://ejb.nwbrower.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ama.epnwcf.com

[U81] JS：初始化项目
来源：http://val.xingfuxueyuan.xyz

npm init -y;  npm i express
来源：http://fsb.pengpengdd.cyou

[U82] JS：package.json 脚本
来源：http://szv.hywenlv.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yqm.yj202588.top

[U83] JS：ES Module 导入导出
来源：http://yzs.zhaomingkeji.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://ibu.xinyue.icu

[U84] JS：CommonJS 写法
来源：http://mjj.cucudq.cn

module.exports = { a };  const { a } = require("./m");
来源：http://erm.iojbl.cn

[U85] JS：可选链
来源：http://hqy.bbcook.cn

a?.b?.c
来源：http://hef.yanxiufei.cn

[U86] JS：空值合并
来源：http://olj.ivvv.top

a ?? b
来源：http://wen.gotoacloud.top

[U87] JS：解构默认值
来源：http://rfk.yuxming.cn

const { a = 1, b = 2 } = obj;
来源：http://ofx.9152youxi.cn

[U88] JS：对象展开合并
来源：http://hjd.zycfv.cn

{ ...a, ...b }
来源：http://swd.sweek.top

[U89] JS：数组去重
来源：http://kws.cheryme.top

[...new Set(arr)]
来源：http://bcx.yj20258888.top

[U90] JS：数字数组排序
来源：http://rvt.gogol.net.cn

[...arr].sort((a, b) => a - b)
来源：http://pgu.sufxvd.cn

[U91] JS：对象键值遍历
来源：http://lbi.ydjk.org.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tud.gaohongyu789.top

[U92] JS：深拷贝
来源：http://zwg.redwolf501.top

structuredClone(obj)
来源：http://dav.hysaishi.cn

[U93] JS：模板字符串
来源：http://iip.jinqigufen.top

`共 ${n} 条`
来源：http://sto.jyoumei.cn

[U94] JS：箭头函数
来源：http://dba.feifeiyinyue.top

const double = x => x * 2;
来源：http://zay.jlsjyb.cn

[U95] JS：Promise 包装
来源：http://lii.shangyingyoupin.top

new Promise((resolve, reject) => {})
来源：http://btp.shuidangran.top

[U96] JS：async/await 与异常
来源：http://nhr.feifeiyinyue.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lae.c1oappe.top

[U97] JS：并发请求
来源：http://ehm.chenlongwang.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://wog.shangyingyoupin.top

[U98] JS：fetch 带 JSON
来源：http://odr.ydjk.org.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zpk.zhaomingkeji.xyz

[U99] JS：事件监听
来源：http://znh.dashuyun.cn

el.addEventListener("click", e => {})
来源：http://zsp.cdnleiting.top

[U100] JS：DOM 查询
来源：http://oxg.shuidangran.top

document.querySelector(".item")
来源：http://hif.ydzc1.top

[U101] JS：classList 操作
来源：http://hpb.bbcook.cn

el.classList.toggle("active")
来源：http://ocv.svipenyu.cn

[U102] JS：本地存储
来源：http://ksj.iojbl.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xwm.hnxiangtu.top

[U103] JS：定时器
来源：http://hah.ydzc1.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cjb.yanxiufei.cn

[U104] JS：防抖
来源：http://ufw.nanxuanxn.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bbk.ppjwa.cn

[U105] JS：节流
来源：http://ahc.fktsv.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zqr.smart0.xyz

[U106] JS：日期格式化
来源：http://iqg.hammf.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ziu.shuidangran.top

[U107] JS：数字千分位
来源：http://sve.cdnleiting.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gsr.andypj.xyz

[U108] JS：随机整数
来源：http://qug.zhixingplan.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jbb.ehwqpu.com

[U109] JS：数组分组
来源：http://qvs.316326.xyz

Object.groupBy(arr, x => x.type)
来源：http://eku.zhaomingkeji.xyz

[U110] JS：数组分块
来源：http://moj.ppjwa.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vzj.cqqwz.cn

[U111] JS：对象转 Map
来源：http://elv.pengpengdd.cyou

new Map(Object.entries(obj))
来源：http://cmr.zdqjudy.top

[U112] JS：字符串补位
来源：http://xzq.meibo888.top

"7".padStart(3, "0")
来源：http://hib.ydzc1.top

[U113] JS：正则替换全部
来源：http://kye.smart0.xyz

s.replaceAll("a", "b")
来源：http://bxp.nwbrower.top

[U114] JS：JSON 深比较
来源：http://kiz.aizwys.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nmw.hywenlv.cn

[U115] JS：生成 UUID
来源：http://miv.quarkkingdee.top

crypto.randomUUID()
来源：http://nty.daxiang520.top

[U116] JS：类型检查（JSDoc）
来源：http://jhr.epnwcf.com

/** @param {string} name */ function f(name) {}
来源：http://kfp.zhiwuduotai.top

[U117] JS：单元测试
来源：http://hcd.yanxiufei.cn

npm i -D vitest;  npx vitest
来源：http://ira.hfpthk.cn

[U118] JS：开发服务器
来源：http://pww.xingfuxueyuan.xyz

npm i -D vite;  npx vite
来源：http://ovz.xziqi.cn

[U119] JS：生产构建
来源：http://ssl.redwolf501.top

npx vite build
来源：http://fca.birdmap.top

[U120] JS：读取环境变量（Vite）
来源：http://usm.ywan-chungtsiang.top

import.meta.env.VITE_API_URL
来源：http://yyd.hcnkem.com

================================================================================
来源：http://fww.yongpay.top

统计汇总
来源：http://rae.uphjek.com

================================================================================
来源：http://bws.9152youxi.cn

按语言统计（条）：
来源：http://dnc.chenjidiqi.icu

Python ......... 252
来源：http://pgy.tanke756.top

PHP ............ 252
来源：http://dpw.andypj.xyz

JavaScript ..... 252
来源：http://olo.hysaishi.cn

TypeScript ..... 212
来源：http://xtg.hywenlv.cn

Java ........... 212
来源：http://wzg.aizwys.cn

Go ............. 212
来源：http://flg.shanyushiyangtech.top

Ruby ........... 212
来源：http://hbv.fzhhl.top

C# ............. 212
来源：http://oxx.cucudq.cn

C .............. 30
来源：http://ixe.aibaodan.cn

C++ ............ 30
来源：http://osu.yueranfly.top

SQL ............ 90
来源：http://ilz.hfpthk.cn

Bash ........... 80
来源：http://tpt.nanxinkj.top

Kotlin ......... 15
来源：http://kww.yj20258888.top

Swift .......... 15
来源：http://neu.gogol.net.cn

Lua ............ 10
来源：http://vul.yanxiufei.cn

Perl ........... 10
来源：http://wus.ydzc1.top

Scala .......... 10
来源：http://hhq.haohaochexian.top

------------------------------------
来源：http://bzg.bbcook.cn

合计 ........... 2106 条
来源：http://hsd.jinyuanbaomall.cn

按章节统计：
来源：http://kmo.epnwcf.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ddn.shanyushiyangkeji.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rrz.ybcxt.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://avn.jqgfzy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://euo.yuanzhike.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ywg.nanxinkj.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nhv.redwolf501.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vqj.xylfe.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sxi.guowangkeji.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mqj.zycfv.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rgj.zhongyouzk.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jpk.pycfn.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xtq.xziqi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xjv.xuanzx.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fbd.yuanzhike.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ntb.chenzaomai.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zmf.hnxiangtu.top

Q SQL 专题                              90
来源：http://irt.yuanzhike.top

R Bash 专题                             80
来源：http://fuh.zhongyouzk.top

S C / C++ 专题                          60
来源：http://bdy.yj20258.top

T 其他语言补充                          60
来源：http://won.ydjk.org.cn

U 高频实用片段                         120
来源：http://avq.wangdashe.top

------------------------------------
来源：http://ezh.daxiang520.top

合计                                  2106 条
来源：http://lof.xziqi.cn

--------------------------------------------------------------------------------
来源：http://mmi.316326.xyz

使用提醒
来源：http://gaz.cheryme.top

--------------------------------------------------------------------------------
来源：http://mcb.gaohongyu789.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://uce.aizwys.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://yuz.guowangkeji.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ili.svipenyu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://iyh.dianchejie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wlu.havefunace.top

—— 文件结束 ——
来源：http://mql.jinghuilouyu.cn

================================================================================
来源：http://vdm.fehbvm.com

程序语言常见例子速查手册（2024 版）
来源：http://mrh.fehbvm.com

Common Programming Examples Cheat Book
来源：http://wbe.uphjek.com

================================================================================
来源：http://imp.ydzc1.top

【收录内容】
来源：http://jec.ydjk.org.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://kpg.hammf.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mjg.wangshuangyany.cn

SQL · Bash · C · C++
来源：http://yyh.gogol.net.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://sym.fengsongda.top

【使用说明】
来源：http://sjw.shangyingyoupin.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qmb.shzxlz.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vch.bjfxy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tkf.yongpay.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gzx.zhiwuduotai.top

Bash:  Shell         C:     C             C++:   C++
来源：http://kls.hammf.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://uwv.uphjek.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xwm.feifeiyinyue.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://sqb.gotoacloud.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kzs.svipenyu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mts.aizwys.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://evr.xingfuxueyuan.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://via.jianghu66.top

【文件统计】
来源：http://eac.yj20258.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pxl.vqdsnc.cn

--------------------------------------------------------------------------------
来源：http://ykw.kuanghao11.cn

目  录
来源：http://piy.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://acu.shanyushiyangtech.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jpv.iojbl.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://okq.zhaomingkeji.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qij.sufxvd.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://llf.cucudq.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yeq.jinqigufen.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rvg.hysaishi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vax.hywenlv.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gzx.iojbl.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jas.hysaishi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jao.sweek.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://kmq.pengpengdd.cyou

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://nmw.vehdjk.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ymj.chenjidiqi.icu

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cvw.bjfxy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://urj.52xcode.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qmt.fanxiaobao.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lso.haohaochexian.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://lxh.nanxuanxn.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://frm.feifeiyinyue.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xxf.zycfv.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://obp.dianchejie.cn

================================================================================
来源：http://olk.jlsjyb.cn

A. 基础语法与类型
来源：http://oht.vehdjk.com

================================================================================
来源：http://kor.sysykeji.top

[A01] Hello World
来源：http://zog.zhiwuduotai.top

Py:   print("Hello, World!")
来源：http://brq.redwolf501.top

PHP:  echo "Hello, World!";
来源：http://rbc.iojbl.cn

JS:   console.log("Hello, World!");
来源：http://ssx.yvedp.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hmm.gotoacloud.top

Java: System.out.println("Hello, World!");
来源：http://yci.kuanghao11.cn

Go:   fmt.Println("Hello, World!")
来源：http://yqy.xingfuxueyuan.xyz

Ruby: puts "Hello, World!"
来源：http://ncr.ppjwa.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://sgw.fanxiaobao.xyz

[A02] 变量声明与赋值
来源：http://nas.sweek.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tzt.xuetiantiany.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://kim.hammf.cn

JS:   let name = "Alex"; const age = 20;
来源：http://odv.cucudq.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xtw.epnwcf.com

Java: String name = "Alex"; int age = 20;
来源：http://jjf.yangfankeji.com

Go:   name := "Alex"; age := 20
来源：http://ged.nwbrower.top

Ruby: name = "Alex"; age = 20
来源：http://bga.sxryk.cn

C#:   string name = "Alex"; int age = 20;
来源：http://zqx.shuidangran.top

[A03] 常量定义
来源：http://aus.zhengqikj.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ahy.316326.xyz

PHP:  const PI = 3.14159;
来源：http://egk.xingfuxueyuan.xyz

JS:   const PI = 3.14159;
来源：http://mzq.zhoulong.xyz

TS:   const PI: number = 3.14159;
来源：http://uoc.nanxuanxn.top

Java: static final double PI = 3.14159;
来源：http://dtz.vehdjk.com

Go:   const PI = 3.14159
来源：http://crh.shuidangran.top

Ruby: PI = 3.14159
来源：http://sgm.aizwys.cn

C#:   const double PI = 3.14159;
来源：http://ysz.tian-w.cn

[A04] 判断变量类型
来源：http://qft.jinyuanbaomall.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://hsb.yonumen.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://axe.yuanzhike.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qnl.hongshengwenyu.top

TS:   typeof x; x instanceof Date
来源：http://lrp.wangdashe.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ytx.sysykeji.top

Go:   reflect.TypeOf(x).Name()
来源：http://dik.jlsjyb.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://bti.yj20258.top

C#:   x.GetType().Name; x is int
来源：http://ctu.aizwys.cn

[A05] 整数除法与取模
来源：http://vzu.jqgufenzy.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://whg.xylfe.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://jvr.xuetiantiany.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ttb.zhoulong.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lln.shangyingyoupin.top

Java: 7 / 2; 7 % 2
来源：http://eii.nanxuanxn.top

Go:   7 / 2; 7 % 2
来源：http://agx.zdbjq.cn

Ruby: 7 / 2; 7 % 2
来源：http://qtt.yj20258888.top

C#:   7 / 2; 7 % 2
来源：http://aiw.xinyue.icu

[A06] 字符串转数字
来源：http://cwk.jiagoushi.top

Py:   int("42"); float("3.14")
来源：http://zsf.hongshengwenyu.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ikx.haohaochexian.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fsh.hnxiangtu.top

TS:   parseInt("42", 10); Number("42")
来源：http://zoq.hywenlv.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jjj.vehdjk.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://vtd.hfpthk.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://otv.meibo888.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dce.hnxiangtu.top

[A07] 数字转字符串
来源：http://smc.guowangkeji.top

Py:   str(42)
来源：http://vvr.bjfxy.top

PHP:  (string) 42; strval(42)
来源：http://cyj.yueranfly.top

JS:   String(42); (42).toString()
来源：http://rmb.cqqwz.cn

TS:   String(42)
来源：http://xwt.guowangkeji.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://wrq.tanke756.top

Go:   strconv.Itoa(42)
来源：http://umu.feifeiyinyue.top


<!-- 参考信息 -->