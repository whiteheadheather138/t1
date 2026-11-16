代发 wailian999

[U65] PHP：会话
来源：http://buq.iojbl.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://aqe.9152youxi.cn

[U66] PHP：设置 Cookie
来源：http://cqq.yj20258.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sqt.bbcook.cn

[U67] PHP：处理文件上传
来源：http://naa.yfazqb.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ksl.fktsv.cn

[U68] PHP：PDO 连接
来源：http://pdi.316326.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wne.mhx1999.top

[U69] PHP：PDO 预处理
来源：http://fqz.yj202588.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vhe.tianlin.xyz

[U70] PHP：PDO 事务
来源：http://miz.jinyuanbaomall.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bwg.0kj1m.cn

[U71] PHP：抛出异常
来源：http://rpx.epnwcf.com

throw new RuntimeException("失败", 500);
来源：http://qsz.sxryk.cn

[U72] PHP：写错误日志
来源：http://sqv.gotoacloud.top

error_log("失败: " . $e->getMessage());
来源：http://jvy.jqgfzy.top

[U73] PHP：读取 ini 配置
来源：http://cmv.guannengcc.top

parse_ini_file("config.ini", true)
来源：http://qpj.haohaochexian.top

[U74] PHP：读取环境变量
来源：http://fis.zhongyouzk.top

getenv("APP_ENV") ?: "production"
来源：http://zpm.xuetiantiany.cn

[U75] PHP：依赖注入
来源：http://xpy.bjfxy.top

composer require psr/container
来源：http://tbt.zhijiandao.cn

[U76] PHP：简单路由
来源：http://nph.yanxiufei.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tbn.gotoacloud.top

[U77] PHP：模板渲染
来源：http://bcl.snrcjt.cn

composer require twig/twig
来源：http://ilm.meibo888.top

[U78] PHP：单元测试
来源：http://ynu.cucudq.cn

composer require --dev phpunit/phpunit
来源：http://vrt.ybcxt.top

[U79] PHP：静态分析
来源：http://apt.sweek.top

composer require --dev phpstan/phpstan
来源：http://dgl.fktsv.cn

[U80] PHP：代码规范修复
来源：http://twm.zhixingplan.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://joy.ywan-chungtsiang.top

[U81] JS：初始化项目
来源：http://jxe.shuidangran.top

npm init -y;  npm i express
来源：http://ily.fengsongda.top

[U82] JS：package.json 脚本
来源：http://unn.shuidangran.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://csf.cucudq.cn

[U83] JS：ES Module 导入导出
来源：http://mzr.daxiang520.top

export const a = 1;  import { a } from "./m.js";
来源：http://yqd.fanxiaobao.xyz

[U84] JS：CommonJS 写法
来源：http://tkw.cucudq.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cnq.tarul.cn

[U85] JS：可选链
来源：http://nlh.shanyushiyangtech.top

a?.b?.c
来源：http://wzm.jlsjyb.cn

[U86] JS：空值合并
来源：http://zry.pycfn.com

a ?? b
来源：http://wjl.fktsv.cn

[U87] JS：解构默认值
来源：http://knv.gzhubu.top

const { a = 1, b = 2 } = obj;
来源：http://tvm.wangshuangyany.cn

[U88] JS：对象展开合并
来源：http://azz.xylfe.cn

{ ...a, ...b }
来源：http://ltk.birdmap.top

[U89] JS：数组去重
来源：http://qnz.jinqigfzy.top

[...new Set(arr)]
来源：http://nvi.zhijiandao.cn

[U90] JS：数字数组排序
来源：http://juh.hnqzz.top

[...arr].sort((a, b) => a - b)
来源：http://pjq.gzhubu.top

[U91] JS：对象键值遍历
来源：http://cll.jiagoushi.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jkm.bjfxy.top

[U92] JS：深拷贝
来源：http://san.jiagoushi.top

structuredClone(obj)
来源：http://nic.kuanghao11.cn

[U93] JS：模板字符串
来源：http://zyj.gogol.net.cn

`共 ${n} 条`
来源：http://kjw.tian-w.cn

[U94] JS：箭头函数
来源：http://kek.cheryme.top

const double = x => x * 2;
来源：http://qte.hammf.cn

[U95] JS：Promise 包装
来源：http://xgb.yj20258888.top

new Promise((resolve, reject) => {})
来源：http://wdi.bbcook.cn

[U96] JS：async/await 与异常
来源：http://efj.bjfxy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hjc.hnqzz.top

[U97] JS：并发请求
来源：http://kfi.wangshuangyany.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hkr.wangshuangyany.cn

[U98] JS：fetch 带 JSON
来源：http://hyd.cashguo.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://isd.zdqjudy.top

[U99] JS：事件监听
来源：http://ocx.jinyuanbaomall.cn

el.addEventListener("click", e => {})
来源：http://hsf.iojbl.cn

[U100] JS：DOM 查询
来源：http://cjd.tanke756.top

document.querySelector(".item")
来源：http://cqx.yj20258.top

[U101] JS：classList 操作
来源：http://vkp.zhongyouzk.top

el.classList.toggle("active")
来源：http://umw.yueranfly.top

[U102] JS：本地存储
来源：http://his.redwolf501.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://pta.cdnleiting.top

[U103] JS：定时器
来源：http://oeh.snrcjt.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xag.xingfuxueyuan.xyz

[U104] JS：防抖
来源：http://ezo.nanxinkj.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qbr.tianlin.xyz

[U105] JS：节流
来源：http://rrt.fehbvm.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://omd.hnxiangtu.top

[U106] JS：日期格式化
来源：http://oya.ctjpmb.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ixx.fengsongda.top

[U107] JS：数字千分位
来源：http://nrb.havefunace.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zkw.ctjpmb.com

[U108] JS：随机整数
来源：http://iyp.52xcode.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ziu.jinqigufen.top

[U109] JS：数组分组
来源：http://jmi.fengsongda.top

Object.groupBy(arr, x => x.type)
来源：http://kol.smart0.xyz

[U110] JS：数组分块
来源：http://ozc.gogol.net.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fpt.ybcxt.top

[U111] JS：对象转 Map
来源：http://fmr.shzxlz.cn

new Map(Object.entries(obj))
来源：http://klk.shangyingyoupin.top

[U112] JS：字符串补位
来源：http://ixp.jqgfzy.top

"7".padStart(3, "0")
来源：http://gjq.birdmap.top

[U113] JS：正则替换全部
来源：http://gkg.zhijiandao.cn

s.replaceAll("a", "b")
来源：http://olw.tanke756.top

[U114] JS：JSON 深比较
来源：http://mrb.sufxvd.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xvf.sufxvd.cn

[U115] JS：生成 UUID
来源：http://nfy.ywan-chungtsiang.top

crypto.randomUUID()
来源：http://hsf.aizwys.cn

[U116] JS：类型检查（JSDoc）
来源：http://dmr.fengsongda.top

/** @param {string} name */ function f(name) {}
来源：http://xxh.sjlbkw.cn

[U117] JS：单元测试
来源：http://xvr.yj202588.top

npm i -D vitest;  npx vitest
来源：http://dtj.nanxinkj.top

[U118] JS：开发服务器
来源：http://zxe.pycfn.com

npm i -D vite;  npx vite
来源：http://drj.sxryk.cn

[U119] JS：生产构建
来源：http://ijd.hywenlv.cn

npx vite build
来源：http://uyn.zhengqikj.top

[U120] JS：读取环境变量（Vite）
来源：http://qpp.yj202588.top

import.meta.env.VITE_API_URL
来源：http://fcy.gaohongyu789.top

================================================================================
来源：http://equ.svipenyu.cn

统计汇总
来源：http://jfs.zycfv.cn

================================================================================
来源：http://snd.yj20258.top

按语言统计（条）：
来源：http://hyv.ctjpmb.com

Python ......... 252
来源：http://ehd.smart0.xyz

PHP ............ 252
来源：http://ife.ybcxt.top

JavaScript ..... 252
来源：http://iqq.xingfuxueyuan.xyz

TypeScript ..... 212
来源：http://paf.zhongyouzk.top

Java ........... 212
来源：http://tpd.yj20258888.top

Go ............. 212
来源：http://ekf.redwolf501.top

Ruby ........... 212
来源：http://cua.vqdsnc.cn

C# ............. 212
来源：http://pgg.ybcxt.top

C .............. 30
来源：http://ore.chenzaomai.com

C++ ............ 30
来源：http://riz.smart0.xyz

SQL ............ 90
来源：http://nyg.chenjidiqi.icu

Bash ........... 80
来源：http://czr.gaohongyu789.top

Kotlin ......... 15
来源：http://alp.havefunace.top

Swift .......... 15
来源：http://jqc.jinqigufen.top

Lua ............ 10
来源：http://aha.shanyushiyangkeji.top

Perl ........... 10
来源：http://eaa.feifeiyinyue.top

Scala .......... 10
来源：http://kxv.xuanzx.com

------------------------------------
来源：http://yvh.cashguo.top

合计 ........... 2106 条
来源：http://upr.yfazqb.com

按章节统计：
来源：http://kns.xuanzx.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://klq.haohaochexian.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ltt.jlsjyb.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xqg.jianghu66.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lsp.shanyushiyangkeji.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pwf.tianlin.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hcd.hysaishi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xgo.chenlongwang.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fwq.jinghuilouyu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hxp.ybcxt.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kyl.jiagoushi.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cxq.ydjk.org.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cir.chenzaomai.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ngu.redwolf501.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://iak.gogol.net.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ulo.zycfv.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://pwc.chenjidiqi.icu

Q SQL 专题                              90
来源：http://dqx.yj202588.top

R Bash 专题                             80
来源：http://nye.cucudq.cn

S C / C++ 专题                          60
来源：http://hgl.havefunace.top

T 其他语言补充                          60
来源：http://vkl.cashguo.top

U 高频实用片段                         120
来源：http://kon.fktsv.cn

------------------------------------
来源：http://dkj.mhx1999.top

合计                                  2106 条
来源：http://fqp.hesvh.cn

--------------------------------------------------------------------------------
来源：http://xeq.zdbjq.cn

使用提醒
来源：http://uca.tian-w.cn

--------------------------------------------------------------------------------
来源：http://kox.ywan-chungtsiang.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fpf.316326.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ltl.ehwqpu.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mbg.zhixingplan.top

在旧版本上使用前请先确认语法支持情况。
来源：http://yrd.zdbjq.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lwg.hesvh.cn

—— 文件结束 ——
来源：http://hvs.yuanzhike.top

================================================================================
来源：http://aki.shanyushiyangtech.top

程序语言常见例子速查手册（2024 版）
来源：http://wvt.gogol.net.cn

Common Programming Examples Cheat Book
来源：http://njt.zhiwuduotai.top

================================================================================
来源：http://kaq.0kj1m.cn

【收录内容】
来源：http://bfc.ydjk.org.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://pwe.dianchejie.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rzc.yuxming.cn

SQL · Bash · C · C++
来源：http://qyi.gotoacloud.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jlv.guowangkeji.top

【使用说明】
来源：http://jmg.mhx1999.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cbq.hcnkem.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ygw.kuanghao11.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ldz.sufxvd.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yfy.ppjwa.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://dvw.nanxinkj.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vzq.fzhhl.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://put.yuanzhike.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://new.aibaodan.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mmj.zdqjudy.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ejb.aibaodan.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ztn.quarkkingdee.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jyw.shangyingyoupin.top

【文件统计】
来源：http://zkg.hcnkem.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fjg.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://ixy.yongpay.top

目  录
来源：http://soa.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://uxf.hcnkem.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fmx.ydzc1.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ihs.epnwcf.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kxr.316326.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ikp.zhixingplan.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tew.tanke756.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vtx.ywan-chungtsiang.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wkn.xuetiantiany.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qtl.ydzc1.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://yxh.birdmap.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mfu.wangdashe.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vli.jianghu66.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://yij.52xcode.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://iqv.daxiang520.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://sqw.ppjwa.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mxn.hongshengwenyu.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mre.redwolf501.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://skk.xylfe.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://gdk.zhijiandao.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zvl.jlsjyb.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://doi.tianlin.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ewk.shanyushiyangkeji.top

================================================================================
来源：http://job.yueranfly.top

A. 基础语法与类型
来源：http://ojh.quarkkingdee.top

================================================================================
来源：http://sgt.yj20258888.top

[A01] Hello World
来源：http://cdq.kuanghao11.cn

Py:   print("Hello, World!")
来源：http://skc.quarkkingdee.top

PHP:  echo "Hello, World!";
来源：http://bep.xinyue.icu

JS:   console.log("Hello, World!");
来源：http://mrp.yanxiufei.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gvx.nanxuanxn.top

Java: System.out.println("Hello, World!");
来源：http://xfr.52xcode.cn

Go:   fmt.Println("Hello, World!")
来源：http://ayc.jiagoushi.top

Ruby: puts "Hello, World!"
来源：http://bel.sufxvd.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://lyz.cdnleiting.top

[A02] 变量声明与赋值
来源：http://mxh.yj20258.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://umh.aibaodan.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://mbb.havefunace.top

JS:   let name = "Alex"; const age = 20;
来源：http://owp.zhixingplan.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wsi.ydjk.org.cn

Java: String name = "Alex"; int age = 20;
来源：http://pag.ppjwa.cn

Go:   name := "Alex"; age := 20
来源：http://mwj.pengpengdd.cyou

Ruby: name = "Alex"; age = 20
来源：http://zuj.0kj1m.cn

C#:   string name = "Alex"; int age = 20;
来源：http://bxu.havefunace.top

[A03] 常量定义
来源：http://bcg.zhongyouzk.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kme.pycfn.com

PHP:  const PI = 3.14159;
来源：http://gxk.tianlin.xyz

JS:   const PI = 3.14159;
来源：http://qzf.nwbrower.top

TS:   const PI: number = 3.14159;
来源：http://fsz.sufxvd.cn

Java: static final double PI = 3.14159;
来源：http://xib.gogol.net.cn

Go:   const PI = 3.14159
来源：http://zlh.cashguo.top

Ruby: PI = 3.14159
来源：http://zqj.9152youxi.cn

C#:   const double PI = 3.14159;
来源：http://ors.ywan-chungtsiang.top

[A04] 判断变量类型
来源：http://mmx.jqgfzy.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://iiw.cdnleiting.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://uhl.yonumen.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bdl.cashguo.top

TS:   typeof x; x instanceof Date
来源：http://boe.andypj.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gpi.jinqigufen.top

Go:   reflect.TypeOf(x).Name()
来源：http://ghl.zdbjq.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://oig.jinyuanbaomall.cn

C#:   x.GetType().Name; x is int
来源：http://knk.sysykeji.top

[A05] 整数除法与取模
来源：http://aiy.ppjwa.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jda.ydzc1.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://hmr.mhx1999.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xdk.vqdsnc.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://snf.guowangkeji.top

Java: 7 / 2; 7 % 2
来源：http://omn.ydzc1.top

Go:   7 / 2; 7 % 2
来源：http://vpl.zhoulong.xyz

Ruby: 7 / 2; 7 % 2
来源：http://qvk.dashuyun.cn

C#:   7 / 2; 7 % 2
来源：http://tcy.chenjidiqi.icu

[A06] 字符串转数字
来源：http://kym.yj202588.top

Py:   int("42"); float("3.14")
来源：http://ict.ydjk.org.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hsj.yvedp.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ayt.wangdashe.top

TS:   parseInt("42", 10); Number("42")
来源：http://fwl.ehwqpu.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qzb.jinqigfzy.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rjp.vqdsnc.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://xdx.aibaodan.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qqx.jinghuilouyu.cn

[A07] 数字转字符串
来源：http://pwo.chenzaomai.com

Py:   str(42)
来源：http://dll.sysykeji.top

PHP:  (string) 42; strval(42)
来源：http://lrw.yj202588.top

JS:   String(42); (42).toString()
来源：http://ujz.hywenlv.cn

TS:   String(42)
来源：http://kve.fengsongda.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ojn.sysykeji.top

Go:   strconv.Itoa(42)
来源：http://zpo.chenzaomai.com

Ruby: 42.to_s
来源：http://ess.zycfv.cn

C#:   42.ToString()
来源：http://zqs.gaohongyu789.top

[A08] 取整与四舍五入
来源：http://mpe.hongshengwenyu.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ohb.zhixingplan.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://cwy.xuanzx.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://eag.ppjwa.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://vxm.chenjidiqi.icu

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rho.316326.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://cqb.sysykeji.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://mrd.yj20258888.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://sze.tanke756.top

[A09] 绝对值与最大最小值
来源：http://wfz.sjlbkw.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qsz.fehbvm.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://uwm.jinghuilouyu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://uue.snrcjt.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gqh.zhoulong.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ooo.hysaishi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zkb.jlsjyb.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wbr.hysaishi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mkb.mhx1999.top


<!-- 参考信息 -->