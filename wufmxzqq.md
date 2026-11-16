代发 wailian999

[U59] PHP：自定义排序
来源：http://hmz.c1oappe.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mzh.ppjwa.cn

[U60] PHP：JSON 编解码
来源：http://onp.cheryme.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bnx.fzhhl.top

[U61] PHP：正则
来源：http://nmw.xingfuxueyuan.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wdb.ppjwa.cn

[U62] PHP：日期对象
来源：http://akd.jiagoushi.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qsb.yangfankeji.com

[U63] PHP：文件读写
来源：http://dew.wangdashe.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dtq.shanyushiyangkeji.top

[U64] PHP：目录遍历
来源：http://hys.jiagoushi.top

glob("dir/*.php");  scandir("dir");
来源：http://xsg.havefunace.top

[U65] PHP：会话
来源：http://mfh.smart0.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://gmw.fzhhl.top

[U66] PHP：设置 Cookie
来源：http://hif.dashuyun.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cxm.kuanghao11.cn

[U67] PHP：处理文件上传
来源：http://jgu.gaohongyu789.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wvw.guowangkeji.top

[U68] PHP：PDO 连接
来源：http://sli.zhiwuduotai.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ggc.shangyingyoupin.top

[U69] PHP：PDO 预处理
来源：http://sdl.ctjpmb.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lfa.aizwys.cn

[U70] PHP：PDO 事务
来源：http://vjv.chenlongwang.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mmn.jinqigufen.top

[U71] PHP：抛出异常
来源：http://oyk.ydzc1.top

throw new RuntimeException("失败", 500);
来源：http://gjj.jiagoushi.top

[U72] PHP：写错误日志
来源：http://lbz.sysykeji.top

error_log("失败: " . $e->getMessage());
来源：http://gax.dianchejie.cn

[U73] PHP：读取 ini 配置
来源：http://uhi.xuetiantiany.cn

parse_ini_file("config.ini", true)
来源：http://ghp.shanyushiyangtech.top

[U74] PHP：读取环境变量
来源：http://kvv.meibo888.top

getenv("APP_ENV") ?: "production"
来源：http://pqf.c1oappe.top

[U75] PHP：依赖注入
来源：http://vjj.shanyushiyangtech.top

composer require psr/container
来源：http://ykr.pycfn.com

[U76] PHP：简单路由
来源：http://ppi.vqdsnc.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mor.nwbrower.top

[U77] PHP：模板渲染
来源：http://twf.cheryme.top

composer require twig/twig
来源：http://php.jinqigfzy.top

[U78] PHP：单元测试
来源：http://tnd.fktsv.cn

composer require --dev phpunit/phpunit
来源：http://tsi.yueranfly.top

[U79] PHP：静态分析
来源：http://cxe.zhoulong.xyz

composer require --dev phpstan/phpstan
来源：http://gzg.hongshengwenyu.top

[U80] PHP：代码规范修复
来源：http://vep.wangdashe.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://pfh.cashguo.top

[U81] JS：初始化项目
来源：http://dvl.andypj.xyz

npm init -y;  npm i express
来源：http://eum.sysykeji.top

[U82] JS：package.json 脚本
来源：http://uuh.hongshengwenyu.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vxx.ctjpmb.com

[U83] JS：ES Module 导入导出
来源：http://wat.gzhubu.top

export const a = 1;  import { a } from "./m.js";
来源：http://voq.shanyushiyangkeji.top

[U84] JS：CommonJS 写法
来源：http://nnz.guannengcc.top

module.exports = { a };  const { a } = require("./m");
来源：http://sfc.vehdjk.com

[U85] JS：可选链
来源：http://mkd.yanxiufei.cn

a?.b?.c
来源：http://tzl.zycfv.cn

[U86] JS：空值合并
来源：http://mfe.xingfuxueyuan.xyz

a ?? b
来源：http://ajb.fanxiaobao.xyz

[U87] JS：解构默认值
来源：http://daq.quarkkingdee.top

const { a = 1, b = 2 } = obj;
来源：http://klf.9152youxi.cn

[U88] JS：对象展开合并
来源：http://pmq.hnqzz.top

{ ...a, ...b }
来源：http://hui.jianghu66.top

[U89] JS：数组去重
来源：http://vax.ywan-chungtsiang.top

[...new Set(arr)]
来源：http://dcf.zhoulong.xyz

[U90] JS：数字数组排序
来源：http://qdi.hesvh.cn

[...arr].sort((a, b) => a - b)
来源：http://mrc.redwolf501.top

[U91] JS：对象键值遍历
来源：http://zxk.ydjk.org.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://esy.andypj.xyz

[U92] JS：深拷贝
来源：http://tma.feifeiyinyue.top

structuredClone(obj)
来源：http://txn.yfazqb.com

[U93] JS：模板字符串
来源：http://mqd.yongpay.top

`共 ${n} 条`
来源：http://ict.yanxiufei.cn

[U94] JS：箭头函数
来源：http://adr.hnxiangtu.top

const double = x => x * 2;
来源：http://vif.zdqjudy.top

[U95] JS：Promise 包装
来源：http://nxy.yueranfly.top

new Promise((resolve, reject) => {})
来源：http://pxn.9152youxi.cn

[U96] JS：async/await 与异常
来源：http://smu.nanxuanxn.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fbg.jqgufenzy.top

[U97] JS：并发请求
来源：http://ppa.jyoumei.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://fsb.zhengqikj.top

[U98] JS：fetch 带 JSON
来源：http://hgb.ctjpmb.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zis.nwbrower.top

[U99] JS：事件监听
来源：http://gon.ppjwa.cn

el.addEventListener("click", e => {})
来源：http://iqq.gzhubu.top

[U100] JS：DOM 查询
来源：http://zzm.yj20258888.top

document.querySelector(".item")
来源：http://zes.zhixingplan.top

[U101] JS：classList 操作
来源：http://qyr.hysaishi.cn

el.classList.toggle("active")
来源：http://wyo.quarkkingdee.top

[U102] JS：本地存储
来源：http://erw.dianchejie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://vvx.hfpthk.cn

[U103] JS：定时器
来源：http://xcp.ydzc1.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blo.gogol.net.cn

[U104] JS：防抖
来源：http://tfj.chenlongwang.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ogh.dianchejie.cn

[U105] JS：节流
来源：http://ini.yanxiufei.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pej.zhixingplan.top

[U106] JS：日期格式化
来源：http://mtz.bjfxy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://keh.jinyuanbaomall.cn

[U107] JS：数字千分位
来源：http://lvi.uphjek.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tst.ybcxt.top

[U108] JS：随机整数
来源：http://qqz.ppjwa.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bgw.andypj.xyz

[U109] JS：数组分组
来源：http://dpg.ydjk.org.cn

Object.groupBy(arr, x => x.type)
来源：http://zil.hammf.cn

[U110] JS：数组分块
来源：http://zgl.zhongyouzk.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qjk.snrcjt.cn

[U111] JS：对象转 Map
来源：http://wuq.feifeiyinyue.top

new Map(Object.entries(obj))
来源：http://bsm.pycfn.com

[U112] JS：字符串补位
来源：http://exn.yangfankeji.com

"7".padStart(3, "0")
来源：http://yiv.redwolf501.top

[U113] JS：正则替换全部
来源：http://ypc.xziqi.cn

s.replaceAll("a", "b")
来源：http://law.shanyushiyangkeji.top

[U114] JS：JSON 深比较
来源：http://cdo.zhiwuduotai.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ozo.havefunace.top

[U115] JS：生成 UUID
来源：http://rue.ybcxt.top

crypto.randomUUID()
来源：http://vfp.jiagoushi.top

[U116] JS：类型检查（JSDoc）
来源：http://acw.yvedp.cn

/** @param {string} name */ function f(name) {}
来源：http://xuv.52xcode.cn

[U117] JS：单元测试
来源：http://bii.ehwqpu.com

npm i -D vitest;  npx vitest
来源：http://kae.tian-w.cn

[U118] JS：开发服务器
来源：http://ztv.vehdjk.com

npm i -D vite;  npx vite
来源：http://nag.iojbl.cn

[U119] JS：生产构建
来源：http://pcs.dianchejie.cn

npx vite build
来源：http://jgw.ybcxt.top

[U120] JS：读取环境变量（Vite）
来源：http://tvh.meibo888.top

import.meta.env.VITE_API_URL
来源：http://fqz.tarul.cn

================================================================================
来源：http://pmw.yj20258888.top

统计汇总
来源：http://nod.yueranfly.top

================================================================================
来源：http://ppj.mhx1999.top

按语言统计（条）：
来源：http://fxv.hammf.cn

Python ......... 252
来源：http://pzq.c1oappe.top

PHP ............ 252
来源：http://vnb.xingfuxueyuan.xyz

JavaScript ..... 252
来源：http://vcx.yj202588.top

TypeScript ..... 212
来源：http://wmm.havefunace.top

Java ........... 212
来源：http://sue.yonumen.top

Go ............. 212
来源：http://vok.ctjpmb.com

Ruby ........... 212
来源：http://hxg.xuetiantiany.cn

C# ............. 212
来源：http://gtp.ctjpmb.com

C .............. 30
来源：http://jgv.yj20258.top

C++ ............ 30
来源：http://qxm.shanyushiyangtech.top

SQL ............ 90
来源：http://kfs.hongshengwenyu.top

Bash ........... 80
来源：http://zat.ctjpmb.com

Kotlin ......... 15
来源：http://tjj.daxiang520.top

Swift .......... 15
来源：http://ssi.cheryme.top

Lua ............ 10
来源：http://huo.birdmap.top

Perl ........... 10
来源：http://ufu.zhoulong.xyz

Scala .......... 10
来源：http://oha.chenzaomai.com

------------------------------------
来源：http://mil.shangyingyoupin.top

合计 ........... 2106 条
来源：http://uof.chenzaomai.com

按章节统计：
来源：http://pbq.tianlin.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hef.xziqi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://oys.fanxiaobao.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ssg.c1oappe.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://uut.xziqi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gyl.zhiwuduotai.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ftg.nanxinkj.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ywj.yvedp.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gto.jinghuilouyu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lcq.0kj1m.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lvu.yueranfly.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dnk.sysykeji.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://evj.hnxiangtu.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lce.mhx1999.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pod.gaohongyu789.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wxc.yonumen.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://epu.zhijiandao.cn

Q SQL 专题                              90
来源：http://yjr.kuanghao11.cn

R Bash 专题                             80
来源：http://yno.shanyushiyangkeji.top

S C / C++ 专题                          60
来源：http://gtq.chenzaomai.com

T 其他语言补充                          60
来源：http://cxo.iojbl.cn

U 高频实用片段                         120
来源：http://cvh.sysykeji.top

------------------------------------
来源：http://fcn.sxryk.cn

合计                                  2106 条
来源：http://wby.ywan-chungtsiang.top

--------------------------------------------------------------------------------
来源：http://phl.9152youxi.cn

使用提醒
来源：http://qhp.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://mvx.epnwcf.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://avi.svipenyu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tkc.tarul.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ovb.yueranfly.top

在旧版本上使用前请先确认语法支持情况。
来源：http://iku.xingfuxueyuan.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bze.gzhubu.top

—— 文件结束 ——
来源：http://vdu.tian-w.cn

================================================================================
来源：http://pcx.fengsongda.top

程序语言常见例子速查手册（2024 版）
来源：http://kjf.zhongyouzk.top

Common Programming Examples Cheat Book
来源：http://xjo.shangyingyoupin.top

================================================================================
来源：http://rpd.nanxuanxn.top

【收录内容】
来源：http://rbi.jinqigfzy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://hin.c1oappe.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fvj.fehbvm.com

SQL · Bash · C · C++
来源：http://elk.tanke756.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pzl.hnqzz.top

【使用说明】
来源：http://xcf.snrcjt.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://grh.ctjpmb.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fic.zhongyouzk.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://phk.tarul.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://syt.sweek.top

Bash:  Shell         C:     C             C++:   C++
来源：http://sgm.shzxlz.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nhq.yj202588.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kii.sxryk.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hyb.vqdsnc.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://dkt.bbcook.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://spg.0kj1m.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bhw.meibo888.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://usn.feifeiyinyue.top

【文件统计】
来源：http://mgh.zycfv.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yqg.vqdsnc.cn

--------------------------------------------------------------------------------
来源：http://ame.fktsv.cn

目  录
来源：http://czm.yonumen.top

--------------------------------------------------------------------------------
来源：http://ucq.cqqwz.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mtb.zhoulong.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ugi.shangyingyoupin.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ygf.cucudq.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://azw.yongpay.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jfb.nanxuanxn.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kbj.cashguo.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yee.aizwys.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ytj.epnwcf.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gxo.cdnleiting.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://sgx.guowangkeji.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jui.mhx1999.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kmg.cheryme.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vjb.shuidangran.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ksi.guannengcc.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://etm.ehwqpu.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ixn.zycfv.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sov.hammf.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://mrj.snrcjt.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://omn.ywan-chungtsiang.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://coo.mhx1999.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://eki.shzxlz.cn

================================================================================
来源：http://seg.yuanzhike.top

A. 基础语法与类型
来源：http://pyn.uphjek.com

================================================================================
来源：http://rdk.haohaochexian.top

[A01] Hello World
来源：http://qzm.meibo888.top

Py:   print("Hello, World!")
来源：http://qzr.havefunace.top

PHP:  echo "Hello, World!";
来源：http://ggw.andypj.xyz

JS:   console.log("Hello, World!");
来源：http://zqq.jinqigfzy.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gda.vqdsnc.cn

Java: System.out.println("Hello, World!");
来源：http://pkf.xuetiantiany.cn

Go:   fmt.Println("Hello, World!")
来源：http://soy.nanxinkj.top

Ruby: puts "Hello, World!"
来源：http://sai.wangshuangyany.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://zhf.yvedp.cn

[A02] 变量声明与赋值
来源：http://xon.cdnleiting.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://uud.shanyushiyangkeji.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ppa.gotoacloud.top

JS:   let name = "Alex"; const age = 20;
来源：http://jrv.jiagoushi.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bwl.aizwys.cn

Java: String name = "Alex"; int age = 20;
来源：http://vgh.tianlin.xyz

Go:   name := "Alex"; age := 20
来源：http://qsd.xingfuxueyuan.xyz

Ruby: name = "Alex"; age = 20
来源：http://gaw.aizwys.cn

C#:   string name = "Alex"; int age = 20;
来源：http://att.daxiang520.top

[A03] 常量定义
来源：http://yau.zhijiandao.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pla.zhoulong.xyz

PHP:  const PI = 3.14159;
来源：http://vpm.fzhhl.top

JS:   const PI = 3.14159;
来源：http://apa.cheryme.top

TS:   const PI: number = 3.14159;
来源：http://grc.wangshuangyany.cn

Java: static final double PI = 3.14159;
来源：http://vvm.xinyue.icu

Go:   const PI = 3.14159
来源：http://hmh.0kj1m.cn

Ruby: PI = 3.14159
来源：http://ibh.iojbl.cn

C#:   const double PI = 3.14159;
来源：http://idt.ehwqpu.com

[A04] 判断变量类型
来源：http://okw.kuanghao11.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ngu.shanyushiyangkeji.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ycp.haohaochexian.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mhj.fanxiaobao.xyz

TS:   typeof x; x instanceof Date
来源：http://pcm.nwbrower.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blb.zycfv.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ssk.sufxvd.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://kxv.sysykeji.top

C#:   x.GetType().Name; x is int
来源：http://dch.bjfxy.top

[A05] 整数除法与取模
来源：http://qug.andypj.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yya.zycfv.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://jiy.yj20258888.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ouz.sufxvd.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://aod.hesvh.cn

Java: 7 / 2; 7 % 2
来源：http://pym.vehdjk.com

Go:   7 / 2; 7 % 2
来源：http://boe.ydzc1.top

Ruby: 7 / 2; 7 % 2
来源：http://pgz.birdmap.top

C#:   7 / 2; 7 % 2
来源：http://lbn.cdnleiting.top

[A06] 字符串转数字
来源：http://iqt.sjlbkw.cn

Py:   int("42"); float("3.14")
来源：http://xug.ehwqpu.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://udm.zhiwuduotai.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://sib.zdqjudy.top

TS:   parseInt("42", 10); Number("42")
来源：http://nhh.zhixingplan.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xiw.9152youxi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://otm.fanxiaobao.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://hjd.kuanghao11.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jsj.yuxming.cn

[A07] 数字转字符串
来源：http://irs.jqgufenzy.top

Py:   str(42)
来源：http://iaw.vehdjk.com

PHP:  (string) 42; strval(42)
来源：http://sui.guowangkeji.top

JS:   String(42); (42).toString()
来源：http://wct.hnxiangtu.top

TS:   String(42)
来源：http://waf.zhixingplan.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://aac.9152youxi.cn

Go:   strconv.Itoa(42)
来源：http://nrc.shuidangran.top

Ruby: 42.to_s
来源：http://exm.xuanzx.com

C#:   42.ToString()
来源：http://fah.jqgufenzy.top

[A08] 取整与四舍五入
来源：http://abj.pycfn.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://eha.svipenyu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://cfl.vehdjk.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gll.cucudq.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cij.smart0.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://djv.nanxinkj.top


<!-- 参考信息 -->