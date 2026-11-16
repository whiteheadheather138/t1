代发 wailian999

[U51] PHP：数组解构
来源：http://uvi.xuanzx.com

[$a, $b] = $arr;
来源：http://ppt.ydzc1.top

[U52] PHP：箭头函数
来源：http://wuj.chenlongwang.top

$double = fn($x) => $x * 2;
来源：http://gpq.yuanzhike.top

[U53] PHP：空合并运算符
来源：http://luv.fengsongda.top

$v = $a ?? $b ?? "default";
来源：http://xis.cashguo.top

[U54] PHP：空安全调用
来源：http://qwu.ydzc1.top

$obj?->method()
来源：http://zjt.fktsv.cn

[U55] PHP：match 表达式
来源：http://chh.mhx1999.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gth.uphjek.com

[U56] PHP：命名参数
来源：http://wtv.fktsv.cn

f(a: 1, b: 2)
来源：http://egx.guannengcc.top

[U57] PHP：字符串插值
来源：http://kkk.daria6918.cn

"值: {$a}"
来源：http://trd.cqqwz.cn

[U58] PHP：数组三件套
来源：http://oxm.redwolf501.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qyt.shanyushiyangkeji.top

[U59] PHP：自定义排序
来源：http://yru.guannengcc.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bfe.shangyingyoupin.top

[U60] PHP：JSON 编解码
来源：http://xsn.aizwys.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fyx.yj202588.top

[U61] PHP：正则
来源：http://yoz.jinqigfzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pyd.hywenlv.cn

[U62] PHP：日期对象
来源：http://mpe.shanyushiyangkeji.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jnt.fktsv.cn

[U63] PHP：文件读写
来源：http://fzc.tanke756.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sey.shuidangran.top

[U64] PHP：目录遍历
来源：http://ied.zhengqikj.top

glob("dir/*.php");  scandir("dir");
来源：http://dlv.9152youxi.cn

[U65] PHP：会话
来源：http://qoe.zycfv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rrm.tarul.cn

[U66] PHP：设置 Cookie
来源：http://oki.vehdjk.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sar.gotoacloud.top

[U67] PHP：处理文件上传
来源：http://sdw.ydjk.org.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://olu.ydjk.org.cn

[U68] PHP：PDO 连接
来源：http://vpa.hcnkem.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://spg.ywan-chungtsiang.top

[U69] PHP：PDO 预处理
来源：http://ojm.nanxuanxn.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cdz.jqgufenzy.top

[U70] PHP：PDO 事务
来源：http://nvu.aizwys.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gob.jqgfzy.top

[U71] PHP：抛出异常
来源：http://poe.shzxlz.cn

throw new RuntimeException("失败", 500);
来源：http://uzx.52xcode.cn

[U72] PHP：写错误日志
来源：http://wdp.shanyushiyangkeji.top

error_log("失败: " . $e->getMessage());
来源：http://rrr.guannengcc.top

[U73] PHP：读取 ini 配置
来源：http://hrs.jinghuilouyu.cn

parse_ini_file("config.ini", true)
来源：http://kwl.yvedp.cn

[U74] PHP：读取环境变量
来源：http://itw.zycfv.cn

getenv("APP_ENV") ?: "production"
来源：http://brj.sweek.top

[U75] PHP：依赖注入
来源：http://rar.fehbvm.com

composer require psr/container
来源：http://jxz.shanyushiyangtech.top

[U76] PHP：简单路由
来源：http://zad.haohaochexian.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pws.tarul.cn

[U77] PHP：模板渲染
来源：http://yvo.hongshengwenyu.top

composer require twig/twig
来源：http://mjm.nanxinkj.top

[U78] PHP：单元测试
来源：http://rcj.zhengqikj.top

composer require --dev phpunit/phpunit
来源：http://ghu.yuanzhike.top

[U79] PHP：静态分析
来源：http://bhe.birdmap.top

composer require --dev phpstan/phpstan
来源：http://ztv.ydzc1.top

[U80] PHP：代码规范修复
来源：http://zps.shanyushiyangkeji.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://lvq.ivvv.top

[U81] JS：初始化项目
来源：http://uzr.cashguo.top

npm init -y;  npm i express
来源：http://ppf.fanxiaobao.xyz

[U82] JS：package.json 脚本
来源：http://yjl.ydzc1.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ele.yj202588.top

[U83] JS：ES Module 导入导出
来源：http://upk.hcnkem.com

export const a = 1;  import { a } from "./m.js";
来源：http://lqm.tanke756.top

[U84] JS：CommonJS 写法
来源：http://xtg.zhixingplan.top

module.exports = { a };  const { a } = require("./m");
来源：http://mko.havefunace.top

[U85] JS：可选链
来源：http://qng.0kj1m.cn

a?.b?.c
来源：http://ghp.sufxvd.cn

[U86] JS：空值合并
来源：http://yjt.yongpay.top

a ?? b
来源：http://ozq.cucudq.cn

[U87] JS：解构默认值
来源：http://uil.316326.xyz

const { a = 1, b = 2 } = obj;
来源：http://nuh.vqdsnc.cn

[U88] JS：对象展开合并
来源：http://zwo.fehbvm.com

{ ...a, ...b }
来源：http://kks.zhaomingkeji.xyz

[U89] JS：数组去重
来源：http://yqp.sxryk.cn

[...new Set(arr)]
来源：http://cll.fktsv.cn

[U90] JS：数字数组排序
来源：http://ime.chenzaomai.com

[...arr].sort((a, b) => a - b)
来源：http://enm.yangfankeji.com

[U91] JS：对象键值遍历
来源：http://jud.yuanzhike.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lsa.uphjek.com

[U92] JS：深拷贝
来源：http://omk.daria6918.cn

structuredClone(obj)
来源：http://etr.ivvv.top

[U93] JS：模板字符串
来源：http://ige.shanyushiyangtech.top

`共 ${n} 条`
来源：http://itd.fzhhl.top

[U94] JS：箭头函数
来源：http://xqi.shangyingyoupin.top

const double = x => x * 2;
来源：http://iqo.dianchejie.cn

[U95] JS：Promise 包装
来源：http://ndw.gaohongyu789.top

new Promise((resolve, reject) => {})
来源：http://wbp.zhongyouzk.top

[U96] JS：async/await 与异常
来源：http://psl.wangdashe.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://eop.redwolf501.top

[U97] JS：并发请求
来源：http://oix.uphjek.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://ecq.ctjpmb.com

[U98] JS：fetch 带 JSON
来源：http://dvn.xinyue.icu

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vrt.ydzc1.top

[U99] JS：事件监听
来源：http://fyb.cqqwz.cn

el.addEventListener("click", e => {})
来源：http://xdx.yonumen.top

[U100] JS：DOM 查询
来源：http://nkb.yfazqb.com

document.querySelector(".item")
来源：http://lvs.shangyingyoupin.top

[U101] JS：classList 操作
来源：http://hkl.bjfxy.top

el.classList.toggle("active")
来源：http://slo.shzxlz.cn

[U102] JS：本地存储
来源：http://xzi.zdqjudy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ach.yonumen.top

[U103] JS：定时器
来源：http://mhh.daria6918.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://otq.shuidangran.top

[U104] JS：防抖
来源：http://yox.yongpay.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iqa.zdbjq.cn

[U105] JS：节流
来源：http://stx.hesvh.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://scm.cucudq.cn

[U106] JS：日期格式化
来源：http://gdg.nanxinkj.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qxh.yj20258888.top

[U107] JS：数字千分位
来源：http://uvl.sufxvd.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pei.shanyushiyangkeji.top

[U108] JS：随机整数
来源：http://lib.ctjpmb.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zek.guowangkeji.top

[U109] JS：数组分组
来源：http://uji.hywenlv.cn

Object.groupBy(arr, x => x.type)
来源：http://uwi.feifeiyinyue.top

[U110] JS：数组分块
来源：http://gpk.nanxinkj.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hzc.chenjidiqi.icu

[U111] JS：对象转 Map
来源：http://knu.quarkkingdee.top

new Map(Object.entries(obj))
来源：http://thg.pycfn.com

[U112] JS：字符串补位
来源：http://lgv.zhixingplan.top

"7".padStart(3, "0")
来源：http://qqo.xuetiantiany.cn

[U113] JS：正则替换全部
来源：http://mei.yuxming.cn

s.replaceAll("a", "b")
来源：http://fzw.tianlin.xyz

[U114] JS：JSON 深比较
来源：http://bfl.dianchejie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://zho.xuanzx.com

[U115] JS：生成 UUID
来源：http://nok.shangyingyoupin.top

crypto.randomUUID()
来源：http://kie.havefunace.top

[U116] JS：类型检查（JSDoc）
来源：http://rfk.aizwys.cn

/** @param {string} name */ function f(name) {}
来源：http://tya.yfazqb.com

[U117] JS：单元测试
来源：http://wxv.zhijiandao.cn

npm i -D vitest;  npx vitest
来源：http://crs.xuetiantiany.cn

[U118] JS：开发服务器
来源：http://lby.gzhubu.top

npm i -D vite;  npx vite
来源：http://qhw.ehwqpu.com

[U119] JS：生产构建
来源：http://zqy.wangdashe.top

npx vite build
来源：http://jxk.hywenlv.cn

[U120] JS：读取环境变量（Vite）
来源：http://nth.0kj1m.cn

import.meta.env.VITE_API_URL
来源：http://scq.cashguo.top

================================================================================
来源：http://xhm.sxryk.cn

统计汇总
来源：http://ole.iojbl.cn

================================================================================
来源：http://tcj.jlsjyb.cn

按语言统计（条）：
来源：http://dih.shanyushiyangkeji.top

Python ......... 252
来源：http://jvc.wangshuangyany.cn

PHP ............ 252
来源：http://pah.tianlin.xyz

JavaScript ..... 252
来源：http://rrk.jqgfzy.top

TypeScript ..... 212
来源：http://mnl.ybcxt.top

Java ........... 212
来源：http://uhj.wangdashe.top

Go ............. 212
来源：http://thk.hesvh.cn

Ruby ........... 212
来源：http://gjp.cucudq.cn

C# ............. 212
来源：http://zwo.aizwys.cn

C .............. 30
来源：http://hgp.fzhhl.top

C++ ............ 30
来源：http://tdv.cheryme.top

SQL ............ 90
来源：http://kfb.cdnleiting.top

Bash ........... 80
来源：http://kud.ywan-chungtsiang.top

Kotlin ......... 15
来源：http://gud.gotoacloud.top

Swift .......... 15
来源：http://kuo.yanxiufei.cn

Lua ............ 10
来源：http://tku.nwbrower.top

Perl ........... 10
来源：http://sdb.tianlin.xyz

Scala .......... 10
来源：http://xyy.smart0.xyz

------------------------------------
来源：http://gcd.snrcjt.cn

合计 ........... 2106 条
来源：http://rlk.gotoacloud.top

按章节统计：
来源：http://ktc.quarkkingdee.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xkg.shangyingyoupin.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dwa.sjlbkw.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gnd.shzxlz.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fof.zhijiandao.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ere.birdmap.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://etz.zhijiandao.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lar.yueranfly.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fxg.ybcxt.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gqh.feifeiyinyue.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cqi.feifeiyinyue.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://azt.shanyushiyangtech.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://coj.pengpengdd.cyou

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rae.xuetiantiany.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pim.pengpengdd.cyou

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pid.sufxvd.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://pjl.fengsongda.top

Q SQL 专题                              90
来源：http://jre.sxryk.cn

R Bash 专题                             80
来源：http://zfi.c1oappe.top

S C / C++ 专题                          60
来源：http://eea.hfpthk.cn

T 其他语言补充                          60
来源：http://euf.zdqjudy.top

U 高频实用片段                         120
来源：http://wom.zhengqikj.top

------------------------------------
来源：http://ihx.316326.xyz

合计                                  2106 条
来源：http://pma.snrcjt.cn

--------------------------------------------------------------------------------
来源：http://dgo.jinghuilouyu.cn

使用提醒
来源：http://fxv.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://jwo.jiagoushi.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://okk.zhiwuduotai.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vxe.c1oappe.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fou.yanxiufei.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://yzu.zhoulong.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pav.feifeiyinyue.top

—— 文件结束 ——
来源：http://txj.jiagoushi.top

================================================================================
来源：http://elq.sweek.top

程序语言常见例子速查手册（2024 版）
来源：http://yuq.yj202588.top

Common Programming Examples Cheat Book
来源：http://apn.yonumen.top

================================================================================
来源：http://sdb.hnxiangtu.top

【收录内容】
来源：http://pyb.zhiwuduotai.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://hyo.jianghu66.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zfd.ppjwa.cn

SQL · Bash · C · C++
来源：http://gxn.nanxuanxn.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ojq.wangshuangyany.cn

【使用说明】
来源：http://nhq.jqgfzy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jgz.dashuyun.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://slt.hesvh.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ogw.hfpthk.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://woz.svipenyu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://muk.zhoulong.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ryn.xuanzx.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wju.zhaomingkeji.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ffv.fanxiaobao.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qgz.sufxvd.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zxl.316326.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ubk.yongpay.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dnq.smart0.xyz

【文件统计】
来源：http://kgb.ppjwa.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://uxa.gaohongyu789.top

--------------------------------------------------------------------------------
来源：http://vlj.zhengqikj.top

目  录
来源：http://ynw.hcnkem.com

--------------------------------------------------------------------------------
来源：http://obm.hongshengwenyu.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wnb.hfpthk.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://sbr.pengpengdd.cyou

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://enk.daxiang520.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://gir.mhx1999.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ree.nwbrower.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://enb.jlsjyb.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://azi.sysykeji.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://lnj.shangyingyoupin.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gvm.cqqwz.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dug.nanxuanxn.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ubr.shzxlz.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://nfg.jianghu66.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ahe.fengsongda.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xjr.jiagoushi.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qer.uphjek.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ncc.xylfe.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fgx.0kj1m.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://yuc.daxiang520.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://dkb.guowangkeji.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lvr.nanxinkj.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ddo.c1oappe.top

================================================================================
来源：http://vnr.sysykeji.top

A. 基础语法与类型
来源：http://bhm.zdqjudy.top

================================================================================
来源：http://dam.jinyuanbaomall.cn

[A01] Hello World
来源：http://abn.havefunace.top

Py:   print("Hello, World!")
来源：http://wta.jinyuanbaomall.cn

PHP:  echo "Hello, World!";
来源：http://buo.hfpthk.cn

JS:   console.log("Hello, World!");
来源：http://ndt.xuanzx.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://psm.yangfankeji.com

Java: System.out.println("Hello, World!");
来源：http://bwy.vqdsnc.cn

Go:   fmt.Println("Hello, World!")
来源：http://vqi.zhiwuduotai.top

Ruby: puts "Hello, World!"
来源：http://jmm.jinghuilouyu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://irl.shanyushiyangkeji.top

[A02] 变量声明与赋值
来源：http://lug.zhaomingkeji.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://lbq.tarul.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://rqx.fengsongda.top

JS:   let name = "Alex"; const age = 20;
来源：http://sst.tanke756.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hxd.yj202588.top

Java: String name = "Alex"; int age = 20;
来源：http://nna.fzhhl.top

Go:   name := "Alex"; age := 20
来源：http://boq.zdbjq.cn

Ruby: name = "Alex"; age = 20
来源：http://vqr.wangshuangyany.cn

C#:   string name = "Alex"; int age = 20;
来源：http://pjn.xuanzx.com

[A03] 常量定义
来源：http://kwt.xinyue.icu

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mhd.jinyuanbaomall.cn

PHP:  const PI = 3.14159;
来源：http://uzp.0kj1m.cn

JS:   const PI = 3.14159;
来源：http://ocu.zhongyouzk.top

TS:   const PI: number = 3.14159;
来源：http://xkf.svipenyu.cn

Java: static final double PI = 3.14159;
来源：http://uia.xuetiantiany.cn

Go:   const PI = 3.14159
来源：http://jum.sjlbkw.cn

Ruby: PI = 3.14159
来源：http://uwm.zycfv.cn

C#:   const double PI = 3.14159;
来源：http://xyy.yuxming.cn

[A04] 判断变量类型
来源：http://wrq.pycfn.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://mee.fanxiaobao.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://cmr.fktsv.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mqq.316326.xyz

TS:   typeof x; x instanceof Date
来源：http://jhh.cashguo.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tlx.ybcxt.top

Go:   reflect.TypeOf(x).Name()
来源：http://axw.jqgufenzy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://thw.dashuyun.cn

C#:   x.GetType().Name; x is int
来源：http://yxn.yanxiufei.cn

[A05] 整数除法与取模
来源：http://rvi.tanke756.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ykj.yvedp.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ysb.yvedp.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mkr.zhijiandao.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://uxh.c1oappe.top

Java: 7 / 2; 7 % 2
来源：http://dey.shuidangran.top

Go:   7 / 2; 7 % 2
来源：http://edj.dianchejie.cn

Ruby: 7 / 2; 7 % 2
来源：http://lwv.shanyushiyangkeji.top

C#:   7 / 2; 7 % 2
来源：http://jyh.tian-w.cn

[A06] 字符串转数字
来源：http://kdd.shuidangran.top

Py:   int("42"); float("3.14")
来源：http://djp.fktsv.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fvs.yangfankeji.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://rhb.nwbrower.top

TS:   parseInt("42", 10); Number("42")
来源：http://dfn.epnwcf.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://yvv.jinghuilouyu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mzp.9152youxi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://nes.jqgfzy.top


<!-- 参考信息 -->