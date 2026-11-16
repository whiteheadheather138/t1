代发 wailian999

[U51] PHP：数组解构
来源：http://rmi.jyoumei.cn

[$a, $b] = $arr;
来源：http://uxc.havefunace.top

[U52] PHP：箭头函数
来源：http://mvs.yangfankeji.com

$double = fn($x) => $x * 2;
来源：http://ujw.yangfankeji.com

[U53] PHP：空合并运算符
来源：http://haa.dianchejie.cn

$v = $a ?? $b ?? "default";
来源：http://blc.zdbjq.cn

[U54] PHP：空安全调用
来源：http://cpf.zhaomingkeji.xyz

$obj?->method()
来源：http://nhm.redwolf501.top

[U55] PHP：match 表达式
来源：http://otu.xylfe.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hqr.yangfankeji.com

[U56] PHP：命名参数
来源：http://vyp.zdqjudy.top

f(a: 1, b: 2)
来源：http://kli.jinghuilouyu.cn

[U57] PHP：字符串插值
来源：http://ebz.jinyuanbaomall.cn

"值: {$a}"
来源：http://qmk.jinghuilouyu.cn

[U58] PHP：数组三件套
来源：http://sem.jlsjyb.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bxs.hammf.cn

[U59] PHP：自定义排序
来源：http://ywq.shuidangran.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cae.smart0.xyz

[U60] PHP：JSON 编解码
来源：http://wij.ywan-chungtsiang.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dxj.sufxvd.cn

[U61] PHP：正则
来源：http://wym.yanxiufei.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zpv.guowangkeji.top

[U62] PHP：日期对象
来源：http://ejp.ehwqpu.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vpb.ydjk.org.cn

[U63] PHP：文件读写
来源：http://pvg.birdmap.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yns.pengpengdd.cyou

[U64] PHP：目录遍历
来源：http://crj.316326.xyz

glob("dir/*.php");  scandir("dir");
来源：http://qec.yj20258.top

[U65] PHP：会话
来源：http://qoz.zhixingplan.top

session_start();  $_SESSION["uid"] = 1;
来源：http://bqc.cqqwz.cn

[U66] PHP：设置 Cookie
来源：http://ohe.hammf.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ebr.snrcjt.cn

[U67] PHP：处理文件上传
来源：http://iyd.jinqigfzy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lhu.tanke756.top

[U68] PHP：PDO 连接
来源：http://khq.shanyushiyangkeji.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nru.tanke756.top

[U69] PHP：PDO 预处理
来源：http://oef.ehwqpu.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ghp.zhoulong.xyz

[U70] PHP：PDO 事务
来源：http://pqm.jlsjyb.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xif.ehwqpu.com

[U71] PHP：抛出异常
来源：http://irm.hesvh.cn

throw new RuntimeException("失败", 500);
来源：http://acm.cheryme.top

[U72] PHP：写错误日志
来源：http://voj.guannengcc.top

error_log("失败: " . $e->getMessage());
来源：http://kyb.nanxuanxn.top

[U73] PHP：读取 ini 配置
来源：http://vec.jyoumei.cn

parse_ini_file("config.ini", true)
来源：http://vas.hywenlv.cn

[U74] PHP：读取环境变量
来源：http://dkn.hongshengwenyu.top

getenv("APP_ENV") ?: "production"
来源：http://jhn.jiagoushi.top

[U75] PHP：依赖注入
来源：http://kdq.zhaomingkeji.xyz

composer require psr/container
来源：http://cgy.fanxiaobao.xyz

[U76] PHP：简单路由
来源：http://bus.hesvh.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vih.snrcjt.cn

[U77] PHP：模板渲染
来源：http://gyd.snrcjt.cn

composer require twig/twig
来源：http://bbr.ydzc1.top

[U78] PHP：单元测试
来源：http://cbn.bbcook.cn

composer require --dev phpunit/phpunit
来源：http://kcs.yonumen.top

[U79] PHP：静态分析
来源：http://tqw.jiagoushi.top

composer require --dev phpstan/phpstan
来源：http://cfo.cqqwz.cn

[U80] PHP：代码规范修复
来源：http://ubg.ppjwa.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://slx.hongshengwenyu.top

[U81] JS：初始化项目
来源：http://pqf.haohaochexian.top

npm init -y;  npm i express
来源：http://zzw.chenzaomai.com

[U82] JS：package.json 脚本
来源：http://fen.tianlin.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nhg.meibo888.top

[U83] JS：ES Module 导入导出
来源：http://afg.vqdsnc.cn

export const a = 1;  import { a } from "./m.js";
来源：http://eyj.sxryk.cn

[U84] JS：CommonJS 写法
来源：http://eph.jinghuilouyu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://jhn.dashuyun.cn

[U85] JS：可选链
来源：http://snn.svipenyu.cn

a?.b?.c
来源：http://ktn.cashguo.top

[U86] JS：空值合并
来源：http://opr.tanke756.top

a ?? b
来源：http://zxg.hywenlv.cn

[U87] JS：解构默认值
来源：http://niz.316326.xyz

const { a = 1, b = 2 } = obj;
来源：http://cyv.nanxinkj.top

[U88] JS：对象展开合并
来源：http://drg.zhixingplan.top

{ ...a, ...b }
来源：http://cmx.jinqigufen.top

[U89] JS：数组去重
来源：http://yvh.gaohongyu789.top

[...new Set(arr)]
来源：http://yvh.cdnleiting.top

[U90] JS：数字数组排序
来源：http://yev.hysaishi.cn

[...arr].sort((a, b) => a - b)
来源：http://yrp.zhixingplan.top

[U91] JS：对象键值遍历
来源：http://ndv.cqqwz.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nzj.uphjek.com

[U92] JS：深拷贝
来源：http://gwv.sjlbkw.cn

structuredClone(obj)
来源：http://kac.vehdjk.com

[U93] JS：模板字符串
来源：http://xrk.hnqzz.top

`共 ${n} 条`
来源：http://kac.zycfv.cn

[U94] JS：箭头函数
来源：http://lfc.xingfuxueyuan.xyz

const double = x => x * 2;
来源：http://zft.shzxlz.cn

[U95] JS：Promise 包装
来源：http://jlq.xylfe.cn

new Promise((resolve, reject) => {})
来源：http://szd.52xcode.cn

[U96] JS：async/await 与异常
来源：http://amj.ydjk.org.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cwl.hfpthk.cn

[U97] JS：并发请求
来源：http://jyl.zhaomingkeji.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://lii.zycfv.cn

[U98] JS：fetch 带 JSON
来源：http://ykz.yvedp.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ygx.jlsjyb.cn

[U99] JS：事件监听
来源：http://hfm.yueranfly.top

el.addEventListener("click", e => {})
来源：http://jst.aibaodan.cn

[U100] JS：DOM 查询
来源：http://ith.yueranfly.top

document.querySelector(".item")
来源：http://bjq.andypj.xyz

[U101] JS：classList 操作
来源：http://cji.zhijiandao.cn

el.classList.toggle("active")
来源：http://wbf.pengpengdd.cyou

[U102] JS：本地存储
来源：http://tia.ydjk.org.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://pcw.pycfn.com

[U103] JS：定时器
来源：http://otk.fanxiaobao.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://okm.zycfv.cn

[U104] JS：防抖
来源：http://bdr.zdbjq.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sca.tianlin.xyz

[U105] JS：节流
来源：http://eco.haohaochexian.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nhf.shuidangran.top

[U106] JS：日期格式化
来源：http://ozo.nanxinkj.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ngo.daxiang520.top

[U107] JS：数字千分位
来源：http://pvj.yj20258888.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qes.yj20258.top

[U108] JS：随机整数
来源：http://lyn.sufxvd.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vhu.gotoacloud.top

[U109] JS：数组分组
来源：http://shc.0kj1m.cn

Object.groupBy(arr, x => x.type)
来源：http://ogj.yanxiufei.cn

[U110] JS：数组分块
来源：http://lar.epnwcf.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tdu.jyoumei.cn

[U111] JS：对象转 Map
来源：http://qso.zycfv.cn

new Map(Object.entries(obj))
来源：http://nmf.jqgfzy.top

[U112] JS：字符串补位
来源：http://xda.fktsv.cn

"7".padStart(3, "0")
来源：http://bxq.cheryme.top

[U113] JS：正则替换全部
来源：http://gds.zhijiandao.cn

s.replaceAll("a", "b")
来源：http://kln.yuanzhike.top

[U114] JS：JSON 深比较
来源：http://gjd.shuidangran.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://aoo.tianlin.xyz

[U115] JS：生成 UUID
来源：http://xlu.yonumen.top

crypto.randomUUID()
来源：http://pnb.aibaodan.cn

[U116] JS：类型检查（JSDoc）
来源：http://rpr.xingfuxueyuan.xyz

/** @param {string} name */ function f(name) {}
来源：http://fhs.xuetiantiany.cn

[U117] JS：单元测试
来源：http://tzj.zhiwuduotai.top

npm i -D vitest;  npx vitest
来源：http://iww.aizwys.cn

[U118] JS：开发服务器
来源：http://xoe.gaohongyu789.top

npm i -D vite;  npx vite
来源：http://huf.ivvv.top

[U119] JS：生产构建
来源：http://mcf.cashguo.top

npx vite build
来源：http://way.xuanzx.com

[U120] JS：读取环境变量（Vite）
来源：http://flj.ehwqpu.com

import.meta.env.VITE_API_URL
来源：http://otk.iojbl.cn

================================================================================
来源：http://cqc.nwbrower.top

统计汇总
来源：http://ltc.cashguo.top

================================================================================
来源：http://qva.jiagoushi.top

按语言统计（条）：
来源：http://xrq.shuidangran.top

Python ......... 252
来源：http://dng.fengsongda.top

PHP ............ 252
来源：http://cco.haohaochexian.top

JavaScript ..... 252
来源：http://ldg.yuanzhike.top

TypeScript ..... 212
来源：http://jow.daria6918.cn

Java ........... 212
来源：http://ijr.zdbjq.cn

Go ............. 212
来源：http://exe.hammf.cn

Ruby ........... 212
来源：http://nyx.shanyushiyangtech.top

C# ............. 212
来源：http://cxr.yuxming.cn

C .............. 30
来源：http://ftm.fengsongda.top

C++ ............ 30
来源：http://vlc.jqgufenzy.top

SQL ............ 90
来源：http://ncn.dashuyun.cn

Bash ........... 80
来源：http://iog.fanxiaobao.xyz

Kotlin ......... 15
来源：http://oxd.haohaochexian.top

Swift .......... 15
来源：http://zln.guannengcc.top

Lua ............ 10
来源：http://smq.jlsjyb.cn

Perl ........... 10
来源：http://zzz.haohaochexian.top

Scala .......... 10
来源：http://knb.jyoumei.cn

------------------------------------
来源：http://uxk.jinqigfzy.top

合计 ........... 2106 条
来源：http://kto.cheryme.top

按章节统计：
来源：http://ksh.aibaodan.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://weh.fanxiaobao.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ftf.ehwqpu.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ifz.tianlin.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jpr.ctjpmb.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yen.ydjk.org.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://byd.chenlongwang.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://csa.daxiang520.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dhv.ppjwa.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mhb.sxryk.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tqc.gzhubu.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lft.chenlongwang.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://eau.jqgufenzy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vmc.redwolf501.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://omm.aibaodan.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vik.ppjwa.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bad.yueranfly.top

Q SQL 专题                              90
来源：http://sie.fktsv.cn

R Bash 专题                             80
来源：http://jcz.c1oappe.top

S C / C++ 专题                          60
来源：http://jly.c1oappe.top

T 其他语言补充                          60
来源：http://sxo.zdbjq.cn

U 高频实用片段                         120
来源：http://ewf.cucudq.cn

------------------------------------
来源：http://qdx.pengpengdd.cyou

合计                                  2106 条
来源：http://vux.fktsv.cn

--------------------------------------------------------------------------------
来源：http://tmf.yueranfly.top

使用提醒
来源：http://onb.52xcode.cn

--------------------------------------------------------------------------------
来源：http://vge.aizwys.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pcl.chenlongwang.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ork.jlsjyb.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://alf.shangyingyoupin.top

在旧版本上使用前请先确认语法支持情况。
来源：http://flf.shangyingyoupin.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zyd.xingfuxueyuan.xyz

—— 文件结束 ——
来源：http://ijt.uphjek.com

================================================================================
来源：http://fos.zycfv.cn

程序语言常见例子速查手册（2024 版）
来源：http://rzb.fengsongda.top

Common Programming Examples Cheat Book
来源：http://vcm.xinyue.icu

================================================================================
来源：http://iic.jqgufenzy.top

【收录内容】
来源：http://aoa.yuxming.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://xys.tanke756.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bha.yj20258888.top

SQL · Bash · C · C++
来源：http://imb.nanxinkj.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://liz.aibaodan.cn

【使用说明】
来源：http://avq.xylfe.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://feu.vqdsnc.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://itr.hnxiangtu.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://irp.hysaishi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bwi.quarkkingdee.top

Bash:  Shell         C:     C             C++:   C++
来源：http://wcf.yj202588.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bhu.hammf.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://txq.sweek.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://azq.hongshengwenyu.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://drb.zdbjq.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qmn.bjfxy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xcy.yonumen.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://myx.fzhhl.top

【文件统计】
来源：http://vlr.c1oappe.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vyz.xylfe.cn

--------------------------------------------------------------------------------
来源：http://kfg.xingfuxueyuan.xyz

目  录
来源：http://jqt.yongpay.top

--------------------------------------------------------------------------------
来源：http://sfe.cheryme.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fqs.jianghu66.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://kkh.tianlin.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qtz.jinghuilouyu.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kxg.cucudq.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ygr.yfazqb.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://uys.fanxiaobao.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ouu.zhixingplan.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vfl.hcnkem.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zvk.yanxiufei.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ncf.havefunace.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nsg.tarul.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wvh.hysaishi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dum.yvedp.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://aal.yanxiufei.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://buk.yj202588.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mge.redwolf501.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://rxb.shangyingyoupin.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://hlf.gaohongyu789.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vtj.meibo888.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zky.jinqigfzy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://eiu.shangyingyoupin.top

================================================================================
来源：http://rfg.quarkkingdee.top

A. 基础语法与类型
来源：http://aks.feifeiyinyue.top

================================================================================
来源：http://weg.quarkkingdee.top

[A01] Hello World
来源：http://xnk.zdqjudy.top

Py:   print("Hello, World!")
来源：http://llk.hesvh.cn

PHP:  echo "Hello, World!";
来源：http://dvi.hongshengwenyu.top

JS:   console.log("Hello, World!");
来源：http://yyx.jqgufenzy.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hgw.yongpay.top

Java: System.out.println("Hello, World!");
来源：http://dvl.hysaishi.cn

Go:   fmt.Println("Hello, World!")
来源：http://scq.zhoulong.xyz

Ruby: puts "Hello, World!"
来源：http://gtw.shanyushiyangkeji.top

C#:   Console.WriteLine("Hello, World!");
来源：http://sgr.9152youxi.cn

[A02] 变量声明与赋值
来源：http://cmm.feifeiyinyue.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kqc.cucudq.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://swl.cashguo.top

JS:   let name = "Alex"; const age = 20;
来源：http://ewi.vehdjk.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://upm.birdmap.top

Java: String name = "Alex"; int age = 20;
来源：http://nbo.ivvv.top

Go:   name := "Alex"; age := 20
来源：http://oll.nanxuanxn.top

Ruby: name = "Alex"; age = 20
来源：http://cdd.zhongyouzk.top

C#:   string name = "Alex"; int age = 20;
来源：http://emp.chenjidiqi.icu

[A03] 常量定义
来源：http://yxr.yj20258888.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://snz.wangdashe.top

PHP:  const PI = 3.14159;
来源：http://lzw.yvedp.cn

JS:   const PI = 3.14159;
来源：http://foh.gzhubu.top

TS:   const PI: number = 3.14159;
来源：http://llh.smart0.xyz

Java: static final double PI = 3.14159;
来源：http://pbn.jlsjyb.cn

Go:   const PI = 3.14159
来源：http://zlk.shanyushiyangtech.top

Ruby: PI = 3.14159
来源：http://xuw.shanyushiyangtech.top

C#:   const double PI = 3.14159;
来源：http://bne.hnqzz.top

[A04] 判断变量类型
来源：http://mix.dashuyun.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://rhr.nanxinkj.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gmn.shuidangran.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wsb.jinqigfzy.top

TS:   typeof x; x instanceof Date
来源：http://vfg.wangdashe.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://eyd.smart0.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://hpx.hesvh.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://vyf.ybcxt.top

C#:   x.GetType().Name; x is int
来源：http://clw.iojbl.cn

[A05] 整数除法与取模
来源：http://oou.tian-w.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://juw.guowangkeji.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://cir.wangdashe.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hrm.yanxiufei.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kxo.yuxming.cn

Java: 7 / 2; 7 % 2
来源：http://epr.shzxlz.cn

Go:   7 / 2; 7 % 2
来源：http://nwe.nanxinkj.top

Ruby: 7 / 2; 7 % 2
来源：http://aio.hysaishi.cn

C#:   7 / 2; 7 % 2
来源：http://okg.gaohongyu789.top

[A06] 字符串转数字
来源：http://joc.haohaochexian.top

Py:   int("42"); float("3.14")
来源：http://ppy.tanke756.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rjk.fanxiaobao.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://sab.zdqjudy.top

TS:   parseInt("42", 10); Number("42")
来源：http://iub.zhaomingkeji.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://bug.hnxiangtu.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gbk.jlsjyb.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://zne.c1oappe.top


<!-- 参考信息 -->