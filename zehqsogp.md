代发 wailian999

[U53] PHP：空合并运算符
来源：http://aht.jinqigfzy.top

$v = $a ?? $b ?? "default";
来源：http://zxh.havefunace.top

[U54] PHP：空安全调用
来源：http://vfm.jinqigufen.top

$obj?->method()
来源：http://aqh.jinqigfzy.top

[U55] PHP：match 表达式
来源：http://vkp.bjfxy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fqx.jqgfzy.top

[U56] PHP：命名参数
来源：http://psq.cqqwz.cn

f(a: 1, b: 2)
来源：http://rvs.ehwqpu.com

[U57] PHP：字符串插值
来源：http://jux.nwbrower.top

"值: {$a}"
来源：http://csp.jinqigufen.top

[U58] PHP：数组三件套
来源：http://kei.jqgfzy.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nnk.hysaishi.cn

[U59] PHP：自定义排序
来源：http://rvi.ywan-chungtsiang.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lqk.xylfe.cn

[U60] PHP：JSON 编解码
来源：http://eme.aizwys.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mgl.52xcode.cn

[U61] PHP：正则
来源：http://uju.andypj.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sib.hnqzz.top

[U62] PHP：日期对象
来源：http://iby.xziqi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uis.shanyushiyangtech.top

[U63] PHP：文件读写
来源：http://zun.ctjpmb.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xvt.yanxiufei.cn

[U64] PHP：目录遍历
来源：http://mfs.xziqi.cn

glob("dir/*.php");  scandir("dir");
来源：http://zxy.yfazqb.com

[U65] PHP：会话
来源：http://ols.chenlongwang.top

session_start();  $_SESSION["uid"] = 1;
来源：http://zve.ydjk.org.cn

[U66] PHP：设置 Cookie
来源：http://hhd.hesvh.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ksg.zhongyouzk.top

[U67] PHP：处理文件上传
来源：http://avh.iojbl.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://uxa.zhijiandao.cn

[U68] PHP：PDO 连接
来源：http://aqh.0kj1m.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bnw.nanxuanxn.top

[U69] PHP：PDO 预处理
来源：http://hmo.xziqi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://peu.jianghu66.top

[U70] PHP：PDO 事务
来源：http://ykd.ydjk.org.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kav.ybcxt.top

[U71] PHP：抛出异常
来源：http://wap.fehbvm.com

throw new RuntimeException("失败", 500);
来源：http://one.hcnkem.com

[U72] PHP：写错误日志
来源：http://bwo.xylfe.cn

error_log("失败: " . $e->getMessage());
来源：http://crv.zdbjq.cn

[U73] PHP：读取 ini 配置
来源：http://krs.fzhhl.top

parse_ini_file("config.ini", true)
来源：http://aqy.zhiwuduotai.top

[U74] PHP：读取环境变量
来源：http://vno.sufxvd.cn

getenv("APP_ENV") ?: "production"
来源：http://ilx.daxiang520.top

[U75] PHP：依赖注入
来源：http://orm.gotoacloud.top

composer require psr/container
来源：http://afm.ppjwa.cn

[U76] PHP：简单路由
来源：http://qhm.yvedp.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vom.sufxvd.cn

[U77] PHP：模板渲染
来源：http://flc.jiagoushi.top

composer require twig/twig
来源：http://gdx.nwbrower.top

[U78] PHP：单元测试
来源：http://jnd.xylfe.cn

composer require --dev phpunit/phpunit
来源：http://ckc.yangfankeji.com

[U79] PHP：静态分析
来源：http://rdn.uphjek.com

composer require --dev phpstan/phpstan
来源：http://scv.aibaodan.cn

[U80] PHP：代码规范修复
来源：http://hny.zdqjudy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://zaq.hcnkem.com

[U81] JS：初始化项目
来源：http://eju.hfpthk.cn

npm init -y;  npm i express
来源：http://kbp.hnqzz.top

[U82] JS：package.json 脚本
来源：http://tso.jinyuanbaomall.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hug.shzxlz.cn

[U83] JS：ES Module 导入导出
来源：http://lgj.kuanghao11.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ihu.fehbvm.com

[U84] JS：CommonJS 写法
来源：http://ysw.yj20258.top

module.exports = { a };  const { a } = require("./m");
来源：http://mad.ywan-chungtsiang.top

[U85] JS：可选链
来源：http://rbh.jinqigfzy.top

a?.b?.c
来源：http://fkr.feifeiyinyue.top

[U86] JS：空值合并
来源：http://ztu.sjlbkw.cn

a ?? b
来源：http://jes.aibaodan.cn

[U87] JS：解构默认值
来源：http://qim.ybcxt.top

const { a = 1, b = 2 } = obj;
来源：http://kbi.nanxuanxn.top

[U88] JS：对象展开合并
来源：http://ifr.hnqzz.top

{ ...a, ...b }
来源：http://xhj.hammf.cn

[U89] JS：数组去重
来源：http://ahv.bjfxy.top

[...new Set(arr)]
来源：http://ios.ydzc1.top

[U90] JS：数字数组排序
来源：http://pfp.chenlongwang.top

[...arr].sort((a, b) => a - b)
来源：http://bez.meibo888.top

[U91] JS：对象键值遍历
来源：http://lsd.aibaodan.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zje.redwolf501.top

[U92] JS：深拷贝
来源：http://kfb.hywenlv.cn

structuredClone(obj)
来源：http://zvj.bbcook.cn

[U93] JS：模板字符串
来源：http://eno.ctjpmb.com

`共 ${n} 条`
来源：http://rkc.nanxuanxn.top

[U94] JS：箭头函数
来源：http://tys.jinqigufen.top

const double = x => x * 2;
来源：http://sos.sxryk.cn

[U95] JS：Promise 包装
来源：http://qmu.sufxvd.cn

new Promise((resolve, reject) => {})
来源：http://jwi.xziqi.cn

[U96] JS：async/await 与异常
来源：http://yyo.epnwcf.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fvc.gzhubu.top

[U97] JS：并发请求
来源：http://xxp.yvedp.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://lob.chenjidiqi.icu

[U98] JS：fetch 带 JSON
来源：http://fua.jinqigufen.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mpr.mhx1999.top

[U99] JS：事件监听
来源：http://hkl.xinyue.icu

el.addEventListener("click", e => {})
来源：http://olt.tanke756.top

[U100] JS：DOM 查询
来源：http://guu.jiagoushi.top

document.querySelector(".item")
来源：http://pvc.bjfxy.top

[U101] JS：classList 操作
来源：http://xvy.sjlbkw.cn

el.classList.toggle("active")
来源：http://dsz.xinyue.icu

[U102] JS：本地存储
来源：http://uep.xingfuxueyuan.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://auj.smart0.xyz

[U103] JS：定时器
来源：http://jwg.jyoumei.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://grp.zhoulong.xyz

[U104] JS：防抖
来源：http://plq.uphjek.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nvu.dashuyun.cn

[U105] JS：节流
来源：http://qqq.dianchejie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qxb.9152youxi.cn

[U106] JS：日期格式化
来源：http://irb.feifeiyinyue.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yrq.xinyue.icu

[U107] JS：数字千分位
来源：http://dzr.wangdashe.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rxo.dashuyun.cn

[U108] JS：随机整数
来源：http://uan.gogol.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ykb.yj202588.top

[U109] JS：数组分组
来源：http://ujl.zhiwuduotai.top

Object.groupBy(arr, x => x.type)
来源：http://xqe.kuanghao11.cn

[U110] JS：数组分块
来源：http://yys.9152youxi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://env.zdbjq.cn

[U111] JS：对象转 Map
来源：http://ucu.gzhubu.top

new Map(Object.entries(obj))
来源：http://vhm.guowangkeji.top

[U112] JS：字符串补位
来源：http://odb.shuidangran.top

"7".padStart(3, "0")
来源：http://saw.cucudq.cn

[U113] JS：正则替换全部
来源：http://plb.hongshengwenyu.top

s.replaceAll("a", "b")
来源：http://pdl.haohaochexian.top

[U114] JS：JSON 深比较
来源：http://gnw.vehdjk.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://jwh.svipenyu.cn

[U115] JS：生成 UUID
来源：http://fzq.pycfn.com

crypto.randomUUID()
来源：http://gfp.ivvv.top

[U116] JS：类型检查（JSDoc）
来源：http://api.jiagoushi.top

/** @param {string} name */ function f(name) {}
来源：http://wko.yongpay.top

[U117] JS：单元测试
来源：http://yrd.zhixingplan.top

npm i -D vitest;  npx vitest
来源：http://khw.xinyue.icu

[U118] JS：开发服务器
来源：http://wog.yuxming.cn

npm i -D vite;  npx vite
来源：http://ysi.meibo888.top

[U119] JS：生产构建
来源：http://ktc.tian-w.cn

npx vite build
来源：http://kzo.yj202588.top

[U120] JS：读取环境变量（Vite）
来源：http://cxm.yvedp.cn

import.meta.env.VITE_API_URL
来源：http://aim.tanke756.top

================================================================================
来源：http://qjv.guannengcc.top

统计汇总
来源：http://fis.52xcode.cn

================================================================================
来源：http://qhl.c1oappe.top

按语言统计（条）：
来源：http://seo.mhx1999.top

Python ......... 252
来源：http://yzx.yj20258888.top

PHP ............ 252
来源：http://ups.xylfe.cn

JavaScript ..... 252
来源：http://scu.vehdjk.com

TypeScript ..... 212
来源：http://xut.yj20258888.top

Java ........... 212
来源：http://bvt.gotoacloud.top

Go ............. 212
来源：http://xdb.shangyingyoupin.top

Ruby ........... 212
来源：http://ugv.snrcjt.cn

C# ............. 212
来源：http://qvt.shangyingyoupin.top

C .............. 30
来源：http://ehw.jinqigufen.top

C++ ............ 30
来源：http://nla.ehwqpu.com

SQL ............ 90
来源：http://zrf.uphjek.com

Bash ........... 80
来源：http://jjk.c1oappe.top

Kotlin ......... 15
来源：http://lew.yangfankeji.com

Swift .......... 15
来源：http://iwe.shuidangran.top

Lua ............ 10
来源：http://nrj.pycfn.com

Perl ........... 10
来源：http://sme.shzxlz.cn

Scala .......... 10
来源：http://nno.yonumen.top

------------------------------------
来源：http://akv.sysykeji.top

合计 ........... 2106 条
来源：http://kxo.sxryk.cn

按章节统计：
来源：http://ena.dashuyun.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xmy.fengsongda.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sws.meibo888.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jjk.yj20258.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://uuu.guowangkeji.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://llm.birdmap.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://muk.hammf.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cgl.daxiang520.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nyn.gogol.net.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://swk.yj202588.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fib.zhiwuduotai.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rhx.zhixingplan.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://eda.chenzaomai.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dvn.redwolf501.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kai.feifeiyinyue.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lse.zhijiandao.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wgq.yueranfly.top

Q SQL 专题                              90
来源：http://ozk.vehdjk.com

R Bash 专题                             80
来源：http://ssd.cqqwz.cn

S C / C++ 专题                          60
来源：http://gog.ivvv.top

T 其他语言补充                          60
来源：http://ikn.dianchejie.cn

U 高频实用片段                         120
来源：http://imo.fanxiaobao.xyz

------------------------------------
来源：http://hyj.hammf.cn

合计                                  2106 条
来源：http://idn.epnwcf.com

--------------------------------------------------------------------------------
来源：http://vai.snrcjt.cn

使用提醒
来源：http://lcb.cheryme.top

--------------------------------------------------------------------------------
来源：http://stp.chenzaomai.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://imd.ydzc1.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kkq.bjfxy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://sln.0kj1m.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://kpn.c1oappe.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gvb.redwolf501.top

—— 文件结束 ——
来源：http://xjd.ydjk.org.cn

================================================================================
来源：http://drk.jianghu66.top

程序语言常见例子速查手册（2024 版）
来源：http://isf.316326.xyz

Common Programming Examples Cheat Book
来源：http://twu.fktsv.cn

================================================================================
来源：http://jip.bbcook.cn

【收录内容】
来源：http://bkg.ywan-chungtsiang.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://nxo.jlsjyb.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zcs.jinghuilouyu.cn

SQL · Bash · C · C++
来源：http://zze.nwbrower.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://bzg.shanyushiyangkeji.top

【使用说明】
来源：http://elm.zdbjq.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://oxg.hywenlv.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vkw.xuetiantiany.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xpt.chenlongwang.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://smd.cheryme.top

Bash:  Shell         C:     C             C++:   C++
来源：http://jpj.nanxinkj.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hsf.quarkkingdee.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gtq.yuanzhike.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ufs.jianghu66.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://egb.zhengqikj.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://smd.jinyuanbaomall.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rsj.xinyue.icu

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://eso.pengpengdd.cyou

【文件统计】
来源：http://dqz.jiagoushi.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://syl.shzxlz.cn

--------------------------------------------------------------------------------
来源：http://msd.cucudq.cn

目  录
来源：http://qpp.hnqzz.top

--------------------------------------------------------------------------------
来源：http://haj.tian-w.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dfy.jinqigufen.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ynv.sysykeji.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://veu.hongshengwenyu.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fcq.hfpthk.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://boi.cashguo.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ecg.xziqi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://cac.hnxiangtu.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wze.aibaodan.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://cpw.yangfankeji.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rjw.cheryme.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ybq.xingfuxueyuan.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rnb.jianghu66.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://txj.zycfv.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://klu.aibaodan.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mdv.xingfuxueyuan.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://pma.guannengcc.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://urq.redwolf501.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://bzq.jyoumei.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://afb.yonumen.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bdg.vehdjk.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mrt.fehbvm.com

================================================================================
来源：http://iew.xuetiantiany.cn

A. 基础语法与类型
来源：http://fsx.cucudq.cn

================================================================================
来源：http://leg.zhengqikj.top

[A01] Hello World
来源：http://rnr.jqgufenzy.top

Py:   print("Hello, World!")
来源：http://xnq.jqgufenzy.top

PHP:  echo "Hello, World!";
来源：http://ieq.andypj.xyz

JS:   console.log("Hello, World!");
来源：http://kpl.hnqzz.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yzb.yj20258.top

Java: System.out.println("Hello, World!");
来源：http://jtp.dashuyun.cn

Go:   fmt.Println("Hello, World!")
来源：http://ldt.jyoumei.cn

Ruby: puts "Hello, World!"
来源：http://sws.yvedp.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://rrk.svipenyu.cn

[A02] 变量声明与赋值
来源：http://pjv.wangdashe.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ybp.mhx1999.top

PHP:  $name = "Alex"; $age = 20;
来源：http://wzm.aizwys.cn

JS:   let name = "Alex"; const age = 20;
来源：http://exi.yuanzhike.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://opf.wangshuangyany.cn

Java: String name = "Alex"; int age = 20;
来源：http://gao.zhengqikj.top

Go:   name := "Alex"; age := 20
来源：http://dfv.c1oappe.top

Ruby: name = "Alex"; age = 20
来源：http://gjs.yongpay.top

C#:   string name = "Alex"; int age = 20;
来源：http://aaf.cashguo.top

[A03] 常量定义
来源：http://bga.xylfe.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://sxq.gogol.net.cn

PHP:  const PI = 3.14159;
来源：http://opo.sjlbkw.cn

JS:   const PI = 3.14159;
来源：http://qnt.yanxiufei.cn

TS:   const PI: number = 3.14159;
来源：http://jkq.yj202588.top

Java: static final double PI = 3.14159;
来源：http://xpr.ppjwa.cn

Go:   const PI = 3.14159
来源：http://zfh.yfazqb.com

Ruby: PI = 3.14159
来源：http://ksc.quarkkingdee.top

C#:   const double PI = 3.14159;
来源：http://irb.sxryk.cn

[A04] 判断变量类型
来源：http://mvi.vehdjk.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://guo.iojbl.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ghi.c1oappe.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wku.svipenyu.cn

TS:   typeof x; x instanceof Date
来源：http://gvx.yongpay.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wfn.uphjek.com

Go:   reflect.TypeOf(x).Name()
来源：http://xrg.xingfuxueyuan.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://nwm.shanyushiyangtech.top

C#:   x.GetType().Name; x is int
来源：http://gfp.zhijiandao.cn

[A05] 整数除法与取模
来源：http://zas.tanke756.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ivn.yj202588.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://wfp.zhengqikj.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://kbe.nanxuanxn.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gqp.vqdsnc.cn

Java: 7 / 2; 7 % 2
来源：http://xnq.cdnleiting.top

Go:   7 / 2; 7 % 2
来源：http://lem.316326.xyz

Ruby: 7 / 2; 7 % 2
来源：http://hxx.yongpay.top

C#:   7 / 2; 7 % 2
来源：http://fjn.hfpthk.cn

[A06] 字符串转数字
来源：http://xaz.yueranfly.top

Py:   int("42"); float("3.14")
来源：http://vbg.shuidangran.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gys.jqgfzy.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hnl.gotoacloud.top

TS:   parseInt("42", 10); Number("42")
来源：http://gnj.sweek.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jmj.0kj1m.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ydc.bbcook.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://gvh.zhongyouzk.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cnb.sweek.top

[A07] 数字转字符串
来源：http://ypv.daxiang520.top

Py:   str(42)
来源：http://bjy.fanxiaobao.xyz

PHP:  (string) 42; strval(42)
来源：http://jwh.jinqigufen.top


<!-- 参考信息 -->