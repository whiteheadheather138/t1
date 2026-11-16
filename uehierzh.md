代发 wailian999

[U51] PHP：数组解构
来源：http://zkj.zhixingplan.top

[$a, $b] = $arr;
来源：http://gpb.tanke756.top

[U52] PHP：箭头函数
来源：http://prn.yj20258888.top

$double = fn($x) => $x * 2;
来源：http://moa.jinqigfzy.top

[U53] PHP：空合并运算符
来源：http://wik.aizwys.cn

$v = $a ?? $b ?? "default";
来源：http://evf.zdbjq.cn

[U54] PHP：空安全调用
来源：http://rov.pengpengdd.cyou

$obj?->method()
来源：http://yjn.yj202588.top

[U55] PHP：match 表达式
来源：http://tqw.yj20258.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rir.ehwqpu.com

[U56] PHP：命名参数
来源：http://rqw.guowangkeji.top

f(a: 1, b: 2)
来源：http://ebk.yanxiufei.cn

[U57] PHP：字符串插值
来源：http://vfe.zhiwuduotai.top

"值: {$a}"
来源：http://qar.52xcode.cn

[U58] PHP：数组三件套
来源：http://hmj.316326.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wpm.andypj.xyz

[U59] PHP：自定义排序
来源：http://mai.nanxuanxn.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qrq.9152youxi.cn

[U60] PHP：JSON 编解码
来源：http://ram.daria6918.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://opg.sufxvd.cn

[U61] PHP：正则
来源：http://lny.xingfuxueyuan.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lov.cqqwz.cn

[U62] PHP：日期对象
来源：http://muq.daxiang520.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ioz.andypj.xyz

[U63] PHP：文件读写
来源：http://ysv.bjfxy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qht.cucudq.cn

[U64] PHP：目录遍历
来源：http://umy.cucudq.cn

glob("dir/*.php");  scandir("dir");
来源：http://cdv.sjlbkw.cn

[U65] PHP：会话
来源：http://pfw.ydzc1.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ptc.yuanzhike.top

[U66] PHP：设置 Cookie
来源：http://ifu.jlsjyb.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://iia.fengsongda.top

[U67] PHP：处理文件上传
来源：http://kch.zycfv.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vtm.sxryk.cn

[U68] PHP：PDO 连接
来源：http://wig.shuidangran.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mnx.cucudq.cn

[U69] PHP：PDO 预处理
来源：http://zjf.ehwqpu.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bei.fzhhl.top

[U70] PHP：PDO 事务
来源：http://quw.gotoacloud.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wdx.fktsv.cn

[U71] PHP：抛出异常
来源：http://uga.yvedp.cn

throw new RuntimeException("失败", 500);
来源：http://arf.andypj.xyz

[U72] PHP：写错误日志
来源：http://ybw.yuxming.cn

error_log("失败: " . $e->getMessage());
来源：http://vsb.ywan-chungtsiang.top

[U73] PHP：读取 ini 配置
来源：http://vnh.zhiwuduotai.top

parse_ini_file("config.ini", true)
来源：http://goo.9152youxi.cn

[U74] PHP：读取环境变量
来源：http://ijg.vehdjk.com

getenv("APP_ENV") ?: "production"
来源：http://hup.gzhubu.top

[U75] PHP：依赖注入
来源：http://lve.iojbl.cn

composer require psr/container
来源：http://frr.yfazqb.com

[U76] PHP：简单路由
来源：http://gxg.vqdsnc.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yus.tanke756.top

[U77] PHP：模板渲染
来源：http://pia.yueranfly.top

composer require twig/twig
来源：http://cjf.sxryk.cn

[U78] PHP：单元测试
来源：http://efq.jinqigufen.top

composer require --dev phpunit/phpunit
来源：http://ypk.chenjidiqi.icu

[U79] PHP：静态分析
来源：http://iai.sjlbkw.cn

composer require --dev phpstan/phpstan
来源：http://lui.yvedp.cn

[U80] PHP：代码规范修复
来源：http://xzm.hnxiangtu.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://vkq.epnwcf.com

[U81] JS：初始化项目
来源：http://pje.dianchejie.cn

npm init -y;  npm i express
来源：http://jkf.chenzaomai.com

[U82] JS：package.json 脚本
来源：http://tih.ivvv.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fty.hammf.cn

[U83] JS：ES Module 导入导出
来源：http://ltn.yj20258888.top

export const a = 1;  import { a } from "./m.js";
来源：http://egz.ybcxt.top

[U84] JS：CommonJS 写法
来源：http://dwk.sweek.top

module.exports = { a };  const { a } = require("./m");
来源：http://vbq.zhaomingkeji.xyz

[U85] JS：可选链
来源：http://wrz.zhaomingkeji.xyz

a?.b?.c
来源：http://fzz.andypj.xyz

[U86] JS：空值合并
来源：http://vqu.yueranfly.top

a ?? b
来源：http://vvs.ydzc1.top

[U87] JS：解构默认值
来源：http://uly.aibaodan.cn

const { a = 1, b = 2 } = obj;
来源：http://jtp.gotoacloud.top

[U88] JS：对象展开合并
来源：http://sjz.shangyingyoupin.top

{ ...a, ...b }
来源：http://urf.gogol.net.cn

[U89] JS：数组去重
来源：http://unm.birdmap.top

[...new Set(arr)]
来源：http://fgl.meibo888.top

[U90] JS：数字数组排序
来源：http://fcb.zhongyouzk.top

[...arr].sort((a, b) => a - b)
来源：http://ukd.yuxming.cn

[U91] JS：对象键值遍历
来源：http://nmi.dianchejie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bez.sufxvd.cn

[U92] JS：深拷贝
来源：http://bft.yj20258888.top

structuredClone(obj)
来源：http://muo.jinqigfzy.top

[U93] JS：模板字符串
来源：http://azx.ppjwa.cn

`共 ${n} 条`
来源：http://fzs.guannengcc.top

[U94] JS：箭头函数
来源：http://azd.jianghu66.top

const double = x => x * 2;
来源：http://heh.wangshuangyany.cn

[U95] JS：Promise 包装
来源：http://jjb.jiagoushi.top

new Promise((resolve, reject) => {})
来源：http://kgc.shanyushiyangtech.top

[U96] JS：async/await 与异常
来源：http://dhl.xinyue.icu

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gqp.dashuyun.cn

[U97] JS：并发请求
来源：http://pgb.gaohongyu789.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://rdh.hesvh.cn

[U98] JS：fetch 带 JSON
来源：http://umz.yueranfly.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hov.yj20258888.top

[U99] JS：事件监听
来源：http://nfx.gotoacloud.top

el.addEventListener("click", e => {})
来源：http://dzf.jiagoushi.top

[U100] JS：DOM 查询
来源：http://cob.yj20258888.top

document.querySelector(".item")
来源：http://rtd.jinqigufen.top

[U101] JS：classList 操作
来源：http://oop.epnwcf.com

el.classList.toggle("active")
来源：http://lzw.snrcjt.cn

[U102] JS：本地存储
来源：http://dnv.fanxiaobao.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://cub.yfazqb.com

[U103] JS：定时器
来源：http://yeb.yj202588.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qpt.yj20258888.top

[U104] JS：防抖
来源：http://jef.jinyuanbaomall.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://esr.ppjwa.cn

[U105] JS：节流
来源：http://btl.yanxiufei.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gwm.hongshengwenyu.top

[U106] JS：日期格式化
来源：http://qvc.hesvh.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cvh.fanxiaobao.xyz

[U107] JS：数字千分位
来源：http://pvb.xuetiantiany.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://peu.snrcjt.cn

[U108] JS：随机整数
来源：http://yjm.bjfxy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://chf.chenjidiqi.icu

[U109] JS：数组分组
来源：http://ukx.hesvh.cn

Object.groupBy(arr, x => x.type)
来源：http://pxw.hnxiangtu.top

[U110] JS：数组分块
来源：http://tpk.nanxuanxn.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kfx.shanyushiyangkeji.top

[U111] JS：对象转 Map
来源：http://wbc.jinqigfzy.top

new Map(Object.entries(obj))
来源：http://kct.cdnleiting.top

[U112] JS：字符串补位
来源：http://wae.ydjk.org.cn

"7".padStart(3, "0")
来源：http://jzx.mhx1999.top

[U113] JS：正则替换全部
来源：http://fcw.zycfv.cn

s.replaceAll("a", "b")
来源：http://mlo.fktsv.cn

[U114] JS：JSON 深比较
来源：http://lmm.pycfn.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://gvx.yj202588.top

[U115] JS：生成 UUID
来源：http://sfo.chenzaomai.com

crypto.randomUUID()
来源：http://hsi.zhiwuduotai.top

[U116] JS：类型检查（JSDoc）
来源：http://twa.gotoacloud.top

/** @param {string} name */ function f(name) {}
来源：http://rst.xuetiantiany.cn

[U117] JS：单元测试
来源：http://mbx.snrcjt.cn

npm i -D vitest;  npx vitest
来源：http://wep.chenjidiqi.icu

[U118] JS：开发服务器
来源：http://oto.hfpthk.cn

npm i -D vite;  npx vite
来源：http://cyg.zhaomingkeji.xyz

[U119] JS：生产构建
来源：http://gac.xinyue.icu

npx vite build
来源：http://kjk.fanxiaobao.xyz

[U120] JS：读取环境变量（Vite）
来源：http://wyl.zhixingplan.top

import.meta.env.VITE_API_URL
来源：http://spi.yanxiufei.cn

================================================================================
来源：http://igz.jinqigufen.top

统计汇总
来源：http://lvc.yongpay.top

================================================================================
来源：http://rfa.ywan-chungtsiang.top

按语言统计（条）：
来源：http://gdk.birdmap.top

Python ......... 252
来源：http://ckc.yonumen.top

PHP ............ 252
来源：http://phf.haohaochexian.top

JavaScript ..... 252
来源：http://ple.xingfuxueyuan.xyz

TypeScript ..... 212
来源：http://nyl.yongpay.top

Java ........... 212
来源：http://lyz.xylfe.cn

Go ............. 212
来源：http://qwf.yj20258.top

Ruby ........... 212
来源：http://tea.shzxlz.cn

C# ............. 212
来源：http://obk.hammf.cn

C .............. 30
来源：http://mex.yongpay.top

C++ ............ 30
来源：http://glu.hesvh.cn

SQL ............ 90
来源：http://gys.redwolf501.top

Bash ........... 80
来源：http://vrd.snrcjt.cn

Kotlin ......... 15
来源：http://qkw.ywan-chungtsiang.top

Swift .......... 15
来源：http://xta.zdqjudy.top

Lua ............ 10
来源：http://qlm.shzxlz.cn

Perl ........... 10
来源：http://ecf.c1oappe.top

Scala .......... 10
来源：http://sto.xylfe.cn

------------------------------------
来源：http://hvx.epnwcf.com

合计 ........... 2106 条
来源：http://vmq.zdqjudy.top

按章节统计：
来源：http://fak.xingfuxueyuan.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://okc.zhijiandao.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yro.shanyushiyangtech.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zno.0kj1m.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://olf.52xcode.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xzh.jqgufenzy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://uzl.bbcook.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tnx.iojbl.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rks.hywenlv.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://eoa.0kj1m.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://slv.wangshuangyany.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vqp.jinghuilouyu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lyr.fengsongda.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tfy.dianchejie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rga.shangyingyoupin.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://izd.hywenlv.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xgw.smart0.xyz

Q SQL 专题                              90
来源：http://byd.xingfuxueyuan.xyz

R Bash 专题                             80
来源：http://hor.xziqi.cn

S C / C++ 专题                          60
来源：http://olh.sweek.top

T 其他语言补充                          60
来源：http://ptb.zhixingplan.top

U 高频实用片段                         120
来源：http://mle.316326.xyz

------------------------------------
来源：http://zjf.zdbjq.cn

合计                                  2106 条
来源：http://jtw.xuanzx.com

--------------------------------------------------------------------------------
来源：http://nsu.jinyuanbaomall.cn

使用提醒
来源：http://ygo.jianghu66.top

--------------------------------------------------------------------------------
来源：http://mmu.chenzaomai.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ybd.xuanzx.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dww.cucudq.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ttw.ywan-chungtsiang.top

在旧版本上使用前请先确认语法支持情况。
来源：http://wva.birdmap.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gqi.zdbjq.cn

—— 文件结束 ——
来源：http://pvg.cqqwz.cn

================================================================================
来源：http://zan.jinghuilouyu.cn

程序语言常见例子速查手册（2024 版）
来源：http://fmh.sufxvd.cn

Common Programming Examples Cheat Book
来源：http://iza.316326.xyz

================================================================================
来源：http://gni.fktsv.cn

【收录内容】
来源：http://cpn.nanxinkj.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://eyq.ydjk.org.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zfp.yfazqb.com

SQL · Bash · C · C++
来源：http://cvi.ywan-chungtsiang.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://epi.dashuyun.cn

【使用说明】
来源：http://zcr.gzhubu.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://iqm.nanxuanxn.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://gzp.dashuyun.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pkz.ehwqpu.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://spd.yueranfly.top

Bash:  Shell         C:     C             C++:   C++
来源：http://mqg.jqgufenzy.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bvw.cqqwz.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ypn.hysaishi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fro.hnqzz.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pxf.sweek.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wwj.iojbl.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qxq.vehdjk.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vhu.gzhubu.top

【文件统计】
来源：http://lsu.xuanzx.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ciw.guowangkeji.top

--------------------------------------------------------------------------------
来源：http://zop.yonumen.top

目  录
来源：http://bwl.hywenlv.cn

--------------------------------------------------------------------------------
来源：http://ewi.ctjpmb.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qnz.feifeiyinyue.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cne.hammf.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://uyd.wangdashe.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://egb.daxiang520.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kiq.cucudq.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wla.shangyingyoupin.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kdt.xuetiantiany.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://doq.tianlin.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://pxl.316326.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://czx.cucudq.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wzp.chenjidiqi.icu

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zzx.zhijiandao.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://thc.cucudq.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vni.c1oappe.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://sns.zhixingplan.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ibr.cashguo.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jwb.yfazqb.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://xco.epnwcf.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://asy.birdmap.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ysc.0kj1m.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://txg.zdqjudy.top

================================================================================
来源：http://cyb.xinyue.icu

A. 基础语法与类型
来源：http://ekv.havefunace.top

================================================================================
来源：http://hyq.chenzaomai.com

[A01] Hello World
来源：http://csb.zdbjq.cn

Py:   print("Hello, World!")
来源：http://kcu.meibo888.top

PHP:  echo "Hello, World!";
来源：http://nhs.shanyushiyangkeji.top

JS:   console.log("Hello, World!");
来源：http://bpq.jiagoushi.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gys.jqgufenzy.top

Java: System.out.println("Hello, World!");
来源：http://wxz.guannengcc.top

Go:   fmt.Println("Hello, World!")
来源：http://rpk.pycfn.com

Ruby: puts "Hello, World!"
来源：http://yre.yongpay.top

C#:   Console.WriteLine("Hello, World!");
来源：http://jfx.zhongyouzk.top

[A02] 变量声明与赋值
来源：http://pea.tanke756.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://owr.nanxinkj.top

PHP:  $name = "Alex"; $age = 20;
来源：http://cre.ivvv.top

JS:   let name = "Alex"; const age = 20;
来源：http://bkk.snrcjt.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://aaw.guannengcc.top

Java: String name = "Alex"; int age = 20;
来源：http://rfz.chenlongwang.top

Go:   name := "Alex"; age := 20
来源：http://iew.cucudq.cn

Ruby: name = "Alex"; age = 20
来源：http://rkr.smart0.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://mcs.52xcode.cn

[A03] 常量定义
来源：http://mvv.9152youxi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ofk.hesvh.cn

PHP:  const PI = 3.14159;
来源：http://ohh.sysykeji.top

JS:   const PI = 3.14159;
来源：http://uev.xinyue.icu

TS:   const PI: number = 3.14159;
来源：http://get.yvedp.cn

Java: static final double PI = 3.14159;
来源：http://ekt.tian-w.cn

Go:   const PI = 3.14159
来源：http://ldk.gaohongyu789.top

Ruby: PI = 3.14159
来源：http://hfo.gogol.net.cn

C#:   const double PI = 3.14159;
来源：http://nbg.zhengqikj.top

[A04] 判断变量类型
来源：http://abm.dashuyun.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://efr.kuanghao11.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xsv.jinqigufen.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tlf.cashguo.top

TS:   typeof x; x instanceof Date
来源：http://elh.iojbl.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://leo.vehdjk.com

Go:   reflect.TypeOf(x).Name()
来源：http://wir.mhx1999.top

Ruby: x.class; x.is_a?(Integer)
来源：http://odn.daxiang520.top

C#:   x.GetType().Name; x is int
来源：http://adc.chenjidiqi.icu

[A05] 整数除法与取模
来源：http://afo.sufxvd.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://uzn.dashuyun.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://sva.316326.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tjz.quarkkingdee.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cyl.52xcode.cn

Java: 7 / 2; 7 % 2
来源：http://txk.yangfankeji.com

Go:   7 / 2; 7 % 2
来源：http://afy.yj202588.top

Ruby: 7 / 2; 7 % 2
来源：http://lts.nanxuanxn.top

C#:   7 / 2; 7 % 2
来源：http://lcj.guowangkeji.top

[A06] 字符串转数字
来源：http://wdg.iojbl.cn

Py:   int("42"); float("3.14")
来源：http://pjd.smart0.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ekn.ywan-chungtsiang.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zkc.guannengcc.top

TS:   parseInt("42", 10); Number("42")
来源：http://srx.pengpengdd.cyou

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gcs.daria6918.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pwt.fehbvm.com

Ruby: "42".to_i; "3.14".to_f
来源：http://ryw.andypj.xyz


<!-- 参考信息 -->