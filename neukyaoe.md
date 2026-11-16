代发 wailian999

[U61] PHP：正则
来源：http://hjb.52xcode.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wpx.nanxinkj.top

[U62] PHP：日期对象
来源：http://voo.andypj.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pkd.guannengcc.top

[U63] PHP：文件读写
来源：http://bix.chenlongwang.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rvn.tianlin.xyz

[U64] PHP：目录遍历
来源：http://rdl.tarul.cn

glob("dir/*.php");  scandir("dir");
来源：http://uqv.sufxvd.cn

[U65] PHP：会话
来源：http://dpc.fanxiaobao.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://yhq.zhixingplan.top

[U66] PHP：设置 Cookie
来源：http://lue.dianchejie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bkd.0kj1m.cn

[U67] PHP：处理文件上传
来源：http://uuo.tianlin.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gtn.ybcxt.top

[U68] PHP：PDO 连接
来源：http://kbf.daria6918.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://oxy.jlsjyb.cn

[U69] PHP：PDO 预处理
来源：http://qgk.yonumen.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://agf.ppjwa.cn

[U70] PHP：PDO 事务
来源：http://xfd.gotoacloud.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ypp.birdmap.top

[U71] PHP：抛出异常
来源：http://tza.vehdjk.com

throw new RuntimeException("失败", 500);
来源：http://wtc.xylfe.cn

[U72] PHP：写错误日志
来源：http://djf.yangfankeji.com

error_log("失败: " . $e->getMessage());
来源：http://flp.zycfv.cn

[U73] PHP：读取 ini 配置
来源：http://jmq.zhongyouzk.top

parse_ini_file("config.ini", true)
来源：http://czb.yuxming.cn

[U74] PHP：读取环境变量
来源：http://ope.ehwqpu.com

getenv("APP_ENV") ?: "production"
来源：http://out.nwbrower.top

[U75] PHP：依赖注入
来源：http://spm.xuanzx.com

composer require psr/container
来源：http://sza.dashuyun.cn

[U76] PHP：简单路由
来源：http://cru.dianchejie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uxc.shangyingyoupin.top

[U77] PHP：模板渲染
来源：http://lgr.xuetiantiany.cn

composer require twig/twig
来源：http://hog.guowangkeji.top

[U78] PHP：单元测试
来源：http://uyv.xylfe.cn

composer require --dev phpunit/phpunit
来源：http://fdf.hnxiangtu.top

[U79] PHP：静态分析
来源：http://qgj.daxiang520.top

composer require --dev phpstan/phpstan
来源：http://dda.hywenlv.cn

[U80] PHP：代码规范修复
来源：http://odq.uphjek.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://tcx.kuanghao11.cn

[U81] JS：初始化项目
来源：http://mms.cdnleiting.top

npm init -y;  npm i express
来源：http://azl.ywan-chungtsiang.top

[U82] JS：package.json 脚本
来源：http://kjd.fktsv.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jtw.cucudq.cn

[U83] JS：ES Module 导入导出
来源：http://wud.aizwys.cn

export const a = 1;  import { a } from "./m.js";
来源：http://rcy.52xcode.cn

[U84] JS：CommonJS 写法
来源：http://eki.sjlbkw.cn

module.exports = { a };  const { a } = require("./m");
来源：http://raq.tianlin.xyz

[U85] JS：可选链
来源：http://lri.zhijiandao.cn

a?.b?.c
来源：http://bts.hammf.cn

[U86] JS：空值合并
来源：http://ewy.yfazqb.com

a ?? b
来源：http://dze.fengsongda.top

[U87] JS：解构默认值
来源：http://ocx.sxryk.cn

const { a = 1, b = 2 } = obj;
来源：http://zyk.aibaodan.cn

[U88] JS：对象展开合并
来源：http://qdk.yj202588.top

{ ...a, ...b }
来源：http://bke.hnqzz.top

[U89] JS：数组去重
来源：http://fyi.zycfv.cn

[...new Set(arr)]
来源：http://rqx.nanxuanxn.top

[U90] JS：数字数组排序
来源：http://vdo.ehwqpu.com

[...arr].sort((a, b) => a - b)
来源：http://nsx.fengsongda.top

[U91] JS：对象键值遍历
来源：http://xpr.jianghu66.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tpj.jqgfzy.top

[U92] JS：深拷贝
来源：http://qqu.feifeiyinyue.top

structuredClone(obj)
来源：http://dai.fengsongda.top

[U93] JS：模板字符串
来源：http://aub.yanxiufei.cn

`共 ${n} 条`
来源：http://gym.ybcxt.top

[U94] JS：箭头函数
来源：http://oco.havefunace.top

const double = x => x * 2;
来源：http://wci.yuanzhike.top

[U95] JS：Promise 包装
来源：http://rdp.jqgufenzy.top

new Promise((resolve, reject) => {})
来源：http://cuk.yj20258888.top

[U96] JS：async/await 与异常
来源：http://deu.ctjpmb.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tgd.zhaomingkeji.xyz

[U97] JS：并发请求
来源：http://gie.zhaomingkeji.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://xem.sweek.top

[U98] JS：fetch 带 JSON
来源：http://qqy.jyoumei.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bof.shzxlz.cn

[U99] JS：事件监听
来源：http://epj.xingfuxueyuan.xyz

el.addEventListener("click", e => {})
来源：http://lls.meibo888.top

[U100] JS：DOM 查询
来源：http://fsf.yuanzhike.top

document.querySelector(".item")
来源：http://oil.gaohongyu789.top

[U101] JS：classList 操作
来源：http://fas.xuetiantiany.cn

el.classList.toggle("active")
来源：http://uou.guowangkeji.top

[U102] JS：本地存储
来源：http://etr.316326.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://gzx.hfpthk.cn

[U103] JS：定时器
来源：http://brk.0kj1m.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lzw.sxryk.cn

[U104] JS：防抖
来源：http://nid.havefunace.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://odo.sysykeji.top

[U105] JS：节流
来源：http://wjs.jinqigfzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nid.jinqigfzy.top

[U106] JS：日期格式化
来源：http://yat.sxryk.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yls.xuetiantiany.cn

[U107] JS：数字千分位
来源：http://mbf.dianchejie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pie.c1oappe.top

[U108] JS：随机整数
来源：http://jlx.sxryk.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dno.yongpay.top

[U109] JS：数组分组
来源：http://jdw.vehdjk.com

Object.groupBy(arr, x => x.type)
来源：http://iqe.wangdashe.top

[U110] JS：数组分块
来源：http://cpe.ydjk.org.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ebp.bbcook.cn

[U111] JS：对象转 Map
来源：http://mhg.aizwys.cn

new Map(Object.entries(obj))
来源：http://qor.cqqwz.cn

[U112] JS：字符串补位
来源：http://muc.ywan-chungtsiang.top

"7".padStart(3, "0")
来源：http://ixj.yangfankeji.com

[U113] JS：正则替换全部
来源：http://lra.bjfxy.top

s.replaceAll("a", "b")
来源：http://lst.zhongyouzk.top

[U114] JS：JSON 深比较
来源：http://rwc.zdbjq.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hun.nwbrower.top

[U115] JS：生成 UUID
来源：http://wzz.havefunace.top

crypto.randomUUID()
来源：http://gil.hammf.cn

[U116] JS：类型检查（JSDoc）
来源：http://mwj.sweek.top

/** @param {string} name */ function f(name) {}
来源：http://zgg.zhijiandao.cn

[U117] JS：单元测试
来源：http://clr.fzhhl.top

npm i -D vitest;  npx vitest
来源：http://wsv.vqdsnc.cn

[U118] JS：开发服务器
来源：http://ykx.zhixingplan.top

npm i -D vite;  npx vite
来源：http://ssp.ppjwa.cn

[U119] JS：生产构建
来源：http://hri.hammf.cn

npx vite build
来源：http://ove.shanyushiyangtech.top

[U120] JS：读取环境变量（Vite）
来源：http://nks.jiagoushi.top

import.meta.env.VITE_API_URL
来源：http://wom.jlsjyb.cn

================================================================================
来源：http://eub.havefunace.top

统计汇总
来源：http://ugn.c1oappe.top

================================================================================
来源：http://com.gzhubu.top

按语言统计（条）：
来源：http://zku.yueranfly.top

Python ......... 252
来源：http://phd.vehdjk.com

PHP ............ 252
来源：http://guu.wangshuangyany.cn

JavaScript ..... 252
来源：http://nwl.9152youxi.cn

TypeScript ..... 212
来源：http://kul.yvedp.cn

Java ........... 212
来源：http://mou.ydjk.org.cn

Go ............. 212
来源：http://pgb.hcnkem.com

Ruby ........... 212
来源：http://fny.jianghu66.top

C# ............. 212
来源：http://pjv.zhaomingkeji.xyz

C .............. 30
来源：http://pit.zdqjudy.top

C++ ............ 30
来源：http://xby.chenzaomai.com

SQL ............ 90
来源：http://amv.hywenlv.cn

Bash ........... 80
来源：http://zit.tarul.cn

Kotlin ......... 15
来源：http://zrc.zhengqikj.top

Swift .......... 15
来源：http://boq.shangyingyoupin.top

Lua ............ 10
来源：http://rgu.gogol.net.cn

Perl ........... 10
来源：http://rdc.zhiwuduotai.top

Scala .......... 10
来源：http://acz.pengpengdd.cyou

------------------------------------
来源：http://nfv.0kj1m.cn

合计 ........... 2106 条
来源：http://fbn.hongshengwenyu.top

按章节统计：
来源：http://pgs.zdqjudy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hte.xziqi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://piy.cdnleiting.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cmo.iojbl.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gwu.zdbjq.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vqx.birdmap.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cwi.gzhubu.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xtx.chenlongwang.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kue.yj20258.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ymk.aizwys.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hio.epnwcf.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zac.sweek.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://bvf.xuetiantiany.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lqa.hnxiangtu.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pzd.xylfe.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qpv.fzhhl.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xdl.daria6918.cn

Q SQL 专题                              90
来源：http://gir.dianchejie.cn

R Bash 专题                             80
来源：http://kzy.mhx1999.top

S C / C++ 专题                          60
来源：http://brm.vehdjk.com

T 其他语言补充                          60
来源：http://lua.nanxinkj.top

U 高频实用片段                         120
来源：http://mzy.ppjwa.cn

------------------------------------
来源：http://gkh.ydjk.org.cn

合计                                  2106 条
来源：http://npl.fzhhl.top

--------------------------------------------------------------------------------
来源：http://jho.zhiwuduotai.top

使用提醒
来源：http://chb.sysykeji.top

--------------------------------------------------------------------------------
来源：http://vpn.zdbjq.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jui.gogol.net.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://joe.jqgfzy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jiv.yongpay.top

在旧版本上使用前请先确认语法支持情况。
来源：http://cyf.epnwcf.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xph.vqdsnc.cn

—— 文件结束 ——
来源：http://ujn.vqdsnc.cn

================================================================================
来源：http://bpp.yj20258.top

程序语言常见例子速查手册（2024 版）
来源：http://nkh.cashguo.top

Common Programming Examples Cheat Book
来源：http://ool.jqgfzy.top

================================================================================
来源：http://hzg.xuetiantiany.cn

【收录内容】
来源：http://yzh.feifeiyinyue.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://mzz.zhaomingkeji.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bng.yuanzhike.top

SQL · Bash · C · C++
来源：http://zzj.9152youxi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://njc.pycfn.com

【使用说明】
来源：http://sub.shzxlz.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jqm.jinqigufen.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kbf.ydzc1.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://cax.sweek.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yyj.wangshuangyany.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://yrj.ctjpmb.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qkz.havefunace.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://uyy.ydjk.org.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xpw.shanyushiyangkeji.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rck.svipenyu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qbz.snrcjt.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://uyu.yonumen.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xbw.sjlbkw.cn

【文件统计】
来源：http://bwx.shangyingyoupin.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gip.jiagoushi.top

--------------------------------------------------------------------------------
来源：http://qyt.chenlongwang.top

目  录
来源：http://eje.gaohongyu789.top

--------------------------------------------------------------------------------
来源：http://hsf.uphjek.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yfx.ywan-chungtsiang.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zos.uphjek.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://diu.chenzaomai.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mix.guowangkeji.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://svb.xingfuxueyuan.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pmr.zhaomingkeji.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ejf.zhixingplan.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://trt.jinghuilouyu.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://nhs.ywan-chungtsiang.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://win.ppjwa.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ohl.9152youxi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dlu.316326.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yzf.yfazqb.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vkc.c1oappe.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zbd.yueranfly.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rfm.yueranfly.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gmu.yanxiufei.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://bqq.cucudq.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://kju.sjlbkw.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lky.jinqigufen.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qtc.yvedp.cn

================================================================================
来源：http://xqe.jqgfzy.top

A. 基础语法与类型
来源：http://mty.hcnkem.com

================================================================================
来源：http://eql.dianchejie.cn

[A01] Hello World
来源：http://hdg.gogol.net.cn

Py:   print("Hello, World!")
来源：http://zde.wangdashe.top

PHP:  echo "Hello, World!";
来源：http://idm.smart0.xyz

JS:   console.log("Hello, World!");
来源：http://otf.yj20258888.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tjf.shzxlz.cn

Java: System.out.println("Hello, World!");
来源：http://dmq.fktsv.cn

Go:   fmt.Println("Hello, World!")
来源：http://let.shzxlz.cn

Ruby: puts "Hello, World!"
来源：http://tou.jqgufenzy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://vsp.dianchejie.cn

[A02] 变量声明与赋值
来源：http://gja.havefunace.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bxu.sxryk.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://rgs.yangfankeji.com

JS:   let name = "Alex"; const age = 20;
来源：http://mdt.tanke756.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hxr.ppjwa.cn

Java: String name = "Alex"; int age = 20;
来源：http://azp.52xcode.cn

Go:   name := "Alex"; age := 20
来源：http://ycc.fzhhl.top

Ruby: name = "Alex"; age = 20
来源：http://yya.redwolf501.top

C#:   string name = "Alex"; int age = 20;
来源：http://gqk.chenzaomai.com

[A03] 常量定义
来源：http://lfw.jinqigufen.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://egw.hywenlv.cn

PHP:  const PI = 3.14159;
来源：http://sdi.jiagoushi.top

JS:   const PI = 3.14159;
来源：http://qcb.snrcjt.cn

TS:   const PI: number = 3.14159;
来源：http://xov.hysaishi.cn

Java: static final double PI = 3.14159;
来源：http://vdo.redwolf501.top

Go:   const PI = 3.14159
来源：http://niu.chenlongwang.top

Ruby: PI = 3.14159
来源：http://qsv.sweek.top

C#:   const double PI = 3.14159;
来源：http://oyk.zhaomingkeji.xyz

[A04] 判断变量类型
来源：http://fxz.kuanghao11.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://qed.zycfv.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ueb.ydjk.org.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bgd.chenjidiqi.icu

TS:   typeof x; x instanceof Date
来源：http://oav.shanyushiyangkeji.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hvj.andypj.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://vvu.zdqjudy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://abw.shanyushiyangtech.top

C#:   x.GetType().Name; x is int
来源：http://kbj.svipenyu.cn

[A05] 整数除法与取模
来源：http://qmi.hnqzz.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mtw.0kj1m.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ils.yj202588.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://fys.xingfuxueyuan.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ynv.uphjek.com

Java: 7 / 2; 7 % 2
来源：http://yzv.ehwqpu.com

Go:   7 / 2; 7 % 2
来源：http://yqt.guowangkeji.top

Ruby: 7 / 2; 7 % 2
来源：http://dsd.fktsv.cn

C#:   7 / 2; 7 % 2
来源：http://wyx.jlsjyb.cn

[A06] 字符串转数字
来源：http://fcs.jqgfzy.top

Py:   int("42"); float("3.14")
来源：http://kmp.guannengcc.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://esi.zdbjq.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://kdw.sysykeji.top

TS:   parseInt("42", 10); Number("42")
来源：http://ktk.tian-w.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rkm.zhongyouzk.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://sng.sweek.top

Ruby: "42".to_i; "3.14".to_f
来源：http://waf.hnxiangtu.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://lbr.ehwqpu.com

[A07] 数字转字符串
来源：http://ofi.epnwcf.com

Py:   str(42)
来源：http://isi.ybcxt.top

PHP:  (string) 42; strval(42)
来源：http://mbq.yfazqb.com

JS:   String(42); (42).toString()
来源：http://kib.dianchejie.cn

TS:   String(42)
来源：http://avk.gogol.net.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://uor.nanxuanxn.top

Go:   strconv.Itoa(42)
来源：http://ddo.nanxuanxn.top

Ruby: 42.to_s
来源：http://trj.zhiwuduotai.top

C#:   42.ToString()
来源：http://vvl.hnxiangtu.top

[A08] 取整与四舍五入
来源：http://fin.jinghuilouyu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dwg.sufxvd.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://pav.jinqigfzy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gys.ppjwa.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dlq.yuxming.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ndm.yanxiufei.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ebx.zycfv.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://qvf.gogol.net.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gou.ctjpmb.com

[A09] 绝对值与最大最小值
来源：http://hor.daria6918.cn


<!-- 参考信息 -->