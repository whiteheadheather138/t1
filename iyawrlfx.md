代发 wailian999

[U53] PHP：空合并运算符
来源：http://wyw.hongshengwenyu.top

$v = $a ?? $b ?? "default";
来源：http://mju.daria6918.cn

[U54] PHP：空安全调用
来源：http://vip.yvedp.cn

$obj?->method()
来源：http://boo.nanxuanxn.top

[U55] PHP：match 表达式
来源：http://stf.gogol.net.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sqh.hfpthk.cn

[U56] PHP：命名参数
来源：http://tzr.fanxiaobao.xyz

f(a: 1, b: 2)
来源：http://rqs.guowangkeji.top

[U57] PHP：字符串插值
来源：http://vlc.bbcook.cn

"值: {$a}"
来源：http://eyg.ppjwa.cn

[U58] PHP：数组三件套
来源：http://hcc.fanxiaobao.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://oez.shangyingyoupin.top

[U59] PHP：自定义排序
来源：http://ckt.epnwcf.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ust.quarkkingdee.top

[U60] PHP：JSON 编解码
来源：http://hsh.zhoulong.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://edm.cashguo.top

[U61] PHP：正则
来源：http://kzh.xylfe.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qtv.shangyingyoupin.top

[U62] PHP：日期对象
来源：http://lns.gaohongyu789.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xjm.daxiang520.top

[U63] PHP：文件读写
来源：http://ahv.tarul.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://khv.quarkkingdee.top

[U64] PHP：目录遍历
来源：http://ucu.epnwcf.com

glob("dir/*.php");  scandir("dir");
来源：http://bsp.daria6918.cn

[U65] PHP：会话
来源：http://krl.cdnleiting.top

session_start();  $_SESSION["uid"] = 1;
来源：http://fxj.tarul.cn

[U66] PHP：设置 Cookie
来源：http://vgf.xuanzx.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nwe.jinghuilouyu.cn

[U67] PHP：处理文件上传
来源：http://rgw.fanxiaobao.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xms.nanxinkj.top

[U68] PHP：PDO 连接
来源：http://wqa.sjlbkw.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gen.smart0.xyz

[U69] PHP：PDO 预处理
来源：http://qdh.xylfe.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wzn.shanyushiyangkeji.top

[U70] PHP：PDO 事务
来源：http://ghp.xinyue.icu

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gaf.pengpengdd.cyou

[U71] PHP：抛出异常
来源：http://rwy.zycfv.cn

throw new RuntimeException("失败", 500);
来源：http://cfv.nanxuanxn.top

[U72] PHP：写错误日志
来源：http://pin.yj20258.top

error_log("失败: " . $e->getMessage());
来源：http://sok.jianghu66.top

[U73] PHP：读取 ini 配置
来源：http://wvk.yfazqb.com

parse_ini_file("config.ini", true)
来源：http://ple.yuxming.cn

[U74] PHP：读取环境变量
来源：http://gsd.jyoumei.cn

getenv("APP_ENV") ?: "production"
来源：http://juv.yj202588.top

[U75] PHP：依赖注入
来源：http://nnr.shanyushiyangtech.top

composer require psr/container
来源：http://rlf.tanke756.top

[U76] PHP：简单路由
来源：http://nrn.zdqjudy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hnv.ehwqpu.com

[U77] PHP：模板渲染
来源：http://evv.hnxiangtu.top

composer require twig/twig
来源：http://tpk.hesvh.cn

[U78] PHP：单元测试
来源：http://tza.9152youxi.cn

composer require --dev phpunit/phpunit
来源：http://yxe.fzhhl.top

[U79] PHP：静态分析
来源：http://avc.epnwcf.com

composer require --dev phpstan/phpstan
来源：http://nzz.ivvv.top

[U80] PHP：代码规范修复
来源：http://lrn.jianghu66.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://lym.xuanzx.com

[U81] JS：初始化项目
来源：http://hfm.cdnleiting.top

npm init -y;  npm i express
来源：http://fva.cashguo.top

[U82] JS：package.json 脚本
来源：http://pmk.shuidangran.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ewq.pycfn.com

[U83] JS：ES Module 导入导出
来源：http://wiw.zhengqikj.top

export const a = 1;  import { a } from "./m.js";
来源：http://ker.hcnkem.com

[U84] JS：CommonJS 写法
来源：http://dkc.fanxiaobao.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://qvf.nanxinkj.top

[U85] JS：可选链
来源：http://bqm.yj20258888.top

a?.b?.c
来源：http://cqk.smart0.xyz

[U86] JS：空值合并
来源：http://aqs.yj202588.top

a ?? b
来源：http://mho.zhaomingkeji.xyz

[U87] JS：解构默认值
来源：http://kuv.zdqjudy.top

const { a = 1, b = 2 } = obj;
来源：http://qks.52xcode.cn

[U88] JS：对象展开合并
来源：http://ddy.zhixingplan.top

{ ...a, ...b }
来源：http://kwh.svipenyu.cn

[U89] JS：数组去重
来源：http://qmr.yongpay.top

[...new Set(arr)]
来源：http://iyg.yonumen.top

[U90] JS：数字数组排序
来源：http://bbz.ehwqpu.com

[...arr].sort((a, b) => a - b)
来源：http://mid.yj20258888.top

[U91] JS：对象键值遍历
来源：http://inh.ybcxt.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pum.bjfxy.top

[U92] JS：深拷贝
来源：http://dnl.yongpay.top

structuredClone(obj)
来源：http://mak.chenlongwang.top

[U93] JS：模板字符串
来源：http://zav.tianlin.xyz

`共 ${n} 条`
来源：http://wyn.pengpengdd.cyou

[U94] JS：箭头函数
来源：http://wpw.hesvh.cn

const double = x => x * 2;
来源：http://oqd.jinyuanbaomall.cn

[U95] JS：Promise 包装
来源：http://gbd.snrcjt.cn

new Promise((resolve, reject) => {})
来源：http://qba.ehwqpu.com

[U96] JS：async/await 与异常
来源：http://hst.sxryk.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zja.yj20258.top

[U97] JS：并发请求
来源：http://hef.ydjk.org.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://dwz.jianghu66.top

[U98] JS：fetch 带 JSON
来源：http://poi.shanyushiyangkeji.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://abi.xuanzx.com

[U99] JS：事件监听
来源：http://wgf.snrcjt.cn

el.addEventListener("click", e => {})
来源：http://amw.dianchejie.cn

[U100] JS：DOM 查询
来源：http://lni.dianchejie.cn

document.querySelector(".item")
来源：http://lod.c1oappe.top

[U101] JS：classList 操作
来源：http://smf.xingfuxueyuan.xyz

el.classList.toggle("active")
来源：http://vew.sxryk.cn

[U102] JS：本地存储
来源：http://qgs.quarkkingdee.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://sdh.pengpengdd.cyou

[U103] JS：定时器
来源：http://saf.hesvh.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://onn.zhijiandao.cn

[U104] JS：防抖
来源：http://ypg.jqgfzy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://swx.fengsongda.top

[U105] JS：节流
来源：http://rqo.jinqigufen.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cuj.sysykeji.top

[U106] JS：日期格式化
来源：http://eno.hesvh.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pzl.zycfv.cn

[U107] JS：数字千分位
来源：http://tar.chenlongwang.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sku.xuetiantiany.cn

[U108] JS：随机整数
来源：http://zht.yonumen.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pko.316326.xyz

[U109] JS：数组分组
来源：http://qcd.aibaodan.cn

Object.groupBy(arr, x => x.type)
来源：http://tty.iojbl.cn

[U110] JS：数组分块
来源：http://nvj.zhoulong.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wvm.chenjidiqi.icu

[U111] JS：对象转 Map
来源：http://wbb.52xcode.cn

new Map(Object.entries(obj))
来源：http://eaz.ybcxt.top

[U112] JS：字符串补位
来源：http://eze.sxryk.cn

"7".padStart(3, "0")
来源：http://kkt.zdqjudy.top

[U113] JS：正则替换全部
来源：http://pvu.gzhubu.top

s.replaceAll("a", "b")
来源：http://jbe.ydzc1.top

[U114] JS：JSON 深比较
来源：http://wqm.feifeiyinyue.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://zcs.uphjek.com

[U115] JS：生成 UUID
来源：http://zwj.tanke756.top

crypto.randomUUID()
来源：http://lob.yueranfly.top

[U116] JS：类型检查（JSDoc）
来源：http://kjk.yanxiufei.cn

/** @param {string} name */ function f(name) {}
来源：http://dty.cheryme.top

[U117] JS：单元测试
来源：http://xpb.ppjwa.cn

npm i -D vitest;  npx vitest
来源：http://lbk.ehwqpu.com

[U118] JS：开发服务器
来源：http://pda.yongpay.top

npm i -D vite;  npx vite
来源：http://qwx.pycfn.com

[U119] JS：生产构建
来源：http://ziw.316326.xyz

npx vite build
来源：http://dlh.jinqigufen.top

[U120] JS：读取环境变量（Vite）
来源：http://mcj.fanxiaobao.xyz

import.meta.env.VITE_API_URL
来源：http://gsz.fktsv.cn

================================================================================
来源：http://lab.hesvh.cn

统计汇总
来源：http://qvt.fehbvm.com

================================================================================
来源：http://ros.zhaomingkeji.xyz

按语言统计（条）：
来源：http://iys.tarul.cn

Python ......... 252
来源：http://lei.shangyingyoupin.top

PHP ............ 252
来源：http://wdu.316326.xyz

JavaScript ..... 252
来源：http://him.cashguo.top

TypeScript ..... 212
来源：http://qhj.yuanzhike.top

Java ........... 212
来源：http://mfi.mhx1999.top

Go ............. 212
来源：http://yij.dashuyun.cn

Ruby ........... 212
来源：http://rju.gotoacloud.top

C# ............. 212
来源：http://jrx.yj20258.top

C .............. 30
来源：http://npx.fengsongda.top

C++ ............ 30
来源：http://ije.jinqigfzy.top

SQL ............ 90
来源：http://vzg.gogol.net.cn

Bash ........... 80
来源：http://anc.xuanzx.com

Kotlin ......... 15
来源：http://lez.hnxiangtu.top

Swift .......... 15
来源：http://noz.guannengcc.top

Lua ............ 10
来源：http://rph.chenzaomai.com

Perl ........... 10
来源：http://iwb.yj20258.top

Scala .......... 10
来源：http://xob.nwbrower.top

------------------------------------
来源：http://rko.jinqigfzy.top

合计 ........... 2106 条
来源：http://ifr.xinyue.icu

按章节统计：
来源：http://gnr.fehbvm.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://usr.kuanghao11.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://brc.xuetiantiany.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bia.cashguo.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pee.bbcook.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hgi.yj20258888.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://reb.andypj.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dav.nwbrower.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tzo.gotoacloud.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rta.shuidangran.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://azx.cashguo.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://and.ydjk.org.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nag.shangyingyoupin.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vjy.zhongyouzk.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rgs.316326.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tsh.redwolf501.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://egp.yj20258888.top

Q SQL 专题                              90
来源：http://kxw.ybcxt.top

R Bash 专题                             80
来源：http://qge.9152youxi.cn

S C / C++ 专题                          60
来源：http://lqd.yangfankeji.com

T 其他语言补充                          60
来源：http://hof.hesvh.cn

U 高频实用片段                         120
来源：http://hdr.yuanzhike.top

------------------------------------
来源：http://mby.fanxiaobao.xyz

合计                                  2106 条
来源：http://zzc.xingfuxueyuan.xyz

--------------------------------------------------------------------------------
来源：http://qhj.shanyushiyangkeji.top

使用提醒
来源：http://gde.52xcode.cn

--------------------------------------------------------------------------------
来源：http://ldy.dashuyun.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://oyq.xuanzx.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zdl.sweek.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://sbw.ehwqpu.com

在旧版本上使用前请先确认语法支持情况。
来源：http://dps.jianghu66.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qtp.quarkkingdee.top

—— 文件结束 ——
来源：http://beg.dianchejie.cn

================================================================================
来源：http://sei.hywenlv.cn

程序语言常见例子速查手册（2024 版）
来源：http://ixc.guowangkeji.top

Common Programming Examples Cheat Book
来源：http://tua.yuanzhike.top

================================================================================
来源：http://aeq.uphjek.com

【收录内容】
来源：http://blr.zhongyouzk.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://szi.dianchejie.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dcu.hammf.cn

SQL · Bash · C · C++
来源：http://pqs.cdnleiting.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mqr.tian-w.cn

【使用说明】
来源：http://pye.jlsjyb.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qez.yuxming.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vcg.yuanzhike.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://puf.svipenyu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://caw.birdmap.top

Bash:  Shell         C:     C             C++:   C++
来源：http://ksb.meibo888.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://fku.tanke756.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://los.andypj.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xld.jiagoushi.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://odu.jiagoushi.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xlt.zycfv.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qfb.aibaodan.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yjp.gotoacloud.top

【文件统计】
来源：http://hxs.hywenlv.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jpb.52xcode.cn

--------------------------------------------------------------------------------
来源：http://myk.tian-w.cn

目  录
来源：http://qak.yj202588.top

--------------------------------------------------------------------------------
来源：http://pqm.zdbjq.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pkd.ehwqpu.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://sub.zhijiandao.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://glk.mhx1999.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cii.0kj1m.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tsg.tianlin.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ejg.jiagoushi.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://sjs.hywenlv.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://oty.smart0.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://eci.yuanzhike.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wgo.fzhhl.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://oui.yvedp.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ytl.hongshengwenyu.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jcc.vqdsnc.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rjt.ctjpmb.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://acs.wangshuangyany.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zzo.shzxlz.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://trl.xinyue.icu

R. Bash 专题                   （第 18 节，80 条）
来源：http://knq.ivvv.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hac.gzhubu.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ucf.bjfxy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fao.hfpthk.cn

================================================================================
来源：http://jly.sysykeji.top

A. 基础语法与类型
来源：http://vvf.kuanghao11.cn

================================================================================
来源：http://cto.yangfankeji.com

[A01] Hello World
来源：http://fig.fanxiaobao.xyz

Py:   print("Hello, World!")
来源：http://mhv.xuetiantiany.cn

PHP:  echo "Hello, World!";
来源：http://gfr.andypj.xyz

JS:   console.log("Hello, World!");
来源：http://sbk.52xcode.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://kuy.fzhhl.top

Java: System.out.println("Hello, World!");
来源：http://vfw.bjfxy.top

Go:   fmt.Println("Hello, World!")
来源：http://wgn.yangfankeji.com

Ruby: puts "Hello, World!"
来源：http://bpk.hfpthk.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://que.iojbl.cn

[A02] 变量声明与赋值
来源：http://wnr.vqdsnc.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rfp.cheryme.top

PHP:  $name = "Alex"; $age = 20;
来源：http://lzn.ctjpmb.com

JS:   let name = "Alex"; const age = 20;
来源：http://fce.ydzc1.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://flw.yonumen.top

Java: String name = "Alex"; int age = 20;
来源：http://qpj.dianchejie.cn

Go:   name := "Alex"; age := 20
来源：http://mkb.cucudq.cn

Ruby: name = "Alex"; age = 20
来源：http://mcz.ppjwa.cn

C#:   string name = "Alex"; int age = 20;
来源：http://psr.52xcode.cn

[A03] 常量定义
来源：http://emx.birdmap.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kts.chenlongwang.top

PHP:  const PI = 3.14159;
来源：http://ivl.ywan-chungtsiang.top

JS:   const PI = 3.14159;
来源：http://yxy.shzxlz.cn

TS:   const PI: number = 3.14159;
来源：http://snb.pycfn.com

Java: static final double PI = 3.14159;
来源：http://oha.nwbrower.top

Go:   const PI = 3.14159
来源：http://lpw.tianlin.xyz

Ruby: PI = 3.14159
来源：http://szl.jianghu66.top

C#:   const double PI = 3.14159;
来源：http://zaj.sysykeji.top

[A04] 判断变量类型
来源：http://stt.guannengcc.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://frm.yj202588.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rkk.fehbvm.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://asi.xinyue.icu

TS:   typeof x; x instanceof Date
来源：http://hag.hnqzz.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zhb.yj202588.top

Go:   reflect.TypeOf(x).Name()
来源：http://mre.yvedp.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ylw.bbcook.cn

C#:   x.GetType().Name; x is int
来源：http://sxc.xylfe.cn

[A05] 整数除法与取模
来源：http://xcl.fengsongda.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rws.316326.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://pxu.shuidangran.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://esh.nanxuanxn.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://znn.meibo888.top

Java: 7 / 2; 7 % 2
来源：http://auu.cdnleiting.top

Go:   7 / 2; 7 % 2
来源：http://zqq.chenzaomai.com

Ruby: 7 / 2; 7 % 2
来源：http://agl.zdbjq.cn

C#:   7 / 2; 7 % 2
来源：http://xhf.yj20258888.top

[A06] 字符串转数字
来源：http://jos.zhiwuduotai.top

Py:   int("42"); float("3.14")
来源：http://ijv.ydjk.org.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hqe.zdbjq.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hdk.tanke756.top

TS:   parseInt("42", 10); Number("42")
来源：http://swp.jqgfzy.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://evw.yvedp.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://krz.hywenlv.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://lhk.hfpthk.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wiu.hfpthk.cn

[A07] 数字转字符串
来源：http://mkd.jinghuilouyu.cn

Py:   str(42)
来源：http://hrr.svipenyu.cn

PHP:  (string) 42; strval(42)
来源：http://lmv.yanxiufei.cn


<!-- 参考信息 -->