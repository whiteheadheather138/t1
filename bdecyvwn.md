代发 wailian999

[U51] PHP：数组解构
来源：http://ynp.ehwqpu.com

[$a, $b] = $arr;
来源：http://zvo.yonumen.top

[U52] PHP：箭头函数
来源：http://xpd.bbcook.cn

$double = fn($x) => $x * 2;
来源：http://oeu.chenlongwang.top

[U53] PHP：空合并运算符
来源：http://eqj.dashuyun.cn

$v = $a ?? $b ?? "default";
来源：http://fdz.hongshengwenyu.top

[U54] PHP：空安全调用
来源：http://qap.9152youxi.cn

$obj?->method()
来源：http://pkg.hcnkem.com

[U55] PHP：match 表达式
来源：http://nju.jianghu66.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ytp.zhengqikj.top

[U56] PHP：命名参数
来源：http://tww.pengpengdd.cyou

f(a: 1, b: 2)
来源：http://qpe.ywan-chungtsiang.top

[U57] PHP：字符串插值
来源：http://oat.zdqjudy.top

"值: {$a}"
来源：http://mha.zhixingplan.top

[U58] PHP：数组三件套
来源：http://sct.bbcook.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qop.zhijiandao.cn

[U59] PHP：自定义排序
来源：http://oih.bbcook.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mko.ydjk.org.cn

[U60] PHP：JSON 编解码
来源：http://ayw.zhongyouzk.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://utu.redwolf501.top

[U61] PHP：正则
来源：http://gsh.nanxinkj.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sca.jiagoushi.top

[U62] PHP：日期对象
来源：http://jjr.zhengqikj.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jdm.yuanzhike.top

[U63] PHP：文件读写
来源：http://rcx.shzxlz.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bvj.zhixingplan.top

[U64] PHP：目录遍历
来源：http://sjg.nwbrower.top

glob("dir/*.php");  scandir("dir");
来源：http://zqs.zhijiandao.cn

[U65] PHP：会话
来源：http://qmx.zhaomingkeji.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://ojr.vqdsnc.cn

[U66] PHP：设置 Cookie
来源：http://byf.shzxlz.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zod.cqqwz.cn

[U67] PHP：处理文件上传
来源：http://awe.0kj1m.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yze.yuanzhike.top

[U68] PHP：PDO 连接
来源：http://sjo.c1oappe.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cmw.jianghu66.top

[U69] PHP：PDO 预处理
来源：http://cys.c1oappe.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vmk.iojbl.cn

[U70] PHP：PDO 事务
来源：http://qkn.yuanzhike.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xxm.ydjk.org.cn

[U71] PHP：抛出异常
来源：http://vvf.birdmap.top

throw new RuntimeException("失败", 500);
来源：http://add.zhengqikj.top

[U72] PHP：写错误日志
来源：http://lhp.jlsjyb.cn

error_log("失败: " . $e->getMessage());
来源：http://dzc.birdmap.top

[U73] PHP：读取 ini 配置
来源：http://sgi.zdbjq.cn

parse_ini_file("config.ini", true)
来源：http://ncj.andypj.xyz

[U74] PHP：读取环境变量
来源：http://vap.hysaishi.cn

getenv("APP_ENV") ?: "production"
来源：http://obx.mhx1999.top

[U75] PHP：依赖注入
来源：http://bmp.hnxiangtu.top

composer require psr/container
来源：http://vre.daria6918.cn

[U76] PHP：简单路由
来源：http://hrr.shangyingyoupin.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://adv.yueranfly.top

[U77] PHP：模板渲染
来源：http://pcu.epnwcf.com

composer require twig/twig
来源：http://juh.gzhubu.top

[U78] PHP：单元测试
来源：http://vgd.sweek.top

composer require --dev phpunit/phpunit
来源：http://ojt.fengsongda.top

[U79] PHP：静态分析
来源：http://wyt.gzhubu.top

composer require --dev phpstan/phpstan
来源：http://wyo.birdmap.top

[U80] PHP：代码规范修复
来源：http://knr.ybcxt.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://rpy.ydjk.org.cn

[U81] JS：初始化项目
来源：http://byv.c1oappe.top

npm init -y;  npm i express
来源：http://wcj.hongshengwenyu.top

[U82] JS：package.json 脚本
来源：http://jaf.hnqzz.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fbs.zhixingplan.top

[U83] JS：ES Module 导入导出
来源：http://bxd.quarkkingdee.top

export const a = 1;  import { a } from "./m.js";
来源：http://jza.fehbvm.com

[U84] JS：CommonJS 写法
来源：http://vlv.ppjwa.cn

module.exports = { a };  const { a } = require("./m");
来源：http://njj.tarul.cn

[U85] JS：可选链
来源：http://kuk.sufxvd.cn

a?.b?.c
来源：http://tja.ybcxt.top

[U86] JS：空值合并
来源：http://poe.jlsjyb.cn

a ?? b
来源：http://lug.hongshengwenyu.top

[U87] JS：解构默认值
来源：http://pdt.meibo888.top

const { a = 1, b = 2 } = obj;
来源：http://whq.jqgufenzy.top

[U88] JS：对象展开合并
来源：http://xnq.guannengcc.top

{ ...a, ...b }
来源：http://usd.daria6918.cn

[U89] JS：数组去重
来源：http://hrm.jiagoushi.top

[...new Set(arr)]
来源：http://jzb.yanxiufei.cn

[U90] JS：数字数组排序
来源：http://pvs.svipenyu.cn

[...arr].sort((a, b) => a - b)
来源：http://zjl.nanxinkj.top

[U91] JS：对象键值遍历
来源：http://usa.yueranfly.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ezi.shanyushiyangtech.top

[U92] JS：深拷贝
来源：http://hki.xylfe.cn

structuredClone(obj)
来源：http://bmb.nanxuanxn.top

[U93] JS：模板字符串
来源：http://ynl.ywan-chungtsiang.top

`共 ${n} 条`
来源：http://ngd.fzhhl.top

[U94] JS：箭头函数
来源：http://ziq.zhongyouzk.top

const double = x => x * 2;
来源：http://aoe.ehwqpu.com

[U95] JS：Promise 包装
来源：http://ter.c1oappe.top

new Promise((resolve, reject) => {})
来源：http://nsn.9152youxi.cn

[U96] JS：async/await 与异常
来源：http://gmt.yuanzhike.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gnd.yongpay.top

[U97] JS：并发请求
来源：http://cnh.iojbl.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://epl.jqgfzy.top

[U98] JS：fetch 带 JSON
来源：http://ycs.9152youxi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zgh.xuetiantiany.cn

[U99] JS：事件监听
来源：http://bqc.epnwcf.com

el.addEventListener("click", e => {})
来源：http://qoh.tian-w.cn

[U100] JS：DOM 查询
来源：http://oqz.chenlongwang.top

document.querySelector(".item")
来源：http://szl.shanyushiyangkeji.top

[U101] JS：classList 操作
来源：http://jcn.shzxlz.cn

el.classList.toggle("active")
来源：http://uuf.zhijiandao.cn

[U102] JS：本地存储
来源：http://cky.cashguo.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ngs.feifeiyinyue.top

[U103] JS：定时器
来源：http://dwa.gaohongyu789.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bxi.yj20258888.top

[U104] JS：防抖
来源：http://pxl.hesvh.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aap.0kj1m.cn

[U105] JS：节流
来源：http://txe.xziqi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mut.xziqi.cn

[U106] JS：日期格式化
来源：http://cyc.guannengcc.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://iiz.xingfuxueyuan.xyz

[U107] JS：数字千分位
来源：http://vyb.hysaishi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mug.snrcjt.cn

[U108] JS：随机整数
来源：http://ajk.0kj1m.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rba.ydjk.org.cn

[U109] JS：数组分组
来源：http://ivh.nanxuanxn.top

Object.groupBy(arr, x => x.type)
来源：http://dcw.aizwys.cn

[U110] JS：数组分块
来源：http://xzp.ydzc1.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vgs.sufxvd.cn

[U111] JS：对象转 Map
来源：http://kjd.cheryme.top

new Map(Object.entries(obj))
来源：http://ubm.andypj.xyz

[U112] JS：字符串补位
来源：http://kas.ppjwa.cn

"7".padStart(3, "0")
来源：http://hor.haohaochexian.top

[U113] JS：正则替换全部
来源：http://zev.haohaochexian.top

s.replaceAll("a", "b")
来源：http://qnv.chenlongwang.top

[U114] JS：JSON 深比较
来源：http://blq.vqdsnc.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://rrn.nanxuanxn.top

[U115] JS：生成 UUID
来源：http://wtr.zhoulong.xyz

crypto.randomUUID()
来源：http://kdl.bjfxy.top

[U116] JS：类型检查（JSDoc）
来源：http://ctl.mhx1999.top

/** @param {string} name */ function f(name) {}
来源：http://gha.gzhubu.top

[U117] JS：单元测试
来源：http://pdx.cucudq.cn

npm i -D vitest;  npx vitest
来源：http://hhc.guowangkeji.top

[U118] JS：开发服务器
来源：http://ege.snrcjt.cn

npm i -D vite;  npx vite
来源：http://ycs.hnxiangtu.top

[U119] JS：生产构建
来源：http://fkc.cqqwz.cn

npx vite build
来源：http://sms.hfpthk.cn

[U120] JS：读取环境变量（Vite）
来源：http://dcs.tarul.cn

import.meta.env.VITE_API_URL
来源：http://ibx.xuanzx.com

================================================================================
来源：http://bak.meibo888.top

统计汇总
来源：http://ixx.yj20258888.top

================================================================================
来源：http://jma.yueranfly.top

按语言统计（条）：
来源：http://lmc.daria6918.cn

Python ......... 252
来源：http://tnt.hammf.cn

PHP ............ 252
来源：http://clw.jqgufenzy.top

JavaScript ..... 252
来源：http://bbw.nanxinkj.top

TypeScript ..... 212
来源：http://lmt.shanyushiyangtech.top

Java ........... 212
来源：http://jjh.zdqjudy.top

Go ............. 212
来源：http://egy.vqdsnc.cn

Ruby ........... 212
来源：http://cgo.snrcjt.cn

C# ............. 212
来源：http://lmn.sjlbkw.cn

C .............. 30
来源：http://qjr.hnqzz.top

C++ ............ 30
来源：http://arl.zycfv.cn

SQL ............ 90
来源：http://pbb.xziqi.cn

Bash ........... 80
来源：http://tck.shzxlz.cn

Kotlin ......... 15
来源：http://gzi.jlsjyb.cn

Swift .......... 15
来源：http://inr.shanyushiyangkeji.top

Lua ............ 10
来源：http://fxz.fktsv.cn

Perl ........... 10
来源：http://tuw.jiagoushi.top

Scala .......... 10
来源：http://gcw.andypj.xyz

------------------------------------
来源：http://eil.ivvv.top

合计 ........... 2106 条
来源：http://ilq.c1oappe.top

按章节统计：
来源：http://ksh.fanxiaobao.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cjm.sysykeji.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://asg.shangyingyoupin.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uqp.jinyuanbaomall.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://imn.yj20258888.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dtw.hammf.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qfm.yueranfly.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ltj.chenlongwang.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jba.cucudq.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rnb.hammf.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qmv.kuanghao11.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dgh.316326.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://duf.snrcjt.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://czg.shangyingyoupin.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qad.xylfe.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ces.jlsjyb.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://exy.zycfv.cn

Q SQL 专题                              90
来源：http://vra.daria6918.cn

R Bash 专题                             80
来源：http://nop.ybcxt.top

S C / C++ 专题                          60
来源：http://eyg.ivvv.top

T 其他语言补充                          60
来源：http://mwp.redwolf501.top

U 高频实用片段                         120
来源：http://mmk.bbcook.cn

------------------------------------
来源：http://uvs.chenjidiqi.icu

合计                                  2106 条
来源：http://ijx.quarkkingdee.top

--------------------------------------------------------------------------------
来源：http://qlj.xuanzx.com

使用提醒
来源：http://inj.cashguo.top

--------------------------------------------------------------------------------
来源：http://lhp.hywenlv.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cyw.yuanzhike.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kbv.yanxiufei.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mxv.fanxiaobao.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://onz.jianghu66.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://azq.c1oappe.top

—— 文件结束 ——
来源：http://aee.vehdjk.com

================================================================================
来源：http://ftw.hysaishi.cn

程序语言常见例子速查手册（2024 版）
来源：http://cpf.cashguo.top

Common Programming Examples Cheat Book
来源：http://yxn.zhiwuduotai.top

================================================================================
来源：http://edk.zhijiandao.cn

【收录内容】
来源：http://fnx.yueranfly.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://qap.ywan-chungtsiang.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://shm.zdqjudy.top

SQL · Bash · C · C++
来源：http://jkz.jlsjyb.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://owi.xylfe.cn

【使用说明】
来源：http://rbs.havefunace.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tpu.fengsongda.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ldo.yj20258.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://npl.iojbl.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://aqg.redwolf501.top

Bash:  Shell         C:     C             C++:   C++
来源：http://lpb.tanke756.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kzb.nanxinkj.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gwx.feifeiyinyue.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lbb.hfpthk.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://emw.xinyue.icu

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jgu.hfpthk.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://eba.yfazqb.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dss.zdqjudy.top

【文件统计】
来源：http://zni.316326.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://trb.bbcook.cn

--------------------------------------------------------------------------------
来源：http://lyh.zhongyouzk.top

目  录
来源：http://dsm.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://lba.yueranfly.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://edh.gaohongyu789.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hxj.vqdsnc.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fbw.tianlin.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://efc.yanxiufei.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vjh.316326.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://dms.dianchejie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ayw.hesvh.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bjh.shuidangran.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://pmm.zhongyouzk.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gzk.bjfxy.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gpo.fktsv.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qlq.zhengqikj.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ebs.yuanzhike.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tpd.0kj1m.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ijw.gaohongyu789.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://smy.shanyushiyangtech.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://yhx.jinqigfzy.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://mvp.zhengqikj.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ohz.52xcode.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tqb.jinghuilouyu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qzb.jinqigfzy.top

================================================================================
来源：http://trq.havefunace.top

A. 基础语法与类型
来源：http://rmi.wangdashe.top

================================================================================
来源：http://mca.shuidangran.top

[A01] Hello World
来源：http://ctf.9152youxi.cn

Py:   print("Hello, World!")
来源：http://onv.andypj.xyz

PHP:  echo "Hello, World!";
来源：http://ktl.quarkkingdee.top

JS:   console.log("Hello, World!");
来源：http://xvc.nanxuanxn.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hfs.yongpay.top

Java: System.out.println("Hello, World!");
来源：http://enb.meibo888.top

Go:   fmt.Println("Hello, World!")
来源：http://lcj.ehwqpu.com

Ruby: puts "Hello, World!"
来源：http://slo.iojbl.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://olm.gotoacloud.top

[A02] 变量声明与赋值
来源：http://sxx.wangdashe.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dex.epnwcf.com

PHP:  $name = "Alex"; $age = 20;
来源：http://btv.haohaochexian.top

JS:   let name = "Alex"; const age = 20;
来源：http://orw.svipenyu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://odg.yvedp.cn

Java: String name = "Alex"; int age = 20;
来源：http://tzn.pengpengdd.cyou

Go:   name := "Alex"; age := 20
来源：http://fpq.zhongyouzk.top

Ruby: name = "Alex"; age = 20
来源：http://snv.uphjek.com

C#:   string name = "Alex"; int age = 20;
来源：http://sja.havefunace.top

[A03] 常量定义
来源：http://fas.ivvv.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ejw.shzxlz.cn

PHP:  const PI = 3.14159;
来源：http://izw.meibo888.top

JS:   const PI = 3.14159;
来源：http://scs.yfazqb.com

TS:   const PI: number = 3.14159;
来源：http://qmk.birdmap.top

Java: static final double PI = 3.14159;
来源：http://coz.yj20258888.top

Go:   const PI = 3.14159
来源：http://eur.yueranfly.top

Ruby: PI = 3.14159
来源：http://xjv.ydzc1.top

C#:   const double PI = 3.14159;
来源：http://cjy.fehbvm.com

[A04] 判断变量类型
来源：http://pay.hammf.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://zqf.zhoulong.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://aqg.xuanzx.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blg.dashuyun.cn

TS:   typeof x; x instanceof Date
来源：http://ept.guannengcc.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://igv.meibo888.top

Go:   reflect.TypeOf(x).Name()
来源：http://jph.zhiwuduotai.top

Ruby: x.class; x.is_a?(Integer)
来源：http://lrk.yangfankeji.com

C#:   x.GetType().Name; x is int
来源：http://awc.wangshuangyany.cn

[A05] 整数除法与取模
来源：http://zok.fktsv.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cct.yj202588.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://fco.xuetiantiany.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://enh.yonumen.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://uaq.hnqzz.top

Java: 7 / 2; 7 % 2
来源：http://udj.c1oappe.top

Go:   7 / 2; 7 % 2
来源：http://mxx.kuanghao11.cn

Ruby: 7 / 2; 7 % 2
来源：http://bof.chenzaomai.com

C#:   7 / 2; 7 % 2
来源：http://ddr.dianchejie.cn

[A06] 字符串转数字
来源：http://peq.fengsongda.top

Py:   int("42"); float("3.14")
来源：http://hmc.jinghuilouyu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mum.0kj1m.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://haw.sysykeji.top

TS:   parseInt("42", 10); Number("42")
来源：http://giv.shuidangran.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fvp.smart0.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zul.yj20258888.top

Ruby: "42".to_i; "3.14".to_f
来源：http://dga.cdnleiting.top


<!-- 参考信息 -->