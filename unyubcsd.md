代发 wailian999

[U51] PHP：数组解构
来源：http://eqr.jinqigfzy.top

[$a, $b] = $arr;
来源：http://pkv.52xcode.cn

[U52] PHP：箭头函数
来源：http://boo.pengpengdd.cyou

$double = fn($x) => $x * 2;
来源：http://cgp.nwbrower.top

[U53] PHP：空合并运算符
来源：http://skt.yuanzhike.top

$v = $a ?? $b ?? "default";
来源：http://alf.cqqwz.cn

[U54] PHP：空安全调用
来源：http://aun.fehbvm.com

$obj?->method()
来源：http://vkp.yanxiufei.cn

[U55] PHP：match 表达式
来源：http://klo.xziqi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fow.cheryme.top

[U56] PHP：命名参数
来源：http://cgq.dianchejie.cn

f(a: 1, b: 2)
来源：http://iwa.fengsongda.top

[U57] PHP：字符串插值
来源：http://yro.ppjwa.cn

"值: {$a}"
来源：http://vxn.jiagoushi.top

[U58] PHP：数组三件套
来源：http://zun.shangyingyoupin.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jpj.zycfv.cn

[U59] PHP：自定义排序
来源：http://wet.mhx1999.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qcu.aibaodan.cn

[U60] PHP：JSON 编解码
来源：http://ybh.snrcjt.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jrp.hnqzz.top

[U61] PHP：正则
来源：http://lwx.havefunace.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rej.mhx1999.top

[U62] PHP：日期对象
来源：http://nig.cheryme.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vmi.ydzc1.top

[U63] PHP：文件读写
来源：http://ymr.shangyingyoupin.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ado.daria6918.cn

[U64] PHP：目录遍历
来源：http://ffq.zhongyouzk.top

glob("dir/*.php");  scandir("dir");
来源：http://psd.shzxlz.cn

[U65] PHP：会话
来源：http://ncr.gogol.net.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ffi.zhoulong.xyz

[U66] PHP：设置 Cookie
来源：http://fmt.ehwqpu.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://upv.zhijiandao.cn

[U67] PHP：处理文件上传
来源：http://zcb.hnxiangtu.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cyp.gogol.net.cn

[U68] PHP：PDO 连接
来源：http://wcv.zhiwuduotai.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://csk.sxryk.cn

[U69] PHP：PDO 预处理
来源：http://mhi.fanxiaobao.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://avq.wangshuangyany.cn

[U70] PHP：PDO 事务
来源：http://sqc.yj20258888.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jsi.ctjpmb.com

[U71] PHP：抛出异常
来源：http://rnj.sjlbkw.cn

throw new RuntimeException("失败", 500);
来源：http://exc.redwolf501.top

[U72] PHP：写错误日志
来源：http://ahx.pengpengdd.cyou

error_log("失败: " . $e->getMessage());
来源：http://uvm.fengsongda.top

[U73] PHP：读取 ini 配置
来源：http://dsf.zhijiandao.cn

parse_ini_file("config.ini", true)
来源：http://mqp.dashuyun.cn

[U74] PHP：读取环境变量
来源：http://sdr.52xcode.cn

getenv("APP_ENV") ?: "production"
来源：http://hqx.jianghu66.top

[U75] PHP：依赖注入
来源：http://kwo.shuidangran.top

composer require psr/container
来源：http://xnd.tianlin.xyz

[U76] PHP：简单路由
来源：http://wpp.zhijiandao.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dsa.guowangkeji.top

[U77] PHP：模板渲染
来源：http://bdu.jiagoushi.top

composer require twig/twig
来源：http://ike.fengsongda.top

[U78] PHP：单元测试
来源：http://duo.fzhhl.top

composer require --dev phpunit/phpunit
来源：http://kow.uphjek.com

[U79] PHP：静态分析
来源：http://nuc.jlsjyb.cn

composer require --dev phpstan/phpstan
来源：http://mhn.smart0.xyz

[U80] PHP：代码规范修复
来源：http://ncl.yj202588.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://boh.jinqigufen.top

[U81] JS：初始化项目
来源：http://sjz.xingfuxueyuan.xyz

npm init -y;  npm i express
来源：http://uod.yanxiufei.cn

[U82] JS：package.json 脚本
来源：http://sir.jiagoushi.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dif.birdmap.top

[U83] JS：ES Module 导入导出
来源：http://qnx.hnqzz.top

export const a = 1;  import { a } from "./m.js";
来源：http://phl.jiagoushi.top

[U84] JS：CommonJS 写法
来源：http://jxz.zhiwuduotai.top

module.exports = { a };  const { a } = require("./m");
来源：http://jus.jiagoushi.top

[U85] JS：可选链
来源：http://vnd.xziqi.cn

a?.b?.c
来源：http://wna.xziqi.cn

[U86] JS：空值合并
来源：http://hvg.guannengcc.top

a ?? b
来源：http://xij.hywenlv.cn

[U87] JS：解构默认值
来源：http://jbu.tian-w.cn

const { a = 1, b = 2 } = obj;
来源：http://vkw.svipenyu.cn

[U88] JS：对象展开合并
来源：http://aaf.yuxming.cn

{ ...a, ...b }
来源：http://uth.shanyushiyangtech.top

[U89] JS：数组去重
来源：http://csa.cucudq.cn

[...new Set(arr)]
来源：http://pfr.c1oappe.top

[U90] JS：数字数组排序
来源：http://oey.meibo888.top

[...arr].sort((a, b) => a - b)
来源：http://wtb.sweek.top

[U91] JS：对象键值遍历
来源：http://azo.sjlbkw.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://htb.yonumen.top

[U92] JS：深拷贝
来源：http://uul.tianlin.xyz

structuredClone(obj)
来源：http://gsc.jianghu66.top

[U93] JS：模板字符串
来源：http://xmx.yonumen.top

`共 ${n} 条`
来源：http://hwx.andypj.xyz

[U94] JS：箭头函数
来源：http://uhi.hfpthk.cn

const double = x => x * 2;
来源：http://xpj.shanyushiyangtech.top

[U95] JS：Promise 包装
来源：http://qve.jinghuilouyu.cn

new Promise((resolve, reject) => {})
来源：http://fho.jinghuilouyu.cn

[U96] JS：async/await 与异常
来源：http://woj.jinyuanbaomall.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wvy.xuetiantiany.cn

[U97] JS：并发请求
来源：http://qrm.dashuyun.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rnv.xingfuxueyuan.xyz

[U98] JS：fetch 带 JSON
来源：http://znc.zhoulong.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sqa.hywenlv.cn

[U99] JS：事件监听
来源：http://nrx.havefunace.top

el.addEventListener("click", e => {})
来源：http://tjk.zhixingplan.top

[U100] JS：DOM 查询
来源：http://rgv.wangdashe.top

document.querySelector(".item")
来源：http://lph.hammf.cn

[U101] JS：classList 操作
来源：http://owm.yueranfly.top

el.classList.toggle("active")
来源：http://vjh.zhijiandao.cn

[U102] JS：本地存储
来源：http://ray.sysykeji.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://gha.cheryme.top

[U103] JS：定时器
来源：http://tqr.hysaishi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dhc.hnqzz.top

[U104] JS：防抖
来源：http://eim.vqdsnc.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pii.guannengcc.top

[U105] JS：节流
来源：http://utr.guannengcc.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hxv.havefunace.top

[U106] JS：日期格式化
来源：http://asl.shanyushiyangtech.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://znl.yj20258.top

[U107] JS：数字千分位
来源：http://njv.fehbvm.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pve.cheryme.top

[U108] JS：随机整数
来源：http://wag.snrcjt.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ika.andypj.xyz

[U109] JS：数组分组
来源：http://gbs.guannengcc.top

Object.groupBy(arr, x => x.type)
来源：http://tur.haohaochexian.top

[U110] JS：数组分块
来源：http://rxj.hywenlv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xay.c1oappe.top

[U111] JS：对象转 Map
来源：http://zet.xuetiantiany.cn

new Map(Object.entries(obj))
来源：http://gmr.snrcjt.cn

[U112] JS：字符串补位
来源：http://hkz.c1oappe.top

"7".padStart(3, "0")
来源：http://agj.hywenlv.cn

[U113] JS：正则替换全部
来源：http://itk.ehwqpu.com

s.replaceAll("a", "b")
来源：http://wfy.jyoumei.cn

[U114] JS：JSON 深比较
来源：http://rgg.hesvh.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://dxs.hysaishi.cn

[U115] JS：生成 UUID
来源：http://znn.kuanghao11.cn

crypto.randomUUID()
来源：http://qzz.cashguo.top

[U116] JS：类型检查（JSDoc）
来源：http://jiy.jinghuilouyu.cn

/** @param {string} name */ function f(name) {}
来源：http://nde.hysaishi.cn

[U117] JS：单元测试
来源：http://zsj.havefunace.top

npm i -D vitest;  npx vitest
来源：http://lyn.zdbjq.cn

[U118] JS：开发服务器
来源：http://xsa.zhijiandao.cn

npm i -D vite;  npx vite
来源：http://hzm.yuanzhike.top

[U119] JS：生产构建
来源：http://msk.yj202588.top

npx vite build
来源：http://rcy.sxryk.cn

[U120] JS：读取环境变量（Vite）
来源：http://jjk.daria6918.cn

import.meta.env.VITE_API_URL
来源：http://yxa.cheryme.top

================================================================================
来源：http://wmb.yvedp.cn

统计汇总
来源：http://zga.wangdashe.top

================================================================================
来源：http://lag.aizwys.cn

按语言统计（条）：
来源：http://ozr.andypj.xyz

Python ......... 252
来源：http://ack.hammf.cn

PHP ............ 252
来源：http://hva.fzhhl.top

JavaScript ..... 252
来源：http://zxd.shanyushiyangtech.top

TypeScript ..... 212
来源：http://qck.nanxinkj.top

Java ........... 212
来源：http://mhq.yangfankeji.com

Go ............. 212
来源：http://wvv.wangshuangyany.cn

Ruby ........... 212
来源：http://ofq.andypj.xyz

C# ............. 212
来源：http://ead.fengsongda.top

C .............. 30
来源：http://mrv.jqgfzy.top

C++ ............ 30
来源：http://mrh.xziqi.cn

SQL ............ 90
来源：http://hqu.cheryme.top

Bash ........... 80
来源：http://iol.aizwys.cn

Kotlin ......... 15
来源：http://jsd.ehwqpu.com

Swift .......... 15
来源：http://klm.zhiwuduotai.top

Lua ............ 10
来源：http://mqn.yj20258888.top

Perl ........... 10
来源：http://air.tarul.cn

Scala .......... 10
来源：http://srm.hysaishi.cn

------------------------------------
来源：http://ycs.dianchejie.cn

合计 ........... 2106 条
来源：http://yyk.wangdashe.top

按章节统计：
来源：http://opo.sufxvd.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jji.smart0.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tcg.quarkkingdee.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yiv.vqdsnc.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://uzb.meibo888.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zfd.jqgfzy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bgi.hnqzz.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dxj.yongpay.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tue.yangfankeji.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dqi.fanxiaobao.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qkb.guowangkeji.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://osf.hesvh.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hdm.ywan-chungtsiang.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bho.fengsongda.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://svq.hnxiangtu.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://oek.ydjk.org.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nct.quarkkingdee.top

Q SQL 专题                              90
来源：http://ikk.cucudq.cn

R Bash 专题                             80
来源：http://dnq.52xcode.cn

S C / C++ 专题                          60
来源：http://pna.xingfuxueyuan.xyz

T 其他语言补充                          60
来源：http://mae.jinghuilouyu.cn

U 高频实用片段                         120
来源：http://luk.zdqjudy.top

------------------------------------
来源：http://gcd.fanxiaobao.xyz

合计                                  2106 条
来源：http://fvh.yj202588.top

--------------------------------------------------------------------------------
来源：http://wlp.pycfn.com

使用提醒
来源：http://luo.shangyingyoupin.top

--------------------------------------------------------------------------------
来源：http://ljf.gogol.net.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lzu.c1oappe.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cgr.zhixingplan.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mpd.cashguo.top

在旧版本上使用前请先确认语法支持情况。
来源：http://oht.fehbvm.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qbi.jinqigufen.top

—— 文件结束 ——
来源：http://mrj.hesvh.cn

================================================================================
来源：http://bqt.redwolf501.top

程序语言常见例子速查手册（2024 版）
来源：http://rec.fktsv.cn

Common Programming Examples Cheat Book
来源：http://xtu.tianlin.xyz

================================================================================
来源：http://ljv.vehdjk.com

【收录内容】
来源：http://hec.cheryme.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ipj.xinyue.icu

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://npr.zycfv.cn

SQL · Bash · C · C++
来源：http://njj.cashguo.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zlt.tanke756.top

【使用说明】
来源：http://wex.zhoulong.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rkn.yfazqb.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lpb.gzhubu.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lcc.iojbl.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gxf.zhongyouzk.top

Bash:  Shell         C:     C             C++:   C++
来源：http://adn.sysykeji.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wiq.cdnleiting.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yig.yj20258.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ubw.xylfe.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jwy.hysaishi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://kxd.hfpthk.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://onr.sufxvd.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tki.sweek.top

【文件统计】
来源：http://wfg.sxryk.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://are.smart0.xyz

--------------------------------------------------------------------------------
来源：http://qsd.gogol.net.cn

目  录
来源：http://iev.yongpay.top

--------------------------------------------------------------------------------
来源：http://nge.aibaodan.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://nor.hywenlv.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xed.cqqwz.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://toc.zycfv.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vve.meibo888.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vvr.guannengcc.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cwx.c1oappe.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://dgv.ivvv.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ghi.hywenlv.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wws.sysykeji.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gfj.havefunace.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ttp.zhoulong.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pnw.yuxming.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pfb.chenjidiqi.icu

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ntw.jqgufenzy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zbb.zhixingplan.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://anl.vehdjk.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jgv.jyoumei.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://vhr.yvedp.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bmo.jqgufenzy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vzs.zhengqikj.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jae.hysaishi.cn

================================================================================
来源：http://xzr.snrcjt.cn

A. 基础语法与类型
来源：http://hwm.shuidangran.top

================================================================================
来源：http://dkk.shzxlz.cn

[A01] Hello World
来源：http://yqi.fehbvm.com

Py:   print("Hello, World!")
来源：http://bhf.feifeiyinyue.top

PHP:  echo "Hello, World!";
来源：http://ywp.epnwcf.com

JS:   console.log("Hello, World!");
来源：http://cbe.shuidangran.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zdt.gogol.net.cn

Java: System.out.println("Hello, World!");
来源：http://bco.sysykeji.top

Go:   fmt.Println("Hello, World!")
来源：http://fdl.yuxming.cn

Ruby: puts "Hello, World!"
来源：http://ufi.shanyushiyangkeji.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ufh.haohaochexian.top

[A02] 变量声明与赋值
来源：http://bvc.smart0.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://oyo.gotoacloud.top

PHP:  $name = "Alex"; $age = 20;
来源：http://xfc.zhixingplan.top

JS:   let name = "Alex"; const age = 20;
来源：http://bxa.sysykeji.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rxo.yuanzhike.top

Java: String name = "Alex"; int age = 20;
来源：http://keo.cqqwz.cn

Go:   name := "Alex"; age := 20
来源：http://ouj.yangfankeji.com

Ruby: name = "Alex"; age = 20
来源：http://ecg.guowangkeji.top

C#:   string name = "Alex"; int age = 20;
来源：http://egu.52xcode.cn

[A03] 常量定义
来源：http://zqk.redwolf501.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ovm.xingfuxueyuan.xyz

PHP:  const PI = 3.14159;
来源：http://fih.zdqjudy.top

JS:   const PI = 3.14159;
来源：http://jmi.cheryme.top

TS:   const PI: number = 3.14159;
来源：http://prc.jqgufenzy.top

Java: static final double PI = 3.14159;
来源：http://svr.hcnkem.com

Go:   const PI = 3.14159
来源：http://old.cashguo.top

Ruby: PI = 3.14159
来源：http://wfv.ehwqpu.com

C#:   const double PI = 3.14159;
来源：http://ahu.guowangkeji.top

[A04] 判断变量类型
来源：http://ddn.cdnleiting.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://wde.vqdsnc.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rwc.hongshengwenyu.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dpm.xuanzx.com

TS:   typeof x; x instanceof Date
来源：http://nig.xuanzx.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://sxc.chenzaomai.com

Go:   reflect.TypeOf(x).Name()
来源：http://wtl.gaohongyu789.top

Ruby: x.class; x.is_a?(Integer)
来源：http://dqo.0kj1m.cn

C#:   x.GetType().Name; x is int
来源：http://hgi.andypj.xyz

[A05] 整数除法与取模
来源：http://mhq.havefunace.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lqe.bbcook.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://nji.316326.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mpj.52xcode.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lrm.vqdsnc.cn

Java: 7 / 2; 7 % 2
来源：http://elb.ehwqpu.com

Go:   7 / 2; 7 % 2
来源：http://xox.zdbjq.cn

Ruby: 7 / 2; 7 % 2
来源：http://fdk.aibaodan.cn

C#:   7 / 2; 7 % 2
来源：http://plz.chenlongwang.top

[A06] 字符串转数字
来源：http://thn.feifeiyinyue.top

Py:   int("42"); float("3.14")
来源：http://kgo.chenjidiqi.icu

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hut.snrcjt.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lgh.bbcook.cn

TS:   parseInt("42", 10); Number("42")
来源：http://xpb.jinghuilouyu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://yih.feifeiyinyue.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pkg.jlsjyb.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://yuy.tanke756.top


<!-- 参考信息 -->