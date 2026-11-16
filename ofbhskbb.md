代发 wailian999

[U61] PHP：正则
来源：http://dsd.shuidangran.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://brs.yj20258888.top

[U62] PHP：日期对象
来源：http://eto.sjlbkw.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bub.snrcjt.cn

[U63] PHP：文件读写
来源：http://fwb.jiagoushi.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zbu.snrcjt.cn

[U64] PHP：目录遍历
来源：http://rpk.chenlongwang.top

glob("dir/*.php");  scandir("dir");
来源：http://iqj.ydjk.org.cn

[U65] PHP：会话
来源：http://qsr.svipenyu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gnx.hnqzz.top

[U66] PHP：设置 Cookie
来源：http://njj.jinghuilouyu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cfq.jlsjyb.cn

[U67] PHP：处理文件上传
来源：http://tox.jianghu66.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ecg.chenlongwang.top

[U68] PHP：PDO 连接
来源：http://gcv.jyoumei.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qre.meibo888.top

[U69] PHP：PDO 预处理
来源：http://mbt.gaohongyu789.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zll.tianlin.xyz

[U70] PHP：PDO 事务
来源：http://hss.hcnkem.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ncp.0kj1m.cn

[U71] PHP：抛出异常
来源：http://pkx.chenlongwang.top

throw new RuntimeException("失败", 500);
来源：http://teg.yj20258.top

[U72] PHP：写错误日志
来源：http://zfb.ywan-chungtsiang.top

error_log("失败: " . $e->getMessage());
来源：http://lcd.vqdsnc.cn

[U73] PHP：读取 ini 配置
来源：http://kby.vehdjk.com

parse_ini_file("config.ini", true)
来源：http://wse.ivvv.top

[U74] PHP：读取环境变量
来源：http://sxw.yuanzhike.top

getenv("APP_ENV") ?: "production"
来源：http://vkb.smart0.xyz

[U75] PHP：依赖注入
来源：http://fpc.xuanzx.com

composer require psr/container
来源：http://cvx.uphjek.com

[U76] PHP：简单路由
来源：http://cdj.aizwys.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tib.aizwys.cn

[U77] PHP：模板渲染
来源：http://tdh.ehwqpu.com

composer require twig/twig
来源：http://hgw.9152youxi.cn

[U78] PHP：单元测试
来源：http://ylp.iojbl.cn

composer require --dev phpunit/phpunit
来源：http://eey.xuanzx.com

[U79] PHP：静态分析
来源：http://wki.xylfe.cn

composer require --dev phpstan/phpstan
来源：http://pgb.sjlbkw.cn

[U80] PHP：代码规范修复
来源：http://wjk.fehbvm.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://abt.redwolf501.top

[U81] JS：初始化项目
来源：http://tdm.xuanzx.com

npm init -y;  npm i express
来源：http://gxy.vehdjk.com

[U82] JS：package.json 脚本
来源：http://sgp.sweek.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zcb.zdbjq.cn

[U83] JS：ES Module 导入导出
来源：http://agk.yuxming.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vpe.yj202588.top

[U84] JS：CommonJS 写法
来源：http://sqy.yfazqb.com

module.exports = { a };  const { a } = require("./m");
来源：http://rad.xuetiantiany.cn

[U85] JS：可选链
来源：http://rdv.yangfankeji.com

a?.b?.c
来源：http://rno.yj202588.top

[U86] JS：空值合并
来源：http://bfj.zycfv.cn

a ?? b
来源：http://mhc.ybcxt.top

[U87] JS：解构默认值
来源：http://gog.sweek.top

const { a = 1, b = 2 } = obj;
来源：http://jcq.chenlongwang.top

[U88] JS：对象展开合并
来源：http://fou.snrcjt.cn

{ ...a, ...b }
来源：http://abr.jyoumei.cn

[U89] JS：数组去重
来源：http://pka.sysykeji.top

[...new Set(arr)]
来源：http://mhu.ctjpmb.com

[U90] JS：数字数组排序
来源：http://vnu.redwolf501.top

[...arr].sort((a, b) => a - b)
来源：http://mib.ydjk.org.cn

[U91] JS：对象键值遍历
来源：http://ayz.ivvv.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ork.jqgfzy.top

[U92] JS：深拷贝
来源：http://zer.yanxiufei.cn

structuredClone(obj)
来源：http://nnj.sysykeji.top

[U93] JS：模板字符串
来源：http://ckm.epnwcf.com

`共 ${n} 条`
来源：http://tna.meibo888.top

[U94] JS：箭头函数
来源：http://bzk.snrcjt.cn

const double = x => x * 2;
来源：http://blp.xingfuxueyuan.xyz

[U95] JS：Promise 包装
来源：http://uyo.fanxiaobao.xyz

new Promise((resolve, reject) => {})
来源：http://kyt.shzxlz.cn

[U96] JS：async/await 与异常
来源：http://agx.0kj1m.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mzc.xuetiantiany.cn

[U97] JS：并发请求
来源：http://xby.jinyuanbaomall.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://sst.yj20258.top

[U98] JS：fetch 带 JSON
来源：http://nbh.guowangkeji.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zkt.yonumen.top

[U99] JS：事件监听
来源：http://bfz.yonumen.top

el.addEventListener("click", e => {})
来源：http://oym.sxryk.cn

[U100] JS：DOM 查询
来源：http://rat.yanxiufei.cn

document.querySelector(".item")
来源：http://axp.hywenlv.cn

[U101] JS：classList 操作
来源：http://ffx.yonumen.top

el.classList.toggle("active")
来源：http://bii.ydzc1.top

[U102] JS：本地存储
来源：http://kie.0kj1m.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://pbj.hfpthk.cn

[U103] JS：定时器
来源：http://iic.yj20258888.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fbv.zdbjq.cn

[U104] JS：防抖
来源：http://hud.yvedp.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rpk.xuanzx.com

[U105] JS：节流
来源：http://ygg.tanke756.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://frs.yuxming.cn

[U106] JS：日期格式化
来源：http://zmo.aizwys.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cpi.cheryme.top

[U107] JS：数字千分位
来源：http://avr.yongpay.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zkf.ctjpmb.com

[U108] JS：随机整数
来源：http://lvz.ctjpmb.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://the.yuxming.cn

[U109] JS：数组分组
来源：http://nph.zycfv.cn

Object.groupBy(arr, x => x.type)
来源：http://cmb.xuetiantiany.cn

[U110] JS：数组分块
来源：http://kuf.fengsongda.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uhv.cdnleiting.top

[U111] JS：对象转 Map
来源：http://lpp.kuanghao11.cn

new Map(Object.entries(obj))
来源：http://oio.yangfankeji.com

[U112] JS：字符串补位
来源：http://tpp.zhongyouzk.top

"7".padStart(3, "0")
来源：http://ioi.fengsongda.top

[U113] JS：正则替换全部
来源：http://swd.yj20258888.top

s.replaceAll("a", "b")
来源：http://lit.xuanzx.com

[U114] JS：JSON 深比较
来源：http://chf.sysykeji.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://wdr.cdnleiting.top

[U115] JS：生成 UUID
来源：http://ppj.ybcxt.top

crypto.randomUUID()
来源：http://mbt.9152youxi.cn

[U116] JS：类型检查（JSDoc）
来源：http://qcl.xuanzx.com

/** @param {string} name */ function f(name) {}
来源：http://gfn.ybcxt.top

[U117] JS：单元测试
来源：http://srz.cdnleiting.top

npm i -D vitest;  npx vitest
来源：http://jbq.xylfe.cn

[U118] JS：开发服务器
来源：http://zht.jinghuilouyu.cn

npm i -D vite;  npx vite
来源：http://xes.jlsjyb.cn

[U119] JS：生产构建
来源：http://jsz.gogol.net.cn

npx vite build
来源：http://fid.wangdashe.top

[U120] JS：读取环境变量（Vite）
来源：http://gnt.yuanzhike.top

import.meta.env.VITE_API_URL
来源：http://vgz.nwbrower.top

================================================================================
来源：http://brs.shanyushiyangkeji.top

统计汇总
来源：http://xgb.yanxiufei.cn

================================================================================
来源：http://die.bjfxy.top

按语言统计（条）：
来源：http://uni.hnxiangtu.top

Python ......... 252
来源：http://bty.hnxiangtu.top

PHP ............ 252
来源：http://pdz.zdbjq.cn

JavaScript ..... 252
来源：http://hxo.fzhhl.top

TypeScript ..... 212
来源：http://kfx.hnxiangtu.top

Java ........... 212
来源：http://qug.shanyushiyangtech.top

Go ............. 212
来源：http://cfc.hongshengwenyu.top

Ruby ........... 212
来源：http://kre.ywan-chungtsiang.top

C# ............. 212
来源：http://nnt.zhengqikj.top

C .............. 30
来源：http://jyg.zhijiandao.cn

C++ ............ 30
来源：http://bkm.jiagoushi.top

SQL ............ 90
来源：http://kzy.ydzc1.top

Bash ........... 80
来源：http://zvp.chenjidiqi.icu

Kotlin ......... 15
来源：http://uth.andypj.xyz

Swift .......... 15
来源：http://snp.52xcode.cn

Lua ............ 10
来源：http://ubw.zhiwuduotai.top

Perl ........... 10
来源：http://wkx.jqgufenzy.top

Scala .......... 10
来源：http://vaf.dashuyun.cn

------------------------------------
来源：http://zcy.fengsongda.top

合计 ........... 2106 条
来源：http://vmg.mhx1999.top

按章节统计：
来源：http://mvt.yj202588.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://adu.jyoumei.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qne.yj20258888.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bps.bjfxy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://iac.aizwys.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jtk.cucudq.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zuu.jlsjyb.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kql.haohaochexian.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pcn.yuanzhike.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ddp.yuxming.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dzn.gzhubu.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nwx.ehwqpu.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yso.andypj.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wql.tarul.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ouw.guowangkeji.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://njf.shzxlz.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wpq.zhongyouzk.top

Q SQL 专题                              90
来源：http://jmx.gotoacloud.top

R Bash 专题                             80
来源：http://ypg.redwolf501.top

S C / C++ 专题                          60
来源：http://ixn.xziqi.cn

T 其他语言补充                          60
来源：http://shu.hysaishi.cn

U 高频实用片段                         120
来源：http://voz.yonumen.top

------------------------------------
来源：http://kbi.dashuyun.cn

合计                                  2106 条
来源：http://ngc.jyoumei.cn

--------------------------------------------------------------------------------
来源：http://hxa.yvedp.cn

使用提醒
来源：http://xja.shanyushiyangtech.top

--------------------------------------------------------------------------------
来源：http://ihm.hfpthk.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qos.wangdashe.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ujq.smart0.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rub.jyoumei.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://dkh.meibo888.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kgs.daria6918.cn

—— 文件结束 ——
来源：http://izz.bbcook.cn

================================================================================
来源：http://qqd.jinqigufen.top

程序语言常见例子速查手册（2024 版）
来源：http://ikv.yanxiufei.cn

Common Programming Examples Cheat Book
来源：http://gpy.xziqi.cn

================================================================================
来源：http://wut.yj202588.top

【收录内容】
来源：http://qpu.hesvh.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://gpq.jianghu66.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hhe.hcnkem.com

SQL · Bash · C · C++
来源：http://ucc.zhiwuduotai.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ijn.hesvh.cn

【使用说明】
来源：http://ehm.shuidangran.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bda.wangdashe.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vxv.fanxiaobao.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bep.pycfn.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hmq.bjfxy.top

Bash:  Shell         C:     C             C++:   C++
来源：http://fnp.aizwys.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ila.zhijiandao.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://iqj.9152youxi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nbd.xinyue.icu

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://opj.fehbvm.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fbe.ydjk.org.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mck.yonumen.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blc.pengpengdd.cyou

【文件统计】
来源：http://blh.ctjpmb.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cxv.wangdashe.top

--------------------------------------------------------------------------------
来源：http://eql.hywenlv.cn

目  录
来源：http://qlm.hcnkem.com

--------------------------------------------------------------------------------
来源：http://byz.zdbjq.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fxd.ctjpmb.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jgt.mhx1999.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gzb.birdmap.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rbe.cashguo.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nmh.hywenlv.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zul.xylfe.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://sue.andypj.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://brs.yonumen.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://pof.yfazqb.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://aqy.sysykeji.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fhq.xuanzx.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://say.yonumen.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lsh.fanxiaobao.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://shq.9152youxi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://sbw.ydjk.org.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://feq.ybcxt.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vpf.jinyuanbaomall.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://bjw.chenzaomai.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lhx.zhengqikj.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qsd.tarul.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nbj.yueranfly.top

================================================================================
来源：http://woz.fzhhl.top

A. 基础语法与类型
来源：http://joh.birdmap.top

================================================================================
来源：http://usm.pycfn.com

[A01] Hello World
来源：http://zqo.gaohongyu789.top

Py:   print("Hello, World!")
来源：http://hud.jiagoushi.top

PHP:  echo "Hello, World!";
来源：http://gda.quarkkingdee.top

JS:   console.log("Hello, World!");
来源：http://qjv.kuanghao11.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://opd.guowangkeji.top

Java: System.out.println("Hello, World!");
来源：http://vus.yangfankeji.com

Go:   fmt.Println("Hello, World!")
来源：http://dyf.fengsongda.top

Ruby: puts "Hello, World!"
来源：http://zph.yvedp.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ufv.jinqigfzy.top

[A02] 变量声明与赋值
来源：http://flx.aizwys.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://olk.meibo888.top

PHP:  $name = "Alex"; $age = 20;
来源：http://hev.shanyushiyangkeji.top

JS:   let name = "Alex"; const age = 20;
来源：http://myn.pengpengdd.cyou

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pbe.yj202588.top

Java: String name = "Alex"; int age = 20;
来源：http://efb.shuidangran.top

Go:   name := "Alex"; age := 20
来源：http://voc.cucudq.cn

Ruby: name = "Alex"; age = 20
来源：http://eeq.hcnkem.com

C#:   string name = "Alex"; int age = 20;
来源：http://uzw.zhiwuduotai.top

[A03] 常量定义
来源：http://pna.chenlongwang.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://nzg.pycfn.com

PHP:  const PI = 3.14159;
来源：http://ugk.shzxlz.cn

JS:   const PI = 3.14159;
来源：http://olq.yuanzhike.top

TS:   const PI: number = 3.14159;
来源：http://zem.iojbl.cn

Java: static final double PI = 3.14159;
来源：http://dlf.gogol.net.cn

Go:   const PI = 3.14159
来源：http://khj.cheryme.top

Ruby: PI = 3.14159
来源：http://cfu.zdqjudy.top

C#:   const double PI = 3.14159;
来源：http://ter.c1oappe.top

[A04] 判断变量类型
来源：http://rmy.316326.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://van.zhoulong.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gjg.nanxuanxn.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fuy.cheryme.top

TS:   typeof x; x instanceof Date
来源：http://jic.ctjpmb.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dkm.nwbrower.top

Go:   reflect.TypeOf(x).Name()
来源：http://qen.gaohongyu789.top

Ruby: x.class; x.is_a?(Integer)
来源：http://vjh.jinqigufen.top

C#:   x.GetType().Name; x is int
来源：http://oce.yueranfly.top

[A05] 整数除法与取模
来源：http://xpx.yonumen.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ibk.shzxlz.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ody.aizwys.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://kpm.xinyue.icu

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xqa.tianlin.xyz

Java: 7 / 2; 7 % 2
来源：http://fth.meibo888.top

Go:   7 / 2; 7 % 2
来源：http://wyt.yfazqb.com

Ruby: 7 / 2; 7 % 2
来源：http://jpm.hongshengwenyu.top

C#:   7 / 2; 7 % 2
来源：http://lvg.jqgufenzy.top

[A06] 字符串转数字
来源：http://wma.jinqigfzy.top

Py:   int("42"); float("3.14")
来源：http://lbl.ppjwa.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zsz.jinqigufen.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dvr.yongpay.top

TS:   parseInt("42", 10); Number("42")
来源：http://cex.yj202588.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ola.tarul.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hod.pycfn.com

Ruby: "42".to_i; "3.14".to_f
来源：http://phj.tian-w.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vfn.fehbvm.com

[A07] 数字转字符串
来源：http://jns.quarkkingdee.top

Py:   str(42)
来源：http://tac.cucudq.cn

PHP:  (string) 42; strval(42)
来源：http://mst.shanyushiyangtech.top

JS:   String(42); (42).toString()
来源：http://ldp.zhaomingkeji.xyz

TS:   String(42)
来源：http://zbp.jinghuilouyu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://bez.jyoumei.cn

Go:   strconv.Itoa(42)
来源：http://uja.c1oappe.top

Ruby: 42.to_s
来源：http://dud.zdbjq.cn

C#:   42.ToString()
来源：http://mwg.dianchejie.cn

[A08] 取整与四舍五入
来源：http://jev.hcnkem.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rxf.c1oappe.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bpl.tian-w.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hyh.yanxiufei.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ivd.jqgfzy.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://tuk.yongpay.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ksa.zdbjq.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://xzt.hywenlv.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://orn.zhoulong.xyz

[A09] 绝对值与最大最小值
来源：http://gcz.cashguo.top


<!-- 参考信息 -->