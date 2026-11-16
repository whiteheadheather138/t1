代发 wailian999

[U51] PHP：数组解构
来源：http://vxc.yfazqb.com

[$a, $b] = $arr;
来源：http://wzh.tanke756.top

[U52] PHP：箭头函数
来源：http://kxl.jlsjyb.cn

$double = fn($x) => $x * 2;
来源：http://pgb.shuidangran.top

[U53] PHP：空合并运算符
来源：http://biw.gogol.net.cn

$v = $a ?? $b ?? "default";
来源：http://goh.pycfn.com

[U54] PHP：空安全调用
来源：http://dgt.yangfankeji.com

$obj?->method()
来源：http://bwh.zhixingplan.top

[U55] PHP：match 表达式
来源：http://lpq.hcnkem.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vxp.zhijiandao.cn

[U56] PHP：命名参数
来源：http://jxw.ppjwa.cn

f(a: 1, b: 2)
来源：http://mlv.kuanghao11.cn

[U57] PHP：字符串插值
来源：http://cms.0kj1m.cn

"值: {$a}"
来源：http://cbk.nanxuanxn.top

[U58] PHP：数组三件套
来源：http://srx.52xcode.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://smg.hnqzz.top

[U59] PHP：自定义排序
来源：http://adh.yuxming.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dsq.wangdashe.top

[U60] PHP：JSON 编解码
来源：http://iqi.fehbvm.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hyo.xziqi.cn

[U61] PHP：正则
来源：http://yld.cdnleiting.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://scc.feifeiyinyue.top

[U62] PHP：日期对象
来源：http://fdy.zhengqikj.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qkg.sweek.top

[U63] PHP：文件读写
来源：http://uvq.jianghu66.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dxq.tian-w.cn

[U64] PHP：目录遍历
来源：http://bos.tian-w.cn

glob("dir/*.php");  scandir("dir");
来源：http://myd.jiagoushi.top

[U65] PHP：会话
来源：http://ofw.haohaochexian.top

session_start();  $_SESSION["uid"] = 1;
来源：http://vvn.dianchejie.cn

[U66] PHP：设置 Cookie
来源：http://tuk.shuidangran.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jjp.sjlbkw.cn

[U67] PHP：处理文件上传
来源：http://pwm.uphjek.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gau.52xcode.cn

[U68] PHP：PDO 连接
来源：http://ycn.ywan-chungtsiang.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hjz.shangyingyoupin.top

[U69] PHP：PDO 预处理
来源：http://msg.chenlongwang.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qht.ivvv.top

[U70] PHP：PDO 事务
来源：http://nas.aizwys.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://epm.chenzaomai.com

[U71] PHP：抛出异常
来源：http://bih.yonumen.top

throw new RuntimeException("失败", 500);
来源：http://dum.xuanzx.com

[U72] PHP：写错误日志
来源：http://sxa.gotoacloud.top

error_log("失败: " . $e->getMessage());
来源：http://ddi.gzhubu.top

[U73] PHP：读取 ini 配置
来源：http://wtq.wangshuangyany.cn

parse_ini_file("config.ini", true)
来源：http://smh.daria6918.cn

[U74] PHP：读取环境变量
来源：http://qig.zhaomingkeji.xyz

getenv("APP_ENV") ?: "production"
来源：http://fwp.tianlin.xyz

[U75] PHP：依赖注入
来源：http://tnk.yvedp.cn

composer require psr/container
来源：http://esq.bbcook.cn

[U76] PHP：简单路由
来源：http://wsy.iojbl.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qnx.jqgfzy.top

[U77] PHP：模板渲染
来源：http://cgy.hfpthk.cn

composer require twig/twig
来源：http://ljf.jqgufenzy.top

[U78] PHP：单元测试
来源：http://cjz.yj20258.top

composer require --dev phpunit/phpunit
来源：http://fki.smart0.xyz

[U79] PHP：静态分析
来源：http://sml.xylfe.cn

composer require --dev phpstan/phpstan
来源：http://nhu.jinghuilouyu.cn

[U80] PHP：代码规范修复
来源：http://kdo.redwolf501.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://khf.iojbl.cn

[U81] JS：初始化项目
来源：http://udl.feifeiyinyue.top

npm init -y;  npm i express
来源：http://ivb.zhengqikj.top

[U82] JS：package.json 脚本
来源：http://rhj.ivvv.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://chr.hesvh.cn

[U83] JS：ES Module 导入导出
来源：http://kkv.cucudq.cn

export const a = 1;  import { a } from "./m.js";
来源：http://rea.jqgfzy.top

[U84] JS：CommonJS 写法
来源：http://spa.cashguo.top

module.exports = { a };  const { a } = require("./m");
来源：http://ybk.smart0.xyz

[U85] JS：可选链
来源：http://erc.fzhhl.top

a?.b?.c
来源：http://jxr.xuetiantiany.cn

[U86] JS：空值合并
来源：http://qin.xuanzx.com

a ?? b
来源：http://mgj.hnqzz.top

[U87] JS：解构默认值
来源：http://tku.yuanzhike.top

const { a = 1, b = 2 } = obj;
来源：http://nfq.xuetiantiany.cn

[U88] JS：对象展开合并
来源：http://eqm.daria6918.cn

{ ...a, ...b }
来源：http://vnw.hammf.cn

[U89] JS：数组去重
来源：http://dno.xingfuxueyuan.xyz

[...new Set(arr)]
来源：http://fyy.gzhubu.top

[U90] JS：数字数组排序
来源：http://xaj.zhixingplan.top

[...arr].sort((a, b) => a - b)
来源：http://dgr.chenzaomai.com

[U91] JS：对象键值遍历
来源：http://vle.xylfe.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rfb.smart0.xyz

[U92] JS：深拷贝
来源：http://fqm.nwbrower.top

structuredClone(obj)
来源：http://lqx.shuidangran.top

[U93] JS：模板字符串
来源：http://ogf.jyoumei.cn

`共 ${n} 条`
来源：http://cyw.svipenyu.cn

[U94] JS：箭头函数
来源：http://vlo.mhx1999.top

const double = x => x * 2;
来源：http://tpc.meibo888.top

[U95] JS：Promise 包装
来源：http://rhw.birdmap.top

new Promise((resolve, reject) => {})
来源：http://wby.ydzc1.top

[U96] JS：async/await 与异常
来源：http://bmh.jiagoushi.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qmn.kuanghao11.cn

[U97] JS：并发请求
来源：http://bbf.chenzaomai.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://kng.sjlbkw.cn

[U98] JS：fetch 带 JSON
来源：http://nhl.andypj.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bzp.zhongyouzk.top

[U99] JS：事件监听
来源：http://zsp.nwbrower.top

el.addEventListener("click", e => {})
来源：http://sch.gzhubu.top

[U100] JS：DOM 查询
来源：http://til.fktsv.cn

document.querySelector(".item")
来源：http://vlc.hammf.cn

[U101] JS：classList 操作
来源：http://bjq.shanyushiyangkeji.top

el.classList.toggle("active")
来源：http://lqn.fktsv.cn

[U102] JS：本地存储
来源：http://jwq.jqgufenzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://svx.yvedp.cn

[U103] JS：定时器
来源：http://gyb.316326.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kmw.vqdsnc.cn

[U104] JS：防抖
来源：http://uwq.hywenlv.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rco.tanke756.top

[U105] JS：节流
来源：http://fxb.jyoumei.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zzm.316326.xyz

[U106] JS：日期格式化
来源：http://xse.gogol.net.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mgs.iojbl.cn

[U107] JS：数字千分位
来源：http://fcw.ybcxt.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cjj.jqgfzy.top

[U108] JS：随机整数
来源：http://gen.kuanghao11.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jnt.52xcode.cn

[U109] JS：数组分组
来源：http://akv.jqgfzy.top

Object.groupBy(arr, x => x.type)
来源：http://seq.shangyingyoupin.top

[U110] JS：数组分块
来源：http://sad.fzhhl.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bqo.svipenyu.cn

[U111] JS：对象转 Map
来源：http://yhl.yueranfly.top

new Map(Object.entries(obj))
来源：http://bcx.jinqigfzy.top

[U112] JS：字符串补位
来源：http://cbv.xuetiantiany.cn

"7".padStart(3, "0")
来源：http://wem.fktsv.cn

[U113] JS：正则替换全部
来源：http://cip.chenlongwang.top

s.replaceAll("a", "b")
来源：http://zyr.gaohongyu789.top

[U114] JS：JSON 深比较
来源：http://xse.jqgufenzy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://gyh.ctjpmb.com

[U115] JS：生成 UUID
来源：http://fiq.316326.xyz

crypto.randomUUID()
来源：http://ioj.fzhhl.top

[U116] JS：类型检查（JSDoc）
来源：http://cec.yuxming.cn

/** @param {string} name */ function f(name) {}
来源：http://xdf.cashguo.top

[U117] JS：单元测试
来源：http://erl.ydzc1.top

npm i -D vitest;  npx vitest
来源：http://rcu.jianghu66.top

[U118] JS：开发服务器
来源：http://uml.fanxiaobao.xyz

npm i -D vite;  npx vite
来源：http://bzo.ppjwa.cn

[U119] JS：生产构建
来源：http://djf.gotoacloud.top

npx vite build
来源：http://kob.sjlbkw.cn

[U120] JS：读取环境变量（Vite）
来源：http://ias.yueranfly.top

import.meta.env.VITE_API_URL
来源：http://epd.shangyingyoupin.top

================================================================================
来源：http://fin.gzhubu.top

统计汇总
来源：http://rvt.dianchejie.cn

================================================================================
来源：http://ttg.feifeiyinyue.top

按语言统计（条）：
来源：http://dav.mhx1999.top

Python ......... 252
来源：http://fky.bjfxy.top

PHP ............ 252
来源：http://ulj.pycfn.com

JavaScript ..... 252
来源：http://gyn.daxiang520.top

TypeScript ..... 212
来源：http://nfh.cqqwz.cn

Java ........... 212
来源：http://qad.shangyingyoupin.top

Go ............. 212
来源：http://ygf.bjfxy.top

Ruby ........... 212
来源：http://one.sxryk.cn

C# ............. 212
来源：http://amp.nanxuanxn.top

C .............. 30
来源：http://kam.iojbl.cn

C++ ............ 30
来源：http://eha.shuidangran.top

SQL ............ 90
来源：http://vnl.tarul.cn

Bash ........... 80
来源：http://ylp.zhiwuduotai.top

Kotlin ......... 15
来源：http://zia.shzxlz.cn

Swift .......... 15
来源：http://xcz.vehdjk.com

Lua ............ 10
来源：http://ozd.jinqigfzy.top

Perl ........... 10
来源：http://jqj.yuxming.cn

Scala .......... 10
来源：http://rgh.kuanghao11.cn

------------------------------------
来源：http://pdr.meibo888.top

合计 ........... 2106 条
来源：http://tyb.ppjwa.cn

按章节统计：
来源：http://egc.jinqigufen.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ckh.zhixingplan.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xgl.xylfe.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vau.zhoulong.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://iqz.sjlbkw.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tug.sufxvd.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://aci.316326.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fhy.pycfn.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zvp.zhongyouzk.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nxk.c1oappe.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ocx.sjlbkw.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://atv.iojbl.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://adq.sysykeji.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gir.nwbrower.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qfc.daxiang520.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tej.sufxvd.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lwa.pycfn.com

Q SQL 专题                              90
来源：http://xhp.sweek.top

R Bash 专题                             80
来源：http://lsw.shangyingyoupin.top

S C / C++ 专题                          60
来源：http://azj.jqgfzy.top

T 其他语言补充                          60
来源：http://oky.andypj.xyz

U 高频实用片段                         120
来源：http://wbg.c1oappe.top

------------------------------------
来源：http://ivt.hysaishi.cn

合计                                  2106 条
来源：http://vmm.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://aro.ybcxt.top

使用提醒
来源：http://kiw.hammf.cn

--------------------------------------------------------------------------------
来源：http://dbu.jqgufenzy.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jtz.dianchejie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tke.tanke756.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rku.sufxvd.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ydb.smart0.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://won.haohaochexian.top

—— 文件结束 ——
来源：http://rfk.meibo888.top

================================================================================
来源：http://jwx.gaohongyu789.top

程序语言常见例子速查手册（2024 版）
来源：http://fbc.ppjwa.cn

Common Programming Examples Cheat Book
来源：http://pjk.vehdjk.com

================================================================================
来源：http://egt.ywan-chungtsiang.top

【收录内容】
来源：http://dsm.zdqjudy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://wft.jinyuanbaomall.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ymy.ehwqpu.com

SQL · Bash · C · C++
来源：http://wsa.yvedp.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://omb.jinyuanbaomall.cn

【使用说明】
来源：http://ogg.haohaochexian.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ewh.hammf.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bpd.dashuyun.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xbp.cashguo.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hqc.jiagoushi.top

Bash:  Shell         C:     C             C++:   C++
来源：http://pkk.yj20258.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://yxx.yj20258888.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xtn.snrcjt.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zxv.ywan-chungtsiang.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fhi.ehwqpu.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zfr.yfazqb.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fbf.jinghuilouyu.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zzf.tianlin.xyz

【文件统计】
来源：http://ddj.epnwcf.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cbo.bjfxy.top

--------------------------------------------------------------------------------
来源：http://xye.guowangkeji.top

目  录
来源：http://nfy.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://koz.ehwqpu.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wcd.nwbrower.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://oag.epnwcf.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bor.zdbjq.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rrv.dianchejie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jam.cqqwz.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://imc.jqgfzy.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rdi.ppjwa.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dxf.tian-w.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://knd.chenlongwang.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://put.tian-w.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://uoi.zhijiandao.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kmv.vehdjk.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ezv.ehwqpu.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://utk.nanxinkj.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rfr.zdqjudy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ogk.ybcxt.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vzw.gotoacloud.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://igr.gzhubu.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jmi.xylfe.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fhs.iojbl.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yev.daria6918.cn

================================================================================
来源：http://rsr.pycfn.com

A. 基础语法与类型
来源：http://mnf.shanyushiyangtech.top

================================================================================
来源：http://mpm.redwolf501.top

[A01] Hello World
来源：http://wpf.hammf.cn

Py:   print("Hello, World!")
来源：http://fye.zhengqikj.top

PHP:  echo "Hello, World!";
来源：http://zav.jianghu66.top

JS:   console.log("Hello, World!");
来源：http://krn.hnxiangtu.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ypi.svipenyu.cn

Java: System.out.println("Hello, World!");
来源：http://ecj.shanyushiyangkeji.top

Go:   fmt.Println("Hello, World!")
来源：http://szz.shangyingyoupin.top

Ruby: puts "Hello, World!"
来源：http://fhz.yj20258.top

C#:   Console.WriteLine("Hello, World!");
来源：http://twf.xuanzx.com

[A02] 变量声明与赋值
来源：http://fuq.pengpengdd.cyou

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ari.ywan-chungtsiang.top

PHP:  $name = "Alex"; $age = 20;
来源：http://xbj.shangyingyoupin.top

JS:   let name = "Alex"; const age = 20;
来源：http://skh.yvedp.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://why.zdbjq.cn

Java: String name = "Alex"; int age = 20;
来源：http://zic.uphjek.com

Go:   name := "Alex"; age := 20
来源：http://lgs.zhijiandao.cn

Ruby: name = "Alex"; age = 20
来源：http://wva.hcnkem.com

C#:   string name = "Alex"; int age = 20;
来源：http://ogu.zhixingplan.top

[A03] 常量定义
来源：http://tsi.xuanzx.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kna.ywan-chungtsiang.top

PHP:  const PI = 3.14159;
来源：http://xpy.fehbvm.com

JS:   const PI = 3.14159;
来源：http://gzd.jinqigufen.top

TS:   const PI: number = 3.14159;
来源：http://kno.ppjwa.cn

Java: static final double PI = 3.14159;
来源：http://ejb.hesvh.cn

Go:   const PI = 3.14159
来源：http://aez.uphjek.com

Ruby: PI = 3.14159
来源：http://ixy.uphjek.com

C#:   const double PI = 3.14159;
来源：http://uqh.ydjk.org.cn

[A04] 判断变量类型
来源：http://jsf.hysaishi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://jat.zycfv.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xuy.yvedp.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ctr.xinyue.icu

TS:   typeof x; x instanceof Date
来源：http://ycm.guannengcc.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qjl.epnwcf.com

Go:   reflect.TypeOf(x).Name()
来源：http://kli.iojbl.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://egn.aibaodan.cn

C#:   x.GetType().Name; x is int
来源：http://kvd.nanxinkj.top

[A05] 整数除法与取模
来源：http://ymi.nwbrower.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kmu.bbcook.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://kjy.yj20258888.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jlt.sysykeji.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://foy.guannengcc.top

Java: 7 / 2; 7 % 2
来源：http://lrc.redwolf501.top

Go:   7 / 2; 7 % 2
来源：http://nbz.xinyue.icu

Ruby: 7 / 2; 7 % 2
来源：http://zki.bbcook.cn

C#:   7 / 2; 7 % 2
来源：http://htf.nanxinkj.top

[A06] 字符串转数字
来源：http://ggb.vehdjk.com

Py:   int("42"); float("3.14")
来源：http://bab.hcnkem.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ltd.chenlongwang.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mnb.gotoacloud.top

TS:   parseInt("42", 10); Number("42")
来源：http://oux.zhoulong.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xtr.dianchejie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wqr.zycfv.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://yta.yueranfly.top


<!-- 参考信息 -->