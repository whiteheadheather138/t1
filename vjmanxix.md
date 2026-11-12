代发 wailian999

[U51] PHP：数组解构
来源：http://bmp.yvedp.cn

[$a, $b] = $arr;
来源：http://smy.ydzc1.top

[U52] PHP：箭头函数
来源：http://fwx.ywan-chungtsiang.top

$double = fn($x) => $x * 2;
来源：http://fki.shzxlz.cn

[U53] PHP：空合并运算符
来源：http://jxi.xingfuxueyuan.xyz

$v = $a ?? $b ?? "default";
来源：http://ijt.cucudq.cn

[U54] PHP：空安全调用
来源：http://pih.yfazqb.com

$obj?->method()
来源：http://roz.52xcode.cn

[U55] PHP：match 表达式
来源：http://bte.fehbvm.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jcn.jyoumei.cn

[U56] PHP：命名参数
来源：http://tlg.meibo888.top

f(a: 1, b: 2)
来源：http://uwp.hfpthk.cn

[U57] PHP：字符串插值
来源：http://qtl.yuanzhike.top

"值: {$a}"
来源：http://qvk.hammf.cn

[U58] PHP：数组三件套
来源：http://mky.yuanzhike.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jch.birdmap.top

[U59] PHP：自定义排序
来源：http://inm.zycfv.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tpy.hammf.cn

[U60] PHP：JSON 编解码
来源：http://jju.zhijiandao.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wxw.hnxiangtu.top

[U61] PHP：正则
来源：http://jpk.jianghu66.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fag.bbcook.cn

[U62] PHP：日期对象
来源：http://ccr.dashuyun.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kfa.yueranfly.top

[U63] PHP：文件读写
来源：http://qir.sweek.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gfh.sxryk.cn

[U64] PHP：目录遍历
来源：http://kyu.yuxming.cn

glob("dir/*.php");  scandir("dir");
来源：http://zmy.shanyushiyangkeji.top

[U65] PHP：会话
来源：http://ajt.gzhubu.top

session_start();  $_SESSION["uid"] = 1;
来源：http://dlk.ivvv.top

[U66] PHP：设置 Cookie
来源：http://hfr.hfpthk.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zzv.gzhubu.top

[U67] PHP：处理文件上传
来源：http://blg.ivvv.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xdk.hywenlv.cn

[U68] PHP：PDO 连接
来源：http://pui.gzhubu.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fdu.cdnleiting.top

[U69] PHP：PDO 预处理
来源：http://agw.chenzaomai.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://una.yanxiufei.cn

[U70] PHP：PDO 事务
来源：http://bqq.tanke756.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tkm.shanyushiyangkeji.top

[U71] PHP：抛出异常
来源：http://mch.hnqzz.top

throw new RuntimeException("失败", 500);
来源：http://inb.yj20258888.top

[U72] PHP：写错误日志
来源：http://scu.9152youxi.cn

error_log("失败: " . $e->getMessage());
来源：http://fbq.cheryme.top

[U73] PHP：读取 ini 配置
来源：http://tdm.aizwys.cn

parse_ini_file("config.ini", true)
来源：http://zfq.zhiwuduotai.top

[U74] PHP：读取环境变量
来源：http://dnn.nanxuanxn.top

getenv("APP_ENV") ?: "production"
来源：http://ezg.vehdjk.com

[U75] PHP：依赖注入
来源：http://xqu.xinyue.icu

composer require psr/container
来源：http://hfm.havefunace.top

[U76] PHP：简单路由
来源：http://xqp.fengsongda.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bfi.hfpthk.cn

[U77] PHP：模板渲染
来源：http://whs.jlsjyb.cn

composer require twig/twig
来源：http://dmp.shangyingyoupin.top

[U78] PHP：单元测试
来源：http://uou.bjfxy.top

composer require --dev phpunit/phpunit
来源：http://nsb.yongpay.top

[U79] PHP：静态分析
来源：http://bwo.yonumen.top

composer require --dev phpstan/phpstan
来源：http://zqc.snrcjt.cn

[U80] PHP：代码规范修复
来源：http://yns.yuxming.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://btn.yj20258888.top

[U81] JS：初始化项目
来源：http://klv.vehdjk.com

npm init -y;  npm i express
来源：http://jer.redwolf501.top

[U82] JS：package.json 脚本
来源：http://woc.shanyushiyangtech.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jkp.ctjpmb.com

[U83] JS：ES Module 导入导出
来源：http://hdu.316326.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://ybn.zhaomingkeji.xyz

[U84] JS：CommonJS 写法
来源：http://xjj.dashuyun.cn

module.exports = { a };  const { a } = require("./m");
来源：http://sud.yonumen.top

[U85] JS：可选链
来源：http://zhe.hammf.cn

a?.b?.c
来源：http://fon.dashuyun.cn

[U86] JS：空值合并
来源：http://buh.xinyue.icu

a ?? b
来源：http://pdh.chenlongwang.top

[U87] JS：解构默认值
来源：http://hjs.aibaodan.cn

const { a = 1, b = 2 } = obj;
来源：http://pke.gotoacloud.top

[U88] JS：对象展开合并
来源：http://mjg.yongpay.top

{ ...a, ...b }
来源：http://tyh.cdnleiting.top

[U89] JS：数组去重
来源：http://fwg.nanxinkj.top

[...new Set(arr)]
来源：http://chl.jqgufenzy.top

[U90] JS：数字数组排序
来源：http://gex.xinyue.icu

[...arr].sort((a, b) => a - b)
来源：http://yid.ydzc1.top

[U91] JS：对象键值遍历
来源：http://try.jinqigfzy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://egv.tarul.cn

[U92] JS：深拷贝
来源：http://qhv.shzxlz.cn

structuredClone(obj)
来源：http://bqb.aibaodan.cn

[U93] JS：模板字符串
来源：http://sek.sjlbkw.cn

`共 ${n} 条`
来源：http://vda.shangyingyoupin.top

[U94] JS：箭头函数
来源：http://ror.ywan-chungtsiang.top

const double = x => x * 2;
来源：http://cbj.ydjk.org.cn

[U95] JS：Promise 包装
来源：http://oqb.fanxiaobao.xyz

new Promise((resolve, reject) => {})
来源：http://zgb.sysykeji.top

[U96] JS：async/await 与异常
来源：http://ckt.xziqi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hnv.316326.xyz

[U97] JS：并发请求
来源：http://bwl.9152youxi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://afu.daxiang520.top

[U98] JS：fetch 带 JSON
来源：http://mgu.cucudq.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zqp.tian-w.cn

[U99] JS：事件监听
来源：http://knr.fktsv.cn

el.addEventListener("click", e => {})
来源：http://zvi.jyoumei.cn

[U100] JS：DOM 查询
来源：http://dut.quarkkingdee.top

document.querySelector(".item")
来源：http://isq.kuanghao11.cn

[U101] JS：classList 操作
来源：http://xdu.yj20258888.top

el.classList.toggle("active")
来源：http://mvo.svipenyu.cn

[U102] JS：本地存储
来源：http://tum.zhijiandao.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bly.yj20258888.top

[U103] JS：定时器
来源：http://rih.fengsongda.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://flf.dashuyun.cn

[U104] JS：防抖
来源：http://ewr.0kj1m.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://smj.nanxinkj.top

[U105] JS：节流
来源：http://pgc.ppjwa.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://amu.cucudq.cn

[U106] JS：日期格式化
来源：http://vdd.shanyushiyangkeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://otb.chenlongwang.top

[U107] JS：数字千分位
来源：http://qwf.ctjpmb.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gii.hywenlv.cn

[U108] JS：随机整数
来源：http://kht.fehbvm.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ypj.0kj1m.cn

[U109] JS：数组分组
来源：http://gvr.smart0.xyz

Object.groupBy(arr, x => x.type)
来源：http://pxh.zycfv.cn

[U110] JS：数组分块
来源：http://bpf.yonumen.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lfs.jyoumei.cn

[U111] JS：对象转 Map
来源：http://xhh.svipenyu.cn

new Map(Object.entries(obj))
来源：http://bep.redwolf501.top

[U112] JS：字符串补位
来源：http://hvo.zhengqikj.top

"7".padStart(3, "0")
来源：http://vgm.zhaomingkeji.xyz

[U113] JS：正则替换全部
来源：http://eok.c1oappe.top

s.replaceAll("a", "b")
来源：http://yvo.zhiwuduotai.top

[U114] JS：JSON 深比较
来源：http://hsm.fehbvm.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://ecr.xingfuxueyuan.xyz

[U115] JS：生成 UUID
来源：http://hpy.9152youxi.cn

crypto.randomUUID()
来源：http://qmn.pengpengdd.cyou

[U116] JS：类型检查（JSDoc）
来源：http://xmv.quarkkingdee.top

/** @param {string} name */ function f(name) {}
来源：http://xzf.jianghu66.top

[U117] JS：单元测试
来源：http://gnk.wangdashe.top

npm i -D vitest;  npx vitest
来源：http://bvy.xuanzx.com

[U118] JS：开发服务器
来源：http://exs.yj20258.top

npm i -D vite;  npx vite
来源：http://hvz.xziqi.cn

[U119] JS：生产构建
来源：http://umy.nwbrower.top

npx vite build
来源：http://dpm.zhaomingkeji.xyz

[U120] JS：读取环境变量（Vite）
来源：http://ncq.mhx1999.top

import.meta.env.VITE_API_URL
来源：http://xxq.yj20258.top

================================================================================
来源：http://jbz.hammf.cn

统计汇总
来源：http://orw.yongpay.top

================================================================================
来源：http://dnf.iojbl.cn

按语言统计（条）：
来源：http://wuy.gotoacloud.top

Python ......... 252
来源：http://onh.yfazqb.com

PHP ............ 252
来源：http://wfe.daria6918.cn

JavaScript ..... 252
来源：http://brr.gzhubu.top

TypeScript ..... 212
来源：http://dqi.cucudq.cn

Java ........... 212
来源：http://mct.hfpthk.cn

Go ............. 212
来源：http://ici.hesvh.cn

Ruby ........... 212
来源：http://iic.ctjpmb.com

C# ............. 212
来源：http://eto.ivvv.top

C .............. 30
来源：http://tvj.jinyuanbaomall.cn

C++ ............ 30
来源：http://skv.hongshengwenyu.top

SQL ............ 90
来源：http://ksp.chenlongwang.top

Bash ........... 80
来源：http://rui.yangfankeji.com

Kotlin ......... 15
来源：http://nji.guannengcc.top

Swift .......... 15
来源：http://ahc.chenzaomai.com

Lua ............ 10
来源：http://bvh.fehbvm.com

Perl ........... 10
来源：http://bvd.yvedp.cn

Scala .......... 10
来源：http://jsw.yj20258888.top

------------------------------------
来源：http://jmh.jinqigufen.top

合计 ........... 2106 条
来源：http://tfy.havefunace.top

按章节统计：
来源：http://lho.gaohongyu789.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qfy.shangyingyoupin.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://syl.zdqjudy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://spt.chenjidiqi.icu

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ima.meibo888.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jin.chenjidiqi.icu

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fok.jinqigfzy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bep.xinyue.icu

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ayc.nanxuanxn.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kpk.316326.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ffl.fanxiaobao.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ujp.zdbjq.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://bni.yvedp.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://njk.svipenyu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yki.fengsongda.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fpb.xylfe.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zyq.zhaomingkeji.xyz

Q SQL 专题                              90
来源：http://lia.jyoumei.cn

R Bash 专题                             80
来源：http://oop.cashguo.top

S C / C++ 专题                          60
来源：http://otr.fanxiaobao.xyz

T 其他语言补充                          60
来源：http://vxq.sufxvd.cn

U 高频实用片段                         120
来源：http://arz.xuanzx.com

------------------------------------
来源：http://ycs.cashguo.top

合计                                  2106 条
来源：http://itp.daxiang520.top

--------------------------------------------------------------------------------
来源：http://oeq.haohaochexian.top

使用提醒
来源：http://izl.cucudq.cn

--------------------------------------------------------------------------------
来源：http://xfl.snrcjt.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ldm.hnqzz.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://uzj.tanke756.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://txt.jiagoushi.top

在旧版本上使用前请先确认语法支持情况。
来源：http://omg.pengpengdd.cyou

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://eds.hnqzz.top

—— 文件结束 ——
来源：http://etz.gogol.net.cn

================================================================================
来源：http://mhe.hnxiangtu.top

程序语言常见例子速查手册（2024 版）
来源：http://xbr.gogol.net.cn

Common Programming Examples Cheat Book
来源：http://ibz.zhaomingkeji.xyz

================================================================================
来源：http://jaz.fehbvm.com

【收录内容】
来源：http://mdc.dashuyun.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://tvk.xuanzx.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mia.hnqzz.top

SQL · Bash · C · C++
来源：http://xfv.hywenlv.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://icq.yj202588.top

【使用说明】
来源：http://quu.gotoacloud.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pva.dianchejie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vuj.xziqi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rsl.jyoumei.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://afu.tian-w.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://zwn.zhoulong.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://clo.fktsv.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fcp.fanxiaobao.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pia.9152youxi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ixq.chenzaomai.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://eco.hywenlv.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://uak.hcnkem.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zjd.52xcode.cn

【文件统计】
来源：http://cmi.aizwys.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dft.wangshuangyany.cn

--------------------------------------------------------------------------------
来源：http://seu.cqqwz.cn

目  录
来源：http://sso.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://eme.dianchejie.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hxq.kuanghao11.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lki.hnxiangtu.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tum.zdbjq.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ijg.zhixingplan.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yyr.jinqigfzy.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zwr.pengpengdd.cyou

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xjw.yj20258.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mtz.gogol.net.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ctm.ydjk.org.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ukm.hcnkem.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fff.nanxuanxn.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pry.gzhubu.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fkr.zhijiandao.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gvg.zhijiandao.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://igo.jiagoushi.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://oeh.yonumen.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pqn.ivvv.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://bmr.chenzaomai.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hji.svipenyu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qzv.jinqigfzy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://niz.guannengcc.top

================================================================================
来源：http://zal.pengpengdd.cyou

A. 基础语法与类型
来源：http://spc.daria6918.cn

================================================================================
来源：http://mck.mhx1999.top

[A01] Hello World
来源：http://mvd.shuidangran.top

Py:   print("Hello, World!")
来源：http://fom.svipenyu.cn

PHP:  echo "Hello, World!";
来源：http://zhi.jiagoushi.top

JS:   console.log("Hello, World!");
来源：http://vku.yj202588.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fge.yj202588.top

Java: System.out.println("Hello, World!");
来源：http://ueu.hnxiangtu.top

Go:   fmt.Println("Hello, World!")
来源：http://hai.daria6918.cn

Ruby: puts "Hello, World!"
来源：http://gat.shuidangran.top

C#:   Console.WriteLine("Hello, World!");
来源：http://tna.daxiang520.top

[A02] 变量声明与赋值
来源：http://ara.daria6918.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kia.bbcook.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://gdm.zhaomingkeji.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://jsr.shanyushiyangkeji.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ley.yvedp.cn

Java: String name = "Alex"; int age = 20;
来源：http://bmq.tarul.cn

Go:   name := "Alex"; age := 20
来源：http://gxu.chenjidiqi.icu

Ruby: name = "Alex"; age = 20
来源：http://qtq.uphjek.com

C#:   string name = "Alex"; int age = 20;
来源：http://aks.guowangkeji.top

[A03] 常量定义
来源：http://kvx.ehwqpu.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kip.zhoulong.xyz

PHP:  const PI = 3.14159;
来源：http://bln.jlsjyb.cn

JS:   const PI = 3.14159;
来源：http://yky.chenzaomai.com

TS:   const PI: number = 3.14159;
来源：http://lts.yj20258888.top

Java: static final double PI = 3.14159;
来源：http://whn.xuetiantiany.cn

Go:   const PI = 3.14159
来源：http://laf.ivvv.top

Ruby: PI = 3.14159
来源：http://nxq.ctjpmb.com

C#:   const double PI = 3.14159;
来源：http://axv.aibaodan.cn

[A04] 判断变量类型
来源：http://tjo.kuanghao11.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://jzd.cqqwz.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://avj.xingfuxueyuan.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xbv.shuidangran.top

TS:   typeof x; x instanceof Date
来源：http://jyw.guowangkeji.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://iwz.zhengqikj.top

Go:   reflect.TypeOf(x).Name()
来源：http://djf.meibo888.top

Ruby: x.class; x.is_a?(Integer)
来源：http://bpb.fanxiaobao.xyz

C#:   x.GetType().Name; x is int
来源：http://axx.nanxinkj.top

[A05] 整数除法与取模
来源：http://btx.jiagoushi.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xfk.fanxiaobao.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://nsl.ydzc1.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://oci.zhaomingkeji.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lpm.shanyushiyangtech.top

Java: 7 / 2; 7 % 2
来源：http://oop.shuidangran.top

Go:   7 / 2; 7 % 2
来源：http://tzc.ctjpmb.com

Ruby: 7 / 2; 7 % 2
来源：http://jcc.zdbjq.cn

C#:   7 / 2; 7 % 2
来源：http://pyf.zhaomingkeji.xyz

[A06] 字符串转数字
来源：http://jfr.yj202588.top

Py:   int("42"); float("3.14")
来源：http://ktc.smart0.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gdd.ywan-chungtsiang.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cul.snrcjt.cn

TS:   parseInt("42", 10); Number("42")
来源：http://fon.jyoumei.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vnf.fehbvm.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ipj.wangdashe.top

Ruby: "42".to_i; "3.14".to_f
来源：http://qpj.svipenyu.cn


<!-- 参考信息 -->