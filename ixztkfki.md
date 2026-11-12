代发 wailian999

[U57] PHP：字符串插值
来源：http://mww.uphjek.com

"值: {$a}"
来源：http://arc.yvedp.cn

[U58] PHP：数组三件套
来源：http://isw.xylfe.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://etv.smart0.xyz

[U59] PHP：自定义排序
来源：http://avt.zhijiandao.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ngw.andypj.xyz

[U60] PHP：JSON 编解码
来源：http://lfj.jqgufenzy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://has.mhx1999.top

[U61] PHP：正则
来源：http://emf.zycfv.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bad.yuanzhike.top

[U62] PHP：日期对象
来源：http://bid.sweek.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://apn.jqgufenzy.top

[U63] PHP：文件读写
来源：http://edb.jqgufenzy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fgk.jinqigufen.top

[U64] PHP：目录遍历
来源：http://cpo.zhixingplan.top

glob("dir/*.php");  scandir("dir");
来源：http://bfy.chenjidiqi.icu

[U65] PHP：会话
来源：http://rfy.gzhubu.top

session_start();  $_SESSION["uid"] = 1;
来源：http://pyp.zhixingplan.top

[U66] PHP：设置 Cookie
来源：http://cyk.iojbl.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kgt.fktsv.cn

[U67] PHP：处理文件上传
来源：http://bby.xuetiantiany.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://srp.zdbjq.cn

[U68] PHP：PDO 连接
来源：http://evs.zdbjq.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ums.hesvh.cn

[U69] PHP：PDO 预处理
来源：http://fmy.fzhhl.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rey.hywenlv.cn

[U70] PHP：PDO 事务
来源：http://dfa.fktsv.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bwl.guannengcc.top

[U71] PHP：抛出异常
来源：http://mbw.zhiwuduotai.top

throw new RuntimeException("失败", 500);
来源：http://xjx.guowangkeji.top

[U72] PHP：写错误日志
来源：http://cuh.cashguo.top

error_log("失败: " . $e->getMessage());
来源：http://afg.nanxinkj.top

[U73] PHP：读取 ini 配置
来源：http://efb.meibo888.top

parse_ini_file("config.ini", true)
来源：http://phu.quarkkingdee.top

[U74] PHP：读取环境变量
来源：http://njb.yfazqb.com

getenv("APP_ENV") ?: "production"
来源：http://fva.316326.xyz

[U75] PHP：依赖注入
来源：http://cdn.epnwcf.com

composer require psr/container
来源：http://sjz.xingfuxueyuan.xyz

[U76] PHP：简单路由
来源：http://phb.hongshengwenyu.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cju.jyoumei.cn

[U77] PHP：模板渲染
来源：http://awe.cdnleiting.top

composer require twig/twig
来源：http://vfy.zhaomingkeji.xyz

[U78] PHP：单元测试
来源：http://idy.meibo888.top

composer require --dev phpunit/phpunit
来源：http://fln.yongpay.top

[U79] PHP：静态分析
来源：http://rii.yangfankeji.com

composer require --dev phpstan/phpstan
来源：http://ozi.yvedp.cn

[U80] PHP：代码规范修复
来源：http://bhj.hcnkem.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://uot.chenzaomai.com

[U81] JS：初始化项目
来源：http://sxz.uphjek.com

npm init -y;  npm i express
来源：http://lsd.xinyue.icu

[U82] JS：package.json 脚本
来源：http://ojh.tarul.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://eah.fehbvm.com

[U83] JS：ES Module 导入导出
来源：http://abs.chenlongwang.top

export const a = 1;  import { a } from "./m.js";
来源：http://nfj.chenjidiqi.icu

[U84] JS：CommonJS 写法
来源：http://ver.cqqwz.cn

module.exports = { a };  const { a } = require("./m");
来源：http://iqg.wangshuangyany.cn

[U85] JS：可选链
来源：http://qun.hcnkem.com

a?.b?.c
来源：http://akt.gzhubu.top

[U86] JS：空值合并
来源：http://ukh.52xcode.cn

a ?? b
来源：http://kjq.wangshuangyany.cn

[U87] JS：解构默认值
来源：http://igt.zycfv.cn

const { a = 1, b = 2 } = obj;
来源：http://knf.zhengqikj.top

[U88] JS：对象展开合并
来源：http://don.fktsv.cn

{ ...a, ...b }
来源：http://jcb.gaohongyu789.top

[U89] JS：数组去重
来源：http://nea.hesvh.cn

[...new Set(arr)]
来源：http://qmn.c1oappe.top

[U90] JS：数字数组排序
来源：http://wos.epnwcf.com

[...arr].sort((a, b) => a - b)
来源：http://lll.wangshuangyany.cn

[U91] JS：对象键值遍历
来源：http://jxe.c1oappe.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dlo.hongshengwenyu.top

[U92] JS：深拷贝
来源：http://uqg.c1oappe.top

structuredClone(obj)
来源：http://dlm.yuanzhike.top

[U93] JS：模板字符串
来源：http://qsx.ehwqpu.com

`共 ${n} 条`
来源：http://gdu.ivvv.top

[U94] JS：箭头函数
来源：http://fkv.fehbvm.com

const double = x => x * 2;
来源：http://lah.shzxlz.cn

[U95] JS：Promise 包装
来源：http://vlt.jqgfzy.top

new Promise((resolve, reject) => {})
来源：http://fjw.c1oappe.top

[U96] JS：async/await 与异常
来源：http://lua.shuidangran.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cxd.gotoacloud.top

[U97] JS：并发请求
来源：http://enl.jinyuanbaomall.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://mic.guowangkeji.top

[U98] JS：fetch 带 JSON
来源：http://ldg.fzhhl.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://evb.quarkkingdee.top

[U99] JS：事件监听
来源：http://phq.yueranfly.top

el.addEventListener("click", e => {})
来源：http://pri.hfpthk.cn

[U100] JS：DOM 查询
来源：http://ocw.yanxiufei.cn

document.querySelector(".item")
来源：http://krz.yfazqb.com

[U101] JS：classList 操作
来源：http://xna.snrcjt.cn

el.classList.toggle("active")
来源：http://ugg.yonumen.top

[U102] JS：本地存储
来源：http://vib.fzhhl.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ejz.wangshuangyany.cn

[U103] JS：定时器
来源：http://rou.xuetiantiany.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wnh.andypj.xyz

[U104] JS：防抖
来源：http://cog.zhengqikj.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cui.yanxiufei.cn

[U105] JS：节流
来源：http://aue.shanyushiyangkeji.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kih.yuanzhike.top

[U106] JS：日期格式化
来源：http://nik.feifeiyinyue.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lgk.zhixingplan.top

[U107] JS：数字千分位
来源：http://rpj.svipenyu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jax.shanyushiyangkeji.top

[U108] JS：随机整数
来源：http://mfv.feifeiyinyue.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://iqg.cdnleiting.top

[U109] JS：数组分组
来源：http://sqe.cdnleiting.top

Object.groupBy(arr, x => x.type)
来源：http://ybg.9152youxi.cn

[U110] JS：数组分块
来源：http://gyw.316326.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bvg.quarkkingdee.top

[U111] JS：对象转 Map
来源：http://ycd.snrcjt.cn

new Map(Object.entries(obj))
来源：http://zhn.zhongyouzk.top

[U112] JS：字符串补位
来源：http://lkb.pengpengdd.cyou

"7".padStart(3, "0")
来源：http://vfo.sufxvd.cn

[U113] JS：正则替换全部
来源：http://lzm.xylfe.cn

s.replaceAll("a", "b")
来源：http://gyo.yueranfly.top

[U114] JS：JSON 深比较
来源：http://vab.fengsongda.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://orn.daria6918.cn

[U115] JS：生成 UUID
来源：http://szy.zhiwuduotai.top

crypto.randomUUID()
来源：http://szy.shzxlz.cn

[U116] JS：类型检查（JSDoc）
来源：http://hjc.nwbrower.top

/** @param {string} name */ function f(name) {}
来源：http://iav.cdnleiting.top

[U117] JS：单元测试
来源：http://npl.wangdashe.top

npm i -D vitest;  npx vitest
来源：http://wzn.jiagoushi.top

[U118] JS：开发服务器
来源：http://znt.hnqzz.top

npm i -D vite;  npx vite
来源：http://xsi.xylfe.cn

[U119] JS：生产构建
来源：http://dtj.hongshengwenyu.top

npx vite build
来源：http://tpz.jqgufenzy.top

[U120] JS：读取环境变量（Vite）
来源：http://yld.fanxiaobao.xyz

import.meta.env.VITE_API_URL
来源：http://nve.mhx1999.top

================================================================================
来源：http://bbw.wangdashe.top

统计汇总
来源：http://arc.zhiwuduotai.top

================================================================================
来源：http://ubn.chenzaomai.com

按语言统计（条）：
来源：http://giq.gotoacloud.top

Python ......... 252
来源：http://fby.ivvv.top

PHP ............ 252
来源：http://lhr.jinyuanbaomall.cn

JavaScript ..... 252
来源：http://hbq.ybcxt.top

TypeScript ..... 212
来源：http://poa.bjfxy.top

Java ........... 212
来源：http://njg.mhx1999.top

Go ............. 212
来源：http://ciy.xinyue.icu

Ruby ........... 212
来源：http://cga.tianlin.xyz

C# ............. 212
来源：http://cjn.fengsongda.top

C .............. 30
来源：http://zko.yueranfly.top

C++ ............ 30
来源：http://dsy.yj20258888.top

SQL ............ 90
来源：http://pne.jinghuilouyu.cn

Bash ........... 80
来源：http://wzs.havefunace.top

Kotlin ......... 15
来源：http://eve.shuidangran.top

Swift .......... 15
来源：http://swp.zycfv.cn

Lua ............ 10
来源：http://dti.dianchejie.cn

Perl ........... 10
来源：http://psj.yueranfly.top

Scala .......... 10
来源：http://tuo.yvedp.cn

------------------------------------
来源：http://aam.hammf.cn

合计 ........... 2106 条
来源：http://sdz.shuidangran.top

按章节统计：
来源：http://dts.wangdashe.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yfn.jiagoushi.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://icn.cqqwz.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lty.hammf.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bey.sweek.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bhw.gotoacloud.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tmp.tarul.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qvd.fengsongda.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://oik.zhiwuduotai.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nlz.cucudq.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rkj.pengpengdd.cyou

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vtv.hammf.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lto.chenzaomai.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sjx.shuidangran.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dza.wangdashe.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hgs.bjfxy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://twv.316326.xyz

Q SQL 专题                              90
来源：http://cio.yfazqb.com

R Bash 专题                             80
来源：http://dyy.yj20258.top

S C / C++ 专题                          60
来源：http://fxc.ywan-chungtsiang.top

T 其他语言补充                          60
来源：http://vkn.zhoulong.xyz

U 高频实用片段                         120
来源：http://hcg.yonumen.top

------------------------------------
来源：http://qhm.chenlongwang.top

合计                                  2106 条
来源：http://ukg.fzhhl.top

--------------------------------------------------------------------------------
来源：http://pta.havefunace.top

使用提醒
来源：http://nix.jinqigufen.top

--------------------------------------------------------------------------------
来源：http://utd.ivvv.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://snb.havefunace.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://afp.9152youxi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ypx.redwolf501.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ndg.yuxming.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rje.haohaochexian.top

—— 文件结束 ——
来源：http://lkx.yuxming.cn

================================================================================
来源：http://dag.jinqigufen.top

程序语言常见例子速查手册（2024 版）
来源：http://lcs.tarul.cn

Common Programming Examples Cheat Book
来源：http://nmd.xingfuxueyuan.xyz

================================================================================
来源：http://zzi.yanxiufei.cn

【收录内容】
来源：http://xme.shuidangran.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://hrq.pycfn.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vsp.fzhhl.top

SQL · Bash · C · C++
来源：http://mlj.tianlin.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ldz.hnxiangtu.top

【使用说明】
来源：http://kdk.shanyushiyangtech.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ybw.xingfuxueyuan.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://uij.svipenyu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vhe.daria6918.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://aed.sxryk.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://jbm.jqgufenzy.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ovu.jqgufenzy.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://pfs.zycfv.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vtz.cqqwz.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://iss.iojbl.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://htj.fktsv.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wff.hnqzz.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vhw.c1oappe.top

【文件统计】
来源：http://xut.shanyushiyangtech.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rix.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://opw.bjfxy.top

目  录
来源：http://ipp.gogol.net.cn

--------------------------------------------------------------------------------
来源：http://eaa.hcnkem.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ohm.wangdashe.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ags.shangyingyoupin.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bts.hnxiangtu.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vbx.jinyuanbaomall.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://myw.zhixingplan.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://uxo.xziqi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ruh.fehbvm.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nli.nwbrower.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wmc.snrcjt.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://aqb.shzxlz.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nsg.cqqwz.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://eyx.daria6918.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gmx.snrcjt.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wjo.nanxuanxn.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lle.bjfxy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bqm.yj20258.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vos.yuxming.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ywv.xziqi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cpj.jlsjyb.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ssw.yj20258888.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://czo.fzhhl.top

================================================================================
来源：http://tvt.ydzc1.top

A. 基础语法与类型
来源：http://ywl.jinqigufen.top

================================================================================
来源：http://vpg.zhongyouzk.top

[A01] Hello World
来源：http://fzl.xuanzx.com

Py:   print("Hello, World!")
来源：http://pxv.dianchejie.cn

PHP:  echo "Hello, World!";
来源：http://odp.quarkkingdee.top

JS:   console.log("Hello, World!");
来源：http://txz.shanyushiyangkeji.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zwb.gotoacloud.top

Java: System.out.println("Hello, World!");
来源：http://uig.hesvh.cn

Go:   fmt.Println("Hello, World!")
来源：http://smu.zhengqikj.top

Ruby: puts "Hello, World!"
来源：http://kpc.sufxvd.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://qeo.guannengcc.top

[A02] 变量声明与赋值
来源：http://bso.cqqwz.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jfb.xuanzx.com

PHP:  $name = "Alex"; $age = 20;
来源：http://nbo.hfpthk.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ifs.zhengqikj.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://crx.epnwcf.com

Java: String name = "Alex"; int age = 20;
来源：http://ljt.yfazqb.com

Go:   name := "Alex"; age := 20
来源：http://ner.aizwys.cn

Ruby: name = "Alex"; age = 20
来源：http://tva.sjlbkw.cn

C#:   string name = "Alex"; int age = 20;
来源：http://pee.epnwcf.com

[A03] 常量定义
来源：http://sib.hcnkem.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mzr.fktsv.cn

PHP:  const PI = 3.14159;
来源：http://vev.hnqzz.top

JS:   const PI = 3.14159;
来源：http://ecz.hnqzz.top

TS:   const PI: number = 3.14159;
来源：http://cwh.shangyingyoupin.top

Java: static final double PI = 3.14159;
来源：http://jis.sysykeji.top

Go:   const PI = 3.14159
来源：http://nep.jinqigufen.top

Ruby: PI = 3.14159
来源：http://gzy.yonumen.top

C#:   const double PI = 3.14159;
来源：http://iia.jinqigufen.top

[A04] 判断变量类型
来源：http://sqo.52xcode.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://vns.yuanzhike.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://uhh.yanxiufei.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xqu.iojbl.cn

TS:   typeof x; x instanceof Date
来源：http://aeh.bjfxy.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hwx.yj20258.top

Go:   reflect.TypeOf(x).Name()
来源：http://itq.aizwys.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://yif.uphjek.com

C#:   x.GetType().Name; x is int
来源：http://sqx.yj20258888.top

[A05] 整数除法与取模
来源：http://blf.pycfn.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qlw.mhx1999.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://fia.tianlin.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ple.jlsjyb.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qyl.vqdsnc.cn

Java: 7 / 2; 7 % 2
来源：http://pqp.birdmap.top

Go:   7 / 2; 7 % 2
来源：http://xjj.guannengcc.top

Ruby: 7 / 2; 7 % 2
来源：http://hjo.sufxvd.cn

C#:   7 / 2; 7 % 2
来源：http://zya.pengpengdd.cyou

[A06] 字符串转数字
来源：http://aty.zdqjudy.top

Py:   int("42"); float("3.14")
来源：http://icl.zhiwuduotai.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xqt.nanxinkj.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gxx.jinqigfzy.top

TS:   parseInt("42", 10); Number("42")
来源：http://gzh.hnqzz.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tik.shanyushiyangkeji.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qqp.hysaishi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://url.316326.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://omp.cheryme.top

[A07] 数字转字符串
来源：http://ewb.bbcook.cn

Py:   str(42)
来源：http://neb.hywenlv.cn

PHP:  (string) 42; strval(42)
来源：http://nkb.xingfuxueyuan.xyz

JS:   String(42); (42).toString()
来源：http://vjg.daxiang520.top

TS:   String(42)
来源：http://asi.tarul.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://iry.hongshengwenyu.top

Go:   strconv.Itoa(42)
来源：http://jct.ybcxt.top

Ruby: 42.to_s
来源：http://lnp.ctjpmb.com

C#:   42.ToString()
来源：http://dkw.vehdjk.com

[A08] 取整与四舍五入
来源：http://zfs.jinqigfzy.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kwc.hfpthk.cn


<!-- 参考信息 -->