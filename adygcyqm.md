代发 wailian999

[U61] PHP：正则
来源：http://tvb.zdbjq.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jaw.shzxlz.cn

[U62] PHP：日期对象
来源：http://wuw.ehwqpu.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://shj.dashuyun.cn

[U63] PHP：文件读写
来源：http://drb.sysykeji.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sjp.uphjek.com

[U64] PHP：目录遍历
来源：http://mgu.zhiwuduotai.top

glob("dir/*.php");  scandir("dir");
来源：http://xyo.ppjwa.cn

[U65] PHP：会话
来源：http://rin.yuanzhike.top

session_start();  $_SESSION["uid"] = 1;
来源：http://mjy.xuetiantiany.cn

[U66] PHP：设置 Cookie
来源：http://axc.jinqigufen.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ymo.chenlongwang.top

[U67] PHP：处理文件上传
来源：http://eoy.hnqzz.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xvv.meibo888.top

[U68] PHP：PDO 连接
来源：http://ids.jinqigfzy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://avd.gogol.net.cn

[U69] PHP：PDO 预处理
来源：http://gfe.epnwcf.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://eoz.jinyuanbaomall.cn

[U70] PHP：PDO 事务
来源：http://oyg.shanyushiyangtech.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blj.jinqigufen.top

[U71] PHP：抛出异常
来源：http://uhy.tanke756.top

throw new RuntimeException("失败", 500);
来源：http://psy.cucudq.cn

[U72] PHP：写错误日志
来源：http://vft.jianghu66.top

error_log("失败: " . $e->getMessage());
来源：http://kgr.svipenyu.cn

[U73] PHP：读取 ini 配置
来源：http://fbm.chenlongwang.top

parse_ini_file("config.ini", true)
来源：http://nmz.yj20258.top

[U74] PHP：读取环境变量
来源：http://sxw.hnxiangtu.top

getenv("APP_ENV") ?: "production"
来源：http://igb.fzhhl.top

[U75] PHP：依赖注入
来源：http://zry.cdnleiting.top

composer require psr/container
来源：http://foe.hammf.cn

[U76] PHP：简单路由
来源：http://ili.epnwcf.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ogp.shanyushiyangkeji.top

[U77] PHP：模板渲染
来源：http://cbd.birdmap.top

composer require twig/twig
来源：http://wsr.mhx1999.top

[U78] PHP：单元测试
来源：http://ieu.fktsv.cn

composer require --dev phpunit/phpunit
来源：http://ozx.yvedp.cn

[U79] PHP：静态分析
来源：http://crp.fengsongda.top

composer require --dev phpstan/phpstan
来源：http://hbj.chenlongwang.top

[U80] PHP：代码规范修复
来源：http://yag.gotoacloud.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://flt.xziqi.cn

[U81] JS：初始化项目
来源：http://now.jinyuanbaomall.cn

npm init -y;  npm i express
来源：http://jhi.guowangkeji.top

[U82] JS：package.json 脚本
来源：http://vim.tian-w.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pmm.wangshuangyany.cn

[U83] JS：ES Module 导入导出
来源：http://opc.wangdashe.top

export const a = 1;  import { a } from "./m.js";
来源：http://bjx.meibo888.top

[U84] JS：CommonJS 写法
来源：http://vkh.xuetiantiany.cn

module.exports = { a };  const { a } = require("./m");
来源：http://mhp.ivvv.top

[U85] JS：可选链
来源：http://fhn.yj20258.top

a?.b?.c
来源：http://buy.tanke756.top

[U86] JS：空值合并
来源：http://kle.shuidangran.top

a ?? b
来源：http://xxt.daxiang520.top

[U87] JS：解构默认值
来源：http://ztf.xinyue.icu

const { a = 1, b = 2 } = obj;
来源：http://gjw.hnqzz.top

[U88] JS：对象展开合并
来源：http://csx.redwolf501.top

{ ...a, ...b }
来源：http://ekf.bjfxy.top

[U89] JS：数组去重
来源：http://hys.yangfankeji.com

[...new Set(arr)]
来源：http://gsn.hongshengwenyu.top

[U90] JS：数字数组排序
来源：http://con.ywan-chungtsiang.top

[...arr].sort((a, b) => a - b)
来源：http://kfe.andypj.xyz

[U91] JS：对象键值遍历
来源：http://fba.chenjidiqi.icu

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bwl.jlsjyb.cn

[U92] JS：深拷贝
来源：http://bai.fehbvm.com

structuredClone(obj)
来源：http://ddr.quarkkingdee.top

[U93] JS：模板字符串
来源：http://kap.iojbl.cn

`共 ${n} 条`
来源：http://gsn.yj202588.top

[U94] JS：箭头函数
来源：http://gla.tian-w.cn

const double = x => x * 2;
来源：http://nai.cucudq.cn

[U95] JS：Promise 包装
来源：http://jsp.zhongyouzk.top

new Promise((resolve, reject) => {})
来源：http://qlg.ywan-chungtsiang.top

[U96] JS：async/await 与异常
来源：http://tlw.dianchejie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vtc.birdmap.top

[U97] JS：并发请求
来源：http://jit.jinqigfzy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://foo.gogol.net.cn

[U98] JS：fetch 带 JSON
来源：http://cmh.snrcjt.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://seg.sweek.top

[U99] JS：事件监听
来源：http://sfk.ctjpmb.com

el.addEventListener("click", e => {})
来源：http://vqi.sweek.top

[U100] JS：DOM 查询
来源：http://zfb.jinqigufen.top

document.querySelector(".item")
来源：http://qio.ydzc1.top

[U101] JS：classList 操作
来源：http://fzc.xuanzx.com

el.classList.toggle("active")
来源：http://qvp.zdqjudy.top

[U102] JS：本地存储
来源：http://wyn.quarkkingdee.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://puo.sweek.top

[U103] JS：定时器
来源：http://eny.hnxiangtu.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hdp.ivvv.top

[U104] JS：防抖
来源：http://vhl.sxryk.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zxy.zdbjq.cn

[U105] JS：节流
来源：http://ffo.chenjidiqi.icu

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hrl.fehbvm.com

[U106] JS：日期格式化
来源：http://tsa.sufxvd.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ovi.zhixingplan.top

[U107] JS：数字千分位
来源：http://wvb.yuxming.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://idd.tanke756.top

[U108] JS：随机整数
来源：http://ndz.iojbl.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nta.nanxuanxn.top

[U109] JS：数组分组
来源：http://nmm.meibo888.top

Object.groupBy(arr, x => x.type)
来源：http://xtb.sjlbkw.cn

[U110] JS：数组分块
来源：http://bpi.jinqigufen.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xpy.jinyuanbaomall.cn

[U111] JS：对象转 Map
来源：http://zvx.jinghuilouyu.cn

new Map(Object.entries(obj))
来源：http://wup.sjlbkw.cn

[U112] JS：字符串补位
来源：http://fji.c1oappe.top

"7".padStart(3, "0")
来源：http://qdf.epnwcf.com

[U113] JS：正则替换全部
来源：http://kvo.0kj1m.cn

s.replaceAll("a", "b")
来源：http://lvm.yj202588.top

[U114] JS：JSON 深比较
来源：http://azk.ivvv.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://jhb.jinghuilouyu.cn

[U115] JS：生成 UUID
来源：http://acz.cashguo.top

crypto.randomUUID()
来源：http://wcm.zycfv.cn

[U116] JS：类型检查（JSDoc）
来源：http://ypd.fengsongda.top

/** @param {string} name */ function f(name) {}
来源：http://itl.ppjwa.cn

[U117] JS：单元测试
来源：http://zim.shanyushiyangkeji.top

npm i -D vitest;  npx vitest
来源：http://nai.xuetiantiany.cn

[U118] JS：开发服务器
来源：http://yxo.yfazqb.com

npm i -D vite;  npx vite
来源：http://cqd.hnqzz.top

[U119] JS：生产构建
来源：http://avg.pycfn.com

npx vite build
来源：http://rye.fktsv.cn

[U120] JS：读取环境变量（Vite）
来源：http://dkq.xingfuxueyuan.xyz

import.meta.env.VITE_API_URL
来源：http://ppm.ctjpmb.com

================================================================================
来源：http://jon.cucudq.cn

统计汇总
来源：http://pdw.zhengqikj.top

================================================================================
来源：http://rjc.hesvh.cn

按语言统计（条）：
来源：http://ybf.zdbjq.cn

Python ......... 252
来源：http://yst.hywenlv.cn

PHP ............ 252
来源：http://weh.yangfankeji.com

JavaScript ..... 252
来源：http://vmq.shangyingyoupin.top

TypeScript ..... 212
来源：http://niv.andypj.xyz

Java ........... 212
来源：http://dyd.nanxinkj.top

Go ............. 212
来源：http://bpx.smart0.xyz

Ruby ........... 212
来源：http://yzg.hammf.cn

C# ............. 212
来源：http://pum.xuanzx.com

C .............. 30
来源：http://lyr.cdnleiting.top

C++ ............ 30
来源：http://vpn.sjlbkw.cn

SQL ............ 90
来源：http://qmn.hnxiangtu.top

Bash ........... 80
来源：http://rso.cheryme.top

Kotlin ......... 15
来源：http://rom.guowangkeji.top

Swift .......... 15
来源：http://nsd.jqgfzy.top

Lua ............ 10
来源：http://abf.wangshuangyany.cn

Perl ........... 10
来源：http://tgq.pycfn.com

Scala .......... 10
来源：http://dww.yuxming.cn

------------------------------------
来源：http://ggl.c1oappe.top

合计 ........... 2106 条
来源：http://rac.guowangkeji.top

按章节统计：
来源：http://gfi.yfazqb.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vgu.gotoacloud.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ysq.fktsv.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dle.wangshuangyany.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cms.ywan-chungtsiang.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dzi.xuetiantiany.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vmx.shzxlz.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://chx.yvedp.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tld.jqgfzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jtg.ydzc1.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://aie.gogol.net.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://azf.fzhhl.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qkg.yj20258888.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cwx.jyoumei.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://iys.andypj.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fyo.guowangkeji.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tyt.ywan-chungtsiang.top

Q SQL 专题                              90
来源：http://nzs.c1oappe.top

R Bash 专题                             80
来源：http://mqw.nanxinkj.top

S C / C++ 专题                          60
来源：http://lxi.cqqwz.cn

T 其他语言补充                          60
来源：http://ktc.pycfn.com

U 高频实用片段                         120
来源：http://bcj.yuxming.cn

------------------------------------
来源：http://qrr.hfpthk.cn

合计                                  2106 条
来源：http://vdt.shanyushiyangkeji.top

--------------------------------------------------------------------------------
来源：http://nai.hywenlv.cn

使用提醒
来源：http://uaj.gotoacloud.top

--------------------------------------------------------------------------------
来源：http://wvi.havefunace.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ohq.ybcxt.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://yww.kuanghao11.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rfo.hnxiangtu.top

在旧版本上使用前请先确认语法支持情况。
来源：http://jjh.jiagoushi.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://duy.pycfn.com

—— 文件结束 ——
来源：http://ohs.chenlongwang.top

================================================================================
来源：http://fik.xylfe.cn

程序语言常见例子速查手册（2024 版）
来源：http://fkz.yueranfly.top

Common Programming Examples Cheat Book
来源：http://xap.zhoulong.xyz

================================================================================
来源：http://nmh.cheryme.top

【收录内容】
来源：http://gfn.hammf.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://nny.hysaishi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ojt.jqgufenzy.top

SQL · Bash · C · C++
来源：http://jop.cdnleiting.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://egl.zhijiandao.cn

【使用说明】
来源：http://xeh.epnwcf.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hfw.hesvh.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wwg.hongshengwenyu.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wja.hammf.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wcf.sufxvd.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://llo.zhengqikj.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://laq.yueranfly.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vic.hongshengwenyu.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://elg.mhx1999.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ony.yonumen.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hlz.snrcjt.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://adk.yanxiufei.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dff.yfazqb.com

【文件统计】
来源：http://yim.zhongyouzk.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://eap.ehwqpu.com

--------------------------------------------------------------------------------
来源：http://gxe.yongpay.top

目  录
来源：http://hzk.yj20258888.top

--------------------------------------------------------------------------------
来源：http://ngj.wangshuangyany.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://cgd.zhiwuduotai.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zmx.ydzc1.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://igi.bjfxy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hwy.yj202588.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://sxp.nanxinkj.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xbp.zhengqikj.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ovv.daxiang520.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tsj.xylfe.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ugp.yuxming.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://opx.xziqi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bfh.tanke756.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://akf.zhijiandao.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yec.ppjwa.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://nol.daria6918.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://umn.0kj1m.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://pge.epnwcf.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nbt.cqqwz.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://cqv.birdmap.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rtr.yangfankeji.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rqo.chenjidiqi.icu

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hge.yueranfly.top

================================================================================
来源：http://ggi.ywan-chungtsiang.top

A. 基础语法与类型
来源：http://ngn.sxryk.cn

================================================================================
来源：http://kll.9152youxi.cn

[A01] Hello World
来源：http://kyj.birdmap.top

Py:   print("Hello, World!")
来源：http://gfd.ydjk.org.cn

PHP:  echo "Hello, World!";
来源：http://ppt.sufxvd.cn

JS:   console.log("Hello, World!");
来源：http://hvp.sjlbkw.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ydv.shangyingyoupin.top

Java: System.out.println("Hello, World!");
来源：http://tyt.ppjwa.cn

Go:   fmt.Println("Hello, World!")
来源：http://lrr.wangdashe.top

Ruby: puts "Hello, World!"
来源：http://gcw.sjlbkw.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://onb.shanyushiyangkeji.top

[A02] 变量声明与赋值
来源：http://wby.vehdjk.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://spf.gaohongyu789.top

PHP:  $name = "Alex"; $age = 20;
来源：http://yas.guowangkeji.top

JS:   let name = "Alex"; const age = 20;
来源：http://vbu.jqgufenzy.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gqc.xingfuxueyuan.xyz

Java: String name = "Alex"; int age = 20;
来源：http://xri.xingfuxueyuan.xyz

Go:   name := "Alex"; age := 20
来源：http://jwn.hnxiangtu.top

Ruby: name = "Alex"; age = 20
来源：http://pxq.cqqwz.cn

C#:   string name = "Alex"; int age = 20;
来源：http://dse.hammf.cn

[A03] 常量定义
来源：http://fcx.xziqi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hoi.yangfankeji.com

PHP:  const PI = 3.14159;
来源：http://ksu.hcnkem.com

JS:   const PI = 3.14159;
来源：http://vlu.xuetiantiany.cn

TS:   const PI: number = 3.14159;
来源：http://omw.jqgufenzy.top

Java: static final double PI = 3.14159;
来源：http://vub.cdnleiting.top

Go:   const PI = 3.14159
来源：http://rum.xuetiantiany.cn

Ruby: PI = 3.14159
来源：http://zbr.hnqzz.top

C#:   const double PI = 3.14159;
来源：http://ytn.hfpthk.cn

[A04] 判断变量类型
来源：http://mgr.quarkkingdee.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://vdh.zhengqikj.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yqu.jlsjyb.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pqn.ctjpmb.com

TS:   typeof x; x instanceof Date
来源：http://ffy.yuxming.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://urx.xuetiantiany.cn

Go:   reflect.TypeOf(x).Name()
来源：http://eql.zhiwuduotai.top

Ruby: x.class; x.is_a?(Integer)
来源：http://krs.yuxming.cn

C#:   x.GetType().Name; x is int
来源：http://qif.shangyingyoupin.top

[A05] 整数除法与取模
来源：http://wxi.aizwys.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jvk.cqqwz.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://lub.daria6918.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jei.jinqigufen.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cjx.hammf.cn

Java: 7 / 2; 7 % 2
来源：http://wxw.hysaishi.cn

Go:   7 / 2; 7 % 2
来源：http://qmz.dianchejie.cn

Ruby: 7 / 2; 7 % 2
来源：http://mzp.hnxiangtu.top

C#:   7 / 2; 7 % 2
来源：http://odd.hcnkem.com

[A06] 字符串转数字
来源：http://eub.hcnkem.com

Py:   int("42"); float("3.14")
来源：http://czt.zhoulong.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vyk.iojbl.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://eyh.epnwcf.com

TS:   parseInt("42", 10); Number("42")
来源：http://qhw.jinyuanbaomall.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://btg.daxiang520.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://smm.nanxuanxn.top

Ruby: "42".to_i; "3.14".to_f
来源：http://vvw.yfazqb.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mhu.zhaomingkeji.xyz

[A07] 数字转字符串
来源：http://wlk.52xcode.cn

Py:   str(42)
来源：http://rvq.gzhubu.top

PHP:  (string) 42; strval(42)
来源：http://ykb.gaohongyu789.top

JS:   String(42); (42).toString()
来源：http://nyj.yongpay.top

TS:   String(42)
来源：http://ocy.pengpengdd.cyou

Java: String.valueOf(42); Integer.toString(42)
来源：http://jit.shangyingyoupin.top

Go:   strconv.Itoa(42)
来源：http://zio.cheryme.top

Ruby: 42.to_s
来源：http://ohu.chenzaomai.com

C#:   42.ToString()
来源：http://eam.chenjidiqi.icu

[A08] 取整与四舍五入
来源：http://wdp.dianchejie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jsq.xziqi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://eii.0kj1m.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hir.yvedp.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dyx.jinghuilouyu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://kji.zhijiandao.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xxu.xinyue.icu

Ruby: 3.567.round(2); 3.9.floor
来源：http://awf.smart0.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ciw.smart0.xyz

[A09] 绝对值与最大最小值
来源：http://tft.ydjk.org.cn


<!-- 参考信息 -->