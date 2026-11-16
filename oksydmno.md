代发 wailian999

[U53] PHP：空合并运算符
来源：http://soi.yangfankeji.com

$v = $a ?? $b ?? "default";
来源：http://wkf.cqqwz.cn

[U54] PHP：空安全调用
来源：http://qvx.zhiwuduotai.top

$obj?->method()
来源：http://bmf.quarkkingdee.top

[U55] PHP：match 表达式
来源：http://tnf.fengsongda.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jyr.jlsjyb.cn

[U56] PHP：命名参数
来源：http://rqb.aibaodan.cn

f(a: 1, b: 2)
来源：http://tqf.daria6918.cn

[U57] PHP：字符串插值
来源：http://xug.nwbrower.top

"值: {$a}"
来源：http://hql.wangdashe.top

[U58] PHP：数组三件套
来源：http://hir.daxiang520.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nhq.yfazqb.com

[U59] PHP：自定义排序
来源：http://tli.yuanzhike.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lkj.chenzaomai.com

[U60] PHP：JSON 编解码
来源：http://cdk.dianchejie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dyv.chenzaomai.com

[U61] PHP：正则
来源：http://yhm.jinqigufen.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ptb.ywan-chungtsiang.top

[U62] PHP：日期对象
来源：http://heh.jinqigufen.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wta.tianlin.xyz

[U63] PHP：文件读写
来源：http://bmt.hcnkem.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dsv.yj20258888.top

[U64] PHP：目录遍历
来源：http://riy.hnqzz.top

glob("dir/*.php");  scandir("dir");
来源：http://bzt.jqgfzy.top

[U65] PHP：会话
来源：http://djn.ydzc1.top

session_start();  $_SESSION["uid"] = 1;
来源：http://uun.hnqzz.top

[U66] PHP：设置 Cookie
来源：http://wti.wangdashe.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nel.jqgfzy.top

[U67] PHP：处理文件上传
来源：http://ami.ydzc1.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nwa.tanke756.top

[U68] PHP：PDO 连接
来源：http://inn.gogol.net.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://owf.feifeiyinyue.top

[U69] PHP：PDO 预处理
来源：http://omz.ydzc1.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fqy.hammf.cn

[U70] PHP：PDO 事务
来源：http://luk.yj202588.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ryv.fengsongda.top

[U71] PHP：抛出异常
来源：http://fol.ydzc1.top

throw new RuntimeException("失败", 500);
来源：http://fdy.yj20258.top

[U72] PHP：写错误日志
来源：http://hxf.haohaochexian.top

error_log("失败: " . $e->getMessage());
来源：http://bib.pycfn.com

[U73] PHP：读取 ini 配置
来源：http://lux.yvedp.cn

parse_ini_file("config.ini", true)
来源：http://btk.mhx1999.top

[U74] PHP：读取环境变量
来源：http://jmv.jinqigfzy.top

getenv("APP_ENV") ?: "production"
来源：http://yik.ivvv.top

[U75] PHP：依赖注入
来源：http://xrx.gotoacloud.top

composer require psr/container
来源：http://gqu.chenjidiqi.icu

[U76] PHP：简单路由
来源：http://czj.daria6918.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ldn.ydzc1.top

[U77] PHP：模板渲染
来源：http://urm.yvedp.cn

composer require twig/twig
来源：http://ofq.yuxming.cn

[U78] PHP：单元测试
来源：http://izw.fktsv.cn

composer require --dev phpunit/phpunit
来源：http://npe.snrcjt.cn

[U79] PHP：静态分析
来源：http://zye.hongshengwenyu.top

composer require --dev phpstan/phpstan
来源：http://adu.hfpthk.cn

[U80] PHP：代码规范修复
来源：http://dtx.316326.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://dcl.nanxuanxn.top

[U81] JS：初始化项目
来源：http://znt.gogol.net.cn

npm init -y;  npm i express
来源：http://hlx.zhixingplan.top

[U82] JS：package.json 脚本
来源：http://wwg.yongpay.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fej.cqqwz.cn

[U83] JS：ES Module 导入导出
来源：http://tra.c1oappe.top

export const a = 1;  import { a } from "./m.js";
来源：http://ndk.birdmap.top

[U84] JS：CommonJS 写法
来源：http://sse.zdbjq.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gza.quarkkingdee.top

[U85] JS：可选链
来源：http://lfp.ehwqpu.com

a?.b?.c
来源：http://ktg.hfpthk.cn

[U86] JS：空值合并
来源：http://nry.meibo888.top

a ?? b
来源：http://jqa.hesvh.cn

[U87] JS：解构默认值
来源：http://trj.zhoulong.xyz

const { a = 1, b = 2 } = obj;
来源：http://mci.tanke756.top

[U88] JS：对象展开合并
来源：http://svp.shzxlz.cn

{ ...a, ...b }
来源：http://pmz.wangdashe.top

[U89] JS：数组去重
来源：http://jfy.mhx1999.top

[...new Set(arr)]
来源：http://ejj.yongpay.top

[U90] JS：数字数组排序
来源：http://bqy.guowangkeji.top

[...arr].sort((a, b) => a - b)
来源：http://hfz.sjlbkw.cn

[U91] JS：对象键值遍历
来源：http://pad.hnxiangtu.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ukc.pycfn.com

[U92] JS：深拷贝
来源：http://mzi.bjfxy.top

structuredClone(obj)
来源：http://sgu.yuanzhike.top

[U93] JS：模板字符串
来源：http://urt.fzhhl.top

`共 ${n} 条`
来源：http://mnz.nanxuanxn.top

[U94] JS：箭头函数
来源：http://rab.nwbrower.top

const double = x => x * 2;
来源：http://hmi.birdmap.top

[U95] JS：Promise 包装
来源：http://ubs.sufxvd.cn

new Promise((resolve, reject) => {})
来源：http://itk.nanxuanxn.top

[U96] JS：async/await 与异常
来源：http://wdn.fengsongda.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ppw.nanxuanxn.top

[U97] JS：并发请求
来源：http://agk.ywan-chungtsiang.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://oew.gogol.net.cn

[U98] JS：fetch 带 JSON
来源：http://skm.chenlongwang.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://krz.ctjpmb.com

[U99] JS：事件监听
来源：http://wgh.ehwqpu.com

el.addEventListener("click", e => {})
来源：http://qcu.ivvv.top

[U100] JS：DOM 查询
来源：http://xyk.smart0.xyz

document.querySelector(".item")
来源：http://bbp.aizwys.cn

[U101] JS：classList 操作
来源：http://ope.guannengcc.top

el.classList.toggle("active")
来源：http://pto.tianlin.xyz

[U102] JS：本地存储
来源：http://yct.jinyuanbaomall.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://yzl.zhaomingkeji.xyz

[U103] JS：定时器
来源：http://mmk.yj202588.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vjn.jianghu66.top

[U104] JS：防抖
来源：http://gph.sysykeji.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ung.sxryk.cn

[U105] JS：节流
来源：http://xhj.gogol.net.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wmr.meibo888.top

[U106] JS：日期格式化
来源：http://jhq.sjlbkw.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qie.shuidangran.top

[U107] JS：数字千分位
来源：http://dap.chenzaomai.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://asw.c1oappe.top

[U108] JS：随机整数
来源：http://bpr.nanxuanxn.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://giv.shanyushiyangtech.top

[U109] JS：数组分组
来源：http://aex.9152youxi.cn

Object.groupBy(arr, x => x.type)
来源：http://jve.ppjwa.cn

[U110] JS：数组分块
来源：http://ari.cheryme.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lnu.guannengcc.top

[U111] JS：对象转 Map
来源：http://rwp.zhongyouzk.top

new Map(Object.entries(obj))
来源：http://jlb.daria6918.cn

[U112] JS：字符串补位
来源：http://qls.jinyuanbaomall.cn

"7".padStart(3, "0")
来源：http://qpl.jinqigfzy.top

[U113] JS：正则替换全部
来源：http://euy.xuanzx.com

s.replaceAll("a", "b")
来源：http://eue.zdqjudy.top

[U114] JS：JSON 深比较
来源：http://ykj.guowangkeji.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://gbb.316326.xyz

[U115] JS：生成 UUID
来源：http://xis.xingfuxueyuan.xyz

crypto.randomUUID()
来源：http://rtw.vqdsnc.cn

[U116] JS：类型检查（JSDoc）
来源：http://jbl.chenzaomai.com

/** @param {string} name */ function f(name) {}
来源：http://gwg.chenjidiqi.icu

[U117] JS：单元测试
来源：http://cyh.xuanzx.com

npm i -D vitest;  npx vitest
来源：http://glf.hfpthk.cn

[U118] JS：开发服务器
来源：http://vqz.zhixingplan.top

npm i -D vite;  npx vite
来源：http://aig.yangfankeji.com

[U119] JS：生产构建
来源：http://zvp.yj20258.top

npx vite build
来源：http://vvh.wangdashe.top

[U120] JS：读取环境变量（Vite）
来源：http://hnq.shuidangran.top

import.meta.env.VITE_API_URL
来源：http://ptk.0kj1m.cn

================================================================================
来源：http://nhi.haohaochexian.top

统计汇总
来源：http://nha.tarul.cn

================================================================================
来源：http://zvq.xinyue.icu

按语言统计（条）：
来源：http://gkg.ehwqpu.com

Python ......... 252
来源：http://tyu.316326.xyz

PHP ............ 252
来源：http://eeb.zhengqikj.top

JavaScript ..... 252
来源：http://lon.yanxiufei.cn

TypeScript ..... 212
来源：http://igk.jianghu66.top

Java ........... 212
来源：http://kwu.zhongyouzk.top

Go ............. 212
来源：http://mgf.haohaochexian.top

Ruby ........... 212
来源：http://idl.chenlongwang.top

C# ............. 212
来源：http://fxg.shzxlz.cn

C .............. 30
来源：http://ahc.jiagoushi.top

C++ ............ 30
来源：http://xlo.aibaodan.cn

SQL ............ 90
来源：http://tku.meibo888.top

Bash ........... 80
来源：http://xte.svipenyu.cn

Kotlin ......... 15
来源：http://hkl.nanxuanxn.top

Swift .......... 15
来源：http://pns.ydzc1.top

Lua ............ 10
来源：http://inb.xingfuxueyuan.xyz

Perl ........... 10
来源：http://uin.9152youxi.cn

Scala .......... 10
来源：http://fuu.xuetiantiany.cn

------------------------------------
来源：http://qwo.sysykeji.top

合计 ........... 2106 条
来源：http://rpz.fanxiaobao.xyz

按章节统计：
来源：http://xuk.kuanghao11.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ckk.nwbrower.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bto.pengpengdd.cyou

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bqh.bbcook.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lop.yongpay.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://foe.jinyuanbaomall.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fgk.tian-w.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gfo.yfazqb.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xym.vehdjk.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://iqa.zycfv.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xew.sufxvd.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kgo.hfpthk.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nhn.chenlongwang.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://etm.andypj.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yhc.bbcook.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dic.nanxinkj.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lay.shanyushiyangtech.top

Q SQL 专题                              90
来源：http://tbt.zhaomingkeji.xyz

R Bash 专题                             80
来源：http://mhr.fktsv.cn

S C / C++ 专题                          60
来源：http://jws.jqgufenzy.top

T 其他语言补充                          60
来源：http://tdu.cashguo.top

U 高频实用片段                         120
来源：http://cjt.yonumen.top

------------------------------------
来源：http://ozw.jinqigufen.top

合计                                  2106 条
来源：http://biz.zhiwuduotai.top

--------------------------------------------------------------------------------
来源：http://mnm.shanyushiyangkeji.top

使用提醒
来源：http://ywt.fktsv.cn

--------------------------------------------------------------------------------
来源：http://eby.bbcook.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vnj.jyoumei.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pse.sufxvd.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mwt.yangfankeji.com

在旧版本上使用前请先确认语法支持情况。
来源：http://pnq.jqgfzy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dtp.chenzaomai.com

—— 文件结束 ——
来源：http://tek.nanxuanxn.top

================================================================================
来源：http://xvy.smart0.xyz

程序语言常见例子速查手册（2024 版）
来源：http://rvm.tanke756.top

Common Programming Examples Cheat Book
来源：http://ixo.zhijiandao.cn

================================================================================
来源：http://xuh.sweek.top

【收录内容】
来源：http://gst.cqqwz.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://xzd.yuanzhike.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://lwu.hysaishi.cn

SQL · Bash · C · C++
来源：http://nyg.nwbrower.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jau.sweek.top

【使用说明】
来源：http://skj.iojbl.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ekc.yueranfly.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://msf.bbcook.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dls.sysykeji.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bkt.cqqwz.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://eat.pycfn.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://scx.jyoumei.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qgu.pengpengdd.cyou

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fni.zhoulong.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jts.shanyushiyangtech.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tre.fktsv.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pxc.hywenlv.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://cev.guowangkeji.top

【文件统计】
来源：http://bre.jiagoushi.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qem.nanxinkj.top

--------------------------------------------------------------------------------
来源：http://aol.iojbl.cn

目  录
来源：http://epi.zhoulong.xyz

--------------------------------------------------------------------------------
来源：http://peu.zhengqikj.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ezq.iojbl.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qte.gogol.net.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bos.aibaodan.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://awu.zhengqikj.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://snb.hnqzz.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://yck.cucudq.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gyx.shanyushiyangtech.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://suf.vqdsnc.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://eup.zhengqikj.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vdz.chenlongwang.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dma.ctjpmb.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://avd.andypj.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cgb.c1oappe.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://thy.ydzc1.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bfe.jqgfzy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://skm.wangdashe.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://rel.uphjek.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://nss.pengpengdd.cyou

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lww.pengpengdd.cyou

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://guf.nanxuanxn.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://tro.yanxiufei.cn

================================================================================
来源：http://srx.fktsv.cn

A. 基础语法与类型
来源：http://iph.cqqwz.cn

================================================================================
来源：http://wcc.yonumen.top

[A01] Hello World
来源：http://fnn.316326.xyz

Py:   print("Hello, World!")
来源：http://gdk.aizwys.cn

PHP:  echo "Hello, World!";
来源：http://jhs.cucudq.cn

JS:   console.log("Hello, World!");
来源：http://ljp.tian-w.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://kro.cashguo.top

Java: System.out.println("Hello, World!");
来源：http://jif.bbcook.cn

Go:   fmt.Println("Hello, World!")
来源：http://tpl.jlsjyb.cn

Ruby: puts "Hello, World!"
来源：http://zxb.jinqigufen.top

C#:   Console.WriteLine("Hello, World!");
来源：http://xtw.chenlongwang.top

[A02] 变量声明与赋值
来源：http://jvi.hammf.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ncz.quarkkingdee.top

PHP:  $name = "Alex"; $age = 20;
来源：http://uex.zdqjudy.top

JS:   let name = "Alex"; const age = 20;
来源：http://cnm.guannengcc.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://okm.guowangkeji.top

Java: String name = "Alex"; int age = 20;
来源：http://lgo.vehdjk.com

Go:   name := "Alex"; age := 20
来源：http://txw.hcnkem.com

Ruby: name = "Alex"; age = 20
来源：http://rvx.52xcode.cn

C#:   string name = "Alex"; int age = 20;
来源：http://dko.hnqzz.top

[A03] 常量定义
来源：http://tvm.hywenlv.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mbf.bbcook.cn

PHP:  const PI = 3.14159;
来源：http://sgn.yongpay.top

JS:   const PI = 3.14159;
来源：http://chv.jqgufenzy.top

TS:   const PI: number = 3.14159;
来源：http://pft.chenlongwang.top

Java: static final double PI = 3.14159;
来源：http://hby.hywenlv.cn

Go:   const PI = 3.14159
来源：http://tcy.yj20258888.top

Ruby: PI = 3.14159
来源：http://moy.jqgufenzy.top

C#:   const double PI = 3.14159;
来源：http://zim.hnqzz.top

[A04] 判断变量类型
来源：http://hey.uphjek.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://ras.zhiwuduotai.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ypi.yonumen.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qro.sjlbkw.cn

TS:   typeof x; x instanceof Date
来源：http://rcp.xuanzx.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://udy.shanyushiyangtech.top

Go:   reflect.TypeOf(x).Name()
来源：http://jxo.wangshuangyany.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://qpu.tianlin.xyz

C#:   x.GetType().Name; x is int
来源：http://ncg.fehbvm.com

[A05] 整数除法与取模
来源：http://xax.shzxlz.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gdn.haohaochexian.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://lty.hongshengwenyu.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bjp.jinghuilouyu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://sdb.epnwcf.com

Java: 7 / 2; 7 % 2
来源：http://crf.0kj1m.cn

Go:   7 / 2; 7 % 2
来源：http://gyn.jinqigfzy.top

Ruby: 7 / 2; 7 % 2
来源：http://stc.sufxvd.cn

C#:   7 / 2; 7 % 2
来源：http://ctk.zhongyouzk.top

[A06] 字符串转数字
来源：http://blg.uphjek.com

Py:   int("42"); float("3.14")
来源：http://pec.hysaishi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://azv.jinqigufen.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ill.jyoumei.cn

TS:   parseInt("42", 10); Number("42")
来源：http://jxh.yvedp.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://sfe.ydjk.org.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://akh.chenlongwang.top

Ruby: "42".to_i; "3.14".to_f
来源：http://nyy.hywenlv.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qvs.yanxiufei.cn

[A07] 数字转字符串
来源：http://gvg.c1oappe.top

Py:   str(42)
来源：http://vwo.gogol.net.cn

PHP:  (string) 42; strval(42)
来源：http://bwe.jyoumei.cn


<!-- 参考信息 -->