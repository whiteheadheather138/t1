代发 wailian999

[U61] PHP：正则
来源：http://mzd.feifeiyinyue.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ohh.daria6918.cn

[U62] PHP：日期对象
来源：http://jst.zhongyouzk.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pqc.feifeiyinyue.top

[U63] PHP：文件读写
来源：http://ghc.shangyingyoupin.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ayn.zhixingplan.top

[U64] PHP：目录遍历
来源：http://wlv.jinqigufen.top

glob("dir/*.php");  scandir("dir");
来源：http://mgl.shanyushiyangkeji.top

[U65] PHP：会话
来源：http://lfn.haohaochexian.top

session_start();  $_SESSION["uid"] = 1;
来源：http://umj.pengpengdd.cyou

[U66] PHP：设置 Cookie
来源：http://juq.gaohongyu789.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ior.jianghu66.top

[U67] PHP：处理文件上传
来源：http://afh.dashuyun.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://iee.xziqi.cn

[U68] PHP：PDO 连接
来源：http://ztw.shzxlz.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ovc.9152youxi.cn

[U69] PHP：PDO 预处理
来源：http://boc.tarul.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hhy.yueranfly.top

[U70] PHP：PDO 事务
来源：http://fhg.ppjwa.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://igb.tian-w.cn

[U71] PHP：抛出异常
来源：http://xuf.shangyingyoupin.top

throw new RuntimeException("失败", 500);
来源：http://gtw.gaohongyu789.top

[U72] PHP：写错误日志
来源：http://vkg.zdqjudy.top

error_log("失败: " . $e->getMessage());
来源：http://ccr.ywan-chungtsiang.top

[U73] PHP：读取 ini 配置
来源：http://rhh.aibaodan.cn

parse_ini_file("config.ini", true)
来源：http://asa.cqqwz.cn

[U74] PHP：读取环境变量
来源：http://yxx.chenzaomai.com

getenv("APP_ENV") ?: "production"
来源：http://wfr.pycfn.com

[U75] PHP：依赖注入
来源：http://mwg.gzhubu.top

composer require psr/container
来源：http://wvd.fengsongda.top

[U76] PHP：简单路由
来源：http://qpn.tianlin.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qkp.feifeiyinyue.top

[U77] PHP：模板渲染
来源：http://dib.xingfuxueyuan.xyz

composer require twig/twig
来源：http://hyg.zhaomingkeji.xyz

[U78] PHP：单元测试
来源：http://wtm.9152youxi.cn

composer require --dev phpunit/phpunit
来源：http://jpg.aibaodan.cn

[U79] PHP：静态分析
来源：http://aic.yanxiufei.cn

composer require --dev phpstan/phpstan
来源：http://fay.ybcxt.top

[U80] PHP：代码规范修复
来源：http://upv.ehwqpu.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://rvp.jinghuilouyu.cn

[U81] JS：初始化项目
来源：http://xoq.svipenyu.cn

npm init -y;  npm i express
来源：http://oqa.svipenyu.cn

[U82] JS：package.json 脚本
来源：http://wri.xinyue.icu

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mte.xingfuxueyuan.xyz

[U83] JS：ES Module 导入导出
来源：http://ytd.zhixingplan.top

export const a = 1;  import { a } from "./m.js";
来源：http://hdl.yonumen.top

[U84] JS：CommonJS 写法
来源：http://uee.xylfe.cn

module.exports = { a };  const { a } = require("./m");
来源：http://dkw.svipenyu.cn

[U85] JS：可选链
来源：http://oal.yvedp.cn

a?.b?.c
来源：http://izl.zycfv.cn

[U86] JS：空值合并
来源：http://pju.snrcjt.cn

a ?? b
来源：http://emn.ehwqpu.com

[U87] JS：解构默认值
来源：http://swy.jqgfzy.top

const { a = 1, b = 2 } = obj;
来源：http://mya.fktsv.cn

[U88] JS：对象展开合并
来源：http://tfj.uphjek.com

{ ...a, ...b }
来源：http://wth.shanyushiyangkeji.top

[U89] JS：数组去重
来源：http://pwf.ywan-chungtsiang.top

[...new Set(arr)]
来源：http://rze.jqgfzy.top

[U90] JS：数字数组排序
来源：http://iid.xziqi.cn

[...arr].sort((a, b) => a - b)
来源：http://hoa.fengsongda.top

[U91] JS：对象键值遍历
来源：http://gwr.tianlin.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cfn.hesvh.cn

[U92] JS：深拷贝
来源：http://apk.zhixingplan.top

structuredClone(obj)
来源：http://wla.hfpthk.cn

[U93] JS：模板字符串
来源：http://ihh.sweek.top

`共 ${n} 条`
来源：http://xkn.fzhhl.top

[U94] JS：箭头函数
来源：http://ong.yanxiufei.cn

const double = x => x * 2;
来源：http://foo.zhijiandao.cn

[U95] JS：Promise 包装
来源：http://kyl.sjlbkw.cn

new Promise((resolve, reject) => {})
来源：http://niz.chenlongwang.top

[U96] JS：async/await 与异常
来源：http://vei.hywenlv.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://whh.0kj1m.cn

[U97] JS：并发请求
来源：http://moc.sxryk.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://tww.hcnkem.com

[U98] JS：fetch 带 JSON
来源：http://wga.xylfe.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wzw.hysaishi.cn

[U99] JS：事件监听
来源：http://bnq.svipenyu.cn

el.addEventListener("click", e => {})
来源：http://epa.gzhubu.top

[U100] JS：DOM 查询
来源：http://ajk.xuetiantiany.cn

document.querySelector(".item")
来源：http://fad.hcnkem.com

[U101] JS：classList 操作
来源：http://bic.shzxlz.cn

el.classList.toggle("active")
来源：http://bxz.epnwcf.com

[U102] JS：本地存储
来源：http://uny.feifeiyinyue.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ybm.gzhubu.top

[U103] JS：定时器
来源：http://ojj.0kj1m.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xif.sweek.top

[U104] JS：防抖
来源：http://icx.jinqigfzy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tzy.vqdsnc.cn

[U105] JS：节流
来源：http://ymj.jianghu66.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rmu.jinghuilouyu.cn

[U106] JS：日期格式化
来源：http://tbz.ppjwa.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mkr.cashguo.top

[U107] JS：数字千分位
来源：http://hem.hfpthk.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xyt.jyoumei.cn

[U108] JS：随机整数
来源：http://wnn.yangfankeji.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yct.tarul.cn

[U109] JS：数组分组
来源：http://ykw.svipenyu.cn

Object.groupBy(arr, x => x.type)
来源：http://daq.jqgfzy.top

[U110] JS：数组分块
来源：http://xkh.hnqzz.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rym.xuetiantiany.cn

[U111] JS：对象转 Map
来源：http://mwl.tian-w.cn

new Map(Object.entries(obj))
来源：http://slj.tanke756.top

[U112] JS：字符串补位
来源：http://zps.jiagoushi.top

"7".padStart(3, "0")
来源：http://xfi.9152youxi.cn

[U113] JS：正则替换全部
来源：http://dij.jinyuanbaomall.cn

s.replaceAll("a", "b")
来源：http://dze.sweek.top

[U114] JS：JSON 深比较
来源：http://pie.shuidangran.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://lcz.fktsv.cn

[U115] JS：生成 UUID
来源：http://zlg.daria6918.cn

crypto.randomUUID()
来源：http://gsj.shzxlz.cn

[U116] JS：类型检查（JSDoc）
来源：http://ljg.birdmap.top

/** @param {string} name */ function f(name) {}
来源：http://lcy.ivvv.top

[U117] JS：单元测试
来源：http://cec.jinghuilouyu.cn

npm i -D vitest;  npx vitest
来源：http://vgt.cdnleiting.top

[U118] JS：开发服务器
来源：http://tuh.shanyushiyangkeji.top

npm i -D vite;  npx vite
来源：http://mam.aibaodan.cn

[U119] JS：生产构建
来源：http://dgi.birdmap.top

npx vite build
来源：http://hig.zhiwuduotai.top

[U120] JS：读取环境变量（Vite）
来源：http://uct.yj202588.top

import.meta.env.VITE_API_URL
来源：http://fkp.cucudq.cn

================================================================================
来源：http://vkg.cashguo.top

统计汇总
来源：http://dls.yuanzhike.top

================================================================================
来源：http://qos.gogol.net.cn

按语言统计（条）：
来源：http://dng.guowangkeji.top

Python ......... 252
来源：http://vfr.gotoacloud.top

PHP ............ 252
来源：http://feb.andypj.xyz

JavaScript ..... 252
来源：http://von.shzxlz.cn

TypeScript ..... 212
来源：http://hfx.jqgfzy.top

Java ........... 212
来源：http://ikc.tanke756.top

Go ............. 212
来源：http://qeq.gotoacloud.top

Ruby ........... 212
来源：http://yzz.xinyue.icu

C# ............. 212
来源：http://qfj.xuanzx.com

C .............. 30
来源：http://jjq.aizwys.cn

C++ ............ 30
来源：http://yii.ctjpmb.com

SQL ............ 90
来源：http://mcb.guowangkeji.top

Bash ........... 80
来源：http://muq.52xcode.cn

Kotlin ......... 15
来源：http://jju.ybcxt.top

Swift .......... 15
来源：http://oej.ivvv.top

Lua ............ 10
来源：http://wgv.yanxiufei.cn

Perl ........... 10
来源：http://feo.xingfuxueyuan.xyz

Scala .......... 10
来源：http://iuh.gaohongyu789.top

------------------------------------
来源：http://hmp.nanxuanxn.top

合计 ........... 2106 条
来源：http://ant.pengpengdd.cyou

按章节统计：
来源：http://cex.yvedp.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dgq.wangshuangyany.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lku.hongshengwenyu.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://asx.hywenlv.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://uyh.cheryme.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qub.ctjpmb.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yog.dianchejie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uxz.ywan-chungtsiang.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://scr.aibaodan.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pbs.cdnleiting.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vtt.yuxming.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://idi.aizwys.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mfs.redwolf501.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mlz.fanxiaobao.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sex.ehwqpu.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vtc.tian-w.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cuh.xingfuxueyuan.xyz

Q SQL 专题                              90
来源：http://hcp.gaohongyu789.top

R Bash 专题                             80
来源：http://oml.bbcook.cn

S C / C++ 专题                          60
来源：http://ujz.yonumen.top

T 其他语言补充                          60
来源：http://exf.cheryme.top

U 高频实用片段                         120
来源：http://qpi.yj202588.top

------------------------------------
来源：http://bat.tianlin.xyz

合计                                  2106 条
来源：http://uwz.guowangkeji.top

--------------------------------------------------------------------------------
来源：http://nmk.gzhubu.top

使用提醒
来源：http://dmb.yj20258888.top

--------------------------------------------------------------------------------
来源：http://knw.ehwqpu.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wme.zdbjq.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://oyh.yj202588.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://kjy.xylfe.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ska.hammf.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://eue.xziqi.cn

—— 文件结束 ——
来源：http://qyc.hcnkem.com

================================================================================
来源：http://mjl.kuanghao11.cn

程序语言常见例子速查手册（2024 版）
来源：http://bfe.yj202588.top

Common Programming Examples Cheat Book
来源：http://nrb.jqgufenzy.top

================================================================================
来源：http://mzo.fanxiaobao.xyz

【收录内容】
来源：http://yys.zhengqikj.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://tpq.xylfe.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ufj.fengsongda.top

SQL · Bash · C · C++
来源：http://rsc.yueranfly.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://djd.yanxiufei.cn

【使用说明】
来源：http://osm.bbcook.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://asw.shuidangran.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bmy.cheryme.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://msc.dianchejie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qim.yj20258.top

Bash:  Shell         C:     C             C++:   C++
来源：http://hfn.tanke756.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lwh.ctjpmb.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lur.zhijiandao.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rep.sweek.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rrd.hysaishi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hla.cashguo.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fjx.sysykeji.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wrr.vehdjk.com

【文件统计】
来源：http://eat.zdbjq.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://kej.yongpay.top

--------------------------------------------------------------------------------
来源：http://kbr.vehdjk.com

目  录
来源：http://oby.sufxvd.cn

--------------------------------------------------------------------------------
来源：http://hwu.jinqigfzy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://guk.svipenyu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://kzv.zhixingplan.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bvb.ydjk.org.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dva.jinghuilouyu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dqk.zhongyouzk.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://jvx.zhijiandao.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://dsi.yj20258888.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://iyc.hesvh.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xtl.hesvh.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nbq.cdnleiting.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hty.ywan-chungtsiang.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://uzi.haohaochexian.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dwd.vqdsnc.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kwt.shangyingyoupin.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cbq.yongpay.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zoy.chenlongwang.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hed.jinghuilouyu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://qhy.zhaomingkeji.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://gdl.cashguo.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rol.yuanzhike.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kes.xuanzx.com

================================================================================
来源：http://aat.jiagoushi.top

A. 基础语法与类型
来源：http://jkx.ctjpmb.com

================================================================================
来源：http://pws.yvedp.cn

[A01] Hello World
来源：http://qla.dashuyun.cn

Py:   print("Hello, World!")
来源：http://rub.andypj.xyz

PHP:  echo "Hello, World!";
来源：http://ywc.hywenlv.cn

JS:   console.log("Hello, World!");
来源：http://djr.andypj.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://oxr.yj20258.top

Java: System.out.println("Hello, World!");
来源：http://afr.zycfv.cn

Go:   fmt.Println("Hello, World!")
来源：http://pqz.yj20258.top

Ruby: puts "Hello, World!"
来源：http://qvf.andypj.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://tse.nanxinkj.top

[A02] 变量声明与赋值
来源：http://ntk.andypj.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jgw.mhx1999.top

PHP:  $name = "Alex"; $age = 20;
来源：http://udv.dashuyun.cn

JS:   let name = "Alex"; const age = 20;
来源：http://lmb.jianghu66.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wsy.hnqzz.top

Java: String name = "Alex"; int age = 20;
来源：http://fua.smart0.xyz

Go:   name := "Alex"; age := 20
来源：http://fam.fanxiaobao.xyz

Ruby: name = "Alex"; age = 20
来源：http://bnh.uphjek.com

C#:   string name = "Alex"; int age = 20;
来源：http://ccq.yongpay.top

[A03] 常量定义
来源：http://aip.tarul.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://meq.ehwqpu.com

PHP:  const PI = 3.14159;
来源：http://ker.zhoulong.xyz

JS:   const PI = 3.14159;
来源：http://out.hnqzz.top

TS:   const PI: number = 3.14159;
来源：http://fos.jianghu66.top

Java: static final double PI = 3.14159;
来源：http://zca.epnwcf.com

Go:   const PI = 3.14159
来源：http://nwf.snrcjt.cn

Ruby: PI = 3.14159
来源：http://hin.fktsv.cn

C#:   const double PI = 3.14159;
来源：http://wpx.snrcjt.cn

[A04] 判断变量类型
来源：http://avz.yonumen.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://poz.cqqwz.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://frr.sysykeji.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ycx.fanxiaobao.xyz

TS:   typeof x; x instanceof Date
来源：http://wom.aibaodan.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://twb.sysykeji.top

Go:   reflect.TypeOf(x).Name()
来源：http://afy.sysykeji.top

Ruby: x.class; x.is_a?(Integer)
来源：http://zkj.ivvv.top

C#:   x.GetType().Name; x is int
来源：http://ote.jinqigufen.top

[A05] 整数除法与取模
来源：http://tng.birdmap.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://phy.vqdsnc.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://wxo.zhoulong.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gia.ybcxt.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qqh.hywenlv.cn

Java: 7 / 2; 7 % 2
来源：http://pzw.pengpengdd.cyou

Go:   7 / 2; 7 % 2
来源：http://jnc.pengpengdd.cyou

Ruby: 7 / 2; 7 % 2
来源：http://ojb.pycfn.com

C#:   7 / 2; 7 % 2
来源：http://ifx.hnqzz.top

[A06] 字符串转数字
来源：http://mew.xinyue.icu

Py:   int("42"); float("3.14")
来源：http://qnb.tianlin.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://eax.tian-w.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dpo.9152youxi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://rmk.jlsjyb.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://pbb.chenjidiqi.icu

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ueu.gaohongyu789.top

Ruby: "42".to_i; "3.14".to_f
来源：http://arg.xuanzx.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hpy.dianchejie.cn

[A07] 数字转字符串
来源：http://shi.daria6918.cn

Py:   str(42)
来源：http://vre.daxiang520.top

PHP:  (string) 42; strval(42)
来源：http://lqx.gogol.net.cn

JS:   String(42); (42).toString()
来源：http://jyw.gaohongyu789.top

TS:   String(42)
来源：http://oep.yuanzhike.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://lew.ydjk.org.cn

Go:   strconv.Itoa(42)
来源：http://xzv.zycfv.cn

Ruby: 42.to_s
来源：http://wqz.snrcjt.cn

C#:   42.ToString()
来源：http://cks.xinyue.icu

[A08] 取整与四舍五入
来源：http://jgu.nanxinkj.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://nlm.hnqzz.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://tcn.zhiwuduotai.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vcq.pycfn.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ugt.zhijiandao.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ltp.smart0.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ahy.cqqwz.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://goa.haohaochexian.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mmi.andypj.xyz

[A09] 绝对值与最大最小值
来源：http://omq.gzhubu.top


<!-- 参考信息 -->