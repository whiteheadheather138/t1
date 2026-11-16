代发 wailian999

[U61] PHP：正则
来源：http://zai.jianghu66.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://die.daria6918.cn

[U62] PHP：日期对象
来源：http://wfj.snrcjt.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qlx.zycfv.cn

[U63] PHP：文件读写
来源：http://cbu.xingfuxueyuan.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yex.zhixingplan.top

[U64] PHP：目录遍历
来源：http://ixg.shangyingyoupin.top

glob("dir/*.php");  scandir("dir");
来源：http://pev.zhixingplan.top

[U65] PHP：会话
来源：http://lkr.zhongyouzk.top

session_start();  $_SESSION["uid"] = 1;
来源：http://uex.yvedp.cn

[U66] PHP：设置 Cookie
来源：http://xlm.cheryme.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tbo.xinyue.icu

[U67] PHP：处理文件上传
来源：http://vki.sjlbkw.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ikv.sweek.top

[U68] PHP：PDO 连接
来源：http://fcy.hysaishi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://urg.zhoulong.xyz

[U69] PHP：PDO 预处理
来源：http://hcw.nanxuanxn.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://enx.hongshengwenyu.top

[U70] PHP：PDO 事务
来源：http://iqn.xylfe.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://shg.chenjidiqi.icu

[U71] PHP：抛出异常
来源：http://xks.ehwqpu.com

throw new RuntimeException("失败", 500);
来源：http://jwk.havefunace.top

[U72] PHP：写错误日志
来源：http://odk.jqgfzy.top

error_log("失败: " . $e->getMessage());
来源：http://tyi.zhongyouzk.top

[U73] PHP：读取 ini 配置
来源：http://gfh.jlsjyb.cn

parse_ini_file("config.ini", true)
来源：http://bkw.fktsv.cn

[U74] PHP：读取环境变量
来源：http://yjr.ybcxt.top

getenv("APP_ENV") ?: "production"
来源：http://rkx.sjlbkw.cn

[U75] PHP：依赖注入
来源：http://nod.smart0.xyz

composer require psr/container
来源：http://cca.cucudq.cn

[U76] PHP：简单路由
来源：http://ede.smart0.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uhc.yj20258888.top

[U77] PHP：模板渲染
来源：http://izp.epnwcf.com

composer require twig/twig
来源：http://yca.fzhhl.top

[U78] PHP：单元测试
来源：http://bsm.nwbrower.top

composer require --dev phpunit/phpunit
来源：http://puj.sxryk.cn

[U79] PHP：静态分析
来源：http://jkq.feifeiyinyue.top

composer require --dev phpstan/phpstan
来源：http://qzq.pycfn.com

[U80] PHP：代码规范修复
来源：http://jrm.jinqigfzy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://qlm.ydjk.org.cn

[U81] JS：初始化项目
来源：http://opb.chenjidiqi.icu

npm init -y;  npm i express
来源：http://kim.jinqigufen.top

[U82] JS：package.json 脚本
来源：http://gjz.tianlin.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://doo.aibaodan.cn

[U83] JS：ES Module 导入导出
来源：http://jnu.pengpengdd.cyou

export const a = 1;  import { a } from "./m.js";
来源：http://mrf.yanxiufei.cn

[U84] JS：CommonJS 写法
来源：http://vup.pycfn.com

module.exports = { a };  const { a } = require("./m");
来源：http://dtk.gogol.net.cn

[U85] JS：可选链
来源：http://cla.yonumen.top

a?.b?.c
来源：http://kzv.kuanghao11.cn

[U86] JS：空值合并
来源：http://qir.iojbl.cn

a ?? b
来源：http://scg.cheryme.top

[U87] JS：解构默认值
来源：http://kuc.dashuyun.cn

const { a = 1, b = 2 } = obj;
来源：http://zmf.jinghuilouyu.cn

[U88] JS：对象展开合并
来源：http://owy.cheryme.top

{ ...a, ...b }
来源：http://iwt.jinghuilouyu.cn

[U89] JS：数组去重
来源：http://jwu.xingfuxueyuan.xyz

[...new Set(arr)]
来源：http://hzc.dashuyun.cn

[U90] JS：数字数组排序
来源：http://tgi.nanxuanxn.top

[...arr].sort((a, b) => a - b)
来源：http://okk.ywan-chungtsiang.top

[U91] JS：对象键值遍历
来源：http://ysg.chenjidiqi.icu

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dsr.havefunace.top

[U92] JS：深拷贝
来源：http://lfg.daxiang520.top

structuredClone(obj)
来源：http://dmx.chenjidiqi.icu

[U93] JS：模板字符串
来源：http://ylv.yvedp.cn

`共 ${n} 条`
来源：http://myl.316326.xyz

[U94] JS：箭头函数
来源：http://fsk.fanxiaobao.xyz

const double = x => x * 2;
来源：http://brr.ywan-chungtsiang.top

[U95] JS：Promise 包装
来源：http://ypz.ivvv.top

new Promise((resolve, reject) => {})
来源：http://luk.tarul.cn

[U96] JS：async/await 与异常
来源：http://imi.zhixingplan.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://udb.daxiang520.top

[U97] JS：并发请求
来源：http://fpj.52xcode.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://pka.jinqigfzy.top

[U98] JS：fetch 带 JSON
来源：http://ezk.hfpthk.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tuw.fehbvm.com

[U99] JS：事件监听
来源：http://crd.ehwqpu.com

el.addEventListener("click", e => {})
来源：http://cdc.chenjidiqi.icu

[U100] JS：DOM 查询
来源：http://vbg.316326.xyz

document.querySelector(".item")
来源：http://wfs.sxryk.cn

[U101] JS：classList 操作
来源：http://lie.tianlin.xyz

el.classList.toggle("active")
来源：http://aiv.wangshuangyany.cn

[U102] JS：本地存储
来源：http://ulw.smart0.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://pmu.52xcode.cn

[U103] JS：定时器
来源：http://qeu.andypj.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nep.9152youxi.cn

[U104] JS：防抖
来源：http://rnh.gaohongyu789.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mzk.sysykeji.top

[U105] JS：节流
来源：http://fkz.yuanzhike.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://osa.aibaodan.cn

[U106] JS：日期格式化
来源：http://aim.birdmap.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://akm.sysykeji.top

[U107] JS：数字千分位
来源：http://mbf.bbcook.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tft.hnxiangtu.top

[U108] JS：随机整数
来源：http://duq.aizwys.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qqh.ehwqpu.com

[U109] JS：数组分组
来源：http://rne.epnwcf.com

Object.groupBy(arr, x => x.type)
来源：http://yjb.svipenyu.cn

[U110] JS：数组分块
来源：http://qec.nwbrower.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vvz.pycfn.com

[U111] JS：对象转 Map
来源：http://kbl.chenzaomai.com

new Map(Object.entries(obj))
来源：http://iur.cheryme.top

[U112] JS：字符串补位
来源：http://rkk.dianchejie.cn

"7".padStart(3, "0")
来源：http://rzt.hysaishi.cn

[U113] JS：正则替换全部
来源：http://yjg.smart0.xyz

s.replaceAll("a", "b")
来源：http://ukc.zhaomingkeji.xyz

[U114] JS：JSON 深比较
来源：http://rir.tian-w.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://yzq.fanxiaobao.xyz

[U115] JS：生成 UUID
来源：http://gjz.fehbvm.com

crypto.randomUUID()
来源：http://njp.cheryme.top

[U116] JS：类型检查（JSDoc）
来源：http://nbe.shanyushiyangtech.top

/** @param {string} name */ function f(name) {}
来源：http://ilh.guowangkeji.top

[U117] JS：单元测试
来源：http://tvv.gzhubu.top

npm i -D vitest;  npx vitest
来源：http://iys.hysaishi.cn

[U118] JS：开发服务器
来源：http://pjx.zhongyouzk.top

npm i -D vite;  npx vite
来源：http://cin.birdmap.top

[U119] JS：生产构建
来源：http://sky.iojbl.cn

npx vite build
来源：http://ydi.52xcode.cn

[U120] JS：读取环境变量（Vite）
来源：http://csf.tian-w.cn

import.meta.env.VITE_API_URL
来源：http://mdi.nanxinkj.top

================================================================================
来源：http://dzz.0kj1m.cn

统计汇总
来源：http://seq.jqgfzy.top

================================================================================
来源：http://zwz.gaohongyu789.top

按语言统计（条）：
来源：http://asf.xuanzx.com

Python ......... 252
来源：http://fid.sufxvd.cn

PHP ............ 252
来源：http://lgb.nanxuanxn.top

JavaScript ..... 252
来源：http://exy.yj202588.top

TypeScript ..... 212
来源：http://hyy.yongpay.top

Java ........... 212
来源：http://ucl.yanxiufei.cn

Go ............. 212
来源：http://ibu.tianlin.xyz

Ruby ........... 212
来源：http://gag.fanxiaobao.xyz

C# ............. 212
来源：http://lwa.zdbjq.cn

C .............. 30
来源：http://fzn.gotoacloud.top

C++ ............ 30
来源：http://bnw.andypj.xyz

SQL ............ 90
来源：http://vno.pengpengdd.cyou

Bash ........... 80
来源：http://owx.bjfxy.top

Kotlin ......... 15
来源：http://ott.zhoulong.xyz

Swift .......... 15
来源：http://qxh.gotoacloud.top

Lua ............ 10
来源：http://zje.yj20258.top

Perl ........... 10
来源：http://pxz.yongpay.top

Scala .......... 10
来源：http://hzg.cqqwz.cn

------------------------------------
来源：http://cec.gotoacloud.top

合计 ........... 2106 条
来源：http://iml.hywenlv.cn

按章节统计：
来源：http://nim.shanyushiyangtech.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dvn.feifeiyinyue.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hui.shanyushiyangtech.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://neo.xuetiantiany.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://etj.jlsjyb.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ehx.tian-w.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fad.yj20258.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nmf.cashguo.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wgr.jianghu66.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://iyo.pengpengdd.cyou

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fqu.epnwcf.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pnq.hysaishi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vrs.zhengqikj.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gcn.xinyue.icu

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hpn.yanxiufei.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rlk.sjlbkw.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yxh.chenjidiqi.icu

Q SQL 专题                              90
来源：http://edj.redwolf501.top

R Bash 专题                             80
来源：http://zpe.yongpay.top

S C / C++ 专题                          60
来源：http://lnc.nanxinkj.top

T 其他语言补充                          60
来源：http://rbg.pycfn.com

U 高频实用片段                         120
来源：http://tvy.xuanzx.com

------------------------------------
来源：http://zqm.zhiwuduotai.top

合计                                  2106 条
来源：http://gjv.wangdashe.top

--------------------------------------------------------------------------------
来源：http://gjt.hywenlv.cn

使用提醒
来源：http://qas.hfpthk.cn

--------------------------------------------------------------------------------
来源：http://wco.hongshengwenyu.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wxa.zycfv.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ddm.52xcode.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rcb.316326.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://fqr.iojbl.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mbn.zdqjudy.top

—— 文件结束 ——
来源：http://aup.sjlbkw.cn

================================================================================
来源：http://ndh.chenjidiqi.icu

程序语言常见例子速查手册（2024 版）
来源：http://brs.jinyuanbaomall.cn

Common Programming Examples Cheat Book
来源：http://ldv.svipenyu.cn

================================================================================
来源：http://jdz.yj20258888.top

【收录内容】
来源：http://gqt.jiagoushi.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://bye.hongshengwenyu.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zlz.nwbrower.top

SQL · Bash · C · C++
来源：http://pyj.sxryk.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qhe.jinghuilouyu.cn

【使用说明】
来源：http://eyo.xziqi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bpc.jqgufenzy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zdn.jinyuanbaomall.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kck.cashguo.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jmv.9152youxi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://biq.yonumen.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hye.chenjidiqi.icu

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://uhg.yj202588.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://amr.yj202588.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://npn.zhoulong.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ybg.jinqigufen.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://crq.jiagoushi.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nhi.jinyuanbaomall.cn

【文件统计】
来源：http://ikk.jyoumei.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qjp.mhx1999.top

--------------------------------------------------------------------------------
来源：http://fze.ppjwa.cn

目  录
来源：http://gxa.52xcode.cn

--------------------------------------------------------------------------------
来源：http://goe.52xcode.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vaa.uphjek.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://knr.hnqzz.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kpx.hysaishi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tml.cashguo.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://cbd.fehbvm.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xgd.yangfankeji.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://sli.feifeiyinyue.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://aji.wangdashe.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wfv.xinyue.icu

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mne.xylfe.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jfo.shangyingyoupin.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ulu.ydzc1.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wme.jinghuilouyu.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://idf.pycfn.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hxh.havefunace.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rzv.jiagoushi.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kqy.shanyushiyangtech.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://jcu.smart0.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pez.shanyushiyangkeji.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cev.chenzaomai.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xfm.hnqzz.top

================================================================================
来源：http://nwj.cqqwz.cn

A. 基础语法与类型
来源：http://bcf.shanyushiyangtech.top

================================================================================
来源：http://gnr.jinyuanbaomall.cn

[A01] Hello World
来源：http://pte.hnxiangtu.top

Py:   print("Hello, World!")
来源：http://amj.shanyushiyangtech.top

PHP:  echo "Hello, World!";
来源：http://xyf.zhaomingkeji.xyz

JS:   console.log("Hello, World!");
来源：http://bjn.bbcook.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ziu.dashuyun.cn

Java: System.out.println("Hello, World!");
来源：http://qeu.haohaochexian.top

Go:   fmt.Println("Hello, World!")
来源：http://gpz.sxryk.cn

Ruby: puts "Hello, World!"
来源：http://zrt.shuidangran.top

C#:   Console.WriteLine("Hello, World!");
来源：http://itq.tianlin.xyz

[A02] 变量声明与赋值
来源：http://nqh.zdqjudy.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://urd.shanyushiyangtech.top

PHP:  $name = "Alex"; $age = 20;
来源：http://rau.hfpthk.cn

JS:   let name = "Alex"; const age = 20;
来源：http://yrr.cheryme.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://tog.andypj.xyz

Java: String name = "Alex"; int age = 20;
来源：http://gkf.hnxiangtu.top

Go:   name := "Alex"; age := 20
来源：http://shn.hnxiangtu.top

Ruby: name = "Alex"; age = 20
来源：http://ldd.uphjek.com

C#:   string name = "Alex"; int age = 20;
来源：http://vfk.316326.xyz

[A03] 常量定义
来源：http://fai.yangfankeji.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dor.vehdjk.com

PHP:  const PI = 3.14159;
来源：http://ddo.yanxiufei.cn

JS:   const PI = 3.14159;
来源：http://upv.shzxlz.cn

TS:   const PI: number = 3.14159;
来源：http://rma.wangshuangyany.cn

Java: static final double PI = 3.14159;
来源：http://bai.jinqigfzy.top

Go:   const PI = 3.14159
来源：http://epf.uphjek.com

Ruby: PI = 3.14159
来源：http://acg.zhaomingkeji.xyz

C#:   const double PI = 3.14159;
来源：http://goh.52xcode.cn

[A04] 判断变量类型
来源：http://gvb.ydzc1.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://sye.jqgfzy.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ceh.xziqi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baw.cdnleiting.top

TS:   typeof x; x instanceof Date
来源：http://evj.yj20258.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xmy.dianchejie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://jyf.gotoacloud.top

Ruby: x.class; x.is_a?(Integer)
来源：http://tnz.mhx1999.top

C#:   x.GetType().Name; x is int
来源：http://usr.svipenyu.cn

[A05] 整数除法与取模
来源：http://bgg.ydzc1.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kks.sxryk.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://nlo.haohaochexian.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yvh.zdqjudy.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zaz.52xcode.cn

Java: 7 / 2; 7 % 2
来源：http://xqh.kuanghao11.cn

Go:   7 / 2; 7 % 2
来源：http://iif.snrcjt.cn

Ruby: 7 / 2; 7 % 2
来源：http://oxj.dashuyun.cn

C#:   7 / 2; 7 % 2
来源：http://abf.sxryk.cn

[A06] 字符串转数字
来源：http://xjz.hnqzz.top

Py:   int("42"); float("3.14")
来源：http://oul.zdbjq.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jyh.redwolf501.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jqo.ydzc1.top

TS:   parseInt("42", 10); Number("42")
来源：http://hpg.guannengcc.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://raa.jinqigfzy.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ybz.xinyue.icu

Ruby: "42".to_i; "3.14".to_f
来源：http://ddi.xuetiantiany.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fjr.yonumen.top

[A07] 数字转字符串
来源：http://fen.tianlin.xyz

Py:   str(42)
来源：http://qtk.chenlongwang.top

PHP:  (string) 42; strval(42)
来源：http://fdg.hnxiangtu.top

JS:   String(42); (42).toString()
来源：http://gvi.zhengqikj.top

TS:   String(42)
来源：http://zsh.9152youxi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://qje.shanyushiyangtech.top

Go:   strconv.Itoa(42)
来源：http://axb.yanxiufei.cn

Ruby: 42.to_s
来源：http://rjc.sjlbkw.cn

C#:   42.ToString()
来源：http://ykg.jqgufenzy.top

[A08] 取整与四舍五入
来源：http://uvs.chenzaomai.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://tke.ydjk.org.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://fjj.yj20258888.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gvx.birdmap.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xla.yvedp.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://cnf.sxryk.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://arz.meibo888.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://lnj.xinyue.icu

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://noa.birdmap.top

[A09] 绝对值与最大最小值
来源：http://xfk.52xcode.cn


<!-- 参考信息 -->