代发 wailian999

[U53] PHP：空合并运算符
来源：http://fus.shuidangran.top

$v = $a ?? $b ?? "default";
来源：http://riw.jianghu66.top

[U54] PHP：空安全调用
来源：http://enr.fehbvm.com

$obj?->method()
来源：http://dlf.xinyue.icu

[U55] PHP：match 表达式
来源：http://ulq.meibo888.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tpu.shangyingyoupin.top

[U56] PHP：命名参数
来源：http://yvj.wangshuangyany.cn

f(a: 1, b: 2)
来源：http://aoj.fanxiaobao.xyz

[U57] PHP：字符串插值
来源：http://dai.tianlin.xyz

"值: {$a}"
来源：http://lqd.52xcode.cn

[U58] PHP：数组三件套
来源：http://cjd.vqdsnc.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jfe.52xcode.cn

[U59] PHP：自定义排序
来源：http://uqs.shangyingyoupin.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zfs.snrcjt.cn

[U60] PHP：JSON 编解码
来源：http://xsv.ctjpmb.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jrd.zhixingplan.top

[U61] PHP：正则
来源：http://ylg.guannengcc.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ccf.mhx1999.top

[U62] PHP：日期对象
来源：http://viw.hammf.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://eso.316326.xyz

[U63] PHP：文件读写
来源：http://uor.hcnkem.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fvu.shanyushiyangtech.top

[U64] PHP：目录遍历
来源：http://ipp.zhaomingkeji.xyz

glob("dir/*.php");  scandir("dir");
来源：http://qkg.fktsv.cn

[U65] PHP：会话
来源：http://zgq.ydjk.org.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://zen.zycfv.cn

[U66] PHP：设置 Cookie
来源：http://adz.daxiang520.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jde.gaohongyu789.top

[U67] PHP：处理文件上传
来源：http://ktt.hysaishi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fnf.shzxlz.cn

[U68] PHP：PDO 连接
来源：http://ial.xuanzx.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://brh.52xcode.cn

[U69] PHP：PDO 预处理
来源：http://off.daria6918.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://drt.jqgufenzy.top

[U70] PHP：PDO 事务
来源：http://vcs.zdbjq.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bau.hfpthk.cn

[U71] PHP：抛出异常
来源：http://ewy.bbcook.cn

throw new RuntimeException("失败", 500);
来源：http://unu.fengsongda.top

[U72] PHP：写错误日志
来源：http://fph.shuidangran.top

error_log("失败: " . $e->getMessage());
来源：http://wsn.hnqzz.top

[U73] PHP：读取 ini 配置
来源：http://tgx.yj20258888.top

parse_ini_file("config.ini", true)
来源：http://cds.sxryk.cn

[U74] PHP：读取环境变量
来源：http://fip.cashguo.top

getenv("APP_ENV") ?: "production"
来源：http://ill.sysykeji.top

[U75] PHP：依赖注入
来源：http://gyb.bbcook.cn

composer require psr/container
来源：http://obn.hcnkem.com

[U76] PHP：简单路由
来源：http://wjv.shuidangran.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://szl.hysaishi.cn

[U77] PHP：模板渲染
来源：http://fgq.sxryk.cn

composer require twig/twig
来源：http://rhq.hcnkem.com

[U78] PHP：单元测试
来源：http://vyk.fktsv.cn

composer require --dev phpunit/phpunit
来源：http://oxw.fzhhl.top

[U79] PHP：静态分析
来源：http://oug.cdnleiting.top

composer require --dev phpstan/phpstan
来源：http://ftw.redwolf501.top

[U80] PHP：代码规范修复
来源：http://dsw.feifeiyinyue.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://zfe.hesvh.cn

[U81] JS：初始化项目
来源：http://arr.jinqigfzy.top

npm init -y;  npm i express
来源：http://hoo.sufxvd.cn

[U82] JS：package.json 脚本
来源：http://cao.nwbrower.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cle.jinqigufen.top

[U83] JS：ES Module 导入导出
来源：http://ylj.ywan-chungtsiang.top

export const a = 1;  import { a } from "./m.js";
来源：http://sua.jinqigfzy.top

[U84] JS：CommonJS 写法
来源：http://eni.jqgfzy.top

module.exports = { a };  const { a } = require("./m");
来源：http://nvk.guannengcc.top

[U85] JS：可选链
来源：http://fjl.zhiwuduotai.top

a?.b?.c
来源：http://oqs.hesvh.cn

[U86] JS：空值合并
来源：http://ezv.gotoacloud.top

a ?? b
来源：http://pgf.birdmap.top

[U87] JS：解构默认值
来源：http://bhb.svipenyu.cn

const { a = 1, b = 2 } = obj;
来源：http://wgw.zhixingplan.top

[U88] JS：对象展开合并
来源：http://ecz.52xcode.cn

{ ...a, ...b }
来源：http://wfr.hnqzz.top

[U89] JS：数组去重
来源：http://hve.smart0.xyz

[...new Set(arr)]
来源：http://fqb.sjlbkw.cn

[U90] JS：数字数组排序
来源：http://kjd.snrcjt.cn

[...arr].sort((a, b) => a - b)
来源：http://sbi.quarkkingdee.top

[U91] JS：对象键值遍历
来源：http://vwn.xuanzx.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qrv.daria6918.cn

[U92] JS：深拷贝
来源：http://qpr.fktsv.cn

structuredClone(obj)
来源：http://rtl.chenlongwang.top

[U93] JS：模板字符串
来源：http://rmd.cheryme.top

`共 ${n} 条`
来源：http://nuv.shanyushiyangkeji.top

[U94] JS：箭头函数
来源：http://ecu.ppjwa.cn

const double = x => x * 2;
来源：http://beg.kuanghao11.cn

[U95] JS：Promise 包装
来源：http://wuu.9152youxi.cn

new Promise((resolve, reject) => {})
来源：http://upj.shuidangran.top

[U96] JS：async/await 与异常
来源：http://dam.hesvh.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ezr.hnqzz.top

[U97] JS：并发请求
来源：http://dqn.yvedp.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://moa.shanyushiyangkeji.top

[U98] JS：fetch 带 JSON
来源：http://jnw.sjlbkw.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jtx.fktsv.cn

[U99] JS：事件监听
来源：http://xkh.cashguo.top

el.addEventListener("click", e => {})
来源：http://jof.birdmap.top

[U100] JS：DOM 查询
来源：http://zjk.yuxming.cn

document.querySelector(".item")
来源：http://dzr.sweek.top

[U101] JS：classList 操作
来源：http://ypy.zhoulong.xyz

el.classList.toggle("active")
来源：http://vch.yongpay.top

[U102] JS：本地存储
来源：http://qty.sysykeji.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://fqy.zhixingplan.top

[U103] JS：定时器
来源：http://fvl.vehdjk.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ncx.zhijiandao.cn

[U104] JS：防抖
来源：http://amt.andypj.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lls.316326.xyz

[U105] JS：节流
来源：http://vrb.jinqigufen.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xbj.hammf.cn

[U106] JS：日期格式化
来源：http://eto.zhijiandao.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sei.hywenlv.cn

[U107] JS：数字千分位
来源：http://ddh.svipenyu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kal.zhaomingkeji.xyz

[U108] JS：随机整数
来源：http://nwe.ybcxt.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://afd.ydjk.org.cn

[U109] JS：数组分组
来源：http://fjb.shangyingyoupin.top

Object.groupBy(arr, x => x.type)
来源：http://ily.cheryme.top

[U110] JS：数组分块
来源：http://vzw.ivvv.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sat.fengsongda.top

[U111] JS：对象转 Map
来源：http://lud.tianlin.xyz

new Map(Object.entries(obj))
来源：http://ikh.yongpay.top

[U112] JS：字符串补位
来源：http://pkq.hfpthk.cn

"7".padStart(3, "0")
来源：http://mpe.yvedp.cn

[U113] JS：正则替换全部
来源：http://hib.guannengcc.top

s.replaceAll("a", "b")
来源：http://mbz.ydjk.org.cn

[U114] JS：JSON 深比较
来源：http://vlq.guowangkeji.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://uww.cucudq.cn

[U115] JS：生成 UUID
来源：http://wnd.xinyue.icu

crypto.randomUUID()
来源：http://uhr.xingfuxueyuan.xyz

[U116] JS：类型检查（JSDoc）
来源：http://znp.yj20258.top

/** @param {string} name */ function f(name) {}
来源：http://luw.guowangkeji.top

[U117] JS：单元测试
来源：http://ece.xylfe.cn

npm i -D vitest;  npx vitest
来源：http://mqj.fehbvm.com

[U118] JS：开发服务器
来源：http://dex.shangyingyoupin.top

npm i -D vite;  npx vite
来源：http://hlu.zhiwuduotai.top

[U119] JS：生产构建
来源：http://tix.yj20258888.top

npx vite build
来源：http://bli.epnwcf.com

[U120] JS：读取环境变量（Vite）
来源：http://yzo.zhixingplan.top

import.meta.env.VITE_API_URL
来源：http://kcv.guowangkeji.top

================================================================================
来源：http://zxi.fengsongda.top

统计汇总
来源：http://fcl.yuxming.cn

================================================================================
来源：http://wgy.cheryme.top

按语言统计（条）：
来源：http://vgi.hysaishi.cn

Python ......... 252
来源：http://lph.xuetiantiany.cn

PHP ............ 252
来源：http://bju.pengpengdd.cyou

JavaScript ..... 252
来源：http://vxc.hnqzz.top

TypeScript ..... 212
来源：http://ndx.daria6918.cn

Java ........... 212
来源：http://jia.zhengqikj.top

Go ............. 212
来源：http://qdz.52xcode.cn

Ruby ........... 212
来源：http://ogz.tanke756.top

C# ............. 212
来源：http://bds.jiagoushi.top

C .............. 30
来源：http://vbv.zhongyouzk.top

C++ ............ 30
来源：http://mnl.hammf.cn

SQL ............ 90
来源：http://odk.meibo888.top

Bash ........... 80
来源：http://lpb.shzxlz.cn

Kotlin ......... 15
来源：http://mcd.gotoacloud.top

Swift .......... 15
来源：http://mjc.hammf.cn

Lua ............ 10
来源：http://scj.sufxvd.cn

Perl ........... 10
来源：http://csk.cucudq.cn

Scala .......... 10
来源：http://ard.chenlongwang.top

------------------------------------
来源：http://lzx.shuidangran.top

合计 ........... 2106 条
来源：http://kef.jinqigufen.top

按章节统计：
来源：http://oqu.pycfn.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pxy.svipenyu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tiv.daria6918.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xgj.tarul.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ieu.fehbvm.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cka.fengsongda.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://puo.zdbjq.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vnf.jyoumei.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zts.fanxiaobao.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ayt.cucudq.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yky.quarkkingdee.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bxa.zhongyouzk.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gkp.andypj.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pjk.andypj.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://iey.jqgufenzy.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mun.zdqjudy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lmc.snrcjt.cn

Q SQL 专题                              90
来源：http://sro.meibo888.top

R Bash 专题                             80
来源：http://wus.sweek.top

S C / C++ 专题                          60
来源：http://egp.tarul.cn

T 其他语言补充                          60
来源：http://toy.xylfe.cn

U 高频实用片段                         120
来源：http://yex.daxiang520.top

------------------------------------
来源：http://tms.jianghu66.top

合计                                  2106 条
来源：http://ryn.nanxuanxn.top

--------------------------------------------------------------------------------
来源：http://fyb.0kj1m.cn

使用提醒
来源：http://tnw.xinyue.icu

--------------------------------------------------------------------------------
来源：http://lbz.meibo888.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lof.yuanzhike.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mbw.wangdashe.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://icj.fktsv.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://jxi.tian-w.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://tyg.shanyushiyangkeji.top

—— 文件结束 ——
来源：http://roc.tian-w.cn

================================================================================
来源：http://rak.9152youxi.cn

程序语言常见例子速查手册（2024 版）
来源：http://rzp.ivvv.top

Common Programming Examples Cheat Book
来源：http://rjz.ydjk.org.cn

================================================================================
来源：http://lnf.aibaodan.cn

【收录内容】
来源：http://gdd.gogol.net.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://tve.wangdashe.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://lek.vqdsnc.cn

SQL · Bash · C · C++
来源：http://rcn.vehdjk.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://egd.hammf.cn

【使用说明】
来源：http://yky.haohaochexian.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://dpg.yj20258.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jds.52xcode.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ket.zhixingplan.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yxe.dianchejie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://tji.yuxming.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ntn.0kj1m.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qyl.hnxiangtu.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://apo.bbcook.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zet.xuanzx.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gws.vqdsnc.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zls.quarkkingdee.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xvp.gaohongyu789.top

【文件统计】
来源：http://tgn.vqdsnc.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tue.wangshuangyany.cn

--------------------------------------------------------------------------------
来源：http://rcx.epnwcf.com

目  录
来源：http://vcu.hfpthk.cn

--------------------------------------------------------------------------------
来源：http://uzk.yanxiufei.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zje.yanxiufei.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rby.fehbvm.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wct.guowangkeji.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bym.jinyuanbaomall.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xii.9152youxi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pbv.shangyingyoupin.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bmh.yvedp.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kty.nwbrower.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ruy.nwbrower.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://uwp.shzxlz.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zbj.nwbrower.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://aao.epnwcf.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://tsr.zhaomingkeji.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://srb.sysykeji.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://iis.zycfv.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zab.yuxming.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bhi.daria6918.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://dfs.zhengqikj.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vkn.sysykeji.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pso.guowangkeji.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://uwh.andypj.xyz

================================================================================
来源：http://hjz.jinqigufen.top

A. 基础语法与类型
来源：http://iyf.tanke756.top

================================================================================
来源：http://fug.fzhhl.top

[A01] Hello World
来源：http://eak.hcnkem.com

Py:   print("Hello, World!")
来源：http://jpb.c1oappe.top

PHP:  echo "Hello, World!";
来源：http://qts.gotoacloud.top

JS:   console.log("Hello, World!");
来源：http://gup.yangfankeji.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cds.fehbvm.com

Java: System.out.println("Hello, World!");
来源：http://xbw.cqqwz.cn

Go:   fmt.Println("Hello, World!")
来源：http://qhu.yongpay.top

Ruby: puts "Hello, World!"
来源：http://vgy.hnxiangtu.top

C#:   Console.WriteLine("Hello, World!");
来源：http://gpr.hammf.cn

[A02] 变量声明与赋值
来源：http://qqs.wangshuangyany.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hke.hongshengwenyu.top

PHP:  $name = "Alex"; $age = 20;
来源：http://hug.jianghu66.top

JS:   let name = "Alex"; const age = 20;
来源：http://yrk.hnqzz.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zgf.jyoumei.cn

Java: String name = "Alex"; int age = 20;
来源：http://osl.jinyuanbaomall.cn

Go:   name := "Alex"; age := 20
来源：http://ggo.52xcode.cn

Ruby: name = "Alex"; age = 20
来源：http://vku.jqgfzy.top

C#:   string name = "Alex"; int age = 20;
来源：http://xrc.redwolf501.top

[A03] 常量定义
来源：http://qer.xuetiantiany.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qdc.tarul.cn

PHP:  const PI = 3.14159;
来源：http://dnl.birdmap.top

JS:   const PI = 3.14159;
来源：http://fna.xingfuxueyuan.xyz

TS:   const PI: number = 3.14159;
来源：http://kcf.zhaomingkeji.xyz

Java: static final double PI = 3.14159;
来源：http://lsb.yvedp.cn

Go:   const PI = 3.14159
来源：http://yrf.yonumen.top

Ruby: PI = 3.14159
来源：http://hpi.tian-w.cn

C#:   const double PI = 3.14159;
来源：http://cms.jyoumei.cn

[A04] 判断变量类型
来源：http://wqq.zhoulong.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://uil.aibaodan.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://oyz.jqgufenzy.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://air.gaohongyu789.top

TS:   typeof x; x instanceof Date
来源：http://qbc.xziqi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://szf.kuanghao11.cn

Go:   reflect.TypeOf(x).Name()
来源：http://pto.ydzc1.top

Ruby: x.class; x.is_a?(Integer)
来源：http://uez.shuidangran.top

C#:   x.GetType().Name; x is int
来源：http://yyq.hfpthk.cn

[A05] 整数除法与取模
来源：http://dzm.xziqi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fia.zdbjq.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://uyu.zhiwuduotai.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ewe.316326.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kfn.0kj1m.cn

Java: 7 / 2; 7 % 2
来源：http://etg.zycfv.cn

Go:   7 / 2; 7 % 2
来源：http://hlo.sweek.top

Ruby: 7 / 2; 7 % 2
来源：http://avw.tarul.cn

C#:   7 / 2; 7 % 2
来源：http://ijy.jinqigfzy.top

[A06] 字符串转数字
来源：http://czr.yvedp.cn

Py:   int("42"); float("3.14")
来源：http://qrs.tianlin.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://azd.snrcjt.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gus.dashuyun.cn

TS:   parseInt("42", 10); Number("42")
来源：http://qmu.kuanghao11.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://yjk.hfpthk.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://uzp.9152youxi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://gst.uphjek.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qcj.jinqigfzy.top

[A07] 数字转字符串
来源：http://lwj.hesvh.cn

Py:   str(42)
来源：http://vzg.chenlongwang.top

PHP:  (string) 42; strval(42)
来源：http://sts.iojbl.cn


<!-- 参考信息 -->