代发 wailian999

[U65] PHP：会话
来源：http://sxs.sxryk.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://lgd.cdnleiting.top

[U66] PHP：设置 Cookie
来源：http://vhp.wangshuangyany.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mjx.iojbl.cn

[U67] PHP：处理文件上传
来源：http://znd.jinghuilouyu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bpe.jinqigufen.top

[U68] PHP：PDO 连接
来源：http://dcz.svipenyu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jbx.daxiang520.top

[U69] PHP：PDO 预处理
来源：http://jup.redwolf501.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lda.fehbvm.com

[U70] PHP：PDO 事务
来源：http://mcy.zhaomingkeji.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://veq.pycfn.com

[U71] PHP：抛出异常
来源：http://dqr.gaohongyu789.top

throw new RuntimeException("失败", 500);
来源：http://uxn.sweek.top

[U72] PHP：写错误日志
来源：http://vrt.xuanzx.com

error_log("失败: " . $e->getMessage());
来源：http://jxg.meibo888.top

[U73] PHP：读取 ini 配置
来源：http://zem.yanxiufei.cn

parse_ini_file("config.ini", true)
来源：http://ifi.chenjidiqi.icu

[U74] PHP：读取环境变量
来源：http://qse.hywenlv.cn

getenv("APP_ENV") ?: "production"
来源：http://cvv.zdqjudy.top

[U75] PHP：依赖注入
来源：http://ulj.chenlongwang.top

composer require psr/container
来源：http://nna.yueranfly.top

[U76] PHP：简单路由
来源：http://zvd.hnxiangtu.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ofr.hnqzz.top

[U77] PHP：模板渲染
来源：http://fvm.meibo888.top

composer require twig/twig
来源：http://oga.ivvv.top

[U78] PHP：单元测试
来源：http://qew.fktsv.cn

composer require --dev phpunit/phpunit
来源：http://nwd.pycfn.com

[U79] PHP：静态分析
来源：http://aio.yfazqb.com

composer require --dev phpstan/phpstan
来源：http://idt.vehdjk.com

[U80] PHP：代码规范修复
来源：http://vqn.haohaochexian.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://qdw.zhiwuduotai.top

[U81] JS：初始化项目
来源：http://grv.shuidangran.top

npm init -y;  npm i express
来源：http://bmm.shanyushiyangkeji.top

[U82] JS：package.json 脚本
来源：http://smu.cqqwz.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://edc.chenlongwang.top

[U83] JS：ES Module 导入导出
来源：http://pld.chenlongwang.top

export const a = 1;  import { a } from "./m.js";
来源：http://txp.nwbrower.top

[U84] JS：CommonJS 写法
来源：http://jdv.bbcook.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gmk.ehwqpu.com

[U85] JS：可选链
来源：http://gxj.shuidangran.top

a?.b?.c
来源：http://arg.pengpengdd.cyou

[U86] JS：空值合并
来源：http://psi.cashguo.top

a ?? b
来源：http://yas.ydzc1.top

[U87] JS：解构默认值
来源：http://sql.zhixingplan.top

const { a = 1, b = 2 } = obj;
来源：http://ivp.vqdsnc.cn

[U88] JS：对象展开合并
来源：http://lkv.meibo888.top

{ ...a, ...b }
来源：http://vld.hfpthk.cn

[U89] JS：数组去重
来源：http://zpy.nanxinkj.top

[...new Set(arr)]
来源：http://osc.xinyue.icu

[U90] JS：数字数组排序
来源：http://sxo.shanyushiyangtech.top

[...arr].sort((a, b) => a - b)
来源：http://aqv.zhoulong.xyz

[U91] JS：对象键值遍历
来源：http://csd.redwolf501.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ipo.guannengcc.top

[U92] JS：深拷贝
来源：http://yag.xuetiantiany.cn

structuredClone(obj)
来源：http://qjx.sxryk.cn

[U93] JS：模板字符串
来源：http://mke.fehbvm.com

`共 ${n} 条`
来源：http://wld.zhixingplan.top

[U94] JS：箭头函数
来源：http://lxq.nanxinkj.top

const double = x => x * 2;
来源：http://vfi.zhaomingkeji.xyz

[U95] JS：Promise 包装
来源：http://hyo.hongshengwenyu.top

new Promise((resolve, reject) => {})
来源：http://nhd.guowangkeji.top

[U96] JS：async/await 与异常
来源：http://kws.gotoacloud.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zfy.cucudq.cn

[U97] JS：并发请求
来源：http://yym.jlsjyb.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ngr.fengsongda.top

[U98] JS：fetch 带 JSON
来源：http://zky.shuidangran.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nau.daxiang520.top

[U99] JS：事件监听
来源：http://yoq.fzhhl.top

el.addEventListener("click", e => {})
来源：http://jin.ppjwa.cn

[U100] JS：DOM 查询
来源：http://thv.jiagoushi.top

document.querySelector(".item")
来源：http://pny.cashguo.top

[U101] JS：classList 操作
来源：http://mac.hongshengwenyu.top

el.classList.toggle("active")
来源：http://rye.yj202588.top

[U102] JS：本地存储
来源：http://dof.hammf.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://pgx.shuidangran.top

[U103] JS：定时器
来源：http://sft.zhaomingkeji.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hcz.aizwys.cn

[U104] JS：防抖
来源：http://mlt.snrcjt.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://krw.yj20258888.top

[U105] JS：节流
来源：http://bgx.sjlbkw.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sln.jinqigfzy.top

[U106] JS：日期格式化
来源：http://pwz.yfazqb.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kbq.daria6918.cn

[U107] JS：数字千分位
来源：http://nuq.shzxlz.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hnl.hnxiangtu.top

[U108] JS：随机整数
来源：http://cph.daria6918.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qbb.shuidangran.top

[U109] JS：数组分组
来源：http://keh.zycfv.cn

Object.groupBy(arr, x => x.type)
来源：http://qoy.quarkkingdee.top

[U110] JS：数组分块
来源：http://lsr.bjfxy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jba.sysykeji.top

[U111] JS：对象转 Map
来源：http://pcn.zhixingplan.top

new Map(Object.entries(obj))
来源：http://lgm.jinyuanbaomall.cn

[U112] JS：字符串补位
来源：http://nwp.fehbvm.com

"7".padStart(3, "0")
来源：http://wjn.ehwqpu.com

[U113] JS：正则替换全部
来源：http://pdz.zhoulong.xyz

s.replaceAll("a", "b")
来源：http://nlb.svipenyu.cn

[U114] JS：JSON 深比较
来源：http://eyu.ppjwa.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jmu.jqgfzy.top

[U115] JS：生成 UUID
来源：http://jqr.ivvv.top

crypto.randomUUID()
来源：http://wtq.jinyuanbaomall.cn

[U116] JS：类型检查（JSDoc）
来源：http://xyc.vqdsnc.cn

/** @param {string} name */ function f(name) {}
来源：http://qnk.zdbjq.cn

[U117] JS：单元测试
来源：http://jtx.yj20258888.top

npm i -D vitest;  npx vitest
来源：http://sop.tianlin.xyz

[U118] JS：开发服务器
来源：http://zeb.xuanzx.com

npm i -D vite;  npx vite
来源：http://dat.tarul.cn

[U119] JS：生产构建
来源：http://huf.iojbl.cn

npx vite build
来源：http://qyn.quarkkingdee.top

[U120] JS：读取环境变量（Vite）
来源：http://myv.daxiang520.top

import.meta.env.VITE_API_URL
来源：http://rqs.cucudq.cn

================================================================================
来源：http://zzg.yuanzhike.top

统计汇总
来源：http://ubg.yj20258.top

================================================================================
来源：http://ybv.zhongyouzk.top

按语言统计（条）：
来源：http://rcw.xziqi.cn

Python ......... 252
来源：http://kuy.shzxlz.cn

PHP ............ 252
来源：http://oti.zycfv.cn

JavaScript ..... 252
来源：http://ovv.andypj.xyz

TypeScript ..... 212
来源：http://gef.gotoacloud.top

Java ........... 212
来源：http://bdh.guannengcc.top

Go ............. 212
来源：http://szq.shanyushiyangtech.top

Ruby ........... 212
来源：http://xfl.daria6918.cn

C# ............. 212
来源：http://ozu.yuxming.cn

C .............. 30
来源：http://idz.yfazqb.com

C++ ............ 30
来源：http://xka.dashuyun.cn

SQL ............ 90
来源：http://zxs.jqgufenzy.top

Bash ........... 80
来源：http://okn.fktsv.cn

Kotlin ......... 15
来源：http://mtt.zhengqikj.top

Swift .......... 15
来源：http://wlh.vqdsnc.cn

Lua ............ 10
来源：http://bpg.jinqigufen.top

Perl ........... 10
来源：http://wis.yj202588.top

Scala .......... 10
来源：http://zek.sjlbkw.cn

------------------------------------
来源：http://dsj.wangshuangyany.cn

合计 ........... 2106 条
来源：http://uqg.tarul.cn

按章节统计：
来源：http://nur.9152youxi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kqw.aibaodan.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://euf.meibo888.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nel.jyoumei.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xyh.smart0.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dkx.zhaomingkeji.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qkm.havefunace.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zdf.zhiwuduotai.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xfh.shangyingyoupin.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kzj.uphjek.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vxv.smart0.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fap.zhengqikj.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hso.xziqi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hui.cashguo.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ksm.sxryk.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hvr.jinyuanbaomall.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dir.ehwqpu.com

Q SQL 专题                              90
来源：http://tlv.hfpthk.cn

R Bash 专题                             80
来源：http://ykm.tanke756.top

S C / C++ 专题                          60
来源：http://zye.aibaodan.cn

T 其他语言补充                          60
来源：http://kuv.smart0.xyz

U 高频实用片段                         120
来源：http://oyv.zdbjq.cn

------------------------------------
来源：http://fiz.cashguo.top

合计                                  2106 条
来源：http://kjf.xuetiantiany.cn

--------------------------------------------------------------------------------
来源：http://qur.9152youxi.cn

使用提醒
来源：http://ctl.hnqzz.top

--------------------------------------------------------------------------------
来源：http://aqv.daxiang520.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xyu.yanxiufei.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://txp.ybcxt.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wpv.haohaochexian.top

在旧版本上使用前请先确认语法支持情况。
来源：http://chy.jinghuilouyu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hbx.mhx1999.top

—— 文件结束 ——
来源：http://oqw.ctjpmb.com

================================================================================
来源：http://ush.birdmap.top

程序语言常见例子速查手册（2024 版）
来源：http://rtk.cheryme.top

Common Programming Examples Cheat Book
来源：http://fjj.smart0.xyz

================================================================================
来源：http://kiy.yj202588.top

【收录内容】
来源：http://pgc.52xcode.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://aco.redwolf501.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://oua.jiagoushi.top

SQL · Bash · C · C++
来源：http://wdj.sysykeji.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vlq.jiagoushi.top

【使用说明】
来源：http://rrs.pycfn.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wtu.hcnkem.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tjd.zhongyouzk.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zpk.fanxiaobao.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://agj.gzhubu.top

Bash:  Shell         C:     C             C++:   C++
来源：http://tod.dianchejie.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dko.hfpthk.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wyz.redwolf501.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yqz.cqqwz.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rxx.sufxvd.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yxm.hnxiangtu.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://udy.jinyuanbaomall.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yar.shanyushiyangtech.top

【文件统计】
来源：http://tvq.zhongyouzk.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jbx.yonumen.top

--------------------------------------------------------------------------------
来源：http://ywh.vehdjk.com

目  录
来源：http://bol.smart0.xyz

--------------------------------------------------------------------------------
来源：http://sik.cucudq.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jcc.hongshengwenyu.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rkb.yongpay.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kkx.shzxlz.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zvp.ydjk.org.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mxo.nanxuanxn.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://acd.gotoacloud.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qod.sjlbkw.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vyo.shuidangran.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kuw.ywan-chungtsiang.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dxi.c1oappe.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wgp.xuanzx.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pkf.fktsv.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ybz.gotoacloud.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://orl.shzxlz.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zrt.zhaomingkeji.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qzq.c1oappe.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://axg.nwbrower.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://smd.xinyue.icu

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ive.jlsjyb.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jcz.c1oappe.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://khe.sxryk.cn

================================================================================
来源：http://gla.shuidangran.top

A. 基础语法与类型
来源：http://dca.xylfe.cn

================================================================================
来源：http://nll.nanxuanxn.top

[A01] Hello World
来源：http://imd.quarkkingdee.top

Py:   print("Hello, World!")
来源：http://eyu.smart0.xyz

PHP:  echo "Hello, World!";
来源：http://zuq.yuxming.cn

JS:   console.log("Hello, World!");
来源：http://hrm.hongshengwenyu.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fsx.shzxlz.cn

Java: System.out.println("Hello, World!");
来源：http://cez.xylfe.cn

Go:   fmt.Println("Hello, World!")
来源：http://tfq.gogol.net.cn

Ruby: puts "Hello, World!"
来源：http://jcl.svipenyu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://zru.epnwcf.com

[A02] 变量声明与赋值
来源：http://ijs.nanxinkj.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mri.ehwqpu.com

PHP:  $name = "Alex"; $age = 20;
来源：http://ovo.svipenyu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://yxs.pengpengdd.cyou

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mob.fktsv.cn

Java: String name = "Alex"; int age = 20;
来源：http://vsf.316326.xyz

Go:   name := "Alex"; age := 20
来源：http://edu.xinyue.icu

Ruby: name = "Alex"; age = 20
来源：http://qme.ybcxt.top

C#:   string name = "Alex"; int age = 20;
来源：http://siv.dianchejie.cn

[A03] 常量定义
来源：http://wwj.fehbvm.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mxx.pycfn.com

PHP:  const PI = 3.14159;
来源：http://kyr.fehbvm.com

JS:   const PI = 3.14159;
来源：http://vtf.bjfxy.top

TS:   const PI: number = 3.14159;
来源：http://par.jqgfzy.top

Java: static final double PI = 3.14159;
来源：http://uoa.guannengcc.top

Go:   const PI = 3.14159
来源：http://dyw.jinqigufen.top

Ruby: PI = 3.14159
来源：http://lgy.gogol.net.cn

C#:   const double PI = 3.14159;
来源：http://zbk.gogol.net.cn

[A04] 判断变量类型
来源：http://dwg.ppjwa.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://qzd.chenzaomai.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://syx.zhoulong.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hfq.vqdsnc.cn

TS:   typeof x; x instanceof Date
来源：http://dml.yvedp.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gxo.ivvv.top

Go:   reflect.TypeOf(x).Name()
来源：http://gvh.tian-w.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://kxo.meibo888.top

C#:   x.GetType().Name; x is int
来源：http://ynd.chenzaomai.com

[A05] 整数除法与取模
来源：http://vfk.ivvv.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rch.fktsv.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://pci.316326.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://uzc.xinyue.icu

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zqy.xuanzx.com

Java: 7 / 2; 7 % 2
来源：http://ovq.xylfe.cn

Go:   7 / 2; 7 % 2
来源：http://fmd.daria6918.cn

Ruby: 7 / 2; 7 % 2
来源：http://esr.xziqi.cn

C#:   7 / 2; 7 % 2
来源：http://zau.jqgufenzy.top

[A06] 字符串转数字
来源：http://joo.yanxiufei.cn

Py:   int("42"); float("3.14")
来源：http://klg.yangfankeji.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lzx.zhixingplan.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gag.yuanzhike.top

TS:   parseInt("42", 10); Number("42")
来源：http://ldr.cashguo.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ztr.andypj.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cwl.yfazqb.com

Ruby: "42".to_i; "3.14".to_f
来源：http://ttg.yuxming.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://npg.jinqigufen.top

[A07] 数字转字符串
来源：http://tdf.chenjidiqi.icu

Py:   str(42)
来源：http://qhu.shanyushiyangkeji.top

PHP:  (string) 42; strval(42)
来源：http://jfu.shanyushiyangkeji.top

JS:   String(42); (42).toString()
来源：http://hel.zdbjq.cn

TS:   String(42)
来源：http://pkz.ppjwa.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://zsg.hywenlv.cn

Go:   strconv.Itoa(42)
来源：http://pqn.yj20258888.top

Ruby: 42.to_s
来源：http://zap.snrcjt.cn

C#:   42.ToString()
来源：http://suo.feifeiyinyue.top

[A08] 取整与四舍五入
来源：http://djo.yfazqb.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://anz.aibaodan.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zfi.jqgufenzy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://iyk.chenzaomai.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nsr.cashguo.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mib.yj20258888.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://iss.kuanghao11.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://uwo.ydjk.org.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qoe.ivvv.top

[A09] 绝对值与最大最小值
来源：http://wyp.xuetiantiany.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vum.sxryk.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jmb.cashguo.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://eml.xziqi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cup.daxiang520.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zux.chenzaomai.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zel.jinghuilouyu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gqq.jianghu66.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hxd.vehdjk.com


<!-- 参考信息 -->